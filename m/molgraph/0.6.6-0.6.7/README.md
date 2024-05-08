# Comparing `tmp/molgraph-0.6.6.tar.gz` & `tmp/molgraph-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.6.6.tar", last modified: Tue Mar 12 14:19:44 2024, max compression
+gzip compressed data, was "molgraph-0.6.7.tar", last modified: Wed May  8 14:41:18 2024, max compression
```

## Comparing `molgraph-0.6.6.tar` & `molgraph-0.6.7.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2024-02-09 14:16:36.000000 molgraph-0.6.6/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     7018 2024-03-12 14:19:44.285030 molgraph-0.6.6/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     6245 2024-03-12 14:18:33.000000 molgraph-0.6.6/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.277030 molgraph-0.6.6/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2024-02-09 14:01:31.000000 molgraph-0.6.6/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2024-03-12 14:18:33.000000 molgraph-0.6.6/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.277030 molgraph-0.6.6/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-08-25 11:53:51.000000 molgraph-0.6.6/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.277030 molgraph-0.6.6/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.6.6/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.6.6/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13588 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8901 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15647 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2720 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10474 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14141 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13791 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20705 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1788 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2716 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/chemistry/vis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      923 2023-07-17 15:20:50.000000 molgraph-0.6.6/molgraph/internal.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.281030 molgraph-0.6.6/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.6.6/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.281030 molgraph-0.6.6/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.6.6/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10445 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10943 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9031 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10971 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9736 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16345 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.281030 molgraph-0.6.6/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.6.6/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9139 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9077 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9635 2024-01-05 10:02:27.000000 molgraph-0.6.6/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9428 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.281030 molgraph-0.6.6/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.6.6/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8706 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9694 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1633 2023-07-17 15:20:50.000000 molgraph-0.6.6/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25628 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.6.6/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.281030 molgraph-0.6.6/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.6.6/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15199 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12619 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.281030 molgraph-0.6.6/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.6.6/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10531 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.281030 molgraph-0.6.6/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.6.6/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3652 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1799 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2806 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.6.6/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9327 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3740 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8640 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3986 2024-02-27 16:49:00.000000 molgraph-0.6.6/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10208 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6437 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17029 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.6.6/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5959 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4035 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3151 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6096 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5205 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.6.6/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2382 2023-07-19 15:00:26.000000 molgraph-0.6.6/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5383 2023-07-17 15:20:50.000000 molgraph-0.6.6/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.6.6/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2083 2023-07-17 15:20:50.000000 molgraph-0.6.6/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      566 2023-07-17 15:20:50.000000 molgraph-0.6.6/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      982 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10140 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/models/dmpnn.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11143 2024-02-09 14:16:36.000000 molgraph-0.6.6/molgraph/models/gin.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.6.6/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3787 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10779 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6617 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.6.6/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    26799 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    19862 2023-08-31 08:08:59.000000 molgraph-0.6.6/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.285030 molgraph-0.6.6/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-11-27 09:26:02.000000 molgraph-0.6.6/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    76901 2024-01-03 14:53:44.000000 molgraph-0.6.6/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 14:19:44.277030 molgraph-0.6.6/molgraph.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     7018 2024-03-12 14:19:44.000000 molgraph-0.6.6/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3178 2024-03-12 14:19:44.000000 molgraph-0.6.6/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-03-12 14:19:44.000000 molgraph-0.6.6/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      101 2024-03-12 14:19:44.000000 molgraph-0.6.6/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2024-03-12 14:19:44.000000 molgraph-0.6.6/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-03-12 14:19:44.285030 molgraph-0.6.6/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1605 2024-03-12 14:18:33.000000 molgraph-0.6.6/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.495480 molgraph-0.6.7/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2024-02-09 14:16:36.000000 molgraph-0.6.7/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6878 2024-05-08 14:41:18.495480 molgraph-0.6.7/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6105 2024-04-26 15:56:50.000000 molgraph-0.6.7/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.479480 molgraph-0.6.7/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2024-02-09 14:01:31.000000 molgraph-0.6.7/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2024-05-08 14:40:27.000000 molgraph-0.6.7/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.479480 molgraph-0.6.7/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-08-25 11:53:51.000000 molgraph-0.6.7/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.483481 molgraph-0.6.7/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.6.7/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.6.7/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13588 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8901 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15647 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2720 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10474 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14141 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13791 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20705 2024-04-18 13:41:07.000000 molgraph-0.6.7/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1788 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2716 2024-04-24 15:50:58.000000 molgraph-0.6.7/molgraph/chemistry/vis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      923 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/internal.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.483481 molgraph-0.6.7/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.483481 molgraph-0.6.7/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.6.7/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10445 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10943 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9031 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11010 2024-05-08 14:40:27.000000 molgraph-0.6.7/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9736 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16345 2024-04-24 13:28:36.000000 molgraph-0.6.7/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.487480 molgraph-0.6.7/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.6.7/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9139 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9077 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9635 2024-01-05 10:02:27.000000 molgraph-0.6.7/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9428 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.487480 molgraph-0.6.7/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.6.7/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8706 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9694 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1633 2023-07-17 15:20:50.000000 molgraph-0.6.7/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    25628 2024-04-18 13:54:20.000000 molgraph-0.6.7/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.6.7/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.487480 molgraph-0.6.7/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.6.7/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15199 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12619 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.487480 molgraph-0.6.7/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.6.7/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10531 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.487480 molgraph-0.6.7/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.6.7/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3652 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1799 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2806 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.491480 molgraph-0.6.7/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.6.7/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9327 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3740 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8640 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3986 2024-02-27 16:49:00.000000 molgraph-0.6.7/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10208 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6437 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17029 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.491480 molgraph-0.6.7/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.6.7/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5959 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4035 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3151 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6096 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5205 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.491480 molgraph-0.6.7/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.6.7/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2382 2023-07-19 15:00:26.000000 molgraph-0.6.7/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5383 2023-07-17 15:20:50.000000 molgraph-0.6.7/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.491480 molgraph-0.6.7/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.6.7/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2083 2023-07-17 15:20:50.000000 molgraph-0.6.7/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      566 2023-07-17 15:20:50.000000 molgraph-0.6.7/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.495480 molgraph-0.6.7/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      982 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10140 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/models/dmpnn.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11143 2024-02-09 14:16:36.000000 molgraph-0.6.7/molgraph/models/gin.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.495480 molgraph-0.6.7/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.6.7/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3787 2024-04-18 08:53:56.000000 molgraph-0.6.7/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10779 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6617 2023-08-31 08:08:59.000000 molgraph-0.6.7/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.495480 molgraph-0.6.7/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.6.7/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26799 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    19862 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.495480 molgraph-0.6.7/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-11-27 09:26:02.000000 molgraph-0.6.7/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    76901 2024-04-26 15:56:50.000000 molgraph-0.6.7/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 14:41:18.479480 molgraph-0.6.7/molgraph.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6878 2024-05-08 14:41:18.000000 molgraph-0.6.7/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3178 2024-05-08 14:41:18.000000 molgraph-0.6.7/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-05-08 14:41:18.000000 molgraph-0.6.7/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      101 2024-05-08 14:41:18.000000 molgraph-0.6.7/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2024-05-08 14:41:18.000000 molgraph-0.6.7/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-05-08 14:41:18.495480 molgraph-0.6.7/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1605 2024-04-26 14:59:24.000000 molgraph-0.6.7/setup.py
```

### Comparing `molgraph-0.6.6/LICENSE` & `molgraph-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/PKG-INFO` & `molgraph-0.6.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.6.6
+Version: 0.6.7
 Summary: Graph Neural Networks for Molecular Machine Learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,graph-neural-networks,graphs,molecular-machine-learning,molecular-graphs,cheminformatics,chemometrics,bioinformatics,chemistry,biology,biochemistry
 Classifier: Programming Language :: Python :: 3
@@ -87,32 +87,30 @@
     - And models for improved interpretability of GNNs:
         - **SaliencyMapping**
         - **IntegratedSaliencyMapping**
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Requirements/dependencies
-- **Python** (version ~= 3.10.0)
-    - **TensorFlow** (version ~= 2.15.0)
-    - **RDKit** (version ~= 2022.3.5)
-    - **Pandas** (version ~= 1.0.3)
-    - **IPython** (version ~= 8.12.0)
-
-> MolGraph should work with the more recent TensorFlow and RDKit versions. If not, try installing earlier versions of TensorFlow and RDKit.
+- **Python** (version >= 3.10)
+    - **TensorFlow** (version 2.15.*)
+    - **RDKit** (version 2023.9.*)
+    - **Pandas**
+    - **IPython**
 
 ## Installation
 
-For **GPU** users:
+For **CPU** users:
 <pre>
-pip install molgraph[gpu]
+pip install molgraph
 </pre>
 
-For **CPU** users:
+For **GPU** users:
 <pre>
-pip install molgraph
+pip install molgraph[gpu]
 </pre>
 
 Now run your first program with **MolGraph**:
 
 ```python
 from tensorflow import keras
 from molgraph import chemistry
@@ -141,14 +139,15 @@
 y_train = esol['train']['y']
 
 x_test = encoder(esol['test']['x'])
 y_test = esol['test']['y']
 
 # Build model via Keras API
 gnn_model = keras.Sequential([
+    keras.layers.Input(type_spec=x_train.spec),
     layers.GATConv(units=32, name='gat_conv_1'),
     layers.GATConv(units=32, name='gat_conv_2'),
     layers.Readout(),
     keras.layers.Dense(units=1024, activation='relu'),
     keras.layers.Dense(units=y_train.shape[-1])
 ])
```

### Comparing `molgraph-0.6.6/README.md` & `molgraph-0.6.7/molgraph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: molgraph
+Version: 0.6.7
+Summary: Graph Neural Networks for Molecular Machine Learning
+Home-page: https://github.com/akensert/molgraph
+Author: Alexander Kensert
+Author-email: alexander.kensert@gmail.com
+License: MIT
+Keywords: machine-learning,deep-learning,graph-neural-networks,graphs,molecular-machine-learning,molecular-graphs,cheminformatics,chemometrics,bioinformatics,chemistry,biology,biochemistry
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: gpu
+License-File: LICENSE
+
 # MolGraph
 
 **Graph Neural Networks** with **TensorFlow** and **Keras**. Focused on **Molecular Machine Learning**.
 
 <img src="https://github.com/akensert/molgraph/blob/main/media/molgraph.jpg" alt="molgraph" width="820">
 
 ## Highlights
@@ -68,32 +87,30 @@
     - And models for improved interpretability of GNNs:
         - **SaliencyMapping**
         - **IntegratedSaliencyMapping**
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Requirements/dependencies
-- **Python** (version ~= 3.10.0)
-    - **TensorFlow** (version ~= 2.15.0)
-    - **RDKit** (version ~= 2022.3.5)
-    - **Pandas** (version ~= 1.0.3)
-    - **IPython** (version ~= 8.12.0)
-
-> MolGraph should work with the more recent TensorFlow and RDKit versions. If not, try installing earlier versions of TensorFlow and RDKit.
+- **Python** (version >= 3.10)
+    - **TensorFlow** (version 2.15.*)
+    - **RDKit** (version 2023.9.*)
+    - **Pandas**
+    - **IPython**
 
 ## Installation
 
-For **GPU** users:
+For **CPU** users:
 <pre>
-pip install molgraph[gpu]
+pip install molgraph
 </pre>
 
-For **CPU** users:
+For **GPU** users:
 <pre>
-pip install molgraph
+pip install molgraph[gpu]
 </pre>
 
 Now run your first program with **MolGraph**:
 
 ```python
 from tensorflow import keras
 from molgraph import chemistry
@@ -122,14 +139,15 @@
 y_train = esol['train']['y']
 
 x_test = encoder(esol['test']['x'])
 y_test = esol['test']['y']
 
 # Build model via Keras API
 gnn_model = keras.Sequential([
+    keras.layers.Input(type_spec=x_train.spec),
     layers.GATConv(units=32, name='gat_conv_1'),
     layers.GATConv(units=32, name='gat_conv_2'),
     layers.Readout(),
     keras.layers.Dense(units=1024, activation='relu'),
     keras.layers.Dense(units=y_train.shape[-1])
 ])
```

### Comparing `molgraph-0.6.6/molgraph/_filter_warnings.py` & `molgraph-0.6.7/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/__init__.py` & `molgraph-0.6.7/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.6.7/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.6.7/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.6.7/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.6.7/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/conformer_generator.py` & `molgraph-0.6.7/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/conformer_utils.py` & `molgraph-0.6.7/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/encoders.py` & `molgraph-0.6.7/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/features.py` & `molgraph-0.6.7/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.6.7/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/ops.py` & `molgraph-0.6.7/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/chemistry/vis.py` & `molgraph-0.6.7/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/internal.py` & `molgraph-0.6.7/molgraph/internal.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/__init__.py` & `molgraph-0.6.7/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.6.7/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.6.7/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.6.7/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.6.7/molgraph/layers/attentional/gatv2_conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,27 +178,24 @@
             if not self.units or (self.units % self.num_heads != 0):
                 raise ValueError(
                     '`merge_mode` was set to `concat` and hence ' +
                     ' need `units` to be divisble by `num_heads`')
             self.units //= self.num_heads
 
         if self.use_edge_features:
-
-            self.edge_projection = self.get_einsum_dense(
-                'ij,jkh->ihk', (self.num_heads, self.units))
-
             if self.update_edge_features:
                 self.edge_out_projection = self.get_einsum_dense(
                     'ihj,jkh->ihk', (self.num_heads, self.units))
 
-        # Future implementation: Allow for non-shared weights?
-        # I.e., implement node_projection_dst and node_projection_src
-        self.node_projection = self.get_einsum_dense(
+        self.projection = self.get_einsum_dense(
             'ij,jkh->ihk', (self.num_heads, self.units))
 
+        self.node_projection = self.get_einsum_dense(
+            'ij,jkh->ihk', (self.num_heads, self.units))
+        
         if self.apply_self_projection:
             self.self_projection = self.get_einsum_dense(
                 'ij,jkh->ihk', (self.num_heads, self.units))
 
         self.attention_projection = self.get_einsum_dense(
             'ihj,jhk->ihk', (self.num_heads, 1))
 
@@ -208,35 +205,39 @@
     def _call(self, tensor: GraphTensor) -> GraphTensor:
 
         if self.apply_self_projection:
             node_feature_residual = self.self_projection(tensor.node_feature)
         else:
             node_feature_residual = None
 
+        # GAT v. GATv2: Concatenation before linear projection
+        if not self.use_edge_features:
+            attention_feature = tf.concat([
+                tf.gather(tensor.node_feature, tensor.edge_dst),
+                tf.gather(tensor.node_feature, tensor.edge_src)], axis=-1)
+        else:
+            attention_feature = tf.concat([
+                tf.gather(tensor.node_feature, tensor.edge_dst),
+                tf.gather(tensor.node_feature, tensor.edge_src),
+                tensor.edge_feature], axis=-1)
+        
         node_feature = self.node_projection(tensor.node_feature)
-        # Add dst and src node features, instead of concatenating them
-        attention_feature = (
-            tf.gather(node_feature, tensor.edge_dst) +
-            tf.gather(node_feature, tensor.edge_src)
-        )
-        if self.use_edge_features:
-            edge_feature = self.edge_projection(tensor.edge_feature)
-            # Similarily, add associated edge features, instead of concatenating them
-            attention_feature += edge_feature
 
+        attention_feature = self.projection(attention_feature)
+
+        if self.use_edge_features:
             if self.update_edge_features:
                 edge_feature = self.edge_out_projection(attention_feature)
                 edge_feature = gnn_ops.reduce_features(
                     feature=edge_feature,
                     mode=self.merge_mode,
                     output_units=self.units)
-
                 tensor = tensor.update({'edge_feature': edge_feature})
 
-        # Apply activation before attention projection
+        # GAT v. GATv2: Activation before linear projection
         edge_weights = self.attention_activation(attention_feature)
         edge_weights = self.attention_projection(edge_weights)
 
         tensor = tensor.update({
             'node_feature': node_feature, 'edge_weight': edge_weights})
         
         return tensor.propagate(
```

### Comparing `molgraph-0.6.6/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.6.7/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.6.7/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.6.7/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.6.7/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.6.7/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.6.7/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.6.7/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.6.7/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.6.7/molgraph/layers/geometric/radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/gnn_layer.py` & `molgraph-0.6.7/molgraph/layers/gnn_layer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/gnn_ops.py` & `molgraph-0.6.7/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.6.7/molgraph/layers/message_passing/edge_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.6.7/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.6.7/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.6.7/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.6.7/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.6.7/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.6.7/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.6.7/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.6.7/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/preprocessing/masking.py` & `molgraph-0.6.7/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.6.7/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/preprocessing/projection.py` & `molgraph-0.6.7/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.6.7/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.6.7/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/readout/node_readout.py` & `molgraph-0.6.7/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/readout/segment_pool.py` & `molgraph-0.6.7/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/readout/set_gather.py` & `molgraph-0.6.7/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.6.7/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/losses/link_losses.py` & `molgraph-0.6.7/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/losses/masked_losses.py` & `molgraph-0.6.7/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/metrics/masked_metrics.py` & `molgraph-0.6.7/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/metrics/mean_relative_error.py` & `molgraph-0.6.7/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/__init__.py` & `molgraph-0.6.7/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/dmpnn.py` & `molgraph-0.6.7/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/gin.py` & `molgraph-0.6.7/molgraph/models/gin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.6.7/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/interpretability/saliency.py` & `molgraph-0.6.7/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/mpnn.py` & `molgraph-0.6.7/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.6.7/molgraph/models/pretraining/autoencoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.6.7/molgraph/models/pretraining/masked_modeling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph/tensors/graph_tensor.py` & `molgraph-0.6.7/molgraph/tensors/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/molgraph.egg-info/PKG-INFO` & `molgraph-0.6.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: molgraph
-Version: 0.6.6
-Summary: Graph Neural Networks for Molecular Machine Learning
-Home-page: https://github.com/akensert/molgraph
-Author: Alexander Kensert
-Author-email: alexander.kensert@gmail.com
-License: MIT
-Keywords: machine-learning,deep-learning,graph-neural-networks,graphs,molecular-machine-learning,molecular-graphs,cheminformatics,chemometrics,bioinformatics,chemistry,biology,biochemistry
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-License-File: LICENSE
-
 # MolGraph
 
 **Graph Neural Networks** with **TensorFlow** and **Keras**. Focused on **Molecular Machine Learning**.
 
 <img src="https://github.com/akensert/molgraph/blob/main/media/molgraph.jpg" alt="molgraph" width="820">
 
 ## Highlights
@@ -87,32 +68,30 @@
     - And models for improved interpretability of GNNs:
         - **SaliencyMapping**
         - **IntegratedSaliencyMapping**
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Requirements/dependencies
-- **Python** (version ~= 3.10.0)
-    - **TensorFlow** (version ~= 2.15.0)
-    - **RDKit** (version ~= 2022.3.5)
-    - **Pandas** (version ~= 1.0.3)
-    - **IPython** (version ~= 8.12.0)
-
-> MolGraph should work with the more recent TensorFlow and RDKit versions. If not, try installing earlier versions of TensorFlow and RDKit.
+- **Python** (version >= 3.10)
+    - **TensorFlow** (version 2.15.*)
+    - **RDKit** (version 2023.9.*)
+    - **Pandas**
+    - **IPython**
 
 ## Installation
 
-For **GPU** users:
+For **CPU** users:
 <pre>
-pip install molgraph[gpu]
+pip install molgraph
 </pre>
 
-For **CPU** users:
+For **GPU** users:
 <pre>
-pip install molgraph
+pip install molgraph[gpu]
 </pre>
 
 Now run your first program with **MolGraph**:
 
 ```python
 from tensorflow import keras
 from molgraph import chemistry
@@ -141,14 +120,15 @@
 y_train = esol['train']['y']
 
 x_test = encoder(esol['test']['x'])
 y_test = esol['test']['y']
 
 # Build model via Keras API
 gnn_model = keras.Sequential([
+    keras.layers.Input(type_spec=x_train.spec),
     layers.GATConv(units=32, name='gat_conv_1'),
     layers.GATConv(units=32, name='gat_conv_2'),
     layers.Readout(),
     keras.layers.Dense(units=1024, activation='relu'),
     keras.layers.Dense(units=y_train.shape[-1])
 ])
```

### Comparing `molgraph-0.6.6/molgraph.egg-info/SOURCES.txt` & `molgraph-0.6.7/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.6.6/setup.py` & `molgraph-0.6.7/setup.py`

 * *Files identical despite different names*


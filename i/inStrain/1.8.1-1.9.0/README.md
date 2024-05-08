# Comparing `tmp/inStrain-1.8.1.tar.gz` & `tmp/inStrain-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inStrain-1.8.1.tar", last modified: Tue Apr 16 20:06:55 2024, max compression
+gzip compressed data, was "inStrain-1.9.0.tar", last modified: Wed May  8 15:42:44 2024, max compression
```

## Comparing `inStrain-1.8.1.tar` & `inStrain-1.9.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.628996 inStrain-1.8.1/
--rw-r--r--   0 mattolm    (501) staff       (20)    10244 2023-02-08 00:15:21.000000 inStrain-1.8.1/.DS_Store
--rw-r--r--   0 mattolm    (501) staff       (20)       74 2021-01-21 18:18:24.000000 inStrain-1.8.1/.gitignore
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.617672 inStrain-1.8.1/.vscode/
--rw-r--r--   0 mattolm    (501) staff       (20)       36 2022-10-22 22:33:02.000000 inStrain-1.8.1/.vscode/settings.json
--rw-r--r--   0 mattolm    (501) staff       (20)    26571 2024-04-12 21:02:12.000000 inStrain-1.8.1/CHANGELOG.md
--rw-r--r--   0 mattolm    (501) staff       (20)     1065 2021-03-26 22:19:41.000000 inStrain-1.8.1/LICENSE
--rw-r--r--   0 mattolm    (501) staff       (20)       76 2024-04-16 20:05:57.000000 inStrain-1.8.1/MANIFEST.in
--rw-r--r--   0 mattolm    (501) staff       (20)      572 2024-04-16 20:06:55.628631 inStrain-1.8.1/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.8.1/README.md
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.618006 inStrain-1.8.1/auxiliary_scripts/
--rwxr-xr-x   0 mattolm    (501) staff       (20)    13618 2023-08-24 21:29:51.000000 inStrain-1.8.1/auxiliary_scripts/rarefaction_curve.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5020 2023-02-25 01:32:59.000000 inStrain-1.8.1/auxiliary_scripts/recluster_instrain_compare.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.618167 inStrain-1.8.1/bin/
--rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.8.1/bin/inStrain
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.618310 inStrain-1.8.1/dist/
--rw-r--r--   0 mattolm    (501) staff       (20)    85716 2021-01-21 18:18:24.000000 inStrain-1.8.1/dist/inStrain-1.0.0.tar.gz
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.621378 inStrain-1.8.1/inStrain/
--rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.8.1/inStrain/GeneProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    42879 2024-04-12 21:01:13.000000 inStrain-1.8.1/inStrain/SNVprofile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)       22 2024-04-12 21:01:21.000000 inStrain-1.8.1/inStrain/_version.py
--rw-r--r--   0 mattolm    (501) staff       (20)    23404 2023-08-24 21:40:49.000000 inStrain-1.8.1/inStrain/argumentParser.py
--rw-r--r--   0 mattolm    (501) staff       (20)    25579 2023-07-26 21:10:33.000000 inStrain-1.8.1/inStrain/compare_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/compare_greedy.py
--rw-r--r--   0 mattolm    (501) staff       (20)     8480 2023-02-25 01:32:59.000000 inStrain-1.8.1/inStrain/compare_utils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    18260 2023-08-24 22:04:23.000000 inStrain-1.8.1/inStrain/controller.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.622961 inStrain-1.8.1/inStrain/deprecated/
--rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.8.1/inStrain/deprecated/DEPRECATEDmapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/deprecated/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/deprecated/deprecated_filter_reads.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/deprecated/deprecated_gene_statistics.py
--rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.8.1/inStrain/deprecated/plottingUtilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.8.1/inStrain/filter_reads.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34630 2023-08-24 21:18:50.000000 inStrain-1.8.1/inStrain/genomeUtilities.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.623144 inStrain-1.8.1/inStrain/helper_files/
--rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/helper_files/NullModel.txt
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.625562 inStrain-1.8.1/inStrain/helper_scripts/
--rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/helper_scripts/NullModel_1000000.txt
--rw-r--r--   0 mattolm    (501) staff       (20)  1072260 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/helper_scripts/NullModel_50000.txt
--rwxr-xr-x   0 mattolm    (501) staff       (20)     2711 2023-02-25 01:31:38.000000 inStrain-1.8.1/inStrain/helper_scripts/calculate_null.py
--rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/irep_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.8.1/inStrain/logUtils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15346 2023-05-16 21:08:22.000000 inStrain-1.8.1/inStrain/parse_annotations.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.626895 inStrain-1.8.1/inStrain/plotting/
--rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.8.1/inStrain/plotting/SNV_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/plotting/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.8.1/inStrain/plotting/compare_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/plotting/gene_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.8.1/inStrain/plotting/linkage_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9075 2023-02-25 00:47:19.000000 inStrain-1.8.1/inStrain/plotting/mapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.8.1/inStrain/plotting/plotting_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    18496 2023-07-26 21:15:53.000000 inStrain-1.8.1/inStrain/plotting/positional_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/plotting/utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    20770 2023-07-26 21:10:50.000000 inStrain-1.8.1/inStrain/polymorpher.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.627940 inStrain-1.8.1/inStrain/profile/
--rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/profile/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/profile/fasta.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/profile/linkage.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.8.1/inStrain/profile/profile_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    32898 2023-08-24 20:15:12.000000 inStrain-1.8.1/inStrain/profile/profile_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)     4682 2023-08-24 22:21:03.000000 inStrain-1.8.1/inStrain/profile/samtools_ops.py
--rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/profile/snv_utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.8.1/inStrain/quickProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.8.1/inStrain/readComparer.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2641 2023-08-24 20:54:04.000000 inStrain-1.8.1/inStrain/utils.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-04-16 20:06:55.628159 inStrain-1.8.1/inStrain.egg-info/
--rw-r--r--   0 mattolm    (501) staff       (20)      572 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1777 2024-04-16 20:06:55.000000 inStrain-1.8.1/inStrain.egg-info/SOURCES.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/dependency_links.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/not-zip-safe
--rw-r--r--   0 mattolm    (501) staff       (20)      113 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/requires.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       16 2024-04-16 20:06:54.000000 inStrain-1.8.1/inStrain.egg-info/top_level.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       38 2024-04-16 20:06:55.629055 inStrain-1.8.1/setup.cfg
--rw-r--r--   0 mattolm    (501) staff       (20)     1020 2024-04-16 20:04:18.000000 inStrain-1.8.1/setup.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.288856 inStrain-1.9.0/
+-rw-r--r--   0 mattolm    (501) staff       (20)    10244 2023-02-08 00:15:21.000000 inStrain-1.9.0/.DS_Store
+-rw-r--r--   0 mattolm    (501) staff       (20)       74 2021-01-21 18:18:24.000000 inStrain-1.9.0/.gitignore
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.257183 inStrain-1.9.0/.vscode/
+-rw-r--r--   0 mattolm    (501) staff       (20)       36 2022-10-22 22:33:02.000000 inStrain-1.9.0/.vscode/settings.json
+-rw-r--r--   0 mattolm    (501) staff       (20)    26761 2024-05-07 22:48:29.000000 inStrain-1.9.0/CHANGELOG.md
+-rw-r--r--   0 mattolm    (501) staff       (20)     1065 2021-03-26 22:19:41.000000 inStrain-1.9.0/LICENSE
+-rw-r--r--   0 mattolm    (501) staff       (20)       76 2024-05-07 22:48:26.000000 inStrain-1.9.0/MANIFEST.in
+-rw-r--r--   0 mattolm    (501) staff       (20)      572 2024-05-08 15:42:44.288503 inStrain-1.9.0/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.9.0/README.md
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.258060 inStrain-1.9.0/auxiliary_scripts/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    13618 2023-08-24 21:29:51.000000 inStrain-1.9.0/auxiliary_scripts/rarefaction_curve.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5020 2023-02-25 01:32:59.000000 inStrain-1.9.0/auxiliary_scripts/recluster_instrain_compare.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.258446 inStrain-1.9.0/bin/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.9.0/bin/inStrain
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.258718 inStrain-1.9.0/dist/
+-rw-r--r--   0 mattolm    (501) staff       (20)    85716 2021-01-21 18:18:24.000000 inStrain-1.9.0/dist/inStrain-1.0.0.tar.gz
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.269317 inStrain-1.9.0/inStrain/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.9.0/inStrain/GeneProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    42879 2024-04-12 21:01:13.000000 inStrain-1.9.0/inStrain/SNVprofile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)       22 2024-05-07 22:48:29.000000 inStrain-1.9.0/inStrain/_version.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    23404 2023-08-24 21:40:49.000000 inStrain-1.9.0/inStrain/argumentParser.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    26230 2024-05-07 22:48:29.000000 inStrain-1.9.0/inStrain/compare_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/compare_greedy.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     8915 2024-05-07 22:48:29.000000 inStrain-1.9.0/inStrain/compare_utils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    18260 2023-08-24 22:04:23.000000 inStrain-1.9.0/inStrain/controller.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.272263 inStrain-1.9.0/inStrain/deprecated/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.9.0/inStrain/deprecated/DEPRECATEDmapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/deprecated/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/deprecated/deprecated_filter_reads.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/deprecated/deprecated_gene_statistics.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.9.0/inStrain/deprecated/plottingUtilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.9.0/inStrain/filter_reads.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34630 2023-08-24 21:18:50.000000 inStrain-1.9.0/inStrain/genomeUtilities.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.275266 inStrain-1.9.0/inStrain/helper_files/
+-rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/helper_files/NullModel.txt
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.280638 inStrain-1.9.0/inStrain/helper_scripts/
+-rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/helper_scripts/NullModel_1000000.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)  1072260 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/helper_scripts/NullModel_50000.txt
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     2711 2023-02-25 01:31:38.000000 inStrain-1.9.0/inStrain/helper_scripts/calculate_null.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/irep_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.9.0/inStrain/logUtils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15346 2023-05-16 21:08:22.000000 inStrain-1.9.0/inStrain/parse_annotations.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.283829 inStrain-1.9.0/inStrain/plotting/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.9.0/inStrain/plotting/SNV_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/plotting/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.9.0/inStrain/plotting/compare_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/plotting/gene_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.9.0/inStrain/plotting/linkage_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9063 2024-05-07 22:48:29.000000 inStrain-1.9.0/inStrain/plotting/mapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.9.0/inStrain/plotting/plotting_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    18643 2024-05-07 22:48:29.000000 inStrain-1.9.0/inStrain/plotting/positional_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/plotting/utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    20770 2023-07-26 21:10:50.000000 inStrain-1.9.0/inStrain/polymorpher.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.287535 inStrain-1.9.0/inStrain/profile/
+-rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/profile/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/profile/fasta.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/profile/linkage.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.9.0/inStrain/profile/profile_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    32898 2023-08-24 20:15:12.000000 inStrain-1.9.0/inStrain/profile/profile_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     4682 2023-08-24 22:21:03.000000 inStrain-1.9.0/inStrain/profile/samtools_ops.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/profile/snv_utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.9.0/inStrain/quickProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.9.0/inStrain/readComparer.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2641 2023-08-24 20:54:04.000000 inStrain-1.9.0/inStrain/utils.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2024-05-08 15:42:44.288061 inStrain-1.9.0/inStrain.egg-info/
+-rw-r--r--   0 mattolm    (501) staff       (20)      572 2024-05-08 15:42:42.000000 inStrain-1.9.0/inStrain.egg-info/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1777 2024-05-08 15:42:44.000000 inStrain-1.9.0/inStrain.egg-info/SOURCES.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2024-05-08 15:42:42.000000 inStrain-1.9.0/inStrain.egg-info/dependency_links.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2024-04-16 20:06:54.000000 inStrain-1.9.0/inStrain.egg-info/not-zip-safe
+-rw-r--r--   0 mattolm    (501) staff       (20)      113 2024-05-08 15:42:42.000000 inStrain-1.9.0/inStrain.egg-info/requires.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       16 2024-05-08 15:42:42.000000 inStrain-1.9.0/inStrain.egg-info/top_level.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       38 2024-05-08 15:42:44.288920 inStrain-1.9.0/setup.cfg
+-rw-r--r--   0 mattolm    (501) staff       (20)     1020 2024-05-07 22:48:26.000000 inStrain-1.9.0/setup.py
```

### Comparing `inStrain-1.8.1/.DS_Store` & `inStrain-1.9.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/CHANGELOG.md` & `inStrain-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project (attempts to) adhere to [Semantic Versioning](http://semver.org/).
 
+## [1.9.0] - 2024-05-07
+- Updates from Jing Wang pull request #181 https://github.com/MrOlm/inStrain/pull/181
+- Efficiency improvements for inStrain compare and Error message clarification
+
 ## [1.8.1] - 2024-04-12
 - Minor update to _get_covt_keys method
 
 ## [1.8.0] - 2023-08-24
 - If you don't have any genomes detected, crash more gracefully
 - Make it so all the genome_info columns are the same whether or not you have a linkage table
 - Add "maximum_reads" argument
```

### Comparing `inStrain-1.8.1/LICENSE` & `inStrain-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/PKG-INFO` & `inStrain-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inStrain
-Version: 1.8.1
+Version: 1.9.0
 Summary: Calculation of strain-level metrics
 Home-page: https://github.com/MrOlm/inStrain
 Author: Matt Olm and Alex Crits-Christoph
 Author-email: mattolm@berkeley.edu
 License: MIT
 Requires-Python: >=3.4.0
 License-File: LICENSE
```

### Comparing `inStrain-1.8.1/README.md` & `inStrain-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/auxiliary_scripts/rarefaction_curve.py` & `inStrain-1.9.0/auxiliary_scripts/rarefaction_curve.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/auxiliary_scripts/recluster_instrain_compare.py` & `inStrain-1.9.0/auxiliary_scripts/recluster_instrain_compare.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/bin/inStrain` & `inStrain-1.9.0/bin/inStrain`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/dist/inStrain-1.0.0.tar.gz` & `inStrain-1.9.0/dist/inStrain-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/GeneProfile.py` & `inStrain-1.9.0/inStrain/GeneProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/SNVprofile.py` & `inStrain-1.9.0/inStrain/SNVprofile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/argumentParser.py` & `inStrain-1.9.0/inStrain/argumentParser.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/compare_controller.py` & `inStrain-1.9.0/inStrain/compare_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging
 import pandas as pd
 from tqdm import tqdm
 import multiprocessing
 import traceback
 from collections import defaultdict
 from tqdm import tqdm
+import time
 
 import inStrain.readComparer
 import inStrain.compare_utils
 import inStrain.genomeUtilities
 import inStrain.controller
 import inStrain.profile
 import inStrain.profile.samtools_ops
@@ -526,46 +527,59 @@
 
         # Make sure no duplicates in names
         assert len(names) == len(set(names)), 'Cannot have 2 of the same named IS {0}'.format(names)
 
         # Load data from the profiles
         name2covT = {}
         name2SNPtable = {}
+        name2SNPtable_hash = {}
         name2Rdic = {}
 
         for S, name in zip(sProfiles, names):
+            logging.debug('Loading %s', name)
+            start = time.time()
             if not for_pooling:
                 name2covT[name] = S.get('covT', scaffolds=scaffolds_to_compare)
+            logging.debug('covT %f', time.time() - start)
+            start = time.time()
             name2SNPtable[name] = S.get('cumulative_snv_table').rename(
                 columns={'conBase': 'con_base', 'refBase': 'ref_base', 'varBase': 'var_base',
                          'baseCoverage': 'position_coverage'})
+            print(name)
+            name2SNPtable_hash[name] = inStrain.compare_utils.hash_SNP_table(name2SNPtable[name])
+            logging.debug('cumulative_snv_table %f', time.time() - start)
             if for_pooling:
+                start = time.time()
                 name2Rdic[name] = S.get("Rdic")
+                logging.debug('Rdic %f', time.time() - start)
 
         if for_pooling:
             self.name2SNPtable = name2SNPtable
             self.name2Rdic = name2Rdic
 
         if not for_pooling:
             # Attach this information to ScaffoldComparison objects
             for SC in self.ScaffoldComparisons:
                 for name in SC.names:
-                    SC.SNPtables.append(inStrain.compare_utils.subset_SNP_table(name2SNPtable[name], SC.scaffold))
+                    # SC.SNPtables.append(inStrain.compare_utils.subset_SNP_table(name2SNPtable[name], SC.scaffold))
+                    SC.SNPtables.append(name2SNPtable_hash[name].get(SC.scaffold, pd.DataFrame()))
                     SC.covTs.append(name2covT[name][SC.scaffold])
 
                     if for_pooling:
                         SC.name2Rdic = {n:r[SC.scaffold] for n, r in name2Rdic.items()}
 
             # Set up a command and result queue
             ctx = multiprocessing.get_context('spawn')
             self.cmd_queue = ctx.Queue()
             self.result_queue = ctx.Queue()
             for SC in self.ScaffoldComparisons:
                 self.cmd_queue.put(SC)
 
+        logging.debug('Load cache done.')
+
     def purge_cache(self):
         """
         Purge information from ISPs from RAM
         """
         for SC in self.ScaffoldComparisons:
             del SC.SNPtables
             del SC.covTs
@@ -674,8 +688,8 @@
         if len(bams) == len(inputs):
             for profile_loc, bam in zip(inputs, bams):
                 ISP = inStrain.SNVprofile.SNVprofile(profile_loc)
                 name = os.path.basename(ISP.get('bam_loc'))
 
                 name2bam[name] = inStrain.profile.samtools_ops.prepare_bam_fie(bam, processes)
 
-    return name2bam
+    return name2bam
```

### Comparing `inStrain-1.8.1/inStrain/compare_greedy.py` & `inStrain-1.9.0/inStrain/compare_greedy.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/compare_utils.py` & `inStrain-1.9.0/inStrain/compare_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,32 @@
             db = db.sort_values('mm')
             #db = db[['position', 'mm', 'con_base', 'ref_base', 'var_base', 'position_coverage', 'A', 'C', 'T', 'G', 'allele_count']]
     else:
         db = pd.DataFrame()
 
     return db
 
+
+def hash_SNP_table(db):
+    """
+    Split SNP table according to scaffold
+    """
+    if len(db) == 0:
+        return {}
+
+    db = db.sort_values(['scaffold', 'mm'])
+    ukeys, index = np.unique(db['scaffold'], True)
+    index = np.append(index, len(db))  # add the index of the last row in db
+    dbhash = {}
+    for key, idx1, idx2 in zip(ukeys, index[:-1], index[1:]):
+        dbhash[key] = db.iloc[idx1:idx2]
+
+    return dbhash
+
+
 def find_relevant_scaffolds(input, bts, kwargs):
     """
     Return a list of scaffolds in the input based on the parameters of kwargs
     """
     GIdb = inStrain.SNVprofile.SNVprofile(input).get('genome_level_info')
     if GIdb is None:
         logging.error(f"Profile {input} does not have genome-level information; needed to run compare in database mode")
```

### Comparing `inStrain-1.8.1/inStrain/controller.py` & `inStrain-1.9.0/inStrain/controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/deprecated/DEPRECATEDmapping_plots.py` & `inStrain-1.9.0/inStrain/deprecated/DEPRECATEDmapping_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/deprecated/__init__.py` & `inStrain-1.9.0/inStrain/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/deprecated/deprecated_filter_reads.py` & `inStrain-1.9.0/inStrain/deprecated/deprecated_filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/deprecated/deprecated_gene_statistics.py` & `inStrain-1.9.0/inStrain/deprecated/deprecated_gene_statistics.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/deprecated/plottingUtilities.py` & `inStrain-1.9.0/inStrain/deprecated/plottingUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/filter_reads.py` & `inStrain-1.9.0/inStrain/filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/genomeUtilities.py` & `inStrain-1.9.0/inStrain/genomeUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/helper_files/NullModel.txt` & `inStrain-1.9.0/inStrain/helper_files/NullModel.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/helper_scripts/NullModel_1000000.txt` & `inStrain-1.9.0/inStrain/helper_scripts/NullModel_1000000.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/helper_scripts/NullModel_50000.txt` & `inStrain-1.9.0/inStrain/helper_scripts/NullModel_50000.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/helper_scripts/calculate_null.py` & `inStrain-1.9.0/inStrain/helper_scripts/calculate_null.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/irep_utilities.py` & `inStrain-1.9.0/inStrain/irep_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/logUtils.py` & `inStrain-1.9.0/inStrain/logUtils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/parse_annotations.py` & `inStrain-1.9.0/inStrain/parse_annotations.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/plotting/SNV_plots.py` & `inStrain-1.9.0/inStrain/plotting/SNV_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/plotting/__init__.py` & `inStrain-1.9.0/inStrain/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/plotting/compare_plots.py` & `inStrain-1.9.0/inStrain/plotting/compare_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/plotting/gene_plots.py` & `inStrain-1.9.0/inStrain/plotting/gene_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/plotting/linkage_plots.py` & `inStrain-1.9.0/inStrain/plotting/linkage_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/plotting/mapping_plots.py` & `inStrain-1.9.0/inStrain/plotting/mapping_plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         # Add the number of read-pairs
         readLen = int(IS.get_read_length())
         Mdb['read_length'] = readLen
         Mdb['mm'] = Mdb['mm'].astype(int)
         Mdb.loc[:, 'ANI_level'] = [(readLen - mm) / readLen for mm in Mdb['mm']]
     except:
         logging.error(
-            "Skipping plot 1 - you don't have all required information. You need to run inStrain genome_wide first")
+            "Skipping plot 1 - Plot 1 cannot be created when run with --database_mode or --skip_mm_profiling")
         if kwargs.get('debug', False):
             traceback.print_exc()
         return
 
     # Make the plot
     logging.info("Plotting plot 1")
     name = 'CoverageAndBreadth_vs_readMismatch.pdf'
@@ -104,15 +104,15 @@
     try:
         Mdb = prepare_read_ani_dist_plot(IS)
         if len(Mdb['ANI_level'].unique()) == 1:
             raise Exception('Plot 3 cannot be created when run with --database_mode or --skip_mm_profiling')
         assert len(Mdb) > 0
     except:
         logging.error(
-            "Skipping plot 3 - you don't have all required information. You need to run inStrain genome_wide first")
+            "Skipping plot 3 - Plot 3 cannot be created when run with --database_mode or --skip_mm_profiling")
         if kwargs.get('debug', False):
             traceback.print_exc()
         return
 
     # Make the plot
     logging.info("Plotting plot 3")
     name = 'readANI_distribution.pdf'
```

### Comparing `inStrain-1.8.1/inStrain/plotting/plotting_controller.py` & `inStrain-1.9.0/inStrain/plotting/plotting_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/plotting/positional_plots.py` & `inStrain-1.9.0/inStrain/plotting/positional_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,35 +28,38 @@
 
         b2s = defaultdict(list)
         for s, b in stb.items():
             b2s[b].append(s)
         assert len(b2s.keys()) > 0
 
         # Load the cache
+        logging.debug('Loading cache')
         covTs = kwargs.get('covT')#, IS.get('covT'))
         clonTs = kwargs.get('clonT')#, IS.get('clonT'))
         raw_linkage_table = kwargs.get('raw_linkage_table')#, IS.get('raw_linkage_table'))
         cumulative_snv_table = kwargs.get('cumulative_snv_table')#, IS.get('cumulative_snv_table'))
         scaffold2length = IS.get('scaffold2length')
         rl = IS.get_read_length()
         profiled_scaffolds = set(scaffold2length.keys())
+        logging.debug('Loading cache finished')
 
     except:
         logging.error("Skipping plot 2 - you don't have all required information. You need to run inStrain genome_wide first")
         if kwargs.get('debug', False):
             traceback.print_exc()
         return
 
     # Make the plot
     logging.info("Plotting plot 2")
     name = 'genomeWide_microdiveristy_metrics.pdf'
     pp = PdfPages(plot_dir + name)
 
 
     for genome, scaffolds in b2s.items():
+        logging.debug('Plotting %s %s', genome, scaffolds)
         if not plot_genome(genome, IS, **kwargs):
             continue
         present_scaffolds = list(set(scaffolds).intersection(set(profiled_scaffolds)))
         Wdb, breaks, midpoints = load_windowed_metrics(present_scaffolds,
                                 scaffold2length,
                                 rl,
                                 report_midpoints=True,
@@ -559,8 +562,8 @@
 
     plt.suptitle(title, y=0.999)
     plt.subplots_adjust(hspace=0.3)
     #plt.gca().xaxis.grid(False)
 
     fig = plt.gcf()
     ylim = inStrain.plotting.utilities._calc_ylim(Wdb['midpoint'].max())
-    fig.set_size_inches(8, ylim)
+    fig.set_size_inches(8, ylim)
```

### Comparing `inStrain-1.8.1/inStrain/plotting/utilities.py` & `inStrain-1.9.0/inStrain/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/polymorpher.py` & `inStrain-1.9.0/inStrain/polymorpher.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/profile/__init__.py` & `inStrain-1.9.0/inStrain/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/profile/fasta.py` & `inStrain-1.9.0/inStrain/profile/fasta.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/profile/linkage.py` & `inStrain-1.9.0/inStrain/profile/linkage.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/profile/profile_controller.py` & `inStrain-1.9.0/inStrain/profile/profile_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/profile/profile_utilities.py` & `inStrain-1.9.0/inStrain/profile/profile_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/profile/samtools_ops.py` & `inStrain-1.9.0/inStrain/profile/samtools_ops.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/profile/snv_utilities.py` & `inStrain-1.9.0/inStrain/profile/snv_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/quickProfile.py` & `inStrain-1.9.0/inStrain/quickProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/readComparer.py` & `inStrain-1.9.0/inStrain/readComparer.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain/utils.py` & `inStrain-1.9.0/inStrain/utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/inStrain.egg-info/PKG-INFO` & `inStrain-1.9.0/inStrain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inStrain
-Version: 1.8.1
+Version: 1.9.0
 Summary: Calculation of strain-level metrics
 Home-page: https://github.com/MrOlm/inStrain
 Author: Matt Olm and Alex Crits-Christoph
 Author-email: mattolm@berkeley.edu
 License: MIT
 Requires-Python: >=3.4.0
 License-File: LICENSE
```

### Comparing `inStrain-1.8.1/inStrain.egg-info/SOURCES.txt` & `inStrain-1.9.0/inStrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.8.1/setup.py` & `inStrain-1.9.0/setup.py`

 * *Files identical despite different names*


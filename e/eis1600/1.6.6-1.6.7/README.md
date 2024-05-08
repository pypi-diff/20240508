# Comparing `tmp/eis1600-1.6.6.tar.gz` & `tmp/eis1600-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-1.6.6.tar", last modified: Mon May  6 17:54:35 2024, max compression
+gzip compressed data, was "eis1600-1.6.7.tar", last modified: Wed May  8 13:57:17 2024, max compression
```

## Comparing `eis1600-1.6.6.tar` & `eis1600-1.6.7.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.701455 eis1600-1.6.6/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1046 2023-08-12 14:27:20.000000 eis1600-1.6.6/LICENSE
--rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-05-06 17:54:35.701455 eis1600-1.6.6/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    13595 2024-03-16 19:46:15.000000 eis1600-1.6.6/README.md
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.685455 eis1600-1.6.6/eis1600/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.685455 eis1600-1.6.6/eis1600/bio/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/bio/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7450 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/bio/md_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3998 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/bio/q_tags_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3108 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/bio/topo_tags_to_bio.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.685455 eis1600-1.6.6/eis1600/corpus_analysis/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-06 14:14:46.000000 eis1600-1.6.6/eis1600/corpus_analysis/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6052 2024-05-05 09:03:01.000000 eis1600-1.6.6/eis1600/corpus_analysis/analyse_all_on_cluster.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1732 2024-03-22 08:47:34.000000 eis1600-1.6.6/eis1600/corpus_analysis/analyse_text.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5156 2024-04-04 09:50:23.000000 eis1600-1.6.6/eis1600/corpus_analysis/miu_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3335 2024-03-27 16:36:35.000000 eis1600-1.6.6/eis1600/corpus_analysis/text_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.685455 eis1600-1.6.6/eis1600/dates/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      911 2023-11-02 15:25:23.000000 eis1600-1.6.6/eis1600/dates/Date.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      755 2024-02-12 17:00:08.000000 eis1600-1.6.6/eis1600/dates/Month.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/dates/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6571 2024-02-12 17:08:43.000000 eis1600-1.6.6/eis1600/dates/date_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7397 2024-03-21 17:57:44.000000 eis1600-1.6.6/eis1600/dates/date_patterns.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2237 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/dates/month_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/gazetteers/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4411 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1267 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/gazetteers/Spellings.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3553 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/gazetteers/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.6.6/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      536 2023-07-19 09:36:14.000000 eis1600-1.6.6/eis1600/gazetteers/data/days_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      587 2023-07-19 09:36:14.000000 eis1600-1.6.6/eis1600/gazetteers/data/months_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    96536 2023-04-17 09:44:13.000000 eis1600-1.6.6/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1448 2023-10-25 09:16:34.000000 eis1600-1.6.6/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)   339886 2023-11-06 12:34:27.000000 eis1600-1.6.6/eis1600/gazetteers/data/toponyms_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2604 2023-07-19 09:36:14.000000 eis1600-1.6.6/eis1600/gazetteers/data/years_gazetteer.csv
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/helper/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3429 2024-03-22 08:56:31.000000 eis1600-1.6.6/eis1600/helper/CheckFileEndingActions.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      186 2023-11-10 14:22:15.000000 eis1600-1.6.6/eis1600/helper/Singleton.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/helper/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1212 2024-02-19 13:06:34.000000 eis1600-1.6.6/eis1600/helper/ar_normalization.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3934 2024-03-27 11:22:04.000000 eis1600-1.6.6/eis1600/helper/chunking.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/helper/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.6/eis1600/helper/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1356 2024-03-18 17:41:21.000000 eis1600-1.6.6/eis1600/helper/files_sizes.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2027 2024-04-04 11:02:16.000000 eis1600-1.6.6/eis1600/helper/fix_dataframe.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      994 2024-03-16 19:46:15.000000 eis1600-1.6.6/eis1600/helper/logging.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6461 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      370 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/helper/parse_range.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      306 2024-03-21 11:13:13.000000 eis1600-1.6.6/eis1600/helper/part_file_names.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/json_to_text/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:40:12.000000 eis1600-1.6.6/eis1600/json_to_text/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4106 2024-04-24 08:16:19.000000 eis1600-1.6.6/eis1600/json_to_text/reconstruct.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/json_to_tsv/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:34:00.000000 eis1600-1.6.6/eis1600/json_to_tsv/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5013 2024-04-04 15:35:16.000000 eis1600-1.6.6/eis1600/json_to_tsv/corpus_dump.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/markdown/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      988 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/markdown/EntityTags.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/markdown/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1606 2024-04-03 11:51:57.000000 eis1600-1.6.6/eis1600/markdown/category.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/markdown/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/markdown/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-02-12 17:00:08.000000 eis1600-1.6.6/eis1600/markdown/data/entity_tags.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      851 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/markdown/markdown_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6628 2024-04-03 09:08:42.000000 eis1600-1.6.6/eis1600/markdown/markdown_patterns.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/miu/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3513 2024-02-13 09:24:54.000000 eis1600-1.6.6/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/miu/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.689455 eis1600-1.6.6/eis1600/model_evaluations/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      393 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/model_evaluations/EvalResultsEncoder.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/model_evaluations/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7701 2024-02-12 17:00:08.000000 eis1600-1.6.6/eis1600/model_evaluations/eval_date_model.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4800 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/model_evaluations/eval_topo_cat_model.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.693455 eis1600-1.6.6/eis1600/models/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      671 2024-02-05 08:54:18.000000 eis1600-1.6.6/eis1600/models/BiosPunctuationModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      566 2024-02-13 10:55:51.000000 eis1600-1.6.6/eis1600/models/Disambiguator.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      660 2024-02-12 17:00:08.000000 eis1600-1.6.6/eis1600/models/EventsPunctuationModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      259 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/models/FamilyContactOpinionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      592 2024-02-13 10:55:51.000000 eis1600-1.6.6/eis1600/models/Lemmatizer.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1762 2024-02-05 08:54:18.000000 eis1600-1.6.6/eis1600/models/Model.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      237 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/models/NERModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      250 2024-02-01 10:44:02.000000 eis1600-1.6.6/eis1600/models/NasabDetectionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      257 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/models/OnomsticElementsModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      582 2024-02-13 10:55:51.000000 eis1600-1.6.6/eis1600/models/POSTagger.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1154 2024-02-16 15:42:32.000000 eis1600-1.6.6/eis1600/models/PoetryDetectionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      258 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/models/StudentTeacherModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      261 2023-11-20 09:22:09.000000 eis1600-1.6.6/eis1600/models/ToponymDescriptionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      246 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/models/ToponymModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-20 09:22:09.000000 eis1600-1.6.6/eis1600/models/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.693455 eis1600-1.6.6/eis1600/nlp/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/nlp/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4464 2024-04-11 12:45:39.000000 eis1600-1.6.6/eis1600/nlp/annotation_utils.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1604 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/nlp/utils.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.693455 eis1600-1.6.6/eis1600/onomastics/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/onomastics/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1364 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/onomastics/initial_annotation.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    10640 2024-04-03 11:14:52.000000 eis1600-1.6.6/eis1600/onomastics/methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1968 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.693455 eis1600-1.6.6/eis1600/paragraphs/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/paragraphs/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     9974 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/paragraphs/paragraph_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2163 2024-02-16 15:42:32.000000 eis1600-1.6.6/eis1600/paragraphs/split_mius_into_paragraphs.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.693455 eis1600-1.6.6/eis1600/processing/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/processing/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.693455 eis1600-1.6.6/eis1600/processing/persistent_ids/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-05-03 11:21:09.000000 eis1600-1.6.6/eis1600/processing/persistent_ids/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-05-03 11:16:17.000000 eis1600-1.6.6/eis1600/processing/persistent_ids/deprecated_long_short_ids_mapping.json
--rw-rw-r--   0 alicia    (1000) alicia    (1000)  2154089 2024-05-05 09:11:54.000000 eis1600-1.6.6/eis1600/processing/persistent_ids/long_short_ids_mapping.json
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5802 2024-04-25 14:11:19.000000 eis1600-1.6.6/eis1600/processing/postprocessing.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6230 2024-02-12 17:00:08.000000 eis1600-1.6.6/eis1600/processing/preprocessing.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3008 2024-05-03 11:16:17.000000 eis1600-1.6.6/eis1600/processing/short_miu_generation.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.693455 eis1600-1.6.6/eis1600/repositories/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/repositories/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    16545 2024-04-04 08:50:01.000000 eis1600-1.6.6/eis1600/repositories/repo.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.697455 eis1600-1.6.6/eis1600/statistics/
--rw-r--r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/statistics/__init__.py
--rw-r--r--   0 alicia    (1000) alicia    (1000)     2786 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/statistics/count_categories.py
--rw-r--r--   0 alicia    (1000) alicia    (1000)     3548 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/statistics/count_tokens_per_miu.py
--rw-r--r--   0 alicia    (1000) alicia    (1000)      958 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/statistics/methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.697455 eis1600-1.6.6/eis1600/texts_to_mius/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      431 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/texts_to_mius/SubIDs.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1820 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/texts_to_mius/UIDs.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/texts_to_mius/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1939 2024-03-16 19:46:15.000000 eis1600-1.6.6/eis1600/texts_to_mius/check_formatting.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7572 2024-04-03 09:09:16.000000 eis1600-1.6.6/eis1600/texts_to_mius/check_formatting_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3696 2024-03-16 19:46:15.000000 eis1600-1.6.6/eis1600/texts_to_mius/check_mius.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3742 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/texts_to_mius/convert_mARkdown_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4179 2024-02-05 08:54:18.000000 eis1600-1.6.6/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1562 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/texts_to_mius/download_text_selection_sheet.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3312 2024-03-16 19:46:15.000000 eis1600-1.6.6/eis1600/texts_to_mius/ids_insert_or_update.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1463 2024-03-01 13:50:55.000000 eis1600-1.6.6/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    14062 2024-04-03 11:49:39.000000 eis1600-1.6.6/eis1600/texts_to_mius/subid_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.697455 eis1600-1.6.6/eis1600/toponym_descriptions/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/toponym_descriptions/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-03-01 13:31:17.000000 eis1600-1.6.6/eis1600/toponym_descriptions/annotate_topd.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2783 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/toponym_descriptions/btopd_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4944 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/toponym_descriptions/topod_extract_incomplete.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4151 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/toponym_descriptions/topod_extract_places_regex.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3709 2024-02-16 15:42:32.000000 eis1600-1.6.6/eis1600/toponym_descriptions/topod_insert_into_miu.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1710 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/toponym_descriptions/topod_sheets_stats.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.697455 eis1600-1.6.6/eis1600/toponyms/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.6/eis1600/toponyms/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1975 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/toponyms/initial_category_annotation.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3199 2023-11-02 14:43:12.000000 eis1600-1.6.6/eis1600/toponyms/methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1659 2023-11-02 14:43:12.000000 eis1600-1.6.6/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.697455 eis1600-1.6.6/eis1600/training_data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/training_data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1535 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/training_data/annotate_onomastics.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1098 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/training_data/online_editor_files.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4121 2024-01-30 08:39:34.000000 eis1600-1.6.6/eis1600/training_data/reannotation.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.697455 eis1600-1.6.6/eis1600/yml/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     9610 2024-04-03 15:04:40.000000 eis1600-1.6.6/eis1600/yml/YAMLHandler.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/yml/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    12820 2024-04-09 11:27:31.000000 eis1600-1.6.6/eis1600/yml/yml_handling.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-01-18 10:18:32.000000 eis1600-1.6.6/eis1600/yml/yml_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-06 17:54:35.697455 eis1600-1.6.6/eis1600.egg-info/
--rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-05-06 17:54:35.000000 eis1600-1.6.6/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4823 2024-05-06 17:54:35.000000 eis1600-1.6.6/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2024-05-06 17:54:35.000000 eis1600-1.6.6/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1851 2024-05-06 17:54:35.000000 eis1600-1.6.6/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      201 2024-05-06 17:54:35.000000 eis1600-1.6.6/eis1600.egg-info/requires.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        8 2024-05-06 17:54:35.000000 eis1600-1.6.6/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2024-05-06 17:54:35.701455 eis1600-1.6.6/setup.cfg
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4214 2024-05-06 17:54:08.000000 eis1600-1.6.6/setup.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1046 2023-08-12 14:27:20.000000 eis1600-1.6.7/LICENSE
+-rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-05-08 13:57:17.692732 eis1600-1.6.7/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    13595 2024-03-16 19:46:15.000000 eis1600-1.6.7/README.md
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/bio/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/bio/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7450 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/bio/md_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3998 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/bio/q_tags_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3108 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/bio/topo_tags_to_bio.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/corpus_analysis/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-06 14:14:46.000000 eis1600-1.6.7/eis1600/corpus_analysis/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6157 2024-05-08 13:03:10.000000 eis1600-1.6.7/eis1600/corpus_analysis/analyse_all_on_cluster.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1732 2024-03-22 08:47:34.000000 eis1600-1.6.7/eis1600/corpus_analysis/analyse_text.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5156 2024-04-04 09:50:23.000000 eis1600-1.6.7/eis1600/corpus_analysis/miu_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3335 2024-03-27 16:36:35.000000 eis1600-1.6.7/eis1600/corpus_analysis/text_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/dates/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      911 2023-11-02 15:25:23.000000 eis1600-1.6.7/eis1600/dates/Date.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      755 2024-02-12 17:00:08.000000 eis1600-1.6.7/eis1600/dates/Month.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/dates/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6571 2024-02-12 17:08:43.000000 eis1600-1.6.7/eis1600/dates/date_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7397 2024-03-21 17:57:44.000000 eis1600-1.6.7/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2237 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/dates/month_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/gazetteers/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4411 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1267 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/gazetteers/Spellings.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3553 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/gazetteers/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.6.7/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      536 2023-07-19 09:36:14.000000 eis1600-1.6.7/eis1600/gazetteers/data/days_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      587 2023-07-19 09:36:14.000000 eis1600-1.6.7/eis1600/gazetteers/data/months_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    96536 2023-04-17 09:44:13.000000 eis1600-1.6.7/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1448 2023-10-25 09:16:34.000000 eis1600-1.6.7/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)   339886 2023-11-06 12:34:27.000000 eis1600-1.6.7/eis1600/gazetteers/data/toponyms_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2604 2023-07-19 09:36:14.000000 eis1600-1.6.7/eis1600/gazetteers/data/years_gazetteer.csv
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/helper/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3577 2024-05-08 13:35:28.000000 eis1600-1.6.7/eis1600/helper/CheckFileEndingActions.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      186 2023-11-10 14:22:15.000000 eis1600-1.6.7/eis1600/helper/Singleton.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/helper/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1212 2024-02-19 13:06:34.000000 eis1600-1.6.7/eis1600/helper/ar_normalization.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3934 2024-03-27 11:22:04.000000 eis1600-1.6.7/eis1600/helper/chunking.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/helper/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.7/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1356 2024-03-18 17:41:21.000000 eis1600-1.6.7/eis1600/helper/files_sizes.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2027 2024-04-04 11:02:16.000000 eis1600-1.6.7/eis1600/helper/fix_dataframe.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      994 2024-03-16 19:46:15.000000 eis1600-1.6.7/eis1600/helper/logging.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6461 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      370 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/helper/parse_range.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      306 2024-03-21 11:13:13.000000 eis1600-1.6.7/eis1600/helper/part_file_names.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/json_to_text/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:40:12.000000 eis1600-1.6.7/eis1600/json_to_text/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4160 2024-05-08 13:04:28.000000 eis1600-1.6.7/eis1600/json_to_text/reconstruct.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/json_to_tsv/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:34:00.000000 eis1600-1.6.7/eis1600/json_to_tsv/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5341 2024-05-08 13:02:06.000000 eis1600-1.6.7/eis1600/json_to_tsv/corpus_dump.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/markdown/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      988 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/markdown/EntityTags.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/markdown/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1606 2024-04-03 11:51:57.000000 eis1600-1.6.7/eis1600/markdown/category.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/markdown/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/markdown/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-02-12 17:00:08.000000 eis1600-1.6.7/eis1600/markdown/data/entity_tags.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      851 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/markdown/markdown_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6628 2024-04-03 09:08:42.000000 eis1600-1.6.7/eis1600/markdown/markdown_patterns.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/miu/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3513 2024-02-13 09:24:54.000000 eis1600-1.6.7/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/miu/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.688732 eis1600-1.6.7/eis1600/model_evaluations/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      393 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/model_evaluations/EvalResultsEncoder.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/model_evaluations/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7701 2024-02-12 17:00:08.000000 eis1600-1.6.7/eis1600/model_evaluations/eval_date_model.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4800 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/model_evaluations/eval_topo_cat_model.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/models/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      671 2024-02-05 08:54:18.000000 eis1600-1.6.7/eis1600/models/BiosPunctuationModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      566 2024-02-13 10:55:51.000000 eis1600-1.6.7/eis1600/models/Disambiguator.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      660 2024-02-12 17:00:08.000000 eis1600-1.6.7/eis1600/models/EventsPunctuationModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      259 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/models/FamilyContactOpinionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      592 2024-02-13 10:55:51.000000 eis1600-1.6.7/eis1600/models/Lemmatizer.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1762 2024-02-05 08:54:18.000000 eis1600-1.6.7/eis1600/models/Model.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      237 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/models/NERModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      250 2024-02-01 10:44:02.000000 eis1600-1.6.7/eis1600/models/NasabDetectionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      257 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/models/OnomsticElementsModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      582 2024-02-13 10:55:51.000000 eis1600-1.6.7/eis1600/models/POSTagger.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1154 2024-02-16 15:42:32.000000 eis1600-1.6.7/eis1600/models/PoetryDetectionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      258 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/models/StudentTeacherModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      261 2023-11-20 09:22:09.000000 eis1600-1.6.7/eis1600/models/ToponymDescriptionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      246 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/models/ToponymModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-20 09:22:09.000000 eis1600-1.6.7/eis1600/models/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/nlp/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/nlp/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4464 2024-04-11 12:45:39.000000 eis1600-1.6.7/eis1600/nlp/annotation_utils.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1604 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/nlp/utils.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/onomastics/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1364 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/onomastics/initial_annotation.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    10640 2024-04-03 11:14:52.000000 eis1600-1.6.7/eis1600/onomastics/methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1968 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/paragraphs/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/paragraphs/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     9974 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/paragraphs/paragraph_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2163 2024-02-16 15:42:32.000000 eis1600-1.6.7/eis1600/paragraphs/split_mius_into_paragraphs.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/processing/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/processing/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/processing/persistent_ids/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-05-03 11:21:09.000000 eis1600-1.6.7/eis1600/processing/persistent_ids/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-05-03 11:16:17.000000 eis1600-1.6.7/eis1600/processing/persistent_ids/deprecated_long_short_ids_mapping.json
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4401 2024-05-08 13:02:23.000000 eis1600-1.6.7/eis1600/processing/persistent_ids/long_short_ids_mapping.json
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5802 2024-05-07 20:41:11.000000 eis1600-1.6.7/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6230 2024-02-12 17:00:08.000000 eis1600-1.6.7/eis1600/processing/preprocessing.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3008 2024-05-03 11:16:17.000000 eis1600-1.6.7/eis1600/processing/short_miu_generation.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/repositories/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/repositories/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    16586 2024-05-08 11:30:07.000000 eis1600-1.6.7/eis1600/repositories/repo.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/statistics/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/statistics/__init__.py
+-rw-r--r--   0 alicia    (1000) alicia    (1000)     2786 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/statistics/count_categories.py
+-rw-r--r--   0 alicia    (1000) alicia    (1000)     3548 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/statistics/count_tokens_per_miu.py
+-rw-r--r--   0 alicia    (1000) alicia    (1000)      958 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/statistics/methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/texts_to_mius/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      431 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/texts_to_mius/SubIDs.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1820 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/texts_to_mius/UIDs.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/texts_to_mius/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1939 2024-03-16 19:46:15.000000 eis1600-1.6.7/eis1600/texts_to_mius/check_formatting.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7572 2024-04-03 09:09:16.000000 eis1600-1.6.7/eis1600/texts_to_mius/check_formatting_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3696 2024-03-16 19:46:15.000000 eis1600-1.6.7/eis1600/texts_to_mius/check_mius.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3742 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/texts_to_mius/convert_mARkdown_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4179 2024-02-05 08:54:18.000000 eis1600-1.6.7/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1562 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/texts_to_mius/download_text_selection_sheet.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3312 2024-03-16 19:46:15.000000 eis1600-1.6.7/eis1600/texts_to_mius/ids_insert_or_update.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1463 2024-03-01 13:50:55.000000 eis1600-1.6.7/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    14062 2024-04-03 11:49:39.000000 eis1600-1.6.7/eis1600/texts_to_mius/subid_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/toponym_descriptions/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/toponym_descriptions/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-03-01 13:31:17.000000 eis1600-1.6.7/eis1600/toponym_descriptions/annotate_topd.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2783 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/toponym_descriptions/btopd_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4944 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/toponym_descriptions/topod_extract_incomplete.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4151 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/toponym_descriptions/topod_extract_places_regex.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3709 2024-02-16 15:42:32.000000 eis1600-1.6.7/eis1600/toponym_descriptions/topod_insert_into_miu.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1710 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/toponym_descriptions/topod_sheets_stats.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/toponyms/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.7/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1975 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/toponyms/initial_category_annotation.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3199 2023-11-02 14:43:12.000000 eis1600-1.6.7/eis1600/toponyms/methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1659 2023-11-02 14:43:12.000000 eis1600-1.6.7/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/training_data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/training_data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1535 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/training_data/annotate_onomastics.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1098 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/training_data/online_editor_files.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4121 2024-01-30 08:39:34.000000 eis1600-1.6.7/eis1600/training_data/reannotation.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600/yml/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     9610 2024-04-03 15:04:40.000000 eis1600-1.6.7/eis1600/yml/YAMLHandler.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/yml/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    12820 2024-04-09 11:27:31.000000 eis1600-1.6.7/eis1600/yml/yml_handling.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-01-18 10:18:32.000000 eis1600-1.6.7/eis1600/yml/yml_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-05-08 13:57:17.692732 eis1600-1.6.7/eis1600.egg-info/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-05-08 13:57:17.000000 eis1600-1.6.7/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4823 2024-05-08 13:57:17.000000 eis1600-1.6.7/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2024-05-08 13:57:17.000000 eis1600-1.6.7/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1851 2024-05-08 13:57:17.000000 eis1600-1.6.7/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      201 2024-05-08 13:57:17.000000 eis1600-1.6.7/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        8 2024-05-08 13:57:17.000000 eis1600-1.6.7/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2024-05-08 13:57:17.692732 eis1600-1.6.7/setup.cfg
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4214 2024-05-08 13:45:42.000000 eis1600-1.6.7/setup.py
```

### Comparing `eis1600-1.6.6/LICENSE` & `eis1600-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/PKG-INFO` & `eis1600-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 1.6.6
+Version: 1.6.7
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-1.6.6/README.md` & `eis1600-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/bio/md_to_bio.py` & `eis1600-1.6.7/eis1600/bio/md_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/bio/q_tags_to_bio.py` & `eis1600-1.6.7/eis1600/bio/q_tags_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/bio/topo_tags_to_bio.py` & `eis1600-1.6.7/eis1600/bio/topo_tags_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/corpus_analysis/analyse_all_on_cluster.py` & `eis1600-1.6.7/eis1600/corpus_analysis/analyse_all_on_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import gzip
 import glob
 import os.path
 from typing import Optional
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from functools import partial
 from pathlib import Path
 from logging import INFO
@@ -41,15 +42,15 @@
     :param bool parallel: Parallel flag for parallel processing, otherwise serial processing.
     :param bool force: Do processing even though file already exists.
     :param bool clean_out_dir: When processing all files, clean json output in case there are previous splitting.
         This param will remove all json files in subfolder when file is original or part 1.
     :param bool debug: Debug flag for more console messages.
     """
     out_path = infile.replace(TEXT_REPO, JSON_REPO)
-    out_path = out_path.replace('.EIS1600', '.json')
+    out_path = out_path.replace('.EIS1600', '.json.gz')
 
     # do not process file if it's already generated and it should not be overwritten
     if Path(out_path).is_file() and not force:
         return
 
     meta_data_header, mius_list = get_text_as_list_of_mius(infile)
 
@@ -70,22 +71,23 @@
     dir_path, _ = os.path.split(out_path)
     Path(dir_path).mkdir(parents=True, exist_ok=True)
 
     # if file is original or part 1, it might be good to remove previous json files
     # to avoid problems with previous chunking
     if clean_out_dir and (PART_NAME_INFIX not in out_path or int(PART_NUM_REGEX.search(out_path).group(1)) == 1):
         if os.path.exists(dir_path):
-            for json_file in glob.iglob(os.path.join(dir_path, "*.json")):
+            for json_file in glob.iglob(os.path.join(dir_path, "*.json.gz")):
                 os.remove(json_file)
 
     # add short id to each miu object
     for miu_obj in res:
-        miu_obj["yml"] = {"id": get_short_miu(miu_obj["yml"]["UID"]), **miu_obj["yml"]}
+        old_id = f'{miu_obj["yml"]["author"]}.{miu_obj["yml"]["text"]}.{miu_obj["yml"]["UID"]}'
+        miu_obj["yml"] = {"id": get_short_miu(old_id), **miu_obj["yml"]}
 
-    with open(out_path, 'w', encoding='utf-8') as fh:
+    with gzip.open(out_path, 'wt', encoding='utf-8') as fh:
         jsonpickle.set_encoder_options('json', indent=4, ensure_ascii=False)
         json_str = jsonpickle.encode(res, unpicklable=False)
         fh.write(json_str)
 
     save_ids()
 
     if error:
```

### Comparing `eis1600-1.6.6/eis1600/corpus_analysis/analyse_text.py` & `eis1600-1.6.7/eis1600/corpus_analysis/analyse_text.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/corpus_analysis/miu_methods.py` & `eis1600-1.6.7/eis1600/corpus_analysis/miu_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/corpus_analysis/text_methods.py` & `eis1600-1.6.7/eis1600/corpus_analysis/text_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/dates/Date.py` & `eis1600-1.6.7/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/dates/Month.py` & `eis1600-1.6.7/eis1600/dates/Month.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/dates/date_methods.py` & `eis1600-1.6.7/eis1600/dates/date_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/dates/date_patterns.py` & `eis1600-1.6.7/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/dates/month_methods.py` & `eis1600-1.6.7/eis1600/dates/month_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/Onomastics.py` & `eis1600-1.6.7/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/Spellings.py` & `eis1600-1.6.7/eis1600/gazetteers/Spellings.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/Toponyms.py` & `eis1600-1.6.7/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/data/days_gazetteer.csv` & `eis1600-1.6.7/eis1600/gazetteers/data/days_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/data/months_gazetteer.csv` & `eis1600-1.6.7/eis1600/gazetteers/data/months_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-1.6.7/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-1.6.7/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/data/toponyms_gazetteer.csv` & `eis1600-1.6.7/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/gazetteers/data/years_gazetteer.csv` & `eis1600-1.6.7/eis1600/gazetteers/data/years_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/helper/CheckFileEndingActions.py` & `eis1600-1.6.7/eis1600/helper/CheckFileEndingActions.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,19 @@
             setattr(namespace, self.dest, None)
 
 
 class CheckFileEndingEIS1600JsonAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
         if input_arg and isfile(input_arg):
             filepath, fileext = splitext(input_arg)
-            if fileext != '.json' and not filepath[-1:-12].isdigit():
-                parser.error('Input must be a single JSON file')
+            if '.' in filepath:
+                filepath, fileext1 = splitext(filepath)
+                fileext = fileext1 + fileext
+            if fileext != '.json.gz' and not filepath[-1:-12].isdigit():
+                parser.error(f'Input must be a single compressed JSON file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 class CheckFileEndingEIS1600OrEIS1600TMPAction(Action):
```

### Comparing `eis1600-1.6.6/eis1600/helper/ar_normalization.py` & `eis1600-1.6.7/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/helper/chunking.py` & `eis1600-1.6.7/eis1600/helper/chunking.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/helper/files_sizes.py` & `eis1600-1.6.7/eis1600/helper/files_sizes.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/helper/fix_dataframe.py` & `eis1600-1.6.7/eis1600/helper/fix_dataframe.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/helper/logging.py` & `eis1600-1.6.7/eis1600/helper/logging.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/helper/miu_random_revisions.py` & `eis1600-1.6.7/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/json_to_text/reconstruct.py` & `eis1600-1.6.7/eis1600/json_to_text/reconstruct.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import gzip
 from sys import argv
 import ujson as json
 import pandas as pd
 from io import StringIO
 from pathlib import Path
 from functools import partial
 from p_tqdm  import p_uimap
@@ -22,38 +23,40 @@
 def reconstruct_file(
         fpath: str,
         tags_list: tuple[str],
         force: bool = False,
         add_annotations_yml: bool = False,
         ):
 
-    if fpath.endswith(".json"):
-        out_fpath = fpath.replace(".json", f"{RECONSTRUCTED_INFIX}.EIS1600")
+    if fpath.endswith(".json.gz"):
+        out_fpath = fpath.replace(".json.gz", f"{RECONSTRUCTED_INFIX}.EIS1600")
     else:
         fpath = fpath.replace(TEXT_REPO, JSON_REPO)
         out_fpath = fpath.replace(".EIS1600", f"{RECONSTRUCTED_INFIX}.EIS1600")
-        fpath = fpath.replace('.EIS1600', '.json')
+        fpath = fpath.replace('.EIS1600', '.json.gz')
 
     out_fpath = out_fpath.replace(JSON_REPO, RECONSTRUCTED_REPO)
 
     if not Path(fpath).is_file():
         print(f"Warning! file {fpath} not found")
         return
 
     # do not process file if it's already generated and it should not be overwritten
     if Path(out_fpath).is_file() and not force:
         return
 
     dir_path, _ = os.path.split(out_fpath)
     Path(dir_path).mkdir(parents=True, exist_ok=True)
 
-    with open(fpath, "r", encoding="utf-8") as fp, \
+    with gzip.open(fpath, "rt", encoding="utf-8") as fp, \
          open(out_fpath, "w", encoding="utf-8") as outfp:
-        data = json.load(fp)
 
+        print(f"{fpath}")
+
+        data = json.load(fp)
         yml = data[0]["yml"]
         yml_handler = YAMLHandler(yml, ignore_annotations=not add_annotations_yml)
         df = pd.concat([pd.read_json(StringIO(miu["df"])) for miu in data], ignore_index=True)
         df = add_missing_columns(df)
         df["TAGS_LISTS"] = None
         if 'ONOM_TAGS' in df:
             df['ONOM_TAGS'] = df['ONOM_TAGS'].map(lambda s: '' if s == '_' else s)
```

### Comparing `eis1600-1.6.6/eis1600/json_to_tsv/corpus_dump.py` & `eis1600-1.6.7/eis1600/json_to_tsv/corpus_dump.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,39 @@
+import gzip
 import os.path
 import jsonpickle
 import ujson as json
 import pandas as pd
 from pathlib import Path
 from sys import argv
 from tqdm import tqdm
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 
-from eis1600.repositories.repo import get_ready_and_double_checked_files, TEXT_REPO, JSON_REPO, TSV_REPO, COLUMNS, \
-    SEP, SEP2
+from eis1600.repositories.repo import get_ready_and_double_checked_files, TEXT_REPO, JSON_REPO, TSV_YML_REPO, \
+    TSV_DF_REPO, COLUMNS, SEP, SEP2
 from eis1600.helper.CheckFileEndingActions import CheckFileEndingEIS1600JsonAction
 
 
 ALL_LABELS = ("SECTIONS", "TOKENS", "TAGS_LISTS", "NER_LABELS", "LEMMAS", "POS_TAGS", "ROOTS", "TOPONYM_LABELS",
               "NER_TAGS", "DATE_TAGS", "MONTH_TAGS", "ONOM_TAGS", "ONOMASTIC_TAGS")
 
 
 def dump_file(fpath: str, label_list: tuple[str] = ALL_LABELS):
 
-    if not fpath.endswith(".json"):
+    if not fpath.endswith(".json.gz"):
         fpath = fpath.replace(TEXT_REPO, JSON_REPO)
-        fpath = fpath.replace('.EIS1600', '.json')
+        fpath = fpath.replace('.EIS1600', '.json.gz')
 
     structural_data, content_data = [], []
 
     if not Path(fpath).is_file():
         print(f"Warning! file {fpath} not found")
         return
 
-    with open(fpath, "r", encoding="utf-8") as fp:
+    with gzip.open(fpath, "rt", encoding="utf-8") as fp:
         data = json.load(fp)
 
     for miu in data:
         header = miu["yml"]
         uid = header["UID"]
 
         # get structural data
@@ -73,25 +74,29 @@
                 continue
             for j, (_, value) in enumerate(miu_df[entity].items(), 1):
                 if type(value) == list:
                     value = SEP2.join(value)
                 if value:
                     content_data.append((uid, entity, f"{j}{SEP}{value}"))
 
-    fbase, _ = os.path.splitext(fpath)
+    fpath_yml = fpath.replace(JSON_REPO, TSV_YML_REPO)
+    fpath_yml = fpath_yml.replace(".json.gz", "")
+    dir_path_yml, _ = os.path.split(fpath_yml)
+    Path(dir_path_yml).mkdir(parents=True, exist_ok=True)
 
-    fbase = fbase.replace(JSON_REPO, TSV_REPO)
-    dir_path, _ = os.path.split(fbase)
-    Path(dir_path).mkdir(parents=True, exist_ok=True)
+    struct_df = pd.DataFrame(structural_data, columns=COLUMNS)
+    struct_df.to_csv(f"{fpath_yml}_yml.tsv.gz", sep="\t", index=False, compression='gzip')
 
-    content_df = pd.DataFrame(content_data, columns=COLUMNS)
-    content_df.to_csv(f"{fbase}_df.tsv", sep="\t", index=False)
+    fpath_df = fpath.replace(JSON_REPO, TSV_DF_REPO)
+    fpath_df = fpath_df.replace(".json.gz", "")
+    dir_path_df, _ = os.path.split(fpath_df)
+    Path(dir_path_df).mkdir(parents=True, exist_ok=True)
 
-    struct_df = pd.DataFrame(structural_data, columns=COLUMNS)
-    struct_df.to_csv(f"{fbase}_yml.tsv", sep="\t", index=False)
+    content_df = pd.DataFrame(content_data, columns=COLUMNS)
+    content_df.to_csv(f"{fpath_df}_df.tsv.gz", sep="\t", index=False, compression='gzip')
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description="Script to dump all eis1600 corpus into a tsv with the structure and "
                         "another tsv file with the enriched textual information."
```

### Comparing `eis1600-1.6.6/eis1600/markdown/EntityTags.py` & `eis1600-1.6.7/eis1600/markdown/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/markdown/category.py` & `eis1600-1.6.7/eis1600/markdown/category.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/markdown/markdown_methods.py` & `eis1600-1.6.7/eis1600/markdown/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/markdown/markdown_patterns.py` & `eis1600-1.6.7/eis1600/markdown/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/miu/HeadingTracker.py` & `eis1600-1.6.7/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/model_evaluations/eval_date_model.py` & `eis1600-1.6.7/eis1600/model_evaluations/eval_date_model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/model_evaluations/eval_topo_cat_model.py` & `eis1600-1.6.7/eis1600/model_evaluations/eval_topo_cat_model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/models/BiosPunctuationModel.py` & `eis1600-1.6.7/eis1600/models/BiosPunctuationModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/models/Disambiguator.py` & `eis1600-1.6.7/eis1600/models/Disambiguator.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/models/EventsPunctuationModel.py` & `eis1600-1.6.7/eis1600/models/EventsPunctuationModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/models/Lemmatizer.py` & `eis1600-1.6.7/eis1600/models/Lemmatizer.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/models/Model.py` & `eis1600-1.6.7/eis1600/models/Model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/models/POSTagger.py` & `eis1600-1.6.7/eis1600/models/POSTagger.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/models/PoetryDetectionModel.py` & `eis1600-1.6.7/eis1600/models/PoetryDetectionModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/nlp/annotation_utils.py` & `eis1600-1.6.7/eis1600/nlp/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/nlp/utils.py` & `eis1600-1.6.7/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/onomastics/initial_annotation.py` & `eis1600-1.6.7/eis1600/onomastics/initial_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/onomastics/methods.py` & `eis1600-1.6.7/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/onomastics/re_pattern.py` & `eis1600-1.6.7/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/paragraphs/paragraph_methods.py` & `eis1600-1.6.7/eis1600/paragraphs/paragraph_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/paragraphs/split_mius_into_paragraphs.py` & `eis1600-1.6.7/eis1600/paragraphs/split_mius_into_paragraphs.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/processing/postprocessing.py` & `eis1600-1.6.7/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/processing/preprocessing.py` & `eis1600-1.6.7/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/processing/short_miu_generation.py` & `eis1600-1.6.7/eis1600/processing/short_miu_generation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/repositories/repo.py` & `eis1600-1.6.7/eis1600/repositories/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 # Path variables
 
 MIU_REPO = 'EIS1600_MIUs/'
 TEXT_REPO = 'OpenITI_EIS1600_Texts/'
 NEW_PARAGRAPHS_REPO_ERROR_LOG = 'OpenITI_EIS1600_Texts_New_Paragraphs/error_log/'
 NEW_PARAGRAPHS_REPO = 'OpenITI_EIS1600_Texts_New_Paragraphs/'
 JSON_REPO = 'EIS1600_JSONs/'
-TSV_REPO = 'EIS1600_TSVs/'
+TSV_YML_REPO = 'EIS1600_TSVs_yml/'
+TSV_DF_REPO = 'EIS1600_TSVs_df/'
 RECONSTRUCTED_REPO = 'EIS1600_Reconstructed/'
 PRETRAINED_MODELS_REPO = 'EIS1600_Pretrained_Models/'
 TOPO_REPO = 'Topo_Data/'
 TRAINING_DATA_REPO = 'Training_Data/'
 RESEARCH_DATA_REPO = 'Research_Data/'
 TRAINING_RESULTS_REPO = 'Training_Results/'
 GAZETTEERS_REPO = 'gazetteers/'
```

### Comparing `eis1600-1.6.6/eis1600/statistics/count_categories.py` & `eis1600-1.6.7/eis1600/statistics/count_categories.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/statistics/count_tokens_per_miu.py` & `eis1600-1.6.7/eis1600/statistics/count_tokens_per_miu.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/statistics/methods.py` & `eis1600-1.6.7/eis1600/statistics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/UIDs.py` & `eis1600-1.6.7/eis1600/texts_to_mius/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/check_formatting.py` & `eis1600-1.6.7/eis1600/texts_to_mius/check_formatting.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/check_formatting_methods.py` & `eis1600-1.6.7/eis1600/texts_to_mius/check_formatting_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/check_mius.py` & `eis1600-1.6.7/eis1600/texts_to_mius/check_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/convert_mARkdown_methods.py` & `eis1600-1.6.7/eis1600/texts_to_mius/convert_mARkdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-1.6.7/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/download_text_selection_sheet.py` & `eis1600-1.6.7/eis1600/texts_to_mius/download_text_selection_sheet.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/ids_insert_or_update.py` & `eis1600-1.6.7/eis1600/texts_to_mius/ids_insert_or_update.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py` & `eis1600-1.6.7/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/texts_to_mius/subid_methods.py` & `eis1600-1.6.7/eis1600/texts_to_mius/subid_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponym_descriptions/annotate_topd.py` & `eis1600-1.6.7/eis1600/toponym_descriptions/annotate_topd.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponym_descriptions/btopd_to_bio.py` & `eis1600-1.6.7/eis1600/toponym_descriptions/btopd_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponym_descriptions/topod_extract_incomplete.py` & `eis1600-1.6.7/eis1600/toponym_descriptions/topod_extract_incomplete.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponym_descriptions/topod_extract_places_regex.py` & `eis1600-1.6.7/eis1600/toponym_descriptions/topod_extract_places_regex.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponym_descriptions/topod_insert_into_miu.py` & `eis1600-1.6.7/eis1600/toponym_descriptions/topod_insert_into_miu.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponym_descriptions/topod_sheets_stats.py` & `eis1600-1.6.7/eis1600/toponym_descriptions/topod_sheets_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponyms/initial_category_annotation.py` & `eis1600-1.6.7/eis1600/toponyms/initial_category_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponyms/methods.py` & `eis1600-1.6.7/eis1600/toponyms/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/toponyms/toponym_categories.py` & `eis1600-1.6.7/eis1600/toponyms/toponym_categories.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/training_data/annotate_onomastics.py` & `eis1600-1.6.7/eis1600/training_data/annotate_onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/training_data/online_editor_files.py` & `eis1600-1.6.7/eis1600/training_data/online_editor_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/training_data/reannotation.py` & `eis1600-1.6.7/eis1600/training_data/reannotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/yml/YAMLHandler.py` & `eis1600-1.6.7/eis1600/yml/YAMLHandler.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600/yml/yml_handling.py` & `eis1600-1.6.7/eis1600/yml/yml_handling.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600.egg-info/PKG-INFO` & `eis1600-1.6.7/eis1600.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 1.6.6
+Version: 1.6.7
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-1.6.6/eis1600.egg-info/SOURCES.txt` & `eis1600-1.6.7/eis1600.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/eis1600.egg-info/entry_points.txt` & `eis1600-1.6.7/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.6/setup.py` & `eis1600-1.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='1.6.6',
+      version='1.6.7',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```


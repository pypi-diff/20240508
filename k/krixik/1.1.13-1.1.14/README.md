# Comparing `tmp/krixik-1.1.13.tar.gz` & `tmp/krixik-1.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krixik-1.1.13.tar", last modified: Wed May  8 19:49:23 2024, max compression
+gzip compressed data, was "krixik-1.1.14.tar", last modified: Wed May  8 20:12:04 2024, max compression
```

## Comparing `krixik-1.1.13.tar` & `krixik-1.1.14.tar`

### file list

```diff
@@ -1,110 +1,209 @@
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.947835 krixik-1.1.13/
--rw-r--r--   0 jeremywatt   (501) staff       (20)     9114 2024-05-08 19:49:23.947291 krixik-1.1.13/PKG-INFO
--rw-r--r--   0 jeremywatt   (501) staff       (20)     7632 2024-05-02 22:24:18.000000 krixik-1.1.13/README.md
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.927252 krixik-1.1.13/krixik/
--rw-r--r--   0 jeremywatt   (501) staff       (20)       73 2024-04-06 04:16:52.000000 krixik-1.1.13/krixik/__base__.py
--rwxr-xr-x   0 jeremywatt   (501) staff       (20)       60 2024-04-04 03:06:43.000000 krixik-1.1.13/krixik/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)       23 2024-05-03 16:02:16.000000 krixik-1.1.13/krixik/__version__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     6003 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/main.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.928490 krixik-1.1.13/krixik/modules/
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1861 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/__init__.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.929783 krixik-1.1.13/krixik/modules/caption/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      353 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/caption/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      937 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/caption/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      832 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/caption/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.931025 krixik-1.1.13/krixik/modules/json-to-txt/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/json-to-txt/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      957 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/json-to-txt/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      900 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/json-to-txt/models.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     4850 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/json-to-txt/params.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.931681 krixik-1.1.13/krixik/modules/keyword-db/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/keyword-db/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      801 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/keyword-db/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      899 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/keyword-db/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.932387 krixik-1.1.13/krixik/modules/ocr/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/ocr/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      922 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/ocr/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      861 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/ocr/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.933347 krixik-1.1.13/krixik/modules/parser/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/parser/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1091 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/parser/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      978 2024-04-25 21:58:39.000000 krixik-1.1.13/krixik/modules/parser/models.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     4850 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/parser/params.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.933908 krixik-1.1.13/krixik/modules/sentiment/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/sentiment/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1095 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/sentiment/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      834 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/sentiment/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.934577 krixik-1.1.13/krixik/modules/summarize/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/summarize/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      819 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/summarize/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      834 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/summarize/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.935825 krixik-1.1.13/krixik/modules/text-embedder/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/text-embedder/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1163 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/text-embedder/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1068 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/text-embedder/models.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      394 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/text-embedder/params.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.936508 krixik-1.1.13/krixik/modules/transcribe/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/transcribe/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     2377 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/transcribe/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      835 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/transcribe/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.937088 krixik-1.1.13/krixik/modules/translate/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/translate/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1095 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/translate/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      834 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/translate/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.938475 krixik-1.1.13/krixik/modules/utilities/
--rw-r--r--   0 jeremywatt   (501) staff       (20)        0 2024-03-30 18:14:50.000000 krixik-1.1.13/krixik/modules/utilities/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1807 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/utilities/decorators.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     2125 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/utilities/io_validator.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     2172 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/utilities/model.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      355 2024-03-31 13:49:58.000000 krixik-1.1.13/krixik/modules/utilities/model_selection.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     4357 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/utilities/module_selections.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1273 2024-04-12 02:36:14.000000 krixik-1.1.13/krixik/modules/utilities/read_config.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.939245 krixik-1.1.13/krixik/modules/vector-db/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      313 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/vector-db/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      863 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/vector-db/io.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      898 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/modules/vector-db/models.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.940566 krixik-1.1.13/krixik/pipeline_builder/
--rw-r--r--   0 jeremywatt   (501) staff       (20)       17 2024-04-29 16:45:23.000000 krixik-1.1.13/krixik/pipeline_builder/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     4180 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_builder/module.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     9363 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_builder/pipeline.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.941711 krixik-1.1.13/krixik/pipeline_builder/utilities/
--rw-r--r--   0 jeremywatt   (501) staff       (20)        0 2024-04-29 16:11:03.000000 krixik-1.1.13/krixik/pipeline_builder/utilities/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      687 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_builder/utilities/chain_checker.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      618 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_builder/utilities/config_checker.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      890 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_builder/utilities/input_checker.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      311 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_builder/utilities/name_checker.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      470 2024-05-08 18:29:56.000000 krixik-1.1.13/krixik/pipeline_builder/utilities/savepath_checker.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1916 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_builder/utilities.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.941975 krixik-1.1.13/krixik/pipeline_examples/
--rw-r--r--   0 jeremywatt   (501) staff       (20)        0 2024-04-12 22:38:52.000000 krixik-1.1.13/krixik/pipeline_examples/__init__.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.942088 krixik-1.1.13/krixik/pipeline_examples/single_module/
--rw-r--r--   0 jeremywatt   (501) staff       (20)        0 2024-04-12 22:39:09.000000 krixik-1.1.13/krixik/pipeline_examples/single_module/__init__.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.942334 krixik-1.1.13/krixik/pipeline_examples/single_module/utilities/
--rw-r--r--   0 jeremywatt   (501) staff       (20)        0 2024-04-13 04:25:01.000000 krixik-1.1.13/krixik/pipeline_examples/single_module/utilities/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)      795 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/pipeline_examples/single_module/utilities/generate_examples.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.942606 krixik-1.1.13/krixik/system_builder/
--rw-r--r--   0 jeremywatt   (501) staff       (20)        0 2024-04-03 16:17:03.000000 krixik-1.1.13/krixik/system_builder/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)    25795 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/base.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.945738 krixik-1.1.13/krixik/system_builder/functions/
--rw-r--r--   0 jeremywatt   (501) staff       (20)      448 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     5432 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/check_process_status.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     2880 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/checkin.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     2774 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/delete.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     4785 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/fetch_output.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     6492 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/keyword_search.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     5097 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/list_files.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     5368 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/process.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     9377 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/semantic_search.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     3246 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/show_tree.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     3803 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/functions/update.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.945992 krixik-1.1.13/krixik/system_builder/utilities/
--rw-r--r--   0 jeremywatt   (501) staff       (20)        0 2024-04-16 21:10:42.000000 krixik-1.1.13/krixik/system_builder/utilities/__init__.py
--rw-r--r--   0 jeremywatt   (501) staff       (20)     2509 2024-05-08 18:56:56.000000 krixik-1.1.13/krixik/system_builder/utilities/decorators.py
-drwxr-xr-x   0 jeremywatt   (501) staff       (20)        0 2024-05-08 19:49:23.928362 krixik-1.1.13/krixik.egg-info/
--rw-r--r--   0 jeremywatt   (501) staff       (20)     9114 2024-05-08 19:49:23.000000 krixik-1.1.13/krixik.egg-info/PKG-INFO
--rw-r--r--   0 jeremywatt   (501) staff       (20)     3112 2024-05-08 19:49:23.000000 krixik-1.1.13/krixik.egg-info/SOURCES.txt
--rw-r--r--   0 jeremywatt   (501) staff       (20)        1 2024-05-08 19:49:23.000000 krixik-1.1.13/krixik.egg-info/dependency_links.txt
--rw-r--r--   0 jeremywatt   (501) staff       (20)      308 2024-05-08 19:49:23.000000 krixik-1.1.13/krixik.egg-info/requires.txt
--rw-r--r--   0 jeremywatt   (501) staff       (20)        7 2024-05-08 19:49:23.000000 krixik-1.1.13/krixik.egg-info/top_level.txt
--rw-r--r--   0 jeremywatt   (501) staff       (20)       38 2024-05-08 19:49:23.947887 krixik-1.1.13/setup.cfg
--rw-r--r--   0 jeremywatt   (501) staff       (20)     1361 2024-05-08 19:47:52.000000 krixik-1.1.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.686639 krixik-1.1.14/
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 20:12:04.686639 krixik-1.1.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-08 20:11:55.000000 krixik-1.1.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/__base__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik/modules/caption/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/caption/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/caption/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik/modules/json-to-txt/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/json-to-txt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/json-to-txt/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/json-to-txt/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/json-to-txt/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik/modules/keyword-db/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/keyword-db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/keyword-db/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/keyword-db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik/modules/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/ocr/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/ocr/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik/modules/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/parser/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/parser/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.666638 krixik-1.1.14/krixik/modules/sentiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/sentiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/sentiment/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/sentiment/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.666638 krixik-1.1.14/krixik/modules/summarize/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/summarize/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/summarize/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.666638 krixik-1.1.14/krixik/modules/text-embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/text-embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/text-embedder/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/text-embedder/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/text-embedder/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.666638 krixik-1.1.14/krixik/modules/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/transcribe/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/transcribe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.666638 krixik-1.1.14/krixik/modules/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/translate/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/translate/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.666638 krixik-1.1.14/krixik/modules/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/utilities/io_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/utilities/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/utilities/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/utilities/module_selections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/utilities/read_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.666638 krixik-1.1.14/krixik/modules/vector-db/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/vector-db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/vector-db/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/modules/vector-db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.670638 krixik-1.1.14/krixik/pipeline_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.670638 krixik-1.1.14/krixik/pipeline_builder/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/utilities/chain_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/utilities/config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/utilities/input_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/utilities/name_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/utilities/savepath_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_builder/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.670638 krixik-1.1.14/krixik/pipeline_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.670638 krixik-1.1.14/krixik/pipeline_examples/single_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_examples/single_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.670638 krixik-1.1.14/krixik/pipeline_examples/single_module/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_examples/single_module/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/pipeline_examples/single_module/utilities/generate_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.670638 krixik-1.1.14/krixik/system_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25795 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.670638 krixik-1.1.14/krixik/system_builder/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/check_process_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/fetch_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/keyword_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/semantic_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/show_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/functions/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.674639 krixik-1.1.14/krixik/system_builder/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/system_builder/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.674639 krixik-1.1.14/krixik/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/cleaners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.674639 krixik-1.1.14/krixik/utilities/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/default_clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/docx_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/pdf_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/pptx_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/read_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/unclean_to_clean_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.674639 krixik-1.1.14/krixik/utilities/converters/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/converters/video_to_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/file_name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/tree_illustrator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1486 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.674639 krixik-1.1.14/krixik/utilities/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.674639 krixik-1.1.14/krixik/utilities/validators/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.678639 krixik-1.1.14/krixik/utilities/validators/data/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/utilities/read_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/data/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.678639 krixik-1.1.14/krixik/utilities/validators/system/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/expire_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/extension_enforcer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1237 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/file_description.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2773 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/file_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5749 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/file_names.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4957 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/file_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/k_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/local_file_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/local_save_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/lower_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/max_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/process_switches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/symbolic_path_splitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9255 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/symbolic_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/timestamp_bookends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/use_default_clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/user_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/base/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/base/wait_for_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/data/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/audio/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/audio/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/data/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/image/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/image/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/image/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/data/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/json/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/json/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/json/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/data/npy/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/npy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/npy/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/npy/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.682639 krixik-1.1.14/krixik/utilities/validators/system/data/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/text/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/text/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/text/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.686639 krixik-1.1.14/krixik/utilities/validators/system/data/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/system/data/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.686639 krixik-1.1.14/krixik/utilities/validators/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 20:11:55.000000 krixik-1.1.14/krixik/utilities/validators/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:12:04.662638 krixik-1.1.14/krixik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 20:12:04.000000 krixik-1.1.14/krixik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-05-08 20:12:04.000000 krixik-1.1.14/krixik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:12:04.000000 krixik-1.1.14/krixik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 20:12:04.000000 krixik-1.1.14/krixik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 20:12:04.000000 krixik-1.1.14/krixik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:12:04.686639 krixik-1.1.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-08 20:11:55.000000 krixik-1.1.14/setup.py
```

### Comparing `krixik-1.1.13/README.md` & `krixik-1.1.14/README.md`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/main.py` & `krixik-1.1.14/krixik/main.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/__init__.py` & `krixik-1.1.14/krixik/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/caption/io.py` & `krixik-1.1.14/krixik/modules/caption/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/caption/models.py` & `krixik-1.1.14/krixik/modules/caption/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/json-to-txt/io.py` & `krixik-1.1.14/krixik/modules/json-to-txt/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/json-to-txt/models.py` & `krixik-1.1.14/krixik/modules/json-to-txt/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/json-to-txt/params.py` & `krixik-1.1.14/krixik/modules/json-to-txt/params.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/keyword-db/io.py` & `krixik-1.1.14/krixik/modules/keyword-db/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/keyword-db/models.py` & `krixik-1.1.14/krixik/modules/keyword-db/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/ocr/io.py` & `krixik-1.1.14/krixik/modules/ocr/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/ocr/models.py` & `krixik-1.1.14/krixik/modules/ocr/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/parser/io.py` & `krixik-1.1.14/krixik/modules/parser/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/parser/models.py` & `krixik-1.1.14/krixik/modules/parser/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/parser/params.py` & `krixik-1.1.14/krixik/modules/parser/params.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/sentiment/io.py` & `krixik-1.1.14/krixik/modules/sentiment/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/sentiment/models.py` & `krixik-1.1.14/krixik/modules/sentiment/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/summarize/io.py` & `krixik-1.1.14/krixik/modules/summarize/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/summarize/models.py` & `krixik-1.1.14/krixik/modules/summarize/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/text-embedder/io.py` & `krixik-1.1.14/krixik/modules/text-embedder/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/text-embedder/models.py` & `krixik-1.1.14/krixik/modules/text-embedder/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/transcribe/io.py` & `krixik-1.1.14/krixik/modules/transcribe/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/transcribe/models.py` & `krixik-1.1.14/krixik/modules/transcribe/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/translate/io.py` & `krixik-1.1.14/krixik/modules/translate/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/translate/models.py` & `krixik-1.1.14/krixik/modules/translate/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/utilities/decorators.py` & `krixik-1.1.14/krixik/modules/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/utilities/io_validator.py` & `krixik-1.1.14/krixik/modules/utilities/io_validator.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/utilities/model.py` & `krixik-1.1.14/krixik/modules/utilities/model.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/utilities/module_selections.py` & `krixik-1.1.14/krixik/modules/utilities/module_selections.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/utilities/read_config.py` & `krixik-1.1.14/krixik/modules/utilities/read_config.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/vector-db/io.py` & `krixik-1.1.14/krixik/modules/vector-db/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/modules/vector-db/models.py` & `krixik-1.1.14/krixik/modules/vector-db/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/pipeline_builder/module.py` & `krixik-1.1.14/krixik/pipeline_builder/module.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/pipeline_builder/pipeline.py` & `krixik-1.1.14/krixik/pipeline_builder/pipeline.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/pipeline_builder/utilities/chain_checker.py` & `krixik-1.1.14/krixik/pipeline_builder/utilities/chain_checker.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/pipeline_builder/utilities/config_checker.py` & `krixik-1.1.14/krixik/pipeline_builder/utilities/config_checker.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/pipeline_builder/utilities/input_checker.py` & `krixik-1.1.14/krixik/pipeline_builder/utilities/input_checker.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/pipeline_builder/utilities.py` & `krixik-1.1.14/krixik/pipeline_builder/utilities.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/pipeline_examples/single_module/utilities/generate_examples.py` & `krixik-1.1.14/krixik/pipeline_examples/single_module/utilities/generate_examples.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/base.py` & `krixik-1.1.14/krixik/system_builder/base.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/check_process_status.py` & `krixik-1.1.14/krixik/system_builder/functions/check_process_status.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/checkin.py` & `krixik-1.1.14/krixik/system_builder/functions/checkin.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/delete.py` & `krixik-1.1.14/krixik/system_builder/functions/delete.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/fetch_output.py` & `krixik-1.1.14/krixik/system_builder/functions/fetch_output.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/keyword_search.py` & `krixik-1.1.14/krixik/system_builder/functions/keyword_search.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/list_files.py` & `krixik-1.1.14/krixik/system_builder/functions/list_files.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/process.py` & `krixik-1.1.14/krixik/system_builder/functions/process.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/semantic_search.py` & `krixik-1.1.14/krixik/system_builder/functions/semantic_search.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/show_tree.py` & `krixik-1.1.14/krixik/system_builder/functions/show_tree.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/functions/update.py` & `krixik-1.1.14/krixik/system_builder/functions/update.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/krixik/system_builder/utilities/decorators.py` & `krixik-1.1.14/krixik/system_builder/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.13/setup.py` & `krixik-1.1.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from setuptools import find_packages
 
 setup(
     name="krixik",
-    version="1.1.13",
+    version="1.1.14",
     description="Easily assemble and serverlessly consume modular AI pipelines through secure Python APIs.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jeremy Watt",
     email="jeremy@krixik.com",
     url="https://github.com/krixik-ai/krixik-cli",
     packages=find_packages(include=["krixik*"]),
```


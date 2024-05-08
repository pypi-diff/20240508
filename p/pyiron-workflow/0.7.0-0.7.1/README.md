# Comparing `tmp/pyiron_workflow-0.7.0.tar.gz` & `tmp/pyiron_workflow-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_workflow-0.7.0.tar", last modified: Tue May  7 00:18:16 2024, max compression
+gzip compressed data, was "pyiron_workflow-0.7.1.tar", last modified: Wed May  8 21:43:19 2024, max compression
```

## Comparing `pyiron_workflow-0.7.0.tar` & `pyiron_workflow-0.7.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.385709 pyiron_workflow-0.7.0/pyiron_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/pyiron_workflow/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/draw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/executors/cloudpickleprocesspool.py
--rw-r--r--   0 runner    (1001) docker     (127)    17674 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/has_interface_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/has_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/injection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/io_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)    39869 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/node_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/pyiron_atomistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/semantics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/single_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/has_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/type_hinting.py
--rw-r--r--   0 runner    (1001) docker     (127)    23787 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/working.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-07 00:18:15.000000 pyiron_workflow-0.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.180070 pyiron_workflow-0.7.1/pyiron_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/pyiron_workflow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/draw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/executors/cloudpickleprocesspool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17951 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/has_interface_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/has_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/io_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39869 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/node_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/pyiron_atomistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_library/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/node_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/single_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/has_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/snippets/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/type_hinting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23787 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/pyiron_workflow/working.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:43:19.184070 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 21:43:19.000000 pyiron_workflow-0.7.1/pyiron_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 21:43:19.188070 pyiron_workflow-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 21:43:18.000000 pyiron_workflow-0.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-08 21:43:16.000000 pyiron_workflow-0.7.1/versioneer.py
```

### Comparing `pyiron_workflow-0.7.0/LICENSE` & `pyiron_workflow-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/PKG-INFO` & `pyiron_workflow-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.7.0
+Version: 0.7.1
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/__init__.py` & `pyiron_workflow-0.7.1/pyiron_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/channels.py` & `pyiron_workflow-0.7.1/pyiron_workflow/channels.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/composite.py` & `pyiron_workflow-0.7.1/pyiron_workflow/composite.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/create.py` & `pyiron_workflow-0.7.1/pyiron_workflow/create.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/draw.py` & `pyiron_workflow-0.7.1/pyiron_workflow/draw.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/executors/cloudpickleprocesspool.py` & `pyiron_workflow-0.7.1/pyiron_workflow/executors/cloudpickleprocesspool.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/for_loop.py` & `pyiron_workflow-0.7.1/pyiron_workflow/for_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,21 @@
                 self.remove_child(label)
             else:
                 # Re-run the user input node so it has up-to-date output, otherwise
                 # when we inject a getitem node -- which will try to run automatically
                 # -- it will see data it can work with, but if that data happens to
                 # have the wrong length it may successfully auto-run on the wrong thing
                 # and throw an error!
-                self.children[label]()
+                self.children[label].run(
+                    run_data_tree=False,
+                    run_parent_trees_too=False,
+                    fetch_input=False,
+                    # Data should simply be coming from the value link
+                    # We just want to refresh the output
+                )
         # TODO: Instead of deleting _everything_ each time, try and re-use stuff
 
     def _build_collector_node(self, row_number):
         # Iterated inputs
         row_specification = {
             key: (self._body_node_class.preview_inputs()[key][0], NOT_DATA)
             for key in self._iter_on + self._zip_on
```

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/function.py` & `pyiron_workflow-0.7.1/pyiron_workflow/function.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/has_interface_mixins.py` & `pyiron_workflow-0.7.1/pyiron_workflow/has_interface_mixins.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/injection.py` & `pyiron_workflow-0.7.1/pyiron_workflow/injection.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/io.py` & `pyiron_workflow-0.7.1/pyiron_workflow/io.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/io_preview.py` & `pyiron_workflow-0.7.1/pyiron_workflow/io_preview.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/job.py` & `pyiron_workflow-0.7.1/pyiron_workflow/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/loops.py` & `pyiron_workflow-0.7.1/pyiron_workflow/loops.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/macro.py` & `pyiron_workflow-0.7.1/pyiron_workflow/macro.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/node.py` & `pyiron_workflow-0.7.1/pyiron_workflow/node.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/calculator.py` & `pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/calculator.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/macro.py` & `pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/macro.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/task.py` & `pyiron_workflow-0.7.1/pyiron_workflow/node_library/atomistics/task.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/node_library/pyiron_atomistics.py` & `pyiron_workflow-0.7.1/pyiron_workflow/node_library/pyiron_atomistics.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/node_library/standard.py` & `pyiron_workflow-0.7.1/pyiron_workflow/node_library/standard.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/node_package.py` & `pyiron_workflow-0.7.1/pyiron_workflow/node_package.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/output_parser.py` & `pyiron_workflow-0.7.1/pyiron_workflow/output_parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/run.py` & `pyiron_workflow-0.7.1/pyiron_workflow/run.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/semantics.py` & `pyiron_workflow-0.7.1/pyiron_workflow/semantics.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/single_output.py` & `pyiron_workflow-0.7.1/pyiron_workflow/single_output.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/colors.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/colors.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/dotdict.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/factory.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/files.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/files.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/has_post.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/has_post.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/logger.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/singleton.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/snippets/testcase.py` & `pyiron_workflow-0.7.1/pyiron_workflow/snippets/testcase.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/storage.py` & `pyiron_workflow-0.7.1/pyiron_workflow/storage.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/topology.py` & `pyiron_workflow-0.7.1/pyiron_workflow/topology.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/transform.py` & `pyiron_workflow-0.7.1/pyiron_workflow/transform.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/type_hinting.py` & `pyiron_workflow-0.7.1/pyiron_workflow/type_hinting.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/workflow.py` & `pyiron_workflow-0.7.1/pyiron_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow/working.py` & `pyiron_workflow-0.7.1/pyiron_workflow/working.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow.egg-info/PKG-INFO` & `pyiron_workflow-0.7.1/pyiron_workflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.7.0
+Version: 0.7.1
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyiron_workflow-0.7.0/pyiron_workflow.egg-info/SOURCES.txt` & `pyiron_workflow-0.7.1/pyiron_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/setup.py` & `pyiron_workflow-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.7.0/versioneer.py` & `pyiron_workflow-0.7.1/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/sequali-0.7.1.tar.gz` & `tmp/sequali-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequali-0.7.1.tar", last modified: Wed Apr 17 07:52:06 2024, max compression
+gzip compressed data, was "sequali-0.8.0.tar", last modified: Wed May  8 14:54:28 2024, max compression
```

## Comparing `sequali-0.7.1.tar` & `sequali-0.8.0.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.598124 sequali-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 07:47:32.000000 sequali-0.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-17 07:47:32.000000 sequali-0.7.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-17 07:47:32.000000 sequali-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 07:47:32.000000 sequali-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-17 07:52:06.598124 sequali-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-17 07:47:32.000000 sequali-0.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-17 07:47:32.000000 sequali-0.7.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.590124 sequali-0.7.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.586124 sequali-0.7.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.590124 sequali-0.7.1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    42483 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/_static/images/fingerprint.fodg
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/_static/images/fingerprint.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48097 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/_static/images/overrepresented_sampling.fodg
--rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/_static/images/overrepresented_sampling.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.590124 sequali-0.7.1/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/includes/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/includes/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/module_options.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 07:47:32.000000 sequali-0.7.1/docs/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-17 07:47:32.000000 sequali-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:52:06.598124 sequali-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-17 07:47:32.000000 sequali-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.590124 sequali-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.594124 sequali-0.7.1/src/sequali/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/_qc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   155348 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/_qcmodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 07:52:06.000000 sequali-0.7.1/src/sequali/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.594124 sequali-0.7.1/src/sequali/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/adapters/adapter_list.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.598124 sequali-0.7.1/src/sequali/contaminants/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/contaminants/README
--rw-r--r--   0 runner    (1001) docker     (127)  1701925 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/contaminants/UniVec.fasta
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/contaminants/oxford_nanopore.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    58889 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/contaminants/oxford_nanopore_barcodes.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/debug_vectors.h
--rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/function_dispatch.h
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/murmur3.h
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.598124 sequali-0.7.1/src/sequali/pygal.js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.598124 sequali-0.7.1/src/sequali/pygal.js/2.0.x/
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-17 07:47:33.000000 sequali-0.7.1/src/sequali/pygal.js/2.0.x/pygal-tooltips.js
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-17 07:47:33.000000 sequali-0.7.1/src/sequali/pygal.js/2.0.x/pygal-tooltips.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-17 07:47:33.000000 sequali-0.7.1/src/sequali/pygal.js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    72749 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/report_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/score_to_error_rate.h
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/sequence_identification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.598124 sequali-0.7.1/src/sequali/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/static/sequali_report.css
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/static/svg_to_download_link.js
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-17 07:47:32.000000 sequali-0.7.1/src/sequali/wanghash.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:52:06.598124 sequali-0.7.1/src/sequali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-17 07:52:06.000000 sequali-0.7.1/src/sequali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-17 07:52:06.000000 sequali-0.7.1/src/sequali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:52:06.000000 sequali-0.7.1/src/sequali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 07:52:06.000000 sequali-0.7.1/src/sequali.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 07:52:06.000000 sequali-0.7.1/src/sequali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 07:52:06.000000 sequali-0.7.1/src/sequali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.067047 sequali-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-08 14:49:30.000000 sequali-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-08 14:49:30.000000 sequali-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-08 14:49:30.000000 sequali-0.8.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-08 14:49:30.000000 sequali-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 14:49:30.000000 sequali-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-08 14:54:28.067047 sequali-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-08 14:49:30.000000 sequali-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-08 14:49:30.000000 sequali-0.8.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.051047 sequali-0.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.047047 sequali-0.8.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.051047 sequali-0.8.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    49695 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/_static/images/fingerprint.fodg
+-rw-r--r--   0 runner    (1001) docker     (127)    17506 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/_static/images/fingerprint.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48097 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/_static/images/overrepresented_sampling.fodg
+-rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/_static/images/overrepresented_sampling.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.051047 sequali-0.8.0/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/includes/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/includes/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/module_options.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.051047 sequali-0.8.0/docs/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)  5201949 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/reports/GM24385_1.fastq.gz.html
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 14:49:30.000000 sequali-0.8.0/docs/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-08 14:49:30.000000 sequali-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:54:28.067047 sequali-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 14:49:30.000000 sequali-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.047047 sequali-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.063048 sequali-0.8.0/src/sequali/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-08 14:49:30.000000 sequali-0.8.0/src/sequali/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-05-08 14:49:30.000000 sequali-0.8.0/src/sequali/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-08 14:49:30.000000 sequali-0.8.0/src/sequali/_qc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   186637 2024-05-08 14:49:30.000000 sequali-0.8.0/src/sequali/_qcmodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 14:54:27.000000 sequali-0.8.0/src/sequali/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.063048 sequali-0.8.0/src/sequali/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-08 14:49:30.000000 sequali-0.8.0/src/sequali/adapters/adapter_list.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-08 14:49:30.000000 sequali-0.8.0/src/sequali/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.067047 sequali-0.8.0/src/sequali/contaminants/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 14:49:30.000000 sequali-0.8.0/src/sequali/contaminants/README
+-rw-r--r--   0 runner    (1001) docker     (127)  1701925 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/contaminants/UniVec.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/contaminants/oxford_nanopore.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    58889 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/contaminants/oxford_nanopore_barcodes.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/debug_vectors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/function_dispatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/murmur3.h
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.067047 sequali-0.8.0/src/sequali/pygal.js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.067047 sequali-0.8.0/src/sequali/pygal.js/2.0.x/
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/pygal.js/2.0.x/pygal-tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/pygal.js/2.0.x/pygal-tooltips.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/pygal.js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    85583 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/report_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/score_to_error_rate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/sequence_identification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.067047 sequali-0.8.0/src/sequali/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/static/sequali_report.css
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/static/svg_to_download_link.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-08 14:49:31.000000 sequali-0.8.0/src/sequali/wanghash.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:54:28.067047 sequali-0.8.0/src/sequali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-08 14:54:27.000000 sequali-0.8.0/src/sequali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-08 14:54:28.000000 sequali-0.8.0/src/sequali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:54:27.000000 sequali-0.8.0/src/sequali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 14:54:27.000000 sequali-0.8.0/src/sequali.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 14:54:27.000000 sequali-0.8.0/src/sequali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 14:54:27.000000 sequali-0.8.0/src/sequali.egg-info/top_level.txt
```

### Comparing `sequali-0.7.1/CHANGELOG.rst` & `sequali-0.8.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 ==========
 
 .. Newest changes should be on top.
 
 .. This document is user facing. Please word the changes in such a way
 .. that users understand how the changes affect the new version.
 
+version 0.8.0
+-----------------
++ A citation file was added to the repository.
++ Calculate insert sizes and used adapters based on overlap between the
+  read pairs.
++ Both reads from paired-end reads are taken into consideration when
+  evaluating the duplication rate.
++ Support for paired-end reads added.
++ Minor performance improvement by providing a non-temporal cache hint in the
+  QCMetrics module.
+
 version 0.7.1
 -----------------
 + Fix a small visual bug in the report sidebar.
 + PyGAL report htmls are now fully HTML5 compliant. HTML5 validation has been
   made a part of the integration testing.
 
 version 0.7.0
```

### Comparing `sequali-0.7.1/LICENSE` & `sequali-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/PKG-INFO` & `sequali-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sequali
-Version: 0.7.1
-Summary: Fast sequencing quality metrics
+Version: 0.8.0
+Summary: Sequali is a QC tool that generates useful graphs for both short and long-read data.
 Author-email: Ruben Vorderman <r.h.p.vorderman@lumc.nl>
 License: AGPL-v3.0
 Project-URL: Documentation, https://sequali.readthedocs.io
 Project-URL: Homepage, https://github.com/rhpvorderman/sequali
 Project-URL: Issue tracker, https://github.com/rhpvorderman/sequali/issues
 Keywords: FASTQ,sequencing quality,uBAM,QC,nanopore,illumina
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,42 +21,45 @@
 Requires-Python: >3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: xopen>=2.0.0
 Requires-Dist: pygal>=3.0.4
 Requires-Dist: tqdm
 
-.. image:: https://img.shields.io/pypi/v/sequali.svg
+.. |python-version-shield| image:: https://img.shields.io/pypi/v/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/conda/v/bioconda/sequali.svg
+.. |conda-version-shield| image:: https://img.shields.io/conda/v/bioconda/sequali.svg
   :target: https://bioconda.github.io/recipes/sequali/README.html
   :alt:
 
-.. image:: https://img.shields.io/pypi/pyversions/sequali.svg
+.. |python-install-version-shield| image:: https://img.shields.io/pypi/pyversions/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/pypi/l/sequali.svg
+.. |license-shield| image:: https://img.shields.io/pypi/l/sequali.svg
   :target: https://github.com/rhpvorderman/sequali/blob/main/LICENSE
   :alt:
 
-.. image:: https://readthedocs.org/projects/sequali/badge/?version=latest
+.. |docs-shield| image:: https://readthedocs.org/projects/sequali/badge/?version=latest
   :target: https://sequali.readthedocs.io/en/latest/?badge=latest
   :alt:
 
-.. image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
+.. |coverage-shield| image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
   :target: https://codecov.io/gh/rhpvorderman/sequali
   :alt:
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
+.. |zenodo-shield| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
   :target: https://doi.org/10.5281/zenodo.10854010
   :alt:
 
+|python-version-shield| |conda-version-shield| |python-install-version-shield|
+|license-shield| |docs-shield| |coverage-shield| |zenodo-shield|
+
 ========
 Sequali
 ========
 
 .. introduction start
 
 Sequence quality metrics for FASTQ and uBAM files.
@@ -67,22 +70,25 @@
 + Informative graphs that allow for judging the quality of a sequence at
   a quick glance.
 + Overrepresentation analysis using 21 bp sequence fragments. Overrepresented
   sequences are checked against the NCBI univec database.
 + Estimate duplication rate using a `fingerprint subsampling technique which is
   also used in filesystem duplication estimation
   <https://www.usenix.org/system/files/conference/atc13/atc13-xie.pdf>`_.
-+ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences.
++ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences
+  for single read data.
++ Determines adapters by overlap analysis for paired read data.
++ Insert size metrics for paired read data.
 + Per tile quality plots for illumina reads.
 + Channel and other plots for nanopore reads.
 + FASTQ and unaligned BAM are supported. See "Supported formats".
 
 Example reports:
 
-+ `GM24385_1.fastq.gz <https://github.com/rhpvorderman/sequali/files/14725146/GM24385_1.fastq.gz.html.zip>`_;
++ `GM24385_1.fastq.gz <https://sequali.readthedocs.io/en/latest/GM24385_1.fastq.gz.html>`_;
   HG002 (Genome In A Bottle) on ultra-long Nanopore Sequencing. `Sequence file download <https://ftp-trace.ncbi.nlm.nih.gov/ReferenceSamples/giab/data/AshkenazimTrio/HG002_NA24385_son/UCSC_Ultralong_OxfordNanopore_Promethion/GM24385_1.fastq.gz>`_.
 
 .. introduction end
 
 For more information check `the documentation <https://sequali.readthedocs.io>`_.
 
 Supported formats
@@ -90,19 +96,19 @@
 
 .. formats start
 
 - FASTQ. Only the Sanger variation with a phred offset of 33 and the error rate
   calculation of 10 ^ (-phred/10) is supported. All sequencers use this
   format today.
 
+  - Paired end sequencing data is supported.
   - For sequences called by illumina base callers an additional plot with the
     per tile quality will be provided.
   - For sequences called by guppy additional plots for nanopore specific
     data will be provided.
-
 - unaligned BAM. Any alignment flags are currently ignored.
 
   - For uBAM data as delivered by dorado additional nanopore plots will be
     provided.
 
 .. formats end
```

### Comparing `sequali-0.7.1/README.rst` & `sequali-0.8.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-.. image:: https://img.shields.io/pypi/v/sequali.svg
+.. |python-version-shield| image:: https://img.shields.io/pypi/v/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/conda/v/bioconda/sequali.svg
+.. |conda-version-shield| image:: https://img.shields.io/conda/v/bioconda/sequali.svg
   :target: https://bioconda.github.io/recipes/sequali/README.html
   :alt:
 
-.. image:: https://img.shields.io/pypi/pyversions/sequali.svg
+.. |python-install-version-shield| image:: https://img.shields.io/pypi/pyversions/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/pypi/l/sequali.svg
+.. |license-shield| image:: https://img.shields.io/pypi/l/sequali.svg
   :target: https://github.com/rhpvorderman/sequali/blob/main/LICENSE
   :alt:
 
-.. image:: https://readthedocs.org/projects/sequali/badge/?version=latest
+.. |docs-shield| image:: https://readthedocs.org/projects/sequali/badge/?version=latest
   :target: https://sequali.readthedocs.io/en/latest/?badge=latest
   :alt:
 
-.. image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
+.. |coverage-shield| image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
   :target: https://codecov.io/gh/rhpvorderman/sequali
   :alt:
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
+.. |zenodo-shield| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
   :target: https://doi.org/10.5281/zenodo.10854010
   :alt:
 
+|python-version-shield| |conda-version-shield| |python-install-version-shield|
+|license-shield| |docs-shield| |coverage-shield| |zenodo-shield|
+
 ========
 Sequali
 ========
 
 .. introduction start
 
 Sequence quality metrics for FASTQ and uBAM files.
@@ -40,22 +43,25 @@
 + Informative graphs that allow for judging the quality of a sequence at
   a quick glance.
 + Overrepresentation analysis using 21 bp sequence fragments. Overrepresented
   sequences are checked against the NCBI univec database.
 + Estimate duplication rate using a `fingerprint subsampling technique which is
   also used in filesystem duplication estimation
   <https://www.usenix.org/system/files/conference/atc13/atc13-xie.pdf>`_.
-+ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences.
++ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences
+  for single read data.
++ Determines adapters by overlap analysis for paired read data.
++ Insert size metrics for paired read data.
 + Per tile quality plots for illumina reads.
 + Channel and other plots for nanopore reads.
 + FASTQ and unaligned BAM are supported. See "Supported formats".
 
 Example reports:
 
-+ `GM24385_1.fastq.gz <https://github.com/rhpvorderman/sequali/files/14725146/GM24385_1.fastq.gz.html.zip>`_;
++ `GM24385_1.fastq.gz <https://sequali.readthedocs.io/en/latest/GM24385_1.fastq.gz.html>`_;
   HG002 (Genome In A Bottle) on ultra-long Nanopore Sequencing. `Sequence file download <https://ftp-trace.ncbi.nlm.nih.gov/ReferenceSamples/giab/data/AshkenazimTrio/HG002_NA24385_son/UCSC_Ultralong_OxfordNanopore_Promethion/GM24385_1.fastq.gz>`_.
 
 .. introduction end
 
 For more information check `the documentation <https://sequali.readthedocs.io>`_.
 
 Supported formats
@@ -63,19 +69,19 @@
 
 .. formats start
 
 - FASTQ. Only the Sanger variation with a phred offset of 33 and the error rate
   calculation of 10 ^ (-phred/10) is supported. All sequencers use this
   format today.
 
+  - Paired end sequencing data is supported.
   - For sequences called by illumina base callers an additional plot with the
     per tile quality will be provided.
   - For sequences called by guppy additional plots for nanopore specific
     data will be provided.
-
 - unaligned BAM. Any alignment flags are currently ignored.
 
   - For uBAM data as delivered by dorado additional nanopore plots will be
     provided.
 
 .. formats end
```

### Comparing `sequali-0.7.1/docs/_static/images/fingerprint.fodg` & `sequali-0.8.0/docs/_static/images/fingerprint.fodg`

 * *Files 20% similar despite different names*

#### Comparing `sequali-0.7.1/docs/_static/images/fingerprint.fodg` & `sequali-0.8.0/docs/_static/images/fingerprint.fodg`

```diff
@@ -1,23 +1,23 @@
 <?xml version="1.0" encoding="utf-8"?>
 <office:document xmlns:anim="urn:oasis:names:tc:opendocument:xmlns:animation:1.0" xmlns:smil="urn:oasis:names:tc:opendocument:xmlns:smil-compatible:1.0" xmlns:presentation="urn:oasis:names:tc:opendocument:xmlns:presentation:1.0" xmlns:css3t="http://www.w3.org/TR/css3-text/" xmlns:grddl="http://www.w3.org/2003/g/data-view#" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xforms="http://www.w3.org/2002/xforms" xmlns:dom="http://www.w3.org/2001/xml-events" xmlns:script="urn:oasis:names:tc:opendocument:xmlns:script:1.0" xmlns:form="urn:oasis:names:tc:opendocument:xmlns:form:1.0" xmlns:math="http://www.w3.org/1998/Math/MathML" xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0" xmlns:ooo="http://openoffice.org/2004/office" xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0" xmlns:config="urn:oasis:names:tc:opendocument:xmlns:config:1.0" xmlns:ooow="http://openoffice.org/2004/writer" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:drawooo="http://openoffice.org/2010/draw" xmlns:oooc="http://openoffice.org/2004/calc" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:calcext="urn:org:documentfoundation:names:experimental:calc:xmlns:calcext:1.0" xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0" xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0" xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2" xmlns:tableooo="http://openoffice.org/2009/table" xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0" xmlns:dr3d="urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0" xmlns:rpt="http://openoffice.org/2005/report" xmlns:formx="urn:openoffice:names:experimental:ooxml-odf-interop:xmlns:form:1.0" xmlns:svg="urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0" xmlns:chart="urn:oasis:names:tc:opendocument:xmlns:chart:1.0" xmlns:officeooo="http://openoffice.org/2009/office" xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0" xmlns:field="urn:openoffice:names:experimental:ooo-ms-interop:xmlns:field:1.0" xmlns:number="urn:oasis:names:tc:opendocument:xmlns:datastyle:1.0" xmlns:meta="urn:oasis:names:tc:opendocument:xmlns:meta:1.0" xmlns:loext="urn:org:documentfoundation:names:experimental:office:xmlns:loext:1.0" office:version="1.3" office:mimetype="application/vnd.oasis.opendocument.graphics">
   <office:meta>
     <meta:initial-creator>Ruben Vorderman</meta:initial-creator>
     <meta:creation-date>2024-03-27T13:04:54.561630813</meta:creation-date>
-    <dc:date>2024-03-27T13:18:01.085215758</dc:date>
-    <dc:creator>Ruben Vorderman</dc:creator>
-    <meta:editing-duration>PT13M5S</meta:editing-duration>
-    <meta:editing-cycles>4</meta:editing-cycles>
+    <dc:date>2024-05-06T12:58:13.871777078</dc:date>
+    <dc:creator>Vorderman, R.H.P. (MOLEPI)</dc:creator>
+    <meta:editing-duration>PT27M17S</meta:editing-duration>
+    <meta:editing-cycles>8</meta:editing-cycles>
     <meta:generator>LibreOffice/7.4.7.2$Linux_X86_64 LibreOffice_project/40$Build-2</meta:generator>
-    <meta:document-statistic meta:object-count="12"/>
+    <meta:document-statistic meta:object-count="16"/>
   </office:meta>
   <office:settings>
     <config:config-item-set config:name="ooo:view-settings">
-      <config:config-item config:name="VisibleAreaTop" config:type="int">-3995</config:config-item>
-      <config:config-item config:name="VisibleAreaLeft" config:type="int">-3332</config:config-item>
+      <config:config-item config:name="VisibleAreaTop" config:type="int">-2465</config:config-item>
+      <config:config-item config:name="VisibleAreaLeft" config:type="int">-12447</config:config-item>
       <config:config-item config:name="VisibleAreaWidth" config:type="int">14099</config:config-item>
       <config:config-item config:name="VisibleAreaHeight" config:type="int">9999</config:config-item>
       <config:config-item-map-indexed config:name="Views">
         <config:config-item-map-entry>
           <config:config-item config:name="ViewId" config:type="string">view1</config:config-item>
           <config:config-item config:name="GridIsVisible" config:type="boolean">true</config:config-item>
           <config:config-item config:name="GridIsFront" config:type="boolean">false</config:config-item>
@@ -39,18 +39,18 @@
           <config:config-item config:name="PageKind" config:type="short">0</config:config-item>
           <config:config-item config:name="SelectedPage" config:type="short">0</config:config-item>
           <config:config-item config:name="IsLayerMode" config:type="boolean">true</config:config-item>
           <config:config-item config:name="IsDoubleClickTextEdit" config:type="boolean">true</config:config-item>
           <config:config-item config:name="IsClickChangeRotation" config:type="boolean">true</config:config-item>
           <config:config-item config:name="SlidesPerRow" config:type="short">4</config:config-item>
           <config:config-item config:name="EditMode" config:type="int">0</config:config-item>
-          <config:config-item config:name="VisibleAreaTop" config:type="int">-3995</config:config-item>
-          <config:config-item config:name="VisibleAreaLeft" config:type="int">-3332</config:config-item>
-          <config:config-item config:name="VisibleAreaWidth" config:type="int">22662</config:config-item>
-          <config:config-item config:name="VisibleAreaHeight" config:type="int">15597</config:config-item>
+          <config:config-item config:name="VisibleAreaTop" config:type="int">-2465</config:config-item>
+          <config:config-item config:name="VisibleAreaLeft" config:type="int">-12447</config:config-item>
+          <config:config-item config:name="VisibleAreaWidth" config:type="int">32316</config:config-item>
+          <config:config-item config:name="VisibleAreaHeight" config:type="int">14733</config:config-item>
           <config:config-item config:name="GridCoarseWidth" config:type="int">1000</config:config-item>
           <config:config-item config:name="GridCoarseHeight" config:type="int">1000</config:config-item>
           <config:config-item config:name="GridFineWidth" config:type="int">500</config:config-item>
           <config:config-item config:name="GridFineHeight" config:type="int">500</config:config-item>
           <config:config-item config:name="GridSnapWidthXNumerator" config:type="int">1000</config:config-item>
           <config:config-item config:name="GridSnapWidthXDenominator" config:type="int">2</config:config-item>
           <config:config-item config:name="GridSnapWidthYNumerator" config:type="int">1000</config:config-item>
@@ -81,15 +81,15 @@
       <config:config-item config:name="LoadReadonly" config:type="boolean">false</config:config-item>
       <config:config-item config:name="GradientTableURL" config:type="string">$(brandbaseurl)/share/palette%3B$(user)/config/standard.sog</config:config-item>
       <config:config-item config:name="EmbedComplexScriptFonts" config:type="boolean">true</config:config-item>
       <config:config-item config:name="EmbedOnlyUsedFonts" config:type="boolean">false</config:config-item>
       <config:config-item config:name="HatchTableURL" config:type="string">$(brandbaseurl)/share/palette%3B$(user)/config/standard.soh</config:config-item>
       <config:config-item config:name="DashTableURL" config:type="string">$(brandbaseurl)/share/palette%3B$(user)/config/standard.sod</config:config-item>
       <config:config-item config:name="UpdateFromTemplate" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="ColorTableURL" config:type="string">$(brandbaseurl)/share/palette%3B$(user)/config/html.soc</config:config-item>
+      <config:config-item config:name="ColorTableURL" config:type="string">$(brandbaseurl)/share/palette%3B$(user)/config/standard.soc</config:config-item>
       <config:config-item config:name="EmbedLatinScriptFonts" config:type="boolean">true</config:config-item>
       <config:config-item config:name="PrintQuality" config:type="int">0</config:config-item>
       <config:config-item config:name="LineEndTableURL" config:type="string">$(brandbaseurl)/share/palette%3B$(user)/config/standard.soe</config:config-item>
       <config:config-item config:name="IsPrintBookletBack" config:type="boolean">true</config:config-item>
       <config:config-item config:name="IsPrintBookletFront" config:type="boolean">true</config:config-item>
       <config:config-item config:name="ScaleDenominator" config:type="int">1</config:config-item>
       <config:config-item config:name="ImagePreferredDPI" config:type="int">0</config:config-item>
@@ -104,30 +104,32 @@
       <config:config-item config:name="SaveThumbnail" config:type="boolean">true</config:config-item>
       <config:config-item config:name="IsPrintTime" config:type="boolean">false</config:config-item>
       <config:config-item config:name="IsPrintDate" config:type="boolean">false</config:config-item>
       <config:config-item config:name="IsPrintPageName" config:type="boolean">false</config:config-item>
       <config:config-item config:name="IsKernAsianPunctuation" config:type="boolean">false</config:config-item>
       <config:config-item config:name="PrinterPaperFromSetup" config:type="boolean">false</config:config-item>
       <config:config-item config:name="ParagraphSummation" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrinterSetup" config:type="base64Binary"/>
-      <config:config-item config:name="PrinterName" config:type="string"/>
+      <config:config-item config:name="PrinterSetup" config:type="base64Binary">oAH+/1JJQ09IX01QX0MzMDdfNTgzODc5MUNGMURCXwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQ1VQUzpSSUNPSF9NUF9DMzA3XzU4Mzg3OTFDRjFEQgAWAAMAwQAAAAAAAAAEAAhSAAAEdAAASm9iRGF0YSAxCnByaW50ZXI9UklDT0hfTVBfQzMwN181ODM4NzkxQ0YxREJfCm9yaWVudGF0aW9uPVBvcnRyYWl0CmNvcGllcz0xCmNvbGxhdGU9ZmFsc2UKbWFyZ2luYWRqdXN0bWVudD0wLDAsMCwwCmNvbG9yZGVwdGg9MjQKcHNsZXZlbD0wCnBkZmRldmljZT0xCmNvbG9yZGV2aWNlPTAKUFBEQ29udGV4dERhdGEKUGFnZVNpemU6QTQAABIAQ09NUEFUX0RVUExFWF9NT0RFDwBEdXBsZXhNb2RlOjpPZmY=</config:config-item>
+      <config:config-item config:name="PrinterName" config:type="string">RICOH_MP_C307_5838791CF1DB_</config:config-item>
       <config:config-item config:name="DefaultTabStop" config:type="int">1250</config:config-item>
     </config:config-item-set>
   </office:settings>
   <office:scripts>
     <office:script script:language="ooo:Basic">
       <ooo:libraries xmlns:ooo="http://openoffice.org/2004/office" xmlns:xlink="http://www.w3.org/1999/xlink"/>
     </office:script>
   </office:scripts>
   <office:font-face-decls>
     <style:font-face style:name="DejaVu Sans" svg:font-family="'DejaVu Sans'" style:font-family-generic="system" style:font-pitch="variable"/>
     <style:font-face style:name="FreeSans" svg:font-family="FreeSans" style:font-family-generic="system" style:font-pitch="variable"/>
     <style:font-face style:name="Liberation Sans" svg:font-family="'Liberation Sans'" style:font-family-generic="roman" style:font-pitch="variable"/>
     <style:font-face style:name="Liberation Serif" svg:font-family="'Liberation Serif'" style:font-family-generic="roman" style:font-pitch="variable"/>
     <style:font-face style:name="Noto Sans" svg:font-family="'Noto Sans'" style:font-family-generic="roman" style:font-pitch="variable"/>
+    <style:font-face style:name="Noto Sans CJK SC" svg:font-family="'Noto Sans CJK SC'" style:font-family-generic="system" style:font-pitch="variable"/>
+    <style:font-face style:name="Noto Sans Devanagari" svg:font-family="'Noto Sans Devanagari'" style:font-family-generic="system" style:font-pitch="variable"/>
   </office:font-face-decls>
   <office:styles>
     <draw:gradient draw:name="Blauw_20_gevuld" draw:display-name="Blauw gevuld" draw:style="linear" draw:start-color="#729fcf" draw:end-color="#355269" draw:start-intensity="100%" draw:end-intensity="100%" draw:angle="30deg" draw:border="0%"/>
     <draw:gradient draw:name="Geel_20_gevuld" draw:display-name="Geel gevuld" draw:style="linear" draw:start-color="#ffde59" draw:end-color="#b47804" draw:start-intensity="100%" draw:end-intensity="100%" draw:angle="30deg" draw:border="0%"/>
     <draw:gradient draw:name="Gevuld" draw:style="linear" draw:start-color="#ffffff" draw:end-color="#cccccc" draw:start-intensity="100%" draw:end-intensity="100%" draw:angle="30deg" draw:border="0%"/>
     <draw:gradient draw:name="Gradient_20_1" draw:display-name="Gradient 1" draw:style="linear" draw:start-color="#3465a4" draw:end-color="#ffffff" draw:start-intensity="100%" draw:end-intensity="100%" draw:angle="0deg" draw:border="0%"/>
     <draw:gradient draw:name="Groen_20_gevuld" draw:display-name="Groen gevuld" draw:style="linear" draw:start-color="#77bc65" draw:end-color="#127622" draw:start-intensity="100%" draw:end-intensity="100%" draw:angle="30deg" draw:border="0%"/>
@@ -155,15 +157,15 @@
     <draw:marker draw:name="Arrow" svg:viewBox="0 0 20 30" svg:d="M10 0l-10 30h20z"/>
     <draw:marker draw:name="Dimension_20_Lines" draw:display-name="Dimension Lines" svg:viewBox="0 0 836 110" svg:d="M0 0h278 278 280v36 36 38h-278-278-280v-36-36z"/>
     <draw:marker draw:name="Pijlpunten_20_1" draw:display-name="Pijlpunten 1" svg:viewBox="0 0 836 110" svg:d="M0 0h278 278 280v36 36 38h-278-278-280v-36-36z"/>
     <draw:marker draw:name="Pijlpunten_20_2" draw:display-name="Pijlpunten 2" svg:viewBox="0 0 836 946" svg:d="M0 0v110h418 418v-110zM418 110l-418 836h836z"/>
     <draw:stroke-dash draw:name="Dash_20_Dot_20_1" draw:display-name="Dash Dot 1" draw:style="rect" draw:dots1="1" draw:dots1-length="0.02cm" draw:dots2="1" draw:dots2-length="0.02cm" draw:distance="0.02cm"/>
     <style:default-style style:family="graphic">
       <style:graphic-properties svg:stroke-color="#3465a4" draw:fill-color="#729fcf" fo:wrap-option="no-wrap"/>
-      <style:paragraph-properties style:text-autospace="ideograph-alpha" style:punctuation-wrap="simple" style:line-break="strict" style:writing-mode="lr-tb" style:font-independent-line-spacing="false">
+      <style:paragraph-properties style:text-autospace="ideograph-alpha" style:punctuation-wrap="simple" style:line-break="strict" style:font-independent-line-spacing="false">
         <style:tab-stops/>
       </style:paragraph-properties>
       <style:text-properties style:use-window-font-color="true" loext:opacity="0%" loext:color-lum-mod="100%" loext:color-lum-off="0%" style:font-name="Liberation Serif" fo:font-size="24pt" fo:language="en" fo:country="US" style:font-name-asian="DejaVu Sans" style:font-size-asian="24pt" style:language-asian="zh" style:country-asian="CN" style:font-name-complex="DejaVu Sans" style:font-size-complex="24pt" style:language-complex="hi" style:country-complex="IN"/>
     </style:default-style>
     <style:style style:name="standard" style:family="graphic">
       <style:graphic-properties draw:stroke="solid" svg:stroke-width="0cm" svg:stroke-color="#3465a4" draw:marker-start-width="0.2cm" draw:marker-start-center="false" draw:marker-end-width="0.2cm" draw:marker-end-center="false" draw:fill="solid" draw:fill-color="#729fcf" draw:textarea-horizontal-align="justify" fo:padding-top="0.125cm" fo:padding-bottom="0.125cm" fo:padding-left="0.25cm" fo:padding-right="0.25cm" fo:wrap-option="wrap" draw:shadow="hidden" draw:shadow-offset-x="0.2cm" draw:shadow-offset-y="0.2cm" draw:shadow-color="#808080">
         <text:list-style style:name="standard">
@@ -209,18 +211,18 @@
           </text:list-level-style-bullet>
         </text:list-style>
       </style:graphic-properties>
       <style:paragraph-properties fo:margin-left="0cm" fo:margin-right="0cm" fo:margin-top="0cm" fo:margin-bottom="0cm" fo:line-height="100%" fo:text-indent="0cm"/>
       <style:text-properties fo:font-variant="normal" fo:text-transform="none" style:use-window-font-color="true" loext:opacity="0%" loext:color-lum-mod="100%" loext:color-lum-off="0%" style:text-outline="false" style:text-line-through-style="none" style:text-line-through-type="none" style:font-name="Liberation Sans" fo:font-family="'Liberation Sans'" style:font-family-generic="roman" style:font-pitch="variable" fo:font-size="18pt" fo:font-style="normal" fo:text-shadow="none" style:text-underline-style="none" fo:font-weight="normal" style:letter-kerning="true" style:font-name-asian="DejaVu Sans" style:font-family-asian="'DejaVu Sans'" style:font-family-generic-asian="system" style:font-pitch-asian="variable" style:font-size-asian="18pt" style:font-style-asian="normal" style:font-weight-asian="normal" style:font-name-complex="FreeSans" style:font-family-complex="FreeSans" style:font-family-generic-complex="system" style:font-pitch-complex="variable" style:font-size-complex="18pt" style:font-style-complex="normal" style:font-weight-complex="normal" style:text-emphasize="none" style:font-relief="none" style:text-overline-style="none" style:text-overline-color="font-color"/>
     </style:style>
     <style:style style:name="objectwithoutfill" style:family="graphic" style:parent-style-name="standard">
-      <style:graphic-properties draw:stroke-dash="Dash_20_Dot_20_1" draw:fill="none" draw:fill-gradient-name="Gradient_20_1" draw:fill-hatch-name="Red_20_90_20_Degrees_20_Crossed_20_1" draw:fill-image-name="Bitmap_20_1" fo:padding-top="0.13cm"/>
+      <style:graphic-properties draw:stroke-dash="Dash_20_Dot_20_1" draw:fill="none" fo:padding-top="0.13cm"/>
       <style:paragraph-properties fo:margin-top="0cm" fo:margin-bottom="0.7cm"/>
     </style:style>
-    <style:style style:name="Object_20_zonder_20_vulling_20_en_20_geen_20_lijn" style:display-name="Object zonder vulling en geen lijn" style:family="graphic" style:parent-style-name="standard">
+    <style:style style:name="Object_20_with_20_no_20_fill_20_and_20_no_20_line" style:display-name="Object with no fill and no line" style:family="graphic" style:parent-style-name="standard">
       <style:graphic-properties draw:stroke="none" draw:fill="none"/>
     </style:style>
     <style:style style:name="Text" style:family="graphic">
       <style:graphic-properties draw:stroke="solid" svg:stroke-color="#cccccc" draw:fill="solid" draw:fill-color="#eeeeee"/>
       <style:text-properties style:font-name="Noto Sans" fo:font-family="'Noto Sans'" style:font-family-generic="roman" style:font-pitch="variable"/>
     </style:style>
     <style:style style:name="A4" style:family="graphic" style:parent-style-name="Text">
@@ -304,14 +306,17 @@
     </style:style>
     <style:style style:name="Arrow_20_Line" style:display-name="Arrow Line" style:family="graphic" style:parent-style-name="Lines">
       <style:graphic-properties draw:marker-start="Arrow" draw:marker-start-width="0.2cm" draw:marker-end="Arrow" draw:marker-end-width="0.2cm" draw:show-unit="true"/>
     </style:style>
     <style:style style:name="Arrow_20_Dashed" style:display-name="Arrow Dashed" style:family="graphic" style:parent-style-name="Lines">
       <style:graphic-properties draw:stroke="dash"/>
     </style:style>
+    <style:style style:name="Object_20_zonder_20_vulling_20_en_20_geen_20_lijn" style:display-name="Object zonder vulling en geen lijn" style:family="graphic" style:parent-style-name="standard">
+      <style:graphic-properties draw:stroke="none" draw:fill="none"/>
+    </style:style>
   </office:styles>
   <office:automatic-styles>
     <style:page-layout style:name="PM0">
       <style:page-layout-properties fo:margin-top="1cm" fo:margin-bottom="1cm" fo:margin-left="1cm" fo:margin-right="1cm" fo:page-width="29.7cm" fo:page-height="21cm" style:print-orientation="landscape"/>
     </style:page-layout>
     <style:style style:name="dp1" style:family="drawing-page">
       <style:drawing-page-properties draw:background-size="border" draw:fill="none"/>
@@ -319,15 +324,14 @@
     <style:style style:name="dp2" style:family="drawing-page"/>
     <style:style style:name="gr1" style:family="graphic" style:parent-style-name="standard">
       <style:graphic-properties draw:stroke="none" draw:fill="solid" draw:fill-color="#6495ed" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.75cm" fo:min-width="11.5cm"/>
       <style:paragraph-properties style:writing-mode="lr-tb"/>
     </style:style>
     <style:style style:name="gr2" style:family="graphic" style:parent-style-name="objectwithoutfill">
       <style:graphic-properties svg:stroke-width="0.053cm" svg:stroke-color="#000000" draw:marker-start="Dimension_20_Lines" draw:marker-start-width="0.5cm" draw:marker-end="Dimension_20_Lines" draw:marker-end-width="0.5cm" svg:stroke-linecap="square" draw:fill="none" draw:textarea-vertical-align="bottom" fo:padding-top="0.151cm" fo:padding-bottom="0.151cm" fo:padding-left="0.276cm" fo:padding-right="0.276cm"/>
-      <style:paragraph-properties style:writing-mode="lr-tb"/>
     </style:style>
     <style:style style:name="gr3" style:family="graphic" style:parent-style-name="standard">
       <style:graphic-properties draw:stroke="none" draw:fill-color="#c0c0c0" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.75cm" fo:min-width="0.5cm"/>
     </style:style>
     <style:style style:name="gr4" style:family="graphic" style:parent-style-name="standard">
       <style:graphic-properties draw:stroke="none" draw:fill="solid" draw:fill-color="#6495ed" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.75cm" fo:min-width="7.5cm"/>
       <style:paragraph-properties style:writing-mode="lr-tb"/>
@@ -335,30 +339,45 @@
     <style:style style:name="gr5" style:family="graphic" style:parent-style-name="standard">
       <style:graphic-properties draw:stroke="none" draw:fill="solid" draw:fill-color="#6495ed" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.75cm" fo:min-width="1cm"/>
       <style:paragraph-properties style:writing-mode="lr-tb"/>
     </style:style>
     <style:style style:name="gr6" style:family="graphic" style:parent-style-name="standard">
       <style:graphic-properties draw:stroke="none" draw:fill-color="#c0c0c0" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.75cm" fo:min-width="1cm"/>
     </style:style>
+    <style:style style:name="gr7" style:family="graphic" style:parent-style-name="standard">
+      <style:graphic-properties draw:stroke="none" svg:stroke-linecap="butt" draw:fill-color="#6495ed" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.751cm" fo:min-width="6.525cm"/>
+      <style:paragraph-properties style:writing-mode="lr-tb"/>
+    </style:style>
+    <style:style style:name="gr8" style:family="graphic" style:parent-style-name="standard">
+      <style:graphic-properties draw:stroke="none" svg:stroke-linecap="butt" draw:fill-color="#c0c0c0" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.751cm" fo:min-width="0.674cm"/>
+    </style:style>
+    <style:style style:name="gr9" style:family="graphic" style:parent-style-name="standard">
+      <style:graphic-properties draw:stroke="none" svg:stroke-linecap="butt" draw:fill-color="#6495ed" draw:textarea-horizontal-align="justify" draw:textarea-vertical-align="middle" draw:auto-grow-height="false" fo:min-height="0.751cm" fo:min-width="6.057cm"/>
+      <style:paragraph-properties style:writing-mode="lr-tb"/>
+    </style:style>
     <style:style style:name="P1" style:family="paragraph">
-      <style:paragraph-properties fo:text-align="center"/>
+      <style:paragraph-properties fo:text-align="center" style:writing-mode="lr-tb"/>
     </style:style>
     <style:style style:name="P2" style:family="paragraph">
       <loext:graphic-properties draw:fill="solid" draw:fill-color="#6495ed"/>
-      <style:paragraph-properties fo:text-align="center"/>
+      <style:paragraph-properties fo:text-align="center" style:writing-mode="lr-tb"/>
     </style:style>
     <style:style style:name="P3" style:family="paragraph">
-      <style:paragraph-properties fo:margin-top="0cm" fo:margin-bottom="0cm" fo:line-height="100%" fo:text-align="center"/>
+      <loext:graphic-properties draw:fill="none"/>
+      <style:paragraph-properties fo:margin-top="0cm" fo:margin-bottom="0cm" fo:line-height="100%" fo:text-align="center" style:writing-mode="lr-tb"/>
     </style:style>
     <style:style style:name="P4" style:family="paragraph">
-      <loext:graphic-properties draw:fill="none"/>
-      <style:paragraph-properties fo:margin-top="0cm" fo:margin-bottom="0cm" fo:line-height="100%" fo:text-align="center"/>
+      <loext:graphic-properties draw:fill-color="#c0c0c0"/>
+      <style:paragraph-properties fo:text-align="center"/>
     </style:style>
     <style:style style:name="P5" style:family="paragraph">
-      <loext:graphic-properties draw:fill-color="#c0c0c0"/>
+      <style:paragraph-properties fo:text-align="center"/>
+    </style:style>
+    <style:style style:name="P6" style:family="paragraph">
+      <loext:graphic-properties draw:fill-color="#6495ed"/>
       <style:paragraph-properties fo:text-align="center"/>
     </style:style>
     <text:list-style style:name="L1">
       <text:list-level-style-bullet text:level="1" text:bullet-char="●">
         <style:list-level-properties text:min-label-width="0.6cm"/>
         <style:text-properties fo:font-family="StarSymbol" style:use-window-font-color="true" fo:font-size="45%"/>
       </text:list-level-style-bullet>
@@ -413,51 +432,107 @@
   <office:body>
     <office:drawing>
       <draw:page draw:name="page1" draw:style-name="dp2" draw:master-page-name="Standaard">
         <draw:custom-shape draw:style-name="gr1" draw:text-style-name="P2" draw:layer="layout" svg:width="12cm" svg:height="1cm" svg:x="1cm" svg:y="1cm">
           <text:p text:style-name="P1">Sequence #1</text:p>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
-        <draw:line draw:style-name="gr2" draw:text-style-name="P4" draw:layer="layout" svg:x1="1cm" svg:y1="3cm" svg:x2="5cm" svg:y2="3cm">
-          <text:p text:style-name="P3"/>
+        <draw:line draw:style-name="gr2" draw:text-style-name="P3" draw:layer="layout" svg:x1="1cm" svg:y1="3cm" svg:x2="5cm" svg:y2="3cm">
+          <text:p/>
         </draw:line>
-        <draw:line draw:style-name="gr2" draw:text-style-name="P4" draw:layer="layout" svg:x1="9cm" svg:y1="3cm" svg:x2="13cm" svg:y2="3cm">
+        <draw:line draw:style-name="gr2" draw:text-style-name="P3" draw:layer="layout" svg:x1="9cm" svg:y1="3cm" svg:x2="13cm" svg:y2="3cm">
           <text:p/>
         </draw:line>
-        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P5" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="5cm" svg:y="2.5cm">
+        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P4" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="5cm" svg:y="2.5cm">
           <text:p/>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
-        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P5" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="8cm" svg:y="2.5cm">
+        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P4" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="8cm" svg:y="2.5cm">
           <text:p/>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
         <draw:custom-shape draw:style-name="gr4" draw:text-style-name="P2" draw:layer="layout" svg:width="8cm" svg:height="1cm" svg:x="1cm" svg:y="4cm">
           <text:p text:style-name="P1">Sequence #2</text:p>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
-        <draw:line draw:style-name="gr2" draw:text-style-name="P4" draw:layer="layout" svg:x1="1cm" svg:y1="6cm" svg:x2="4cm" svg:y2="6cm">
+        <draw:line draw:style-name="gr2" draw:text-style-name="P3" draw:layer="layout" svg:x1="1cm" svg:y1="6cm" svg:x2="4cm" svg:y2="6cm">
           <text:p/>
         </draw:line>
-        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P5" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="4cm" svg:y="5.5cm">
+        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P4" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="4cm" svg:y="5.5cm">
           <text:p/>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
-        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P5" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="5cm" svg:y="5.5cm">
+        <draw:custom-shape draw:style-name="gr3" draw:text-style-name="P4" draw:layer="layout" svg:width="1cm" svg:height="1cm" svg:x="5cm" svg:y="5.5cm">
           <text:p/>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
         <draw:custom-shape draw:style-name="gr5" draw:text-style-name="P2" draw:layer="layout" svg:width="1.5cm" svg:height="1cm" svg:x="11.5cm" svg:y="4cm">
           <text:p text:style-name="P1">#3</text:p>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
-        <draw:custom-shape draw:style-name="gr6" draw:text-style-name="P5" draw:layer="layout" svg:width="1.5cm" svg:height="1cm" svg:x="11.5cm" svg:y="5.5cm">
+        <draw:custom-shape draw:style-name="gr6" draw:text-style-name="P4" draw:layer="layout" svg:width="1.5cm" svg:height="1cm" svg:x="11.5cm" svg:y="5.5cm">
           <text:p/>
           <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:type="rectangle" draw:enhanced-path="M 0 0 L 21600 0 21600 21600 0 21600 0 0 Z N"/>
         </draw:custom-shape>
-        <draw:line draw:style-name="gr2" draw:text-style-name="P4" draw:layer="layout" svg:x1="6cm" svg:y1="6cm" svg:x2="9cm" svg:y2="6cm">
+        <draw:line draw:style-name="gr2" draw:text-style-name="P3" draw:layer="layout" svg:x1="6cm" svg:y1="6cm" svg:x2="9cm" svg:y2="6cm">
           <text:p/>
         </draw:line>
+        <draw:custom-shape draw:style-name="gr7" draw:text-style-name="P6" draw:layer="layout" svg:width="7.5cm" svg:height="1cm" svg:x="5.5cm" svg:y="8cm">
+          <text:p text:style-name="P5">Sequence #4 R2</text:p>
+          <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:text-areas="?f7 ?f0 21600 ?f2" draw:type="left-arrow" draw:modifiers="1370.69724036795 0" draw:enhanced-path="M 21600 ?f0 L ?f1 ?f0 ?f1 0 0 10800 ?f1 21600 ?f1 ?f2 21600 ?f2 Z N">
+            <draw:equation draw:name="f0" draw:formula="$1 "/>
+            <draw:equation draw:name="f1" draw:formula="$0 "/>
+            <draw:equation draw:name="f2" draw:formula="21600-$1 "/>
+            <draw:equation draw:name="f3" draw:formula="21600-?f1 "/>
+            <draw:equation draw:name="f4" draw:formula="?f3 *?f0 /10800"/>
+            <draw:equation draw:name="f5" draw:formula="?f1 +?f4 "/>
+            <draw:equation draw:name="f6" draw:formula="?f1 *?f0 /10800"/>
+            <draw:equation draw:name="f7" draw:formula="?f1 -?f6 "/>
+            <draw:handle draw:handle-position="$0 $1" draw:handle-range-x-minimum="0" draw:handle-range-x-maximum="21600" draw:handle-range-y-minimum="0" draw:handle-range-y-maximum="10800"/>
+          </draw:enhanced-geometry>
+        </draw:custom-shape>
+        <draw:custom-shape draw:style-name="gr8" draw:text-style-name="P4" draw:layer="layout" svg:width="1.5cm" svg:height="1cm" svg:x="11.5cm" svg:y="7cm">
+          <text:p/>
+          <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:text-areas="?f7 ?f0 21600 ?f2" draw:type="left-arrow" draw:modifiers="4716.49670065987 0" draw:enhanced-path="M 21600 ?f0 L ?f1 ?f0 ?f1 0 0 10800 ?f1 21600 ?f1 ?f2 21600 ?f2 Z N">
+            <draw:equation draw:name="f0" draw:formula="$1 "/>
+            <draw:equation draw:name="f1" draw:formula="$0 "/>
+            <draw:equation draw:name="f2" draw:formula="21600-$1 "/>
+            <draw:equation draw:name="f3" draw:formula="21600-?f1 "/>
+            <draw:equation draw:name="f4" draw:formula="?f3 *?f0 /10800"/>
+            <draw:equation draw:name="f5" draw:formula="?f1 +?f4 "/>
+            <draw:equation draw:name="f6" draw:formula="?f1 *?f0 /10800"/>
+            <draw:equation draw:name="f7" draw:formula="?f1 -?f6 "/>
+            <draw:handle draw:handle-position="$0 $1" draw:handle-range-x-minimum="0" draw:handle-range-x-maximum="21600" draw:handle-range-y-minimum="0" draw:handle-range-y-maximum="10800"/>
+          </draw:enhanced-geometry>
+        </draw:custom-shape>
+        <draw:custom-shape draw:style-name="gr8" draw:text-style-name="P4" draw:layer="layout" svg:width="1.5cm" svg:height="1cm" draw:transform="rotate (-3.14159265358979) translate (2.5cm 9cm)">
+          <text:p/>
+          <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:text-areas="?f7 ?f0 21600 ?f2" draw:type="left-arrow" draw:modifiers="4716.49670065987 0" draw:enhanced-path="M 21600 ?f0 L ?f1 ?f0 ?f1 0 0 10800 ?f1 21600 ?f1 ?f2 21600 ?f2 Z N">
+            <draw:equation draw:name="f0" draw:formula="$1 "/>
+            <draw:equation draw:name="f1" draw:formula="$0 "/>
+            <draw:equation draw:name="f2" draw:formula="21600-$1 "/>
+            <draw:equation draw:name="f3" draw:formula="21600-?f1 "/>
+            <draw:equation draw:name="f4" draw:formula="?f3 *?f0 /10800"/>
+            <draw:equation draw:name="f5" draw:formula="?f1 +?f4 "/>
+            <draw:equation draw:name="f6" draw:formula="?f1 *?f0 /10800"/>
+            <draw:equation draw:name="f7" draw:formula="?f1 -?f6 "/>
+            <draw:handle draw:handle-position="$0 $1" draw:handle-range-x-minimum="0" draw:handle-range-x-maximum="21600" draw:handle-range-y-minimum="0" draw:handle-range-y-maximum="10800"/>
+          </draw:enhanced-geometry>
+        </draw:custom-shape>
+        <draw:custom-shape draw:style-name="gr9" draw:text-style-name="P6" draw:layer="layout" svg:width="7cm" svg:height="1cm" svg:x="1cm" svg:y="7cm">
+          <text:p text:style-name="P5">Sequence #4 R1</text:p>
+          <draw:enhanced-geometry svg:viewBox="0 0 21600 21600" draw:text-areas="?f7 ?f0 21600 ?f2" draw:mirror-horizontal="true" draw:type="left-arrow" draw:modifiers="1370.69724036795 0" draw:enhanced-path="M 21600 ?f0 L ?f1 ?f0 ?f1 0 0 10800 ?f1 21600 ?f1 ?f2 21600 ?f2 Z N">
+            <draw:equation draw:name="f0" draw:formula="$1 "/>
+            <draw:equation draw:name="f1" draw:formula="$0 "/>
+            <draw:equation draw:name="f2" draw:formula="21600-$1 "/>
+            <draw:equation draw:name="f3" draw:formula="21600-?f1 "/>
+            <draw:equation draw:name="f4" draw:formula="?f3 *?f0 /10800"/>
+            <draw:equation draw:name="f5" draw:formula="?f1 +?f4 "/>
+            <draw:equation draw:name="f6" draw:formula="?f1 *?f0 /10800"/>
+            <draw:equation draw:name="f7" draw:formula="?f1 -?f6 "/>
+            <draw:handle draw:handle-position="$0 $1" draw:handle-range-x-minimum="0" draw:handle-range-x-maximum="21600" draw:handle-range-y-minimum="0" draw:handle-range-y-maximum="10800"/>
+          </draw:enhanced-geometry>
+        </draw:custom-shape>
       </draw:page>
     </office:drawing>
   </office:body>
 </office:document>
```

### Comparing `sequali-0.7.1/docs/_static/images/fingerprint.svg` & `sequali-0.8.0/docs/_static/images/fingerprint.svg`

 * *Files 9% similar despite different names*

```diff
@@ -4,934 +4,1092 @@
 00000030: 2073 7667 2050 5542 4c49 4320 222d 2f2f   svg PUBLIC "-//
 00000040: 5733 432f 2f44 5444 2053 5647 2031 2e31  W3C//DTD SVG 1.1
 00000050: 2f2f 454e 2220 2268 7474 703a 2f2f 7777  //EN" "http://ww
 00000060: 772e 7733 2e6f 7267 2f47 7261 7068 6963  w.w3.org/Graphic
 00000070: 732f 5356 472f 312e 312f 4454 442f 7376  s/SVG/1.1/DTD/sv
 00000080: 6731 312e 6474 6422 3e0a 3c73 7667 2076  g11.dtd">.<svg v
 00000090: 6572 7369 6f6e 3d22 312e 3222 2077 6964  ersion="1.2" wid
-000000a0: 7468 3d22 3132 302e 3031 6d6d 2220 6865  th="120.01mm" he
-000000b0: 6967 6874 3d22 3535 2e30 316d 6d22 2076  ight="55.01mm" v
-000000c0: 6965 7742 6f78 3d22 3130 3030 2031 3030  iewBox="1000 100
-000000d0: 3020 3132 3030 3120 3535 3031 2220 7072  0 12001 5501" pr
-000000e0: 6573 6572 7665 4173 7065 6374 5261 7469  eserveAspectRati
-000000f0: 6f3d 2278 4d69 6459 4d69 6422 2066 696c  o="xMidYMid" fil
-00000100: 6c2d 7275 6c65 3d22 6576 656e 6f64 6422  l-rule="evenodd"
-00000110: 2073 7472 6f6b 652d 7769 6474 683d 2232   stroke-width="2
-00000120: 382e 3232 3222 2073 7472 6f6b 652d 6c69  8.222" stroke-li
-00000130: 6e65 6a6f 696e 3d22 726f 756e 6422 2078  nejoin="round" x
-00000140: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
-00000150: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-00000160: 2220 786d 6c6e 733a 6f6f 6f3d 2268 7474  " xmlns:ooo="htt
-00000170: 703a 2f2f 786d 6c2e 6f70 656e 6f66 6669  p://xml.openoffi
-00000180: 6365 2e6f 7267 2f73 7667 2f65 7870 6f72  ce.org/svg/expor
-00000190: 7422 2078 6d6c 6e73 3a78 6c69 6e6b 3d22  t" xmlns:xlink="
-000001a0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-000001b0: 672f 3139 3939 2f78 6c69 6e6b 2220 786d  g/1999/xlink" xm
-000001c0: 6c6e 733a 7072 6573 656e 7461 7469 6f6e  lns:presentation
-000001d0: 3d22 6874 7470 3a2f 2f73 756e 2e63 6f6d  ="http://sun.com
-000001e0: 2f78 6d6c 6e73 2f73 7461 726f 6666 6963  /xmlns/staroffic
-000001f0: 652f 7072 6573 656e 7461 7469 6f6e 2220  e/presentation" 
-00000200: 786d 6c6e 733a 736d 696c 3d22 6874 7470  xmlns:smil="http
-00000210: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00000220: 3031 2f53 4d49 4c32 302f 2220 786d 6c6e  01/SMIL20/" xmln
-00000230: 733a 616e 696d 3d22 7572 6e3a 6f61 7369  s:anim="urn:oasi
-00000240: 733a 6e61 6d65 733a 7463 3a6f 7065 6e64  s:names:tc:opend
-00000250: 6f63 756d 656e 743a 786d 6c6e 733a 616e  ocument:xmlns:an
-00000260: 696d 6174 696f 6e3a 312e 3022 2078 6d6c  imation:1.0" xml
-00000270: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-00000280: 223e 0a20 3c64 6566 733e 0a20 203c 666f  ">. <defs>.  <fo
-00000290: 6e74 2069 643d 2245 6d62 6564 6465 6446  nt id="EmbeddedF
-000002a0: 6f6e 745f 3122 2068 6f72 697a 2d61 6476  ont_1" horiz-adv
-000002b0: 2d78 3d22 3230 3438 223e 0a20 2020 3c66  -x="2048">.   <f
-000002c0: 6f6e 742d 6661 6365 2066 6f6e 742d 6661  ont-face font-fa
-000002d0: 6d69 6c79 3d22 4c69 6265 7261 7469 6f6e  mily="Liberation
-000002e0: 2053 616e 7320 656d 6265 6464 6564 2220   Sans embedded" 
-000002f0: 756e 6974 732d 7065 722d 656d 3d22 3230  units-per-em="20
-00000300: 3438 2220 666f 6e74 2d77 6569 6768 743d  48" font-weight=
-00000310: 226e 6f72 6d61 6c22 2066 6f6e 742d 7374  "normal" font-st
-00000320: 796c 653d 226e 6f72 6d61 6c22 2061 7363  yle="normal" asc
-00000330: 656e 743d 2231 3834 3222 2064 6573 6365  ent="1842" desce
-00000340: 6e74 3d22 3431 3922 2f3e 0a20 2020 3c6d  nt="419"/>.   <m
-00000350: 6973 7369 6e67 2d67 6c79 7068 2068 6f72  issing-glyph hor
-00000360: 697a 2d61 6476 2d78 3d22 3230 3438 2220  iz-adv-x="2048" 
-00000370: 643d 224d 2030 2c30 204c 2032 3034 372c  d="M 0,0 L 2047,
-00000380: 3020 3230 3437 2c32 3034 3720 302c 3230  0 2047,2047 0,20
-00000390: 3437 2030 2c30 205a 222f 3e0a 2020 203c  47 0,0 Z"/>.   <
-000003a0: 676c 7970 6820 756e 6963 6f64 653d 2275  glyph unicode="u
-000003b0: 2220 686f 7269 7a2d 6164 762d 783d 2238  " horiz-adv-x="8
-000003c0: 3934 2220 643d 224d 2033 3134 2c31 3038  94" d="M 314,108
-000003d0: 3220 4c20 3331 342c 3339 3620 4320 3331  2 L 314,396 C 31
-000003e0: 342c 3332 3520 3332 312c 3236 3920 3333  4,325 321,269 33
-000003f0: 352c 3233 3020 3334 392c 3139 3120 3337  5,230 349,191 37
-00000400: 312c 3136 3220 3430 322c 3134 3520 3433  1,162 402,145 43
-00000410: 332c 3132 3820 3437 382c 3131 3920 3533  3,128 478,119 53
-00000420: 372c 3131 3920 3632 342c 3131 3920 3639  7,119 624,119 69
-00000430: 322c 3134 3920 3734 322c 3230 3820 3739  2,149 742,208 79
-00000440: 322c 3236 3720 3831 372c 3335 3020 3831  2,267 817,350 81
-00000450: 372c 3435 3520 4c20 3831 372c 3130 3832  7,455 L 817,1082
-00000460: 2039 3937 2c31 3038 3220 3939 372c 3233   997,1082 997,23
-00000470: 3120 4320 3939 372c 3130 3520 3939 392c  1 C 997,105 999,
-00000480: 3238 2031 3030 332c 3020 4c20 3833 332c  28 1003,0 L 833,
-00000490: 3020 4320 3833 322c 3320 3833 322c 3132  0 C 832,3 832,12
-000004a0: 2038 3331 2c32 3720 3833 302c 3432 2038   831,27 830,42 8
-000004b0: 3330 2c35 3920 3832 392c 3738 2038 3238  30,59 829,78 828
-000004c0: 2c39 3720 3832 362c 3133 3220 3832 352c  ,97 826,132 825,
-000004d0: 3138 3520 4c20 3832 322c 3138 3520 4320  185 L 822,185 C 
-000004e0: 3738 312c 3131 3020 3733 332c 3538 2036  781,110 733,58 6
-000004f0: 3739 2c32 3720 3632 342c 2d34 2035 3537  79,27 624,-4 557
-00000500: 2c2d 3230 2034 3736 2c2d 3230 2033 3537  ,-20 476,-20 357
-00000510: 2c2d 3230 2032 3731 2c31 3020 3231 362c  ,-20 271,10 216,
-00000520: 3639 2031 3631 2c31 3238 2031 3333 2c32  69 161,128 133,2
-00000530: 3235 2031 3333 2c33 3631 204c 2031 3333  25 133,361 L 133
-00000540: 2c31 3038 3220 3331 342c 3130 3832 205a  ,1082 314,1082 Z
-00000550: 222f 3e0a 2020 203c 676c 7970 6820 756e  "/>.   <glyph un
-00000560: 6963 6f64 653d 2271 2220 686f 7269 7a2d  icode="q" horiz-
-00000570: 6164 762d 783d 2239 3232 2220 643d 224d  adv-x="922" d="M
-00000580: 2034 3834 2c2d 3230 2043 2033 3437 2c2d   484,-20 C 347,-
-00000590: 3230 2032 3436 2c32 3620 3138 322c 3131  20 246,26 182,11
-000005a0: 3920 3131 382c 3231 3220 3836 2c33 3531  9 118,212 86,351
-000005b0: 2038 362c 3533 3620 3836 2c39 3133 2032   86,536 86,913 2
-000005c0: 3139 2c31 3130 3220 3438 342c 3131 3032  19,1102 484,1102
-000005d0: 2035 3636 2c31 3130 3220 3633 342c 3130   566,1102 634,10
-000005e0: 3838 2036 3837 2c31 3035 3920 3734 302c  88 687,1059 740,
-000005f0: 3130 3330 2037 3835 2c39 3831 2038 3231  1030 785,981 821
-00000600: 2c39 3134 204c 2038 3233 2c39 3134 2043  ,914 L 823,914 C
-00000610: 2038 3233 2c39 3334 2038 3234 2c39 3639   823,934 824,969
-00000620: 2038 3237 2c31 3031 3820 3833 302c 3130   827,1018 830,10
-00000630: 3637 2038 3332 2c31 3039 3320 3833 352c  67 832,1093 835,
-00000640: 3130 3936 204c 2031 3030 382c 3130 3936  1096 L 1008,1096
-00000650: 2043 2031 3030 332c 3130 3537 2031 3030   C 1003,1057 100
-00000660: 312c 3935 3820 3130 3031 2c38 3031 204c  1,958 1001,801 L
-00000670: 2031 3030 312c 2d34 3235 2038 3231 2c2d   1001,-425 821,-
-00000680: 3432 3520 3832 312c 3134 2038 3235 2c31  425 821,14 825,1
-00000690: 3738 2038 3233 2c31 3738 2043 2037 3837  78 823,178 C 787
-000006a0: 2c31 3037 2037 3433 2c35 3620 3639 302c  ,107 743,56 690,
-000006b0: 3236 2036 3337 2c2d 3520 3536 392c 2d32  26 637,-5 569,-2
-000006c0: 3020 3438 342c 2d32 3020 5a20 4d20 3832  0 484,-20 Z M 82
-000006d0: 312c 3535 3420 4320 3832 312c 3639 3520  1,554 C 821,695 
-000006e0: 3739 382c 3739 3920 3735 322c 3836 3720  798,799 752,867 
-000006f0: 3730 362c 3933 3520 3633 332c 3936 3920  706,935 633,969 
-00000700: 3533 322c 3936 3920 3434 312c 3936 3920  532,969 441,969 
-00000710: 3337 352c 3933 3520 3333 352c 3836 3720  375,935 335,867 
-00000720: 3239 352c 3739 3920 3237 352c 3639 3120  295,799 275,691 
-00000730: 3237 352c 3534 3220 3237 352c 3339 3120  275,542 275,391 
-00000740: 3239 352c 3238 3220 3333 362c 3231 3720  295,282 336,217 
-00000750: 3337 362c 3135 3220 3434 312c 3131 3920  376,152 441,119 
-00000760: 3533 302c 3131 3920 3633 322c 3131 3920  530,119 632,119 
-00000770: 3730 362c 3135 3520 3735 322c 3232 3820  706,155 752,228 
-00000780: 3739 382c 3330 3120 3832 312c 3430 3920  798,301 821,409 
-00000790: 3832 312c 3535 3420 5a22 2f3e 0a20 2020  821,554 Z"/>.   
-000007a0: 3c67 6c79 7068 2075 6e69 636f 6465 3d22  <glyph unicode="
-000007b0: 6e22 2068 6f72 697a 2d61 6476 2d78 3d22  n" horiz-adv-x="
-000007c0: 3839 3422 2064 3d22 4d20 3832 352c 3020  894" d="M 825,0 
-000007d0: 4c20 3832 352c 3638 3620 4320 3832 352c  L 825,686 C 825,
-000007e0: 3735 3720 3831 382c 3831 3320 3830 342c  757 818,813 804,
-000007f0: 3835 3220 3739 302c 3839 3120 3736 382c  852 790,891 768,
-00000800: 3932 3020 3733 372c 3933 3720 3730 362c  920 737,937 706,
-00000810: 3935 3420 3636 312c 3936 3320 3630 322c  954 661,963 602,
-00000820: 3936 3320 3531 352c 3936 3320 3434 372c  963 515,963 447,
-00000830: 3933 3320 3339 372c 3837 3420 3334 372c  933 397,874 347,
-00000840: 3831 3520 3332 322c 3733 3220 3332 322c  815 322,732 322,
-00000850: 3632 3720 4c20 3332 322c 3020 3134 322c  627 L 322,0 142,
-00000860: 3020 3134 322c 3835 3120 4320 3134 322c  0 142,851 C 142,
-00000870: 3937 3720 3134 302c 3130 3534 2031 3336  977 140,1054 136
-00000880: 2c31 3038 3220 4c20 3330 362c 3130 3832  ,1082 L 306,1082
-00000890: 2043 2033 3037 2c31 3037 3920 3330 372c   C 307,1079 307,
-000008a0: 3130 3730 2033 3038 2c31 3035 3520 3330  1070 308,1055 30
-000008b0: 392c 3130 3430 2033 3130 2c31 3032 3420  9,1040 310,1024 
-000008c0: 3331 312c 3130 3035 2033 3132 2c39 3836  311,1005 312,986
-000008d0: 2033 3133 2c39 3530 2033 3134 2c38 3937   313,950 314,897
-000008e0: 204c 2033 3137 2c38 3937 2043 2033 3538   L 317,897 C 358
-000008f0: 2c39 3732 2034 3036 2c31 3032 3520 3436  ,972 406,1025 46
-00000900: 312c 3130 3536 2035 3135 2c31 3038 3720  1,1056 515,1087 
-00000910: 3538 322c 3131 3032 2036 3633 2c31 3130  582,1102 663,110
-00000920: 3220 3738 322c 3131 3032 2038 3639 2c31  2 782,1102 869,1
-00000930: 3037 3320 3932 342c 3130 3134 2039 3739  073 924,1014 979
-00000940: 2c39 3535 2031 3030 362c 3835 3720 3130  ,955 1006,857 10
-00000950: 3036 2c37 3231 204c 2031 3030 362c 3020  06,721 L 1006,0 
-00000960: 3832 352c 3020 5a22 2f3e 0a20 2020 3c67  825,0 Z"/>.   <g
-00000970: 6c79 7068 2075 6e69 636f 6465 3d22 6522  lyph unicode="e"
-00000980: 2068 6f72 697a 2d61 6476 2d78 3d22 3937   horiz-adv-x="97
-00000990: 3822 2064 3d22 4d20 3237 362c 3530 3320  8" d="M 276,503 
-000009a0: 4320 3237 362c 3337 3920 3330 322c 3238  C 276,379 302,28
-000009b0: 3320 3335 332c 3231 3620 3430 342c 3134  3 353,216 404,14
-000009c0: 3920 3437 392c 3131 3520 3537 382c 3131  9 479,115 578,11
-000009d0: 3520 3635 362c 3131 3520 3731 392c 3133  5 656,115 719,13
-000009e0: 3120 3736 362c 3136 3220 3831 332c 3139  1 766,162 813,19
-000009f0: 3320 3834 342c 3233 3320 3836 312c 3238  3 844,233 861,28
-00000a00: 3120 4c20 3130 3139 2c32 3336 2043 2039  1 L 1019,236 C 9
-00000a10: 3534 2c36 3520 3830 372c 2d32 3020 3537  54,65 807,-20 57
-00000a20: 382c 2d32 3020 3431 382c 2d32 3020 3239  8,-20 418,-20 29
-00000a30: 362c 3238 2032 3133 2c31 3233 2031 3239  6,28 213,123 129
-00000a40: 2c32 3138 2038 372c 3336 3020 3837 2c35  ,218 87,360 87,5
-00000a50: 3438 2038 372c 3732 3720 3132 392c 3836  48 87,727 129,86
-00000a60: 3420 3231 332c 3935 3920 3239 362c 3130  4 213,959 296,10
-00000a70: 3534 2034 3136 2c31 3130 3220 3537 312c  54 416,1102 571,
-00000a80: 3131 3032 2038 3839 2c31 3130 3220 3130  1102 889,1102 10
-00000a90: 3438 2c39 3130 2031 3034 382c 3532 3720  48,910 1048,527 
-00000aa0: 4c20 3130 3438 2c35 3033 2032 3736 2c35  L 1048,503 276,5
-00000ab0: 3033 205a 204d 2038 3632 2c36 3431 2043  03 Z M 862,641 C
-00000ac0: 2038 3532 2c37 3535 2038 3233 2c38 3338   852,755 823,838
-00000ad0: 2037 3735 2c38 3931 2037 3237 2c39 3433   775,891 727,943
-00000ae0: 2036 3538 2c39 3639 2035 3638 2c39 3639   658,969 568,969
-00000af0: 2034 3831 2c39 3639 2034 3132 2c39 3430   481,969 412,940
-00000b00: 2033 3631 2c38 3832 2033 3130 2c38 3233   361,882 310,823
-00000b10: 2032 3832 2c37 3433 2032 3738 2c36 3431   282,743 278,641
-00000b20: 204c 2038 3632 2c36 3431 205a 222f 3e0a   L 862,641 Z"/>.
-00000b30: 2020 203c 676c 7970 6820 756e 6963 6f64     <glyph unicod
-00000b40: 653d 2263 2220 686f 7269 7a2d 6164 762d  e="c" horiz-adv-
-00000b50: 783d 2238 3934 2220 643d 224d 2032 3735  x="894" d="M 275
-00000b60: 2c35 3436 2043 2032 3735 2c34 3032 2032  ,546 C 275,402 2
-00000b70: 3938 2c32 3935 2033 3433 2c32 3236 2033  98,295 343,226 3
-00000b80: 3838 2c31 3537 2034 3537 2c31 3232 2035  88,157 457,122 5
-00000b90: 3438 2c31 3232 2036 3132 2c31 3232 2036  48,122 612,122 6
-00000ba0: 3636 2c31 3339 2037 3039 2c31 3734 2037  66,139 709,174 7
-00000bb0: 3532 2c32 3039 2037 3738 2c32 3632 2037  52,209 778,262 7
-00000bc0: 3838 2c33 3334 204c 2039 3730 2c33 3232  88,334 L 970,322
-00000bd0: 2043 2039 3536 2c32 3138 2039 3132 2c31   C 956,218 912,1
-00000be0: 3335 2038 3337 2c37 3320 3736 322c 3131  35 837,73 762,11
-00000bf0: 2036 3638 2c2d 3230 2035 3533 2c2d 3230   668,-20 553,-20
-00000c00: 2034 3032 2c2d 3230 2032 3836 2c32 3820   402,-20 286,28 
-00000c10: 3230 372c 3132 3420 3132 372c 3231 3920  207,124 127,219 
-00000c20: 3837 2c33 3539 2038 372c 3534 3220 3837  87,359 87,542 87
-00000c30: 2c37 3234 2031 3237 2c38 3633 2032 3037  ,724 127,863 207
-00000c40: 2c39 3539 2032 3837 2c31 3035 3420 3430  ,959 287,1054 40
-00000c50: 322c 3131 3032 2035 3531 2c31 3130 3220  2,1102 551,1102 
-00000c60: 3636 322c 3131 3032 2037 3534 2c31 3037  662,1102 754,107
-00000c70: 3320 3832 372c 3130 3136 2039 3030 2c39  3 827,1016 900,9
-00000c80: 3539 2039 3435 2c38 3830 2039 3634 2c37  59 945,880 964,7
-00000c90: 3739 204c 2037 3739 2c37 3635 2043 2037  79 L 779,765 C 7
-00000ca0: 3730 2c38 3235 2037 3436 2c38 3733 2037  70,825 746,873 7
-00000cb0: 3038 2c39 3038 2036 3730 2c39 3433 2036  08,908 670,943 6
-00000cc0: 3136 2c39 3631 2035 3436 2c39 3631 2034  16,961 546,961 4
-00000cd0: 3531 2c39 3631 2033 3832 2c39 3239 2033  51,961 382,929 3
-00000ce0: 3339 2c38 3636 2032 3936 2c38 3033 2032  39,866 296,803 2
-00000cf0: 3735 2c36 3936 2032 3735 2c35 3436 205a  75,696 275,546 Z
-00000d00: 222f 3e0a 2020 203c 676c 7970 6820 756e  "/>.   <glyph un
-00000d10: 6963 6f64 653d 2253 2220 686f 7269 7a2d  icode="S" horiz-
-00000d20: 6164 762d 783d 2231 3230 3122 2064 3d22  adv-x="1201" d="
-00000d30: 4d20 3132 3732 2c33 3839 2043 2031 3237  M 1272,389 C 127
-00000d40: 322c 3235 3920 3132 3231 2c31 3538 2031  2,259 1221,158 1
-00000d50: 3132 302c 3837 2031 3031 382c 3136 2038  120,87 1018,16 8
-00000d60: 3735 2c2d 3230 2036 3930 2c2d 3230 2033  75,-20 690,-20 3
-00000d70: 3437 2c2d 3230 2031 3438 2c39 3920 3933  47,-20 148,99 93
-00000d80: 2c33 3338 204c 2032 3738 2c33 3735 2043  ,338 L 278,375 C
-00000d90: 2032 3939 2c32 3930 2033 3435 2c32 3238   299,290 345,228
-00000da0: 2034 3134 2c31 3839 2034 3833 2c31 3439   414,189 483,149
-00000db0: 2035 3738 2c31 3239 2036 3937 2c31 3239   578,129 697,129
-00000dc0: 2038 3230 2c31 3239 2039 3136 2c31 3530   820,129 916,150
-00000dd0: 2039 3833 2c31 3933 2031 3035 302c 3233   983,193 1050,23
-00000de0: 3520 3130 3833 2c32 3937 2031 3038 332c  5 1083,297 1083,
-00000df0: 3337 3920 3130 3833 2c34 3235 2031 3037  379 1083,425 107
-00000e00: 332c 3436 3220 3130 3532 2c34 3931 2031  3,462 1052,491 1
-00000e10: 3033 312c 3532 3020 3130 3031 2c35 3433  031,520 1001,543
-00000e20: 2039 3633 2c35 3632 2039 3235 2c35 3831   963,562 925,581
-00000e30: 2038 3830 2c35 3936 2038 3237 2c36 3039   880,596 827,609
-00000e40: 2037 3734 2c36 3232 2037 3136 2c36 3335   774,622 716,635
-00000e50: 2036 3532 2c36 3530 2035 3431 2c36 3735   652,650 541,675
-00000e60: 2034 3536 2c36 3939 2033 3939 2c37 3234   456,699 399,724
-00000e70: 2033 3431 2c37 3439 2032 3935 2c37 3736   341,749 295,776
-00000e80: 2032 3632 2c38 3037 2032 3239 2c38 3337   262,807 229,837
-00000e90: 2032 3033 2c38 3732 2031 3836 2c39 3133   203,872 186,913
-00000ea0: 2031 3638 2c39 3534 2031 3539 2c31 3030   168,954 159,100
-00000eb0: 3020 3135 392c 3130 3533 2031 3539 2c31  0 159,1053 159,1
-00000ec0: 3137 3420 3230 352c 3132 3637 2032 3938  174 205,1267 298
-00000ed0: 2c31 3333 3220 3339 302c 3133 3937 2035  ,1332 390,1397 5
-00000ee0: 3232 2c31 3433 3020 3639 342c 3134 3330  22,1430 694,1430
-00000ef0: 2038 3534 2c31 3433 3020 3937 362c 3134   854,1430 976,14
-00000f00: 3036 2031 3036 312c 3133 3537 2031 3134  06 1061,1357 114
-00000f10: 362c 3133 3038 2031 3230 352c 3132 3234  6,1308 1205,1224
-00000f20: 2031 3233 392c 3131 3036 204c 2031 3035   1239,1106 L 105
-00000f30: 312c 3130 3733 2043 2031 3033 302c 3131  1,1073 C 1030,11
-00000f40: 3438 2039 3931 2c31 3230 3220 3933 332c  48 991,1202 933,
-00000f50: 3132 3336 2038 3735 2c31 3236 3920 3739  1236 875,1269 79
-00000f60: 352c 3132 3836 2036 3932 2c31 3238 3620  5,1286 692,1286 
-00000f70: 3537 392c 3132 3836 2034 3933 2c31 3236  579,1286 493,126
-00000f80: 3720 3433 342c 3132 3330 2033 3735 2c31  7 434,1230 375,1
-00000f90: 3139 3320 3334 352c 3131 3337 2033 3435  193 345,1137 345
-00000fa0: 2c31 3036 3320 3334 352c 3130 3230 2033  ,1063 345,1020 3
-00000fb0: 3537 2c39 3834 2033 3830 2c39 3536 2034  57,984 380,956 4
-00000fc0: 3033 2c39 3237 2034 3336 2c39 3033 2034  03,927 436,903 4
-00000fd0: 3739 2c38 3834 2035 3232 2c38 3634 2036  79,884 522,864 6
-00000fe0: 3039 2c38 3430 2037 3338 2c38 3131 2037  09,840 738,811 7
-00000ff0: 3831 2c38 3031 2038 3235 2c37 3931 2038  81,801 825,791 8
-00001000: 3638 2c37 3831 2039 3131 2c37 3730 2039  68,781 911,770 9
-00001010: 3532 2c37 3538 2039 3931 2c37 3434 2031  52,758 991,744 1
-00001020: 3033 302c 3732 3920 3130 3637 2c37 3132  030,729 1067,712
-00001030: 2031 3130 322c 3639 3320 3131 3336 2c36   1102,693 1136,6
-00001040: 3734 2031 3136 362c 3635 3020 3131 3931  74 1166,650 1191
-00001050: 2c36 3232 2031 3231 362c 3539 3420 3132  ,622 1216,594 12
-00001060: 3336 2c35 3631 2031 3235 312c 3532 3320  36,561 1251,523 
-00001070: 3132 3635 2c34 3835 2031 3237 322c 3434  1265,485 1272,44
-00001080: 3020 3132 3732 2c33 3839 205a 222f 3e0a  0 1272,389 Z"/>.
-00001090: 2020 203c 676c 7970 6820 756e 6963 6f64     <glyph unicod
-000010a0: 653d 2233 2220 686f 7269 7a2d 6164 762d  e="3" horiz-adv-
-000010b0: 783d 2231 3030 3622 2064 3d22 4d20 3130  x="1006" d="M 10
-000010c0: 3439 2c33 3839 2043 2031 3034 392c 3235  49,389 C 1049,25
-000010d0: 3920 3130 3038 2c31 3538 2039 3235 2c38  9 1008,158 925,8
-000010e0: 3720 3834 322c 3136 2037 3234 2c2d 3230  7 842,16 724,-20
-000010f0: 2035 3731 2c2d 3230 2034 3238 2c2d 3230   571,-20 428,-20
-00001100: 2033 3135 2c31 3220 3233 302c 3737 2031   315,12 230,77 1
-00001110: 3435 2c31 3431 2039 342c 3233 3620 3738  45,141 94,236 78
-00001120: 2c33 3632 204c 2032 3634 2c33 3739 2043  ,362 L 264,379 C
-00001130: 2032 3838 2c32 3132 2033 3930 2c31 3239   288,212 390,129
-00001140: 2035 3731 2c31 3239 2036 3632 2c31 3239   571,129 662,129
-00001150: 2037 3333 2c31 3531 2037 3835 2c31 3936   733,151 785,196
-00001160: 2038 3336 2c32 3431 2038 3632 2c33 3037   836,241 862,307
-00001170: 2038 3632 2c33 3935 2038 3632 2c34 3732   862,395 862,472
-00001180: 2038 3333 2c35 3332 2037 3734 2c35 3735   833,532 774,575
-00001190: 2037 3135 2c36 3138 2036 3239 2c36 3339   715,618 629,639
-000011a0: 2035 3138 2c36 3339 204c 2034 3136 2c36   518,639 L 416,6
-000011b0: 3339 2034 3136 2c37 3935 2035 3134 2c37  39 416,795 514,7
-000011c0: 3935 2043 2036 3133 2c37 3935 2036 3839  95 C 613,795 689
-000011d0: 2c38 3137 2037 3434 2c38 3630 2037 3938  ,817 744,860 798
-000011e0: 2c39 3033 2038 3235 2c39 3632 2038 3235  ,903 825,962 825
-000011f0: 2c31 3033 3820 3832 352c 3131 3133 2038  ,1038 825,1113 8
-00001200: 3033 2c31 3137 3320 3735 392c 3132 3137  03,1173 759,1217
-00001210: 2037 3134 2c31 3236 3020 3634 382c 3132   714,1260 648,12
-00001220: 3832 2035 3631 2c31 3238 3220 3438 322c  82 561,1282 482,
-00001230: 3132 3832 2034 3138 2c31 3236 3220 3336  1282 418,1262 36
-00001240: 392c 3132 3231 2033 3230 2c31 3138 3020  9,1221 320,1180 
-00001250: 3239 312c 3131 3233 2032 3833 2c31 3034  291,1123 283,104
-00001260: 3920 4c20 3130 322c 3130 3633 2043 2031  9 L 102,1063 C 1
-00001270: 3135 2c31 3137 3820 3136 332c 3132 3638  15,1178 163,1268
-00001280: 2032 3436 2c31 3333 3320 3332 382c 3133   246,1333 328,13
-00001290: 3938 2034 3334 2c31 3433 3020 3536 332c  98 434,1430 563,
-000012a0: 3134 3330 2037 3034 2c31 3433 3020 3831  1430 704,1430 81
-000012b0: 342c 3133 3937 2038 3933 2c31 3333 3220  4,1397 893,1332 
-000012c0: 3937 312c 3132 3636 2031 3031 302c 3131  971,1266 1010,11
-000012d0: 3734 2031 3031 302c 3130 3537 2031 3031  74 1010,1057 101
-000012e0: 302c 3936 3720 3938 352c 3839 3420 3933  0,967 985,894 93
-000012f0: 352c 3833 3820 3838 342c 3738 3120 3831  5,838 884,781 81
-00001300: 312c 3734 3320 3731 352c 3732 3320 4c20  1,743 715,723 L 
-00001310: 3731 352c 3731 3920 4320 3832 302c 3730  715,719 C 820,70
-00001320: 3820 3930 322c 3637 3220 3936 312c 3631  8 902,672 961,61
-00001330: 3320 3130 3230 2c35 3534 2031 3034 392c  3 1020,554 1049,
-00001340: 3437 3920 3130 3439 2c33 3839 205a 222f  479 1049,389 Z"/
-00001350: 3e0a 2020 203c 676c 7970 6820 756e 6963  >.   <glyph unic
-00001360: 6f64 653d 2232 2220 686f 7269 7a2d 6164  ode="2" horiz-ad
-00001370: 762d 783d 2239 3530 2220 643d 224d 2031  v-x="950" d="M 1
-00001380: 3033 2c30 204c 2031 3033 2c31 3237 2043  03,0 L 103,127 C
-00001390: 2031 3337 2c32 3035 2031 3739 2c32 3734   137,205 179,274
-000013a0: 2032 3238 2c33 3334 2032 3737 2c33 3933   228,334 277,393
-000013b0: 2033 3238 2c34 3437 2033 3832 2c34 3936   328,447 382,496
-000013c0: 2034 3336 2c35 3434 2034 3930 2c35 3839   436,544 490,589
-000013d0: 2035 3433 2c36 3330 2035 3936 2c36 3731   543,630 596,671
-000013e0: 2036 3433 2c37 3133 2036 3836 2c37 3534   643,713 686,754
-000013f0: 2037 3239 2c37 3935 2037 3633 2c38 3339   729,795 763,839
-00001400: 2037 3930 2c38 3834 2038 3136 2c39 3239   790,884 816,929
-00001410: 2038 3239 2c39 3831 2038 3239 2c31 3033   829,981 829,103
-00001420: 3820 3832 392c 3131 3135 2038 3036 2c31  8 829,1115 806,1
-00001430: 3137 3520 3736 312c 3132 3138 2037 3136  175 761,1218 716
-00001440: 2c31 3236 3120 3635 332c 3132 3832 2035  ,1261 653,1282 5
-00001450: 3732 2c31 3238 3220 3439 352c 3132 3832  72,1282 495,1282
-00001460: 2034 3332 2c31 3236 3120 3338 332c 3132   432,1261 383,12
-00001470: 3230 2033 3333 2c31 3137 3820 3330 342c  20 333,1178 304,
-00001480: 3131 3139 2032 3935 2c31 3034 3420 4c20  1119 295,1044 L 
-00001490: 3131 312c 3130 3631 2043 2031 3234 2c31  111,1061 C 124,1
-000014a0: 3137 3420 3137 322c 3132 3633 2032 3535  174 172,1263 255
-000014b0: 2c31 3333 3020 3333 372c 3133 3937 2034  ,1330 337,1397 4
-000014c0: 3433 2c31 3433 3020 3537 322c 3134 3330  43,1430 572,1430
-000014d0: 2037 3134 2c31 3433 3020 3832 332c 3133   714,1430 823,13
-000014e0: 3937 2039 3030 2c31 3333 3020 3937 362c  97 900,1330 976,
-000014f0: 3132 3633 2031 3031 342c 3131 3637 2031  1263 1014,1167 1
-00001500: 3031 342c 3130 3434 2031 3031 342c 3938  014,1044 1014,98
-00001510: 3920 3130 3032 2c39 3335 2039 3737 2c38  9 1002,935 977,8
-00001520: 3831 2039 3532 2c38 3237 2039 3134 2c37  81 952,827 914,7
-00001530: 3733 2038 3635 2c37 3139 2038 3136 2c36  73 865,719 816,6
-00001540: 3635 2037 3231 2c35 3831 2035 3832 2c34  65 721,581 582,4
-00001550: 3638 2035 3035 2c34 3035 2034 3434 2c33  68 505,405 444,3
-00001560: 3439 2033 3939 2c32 3939 2033 3534 2c32  49 399,299 354,2
-00001570: 3438 2033 3231 2c32 3030 2033 3031 2c31  48 321,200 301,1
-00001580: 3533 204c 2031 3033 362c 3135 3320 3130  53 L 1036,153 10
-00001590: 3336 2c30 2031 3033 2c30 205a 222f 3e0a  36,0 103,0 Z"/>.
-000015a0: 2020 203c 676c 7970 6820 756e 6963 6f64     <glyph unicod
-000015b0: 653d 2231 2220 686f 7269 7a2d 6164 762d  e="1" horiz-adv-
-000015c0: 783d 2239 3232 2220 643d 224d 2031 3536  x="922" d="M 156
-000015d0: 2c30 204c 2031 3536 2c31 3533 2035 3135  ,0 L 156,153 515
-000015e0: 2c31 3533 2035 3135 2c31 3233 3720 3139  ,153 515,1237 19
-000015f0: 372c 3130 3130 2031 3937 2c31 3138 3020  7,1010 197,1180 
-00001600: 3533 302c 3134 3039 2036 3936 2c31 3430  530,1409 696,140
-00001610: 3920 3639 362c 3135 3320 3130 3339 2c31  9 696,153 1039,1
-00001620: 3533 2031 3033 392c 3020 3135 362c 3020  53 1039,0 156,0 
-00001630: 5a22 2f3e 0a20 2020 3c67 6c79 7068 2075  Z"/>.   <glyph u
-00001640: 6e69 636f 6465 3d22 2322 2068 6f72 697a  nicode="#" horiz
-00001650: 2d61 6476 2d78 3d22 3131 3435 2220 643d  -adv-x="1145" d=
-00001660: 224d 2038 3936 2c38 3835 204c 2038 3138  "M 896,885 L 818
-00001670: 2c35 3136 2031 3037 382c 3531 3620 3130  ,516 1078,516 10
-00001680: 3738 2c34 3038 2037 3935 2c34 3038 2037  78,408 795,408 7
-00001690: 3037 2c30 2035 3937 2c30 2036 3833 2c34  07,0 597,0 683,4
-000016a0: 3038 2033 3230 2c34 3038 2032 3336 2c30  08 320,408 236,0
-000016b0: 2031 3236 2c30 2032 3130 2c34 3038 2039   126,0 210,408 9
-000016c0: 2c34 3038 2039 2c35 3136 2032 3334 2c35  ,408 9,516 234,5
-000016d0: 3136 2033 3132 2c38 3835 2036 302c 3838  16 312,885 60,88
-000016e0: 3520 3630 2c39 3933 2033 3334 2c39 3933  5 60,993 334,993
-000016f0: 2034 3233 2c31 3430 3120 3533 332c 3134   423,1401 533,14
-00001700: 3031 2034 3435 2c39 3933 2038 3038 2c39  01 445,993 808,9
-00001710: 3933 2038 3936 2c31 3430 3120 3130 3036  93 896,1401 1006
-00001720: 2c31 3430 3120 3931 382c 3939 3320 3131  ,1401 918,993 11
-00001730: 3239 2c39 3933 2031 3132 392c 3838 3520  29,993 1129,885 
-00001740: 3839 362c 3838 3520 5a20 4d20 3432 352c  896,885 Z M 425,
-00001750: 3838 3520 4c20 3334 352c 3531 3620 3730  885 L 345,516 70
-00001760: 372c 3531 3620 3738 352c 3838 3520 3432  7,516 785,885 42
-00001770: 352c 3838 3520 5a22 2f3e 0a20 2020 3c67  5,885 Z"/>.   <g
-00001780: 6c79 7068 2075 6e69 636f 6465 3d22 2022  lyph unicode=" "
-00001790: 2068 6f72 697a 2d61 6476 2d78 3d22 3535   horiz-adv-x="55
-000017a0: 3822 2f3e 0a20 203c 2f66 6f6e 743e 0a20  8"/>.  </font>. 
-000017b0: 3c2f 6465 6673 3e0a 203c 6465 6673 2063  </defs>. <defs c
-000017c0: 6c61 7373 3d22 456d 6265 6464 6564 4275  lass="EmbeddedBu
-000017d0: 6c6c 6574 4368 6172 7322 3e0a 2020 3c67  lletChars">.  <g
-000017e0: 2069 643d 2262 756c 6c65 742d 6368 6172   id="bullet-char
-000017f0: 2d74 656d 706c 6174 652d 3537 3335 3622  -template-57356"
-00001800: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
-00001810: 6528 302e 3030 3034 3838 3238 3132 352c  e(0.00048828125,
-00001820: 2d30 2e30 3030 3438 3832 3831 3235 2922  -0.00048828125)"
-00001830: 3e0a 2020 203c 7061 7468 2064 3d22 4d20  >.   <path d="M 
-00001840: 3538 302c 3131 3431 204c 2031 3136 332c  580,1141 L 1163,
-00001850: 3537 3120 3538 302c 3020 2d34 2c35 3731  571 580,0 -4,571
-00001860: 2035 3830 2c31 3134 3120 5a22 2f3e 0a20   580,1141 Z"/>. 
-00001870: 203c 2f67 3e0a 2020 3c67 2069 643d 2262   </g>.  <g id="b
-00001880: 756c 6c65 742d 6368 6172 2d74 656d 706c  ullet-char-templ
-00001890: 6174 652d 3537 3335 3422 2074 7261 6e73  ate-57354" trans
-000018a0: 666f 726d 3d22 7363 616c 6528 302e 3030  form="scale(0.00
-000018b0: 3034 3838 3238 3132 352c 2d30 2e30 3030  048828125,-0.000
-000018c0: 3438 3832 3831 3235 2922 3e0a 2020 203c  48828125)">.   <
-000018d0: 7061 7468 2064 3d22 4d20 382c 3131 3238  path d="M 8,1128
-000018e0: 204c 2031 3133 372c 3131 3238 2031 3133   L 1137,1128 113
-000018f0: 372c 3020 382c 3020 382c 3131 3238 205a  7,0 8,0 8,1128 Z
-00001900: 222f 3e0a 2020 3c2f 673e 0a20 203c 6720  "/>.  </g>.  <g 
-00001910: 6964 3d22 6275 6c6c 6574 2d63 6861 722d  id="bullet-char-
-00001920: 7465 6d70 6c61 7465 2d31 3031 3436 2220  template-10146" 
-00001930: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
-00001940: 2830 2e30 3030 3438 3832 3831 3235 2c2d  (0.00048828125,-
-00001950: 302e 3030 3034 3838 3238 3132 3529 223e  0.00048828125)">
-00001960: 0a20 2020 3c70 6174 6820 643d 224d 2031  .   <path d="M 1
-00001970: 3734 2c30 204c 2036 3032 2c37 3339 2031  74,0 L 602,739 1
-00001980: 3734 2c31 3438 3120 3134 3536 2c37 3339  74,1481 1456,739
-00001990: 2031 3734 2c30 205a 204d 2031 3335 382c   174,0 Z M 1358,
-000019a0: 3733 3920 4c20 3330 392c 3133 3436 2036  739 L 309,1346 6
-000019b0: 3539 2c37 3339 2031 3335 382c 3733 3920  59,739 1358,739 
-000019c0: 5a22 2f3e 0a20 203c 2f67 3e0a 2020 3c67  Z"/>.  </g>.  <g
-000019d0: 2069 643d 2262 756c 6c65 742d 6368 6172   id="bullet-char
-000019e0: 2d74 656d 706c 6174 652d 3130 3133 3222  -template-10132"
-000019f0: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
-00001a00: 6528 302e 3030 3034 3838 3238 3132 352c  e(0.00048828125,
-00001a10: 2d30 2e30 3030 3438 3832 3831 3235 2922  -0.00048828125)"
-00001a20: 3e0a 2020 203c 7061 7468 2064 3d22 4d20  >.   <path d="M 
-00001a30: 3230 3135 2c37 3339 204c 2031 3237 362c  2015,739 L 1276,
-00001a40: 3020 3731 372c 3020 3132 3630 2c35 3433  0 717,0 1260,543
-00001a50: 2031 3734 2c35 3433 2031 3734 2c39 3336   174,543 174,936
-00001a60: 2031 3236 302c 3933 3620 3731 372c 3134   1260,936 717,14
-00001a70: 3831 2031 3237 342c 3134 3831 2032 3031  81 1274,1481 201
-00001a80: 352c 3733 3920 5a22 2f3e 0a20 203c 2f67  5,739 Z"/>.  </g
-00001a90: 3e0a 2020 3c67 2069 643d 2262 756c 6c65  >.  <g id="bulle
-00001aa0: 742d 6368 6172 2d74 656d 706c 6174 652d  t-char-template-
-00001ab0: 3130 3030 3722 2074 7261 6e73 666f 726d  10007" transform
-00001ac0: 3d22 7363 616c 6528 302e 3030 3034 3838  ="scale(0.000488
-00001ad0: 3238 3132 352c 2d30 2e30 3030 3438 3832  28125,-0.0004882
-00001ae0: 3831 3235 2922 3e0a 2020 203c 7061 7468  8125)">.   <path
-00001af0: 2064 3d22 4d20 302c 2d32 2043 202d 372c   d="M 0,-2 C -7,
-00001b00: 3134 202d 3136 2c32 3720 2d32 352c 3337  14 -16,27 -25,37
-00001b10: 204c 2033 3536 2c35 3637 2043 2032 3632   L 356,567 C 262
-00001b20: 2c38 3233 2032 3135 2c39 3532 2032 3135  ,823 215,952 215
-00001b30: 2c39 3534 2032 3135 2c39 3739 2032 3238  ,954 215,979 228
-00001b40: 2c39 3932 2032 3535 2c39 3932 2032 3634  ,992 255,992 264
-00001b50: 2c39 3932 2032 3736 2c39 3930 2032 3839  ,992 276,990 289
-00001b60: 2c39 3837 2033 3130 2c39 3931 2033 3331  ,987 310,991 331
-00001b70: 2c39 3939 2033 3534 2c31 3031 3220 4c20  ,999 354,1012 L 
-00001b80: 3338 312c 3939 3920 3439 322c 3734 3820  381,999 492,748 
-00001b90: 3737 322c 3130 3439 2038 3336 2c31 3032  772,1049 836,102
-00001ba0: 3420 3836 302c 3130 3439 2043 2038 3831  4 860,1049 C 881
-00001bb0: 2c31 3033 3920 3930 312c 3130 3235 2039  ,1039 901,1025 9
-00001bc0: 3232 2c31 3030 3620 3838 362c 3933 3720  22,1006 886,937 
-00001bd0: 3833 352c 3836 3320 3737 302c 3738 3420  835,863 770,784 
-00001be0: 3736 392c 3738 3320 3731 302c 3731 3620  769,783 710,716 
-00001bf0: 3539 342c 3538 3420 4c20 3737 342c 3232  594,584 L 774,22
-00001c00: 3320 4320 3737 342c 3139 3620 3735 332c  3 C 774,196 753,
-00001c10: 3136 3820 3731 312c 3133 3920 4c20 3732  168 711,139 L 72
-00001c20: 372c 3131 3920 4320 3731 372c 3930 2036  7,119 C 717,90 6
-00001c30: 3939 2c37 3620 3637 322c 3736 2036 3431  99,76 672,76 641
-00001c40: 2c37 3620 3537 302c 3137 3820 3435 372c  ,76 570,178 457,
-00001c50: 3338 3120 4c20 3136 342c 2d37 3620 4320  381 L 164,-76 C 
-00001c60: 3134 322c 2d31 3130 2031 3131 2c2d 3132  142,-110 111,-12
-00001c70: 3720 3732 2c2d 3132 3720 3330 2c2d 3132  7 72,-127 30,-12
-00001c80: 3720 392c 2d31 3130 2038 2c2d 3736 2031  7 9,-110 8,-76 1
-00001c90: 2c2d 3637 202d 322c 2d35 3220 2d32 2c2d  ,-67 -2,-52 -2,-
-00001ca0: 3332 202d 322c 2d32 3320 2d31 2c2d 3133  32 -2,-23 -1,-13
-00001cb0: 2030 2c2d 3220 5a22 2f3e 0a20 203c 2f67   0,-2 Z"/>.  </g
-00001cc0: 3e0a 2020 3c67 2069 643d 2262 756c 6c65  >.  <g id="bulle
-00001cd0: 742d 6368 6172 2d74 656d 706c 6174 652d  t-char-template-
-00001ce0: 3130 3030 3422 2074 7261 6e73 666f 726d  10004" transform
-00001cf0: 3d22 7363 616c 6528 302e 3030 3034 3838  ="scale(0.000488
-00001d00: 3238 3132 352c 2d30 2e30 3030 3438 3832  28125,-0.0004882
-00001d10: 3831 3235 2922 3e0a 2020 203c 7061 7468  8125)">.   <path
-00001d20: 2064 3d22 4d20 3238 352c 2d33 3320 4320   d="M 285,-33 C 
-00001d30: 3138 322c 2d33 3320 3131 312c 3330 2037  182,-33 111,30 7
-00001d40: 342c 3135 3620 3532 2c32 3238 2034 312c  4,156 52,228 41,
-00001d50: 3333 3320 3431 2c34 3731 2034 312c 3534  333 41,471 41,54
-00001d60: 3920 3535 2c36 3136 2038 322c 3637 3220  9 55,616 82,672 
-00001d70: 3131 362c 3734 3320 3136 392c 3737 3820  116,743 169,778 
-00001d80: 3234 302c 3737 3820 3239 332c 3737 3820  240,778 293,778 
-00001d90: 3332 382c 3734 3720 3334 362c 3638 3420  328,747 346,684 
-00001da0: 4c20 3336 392c 3530 3820 4320 3337 372c  L 369,508 C 377,
-00001db0: 3434 3420 3339 372c 3431 3120 3432 382c  444 397,411 428,
-00001dc0: 3431 3020 4c20 3131 3633 2c31 3131 3620  410 L 1163,1116 
-00001dd0: 4320 3131 3734 2c31 3132 3720 3131 3936  C 1174,1127 1196
-00001de0: 2c31 3133 3320 3132 3239 2c31 3133 3320  ,1133 1229,1133 
-00001df0: 3132 3731 2c31 3133 3320 3132 3932 2c31  1271,1133 1292,1
-00001e00: 3131 3820 3132 3932 2c31 3038 3720 4c20  118 1292,1087 L 
-00001e10: 3132 3932 2c39 3635 2043 2031 3239 322c  1292,965 C 1292,
-00001e20: 3932 3920 3132 3832 2c39 3031 2031 3236  929 1282,901 126
-00001e30: 322c 3838 3120 4c20 3434 322c 3437 2043  2,881 L 442,47 C
-00001e40: 2033 3930 2c2d 3620 3333 382c 2d33 3320   390,-6 338,-33 
-00001e50: 3238 352c 2d33 3320 5a22 2f3e 0a20 203c  285,-33 Z"/>.  <
-00001e60: 2f67 3e0a 2020 3c67 2069 643d 2262 756c  /g>.  <g id="bul
-00001e70: 6c65 742d 6368 6172 2d74 656d 706c 6174  let-char-templat
-00001e80: 652d 3936 3739 2220 7472 616e 7366 6f72  e-9679" transfor
-00001e90: 6d3d 2273 6361 6c65 2830 2e30 3030 3438  m="scale(0.00048
-00001ea0: 3832 3831 3235 2c2d 302e 3030 3034 3838  828125,-0.000488
-00001eb0: 3238 3132 3529 223e 0a20 2020 3c70 6174  28125)">.   <pat
-00001ec0: 6820 643d 224d 2038 3133 2c30 2043 2036  h d="M 813,0 C 6
-00001ed0: 3332 2c30 2034 3839 2c35 3420 3338 332c  32,0 489,54 383,
-00001ee0: 3136 3120 3237 362c 3236 3820 3232 332c  161 276,268 223,
-00001ef0: 3431 3120 3232 332c 3539 3220 3232 332c  411 223,592 223,
-00001f00: 3737 3320 3237 362c 3931 3620 3338 332c  773 276,916 383,
-00001f10: 3130 3233 2034 3839 2c31 3133 3020 3633  1023 489,1130 63
-00001f20: 322c 3131 3834 2038 3133 2c31 3138 3420  2,1184 813,1184 
-00001f30: 3939 322c 3131 3834 2031 3133 362c 3131  992,1184 1136,11
-00001f40: 3330 2031 3234 352c 3130 3233 2031 3335  30 1245,1023 135
-00001f50: 332c 3931 3620 3134 3037 2c37 3732 2031  3,916 1407,772 1
-00001f60: 3430 372c 3539 3220 3134 3037 2c34 3132  407,592 1407,412
-00001f70: 2031 3335 332c 3236 3820 3132 3435 2c31   1353,268 1245,1
-00001f80: 3631 2031 3133 362c 3534 2039 3932 2c30  61 1136,54 992,0
-00001f90: 2038 3133 2c30 205a 222f 3e0a 2020 3c2f   813,0 Z"/>.  </
-00001fa0: 673e 0a20 203c 6720 6964 3d22 6275 6c6c  g>.  <g id="bull
-00001fb0: 6574 2d63 6861 722d 7465 6d70 6c61 7465  et-char-template
-00001fc0: 2d38 3232 3622 2074 7261 6e73 666f 726d  -8226" transform
-00001fd0: 3d22 7363 616c 6528 302e 3030 3034 3838  ="scale(0.000488
-00001fe0: 3238 3132 352c 2d30 2e30 3030 3438 3832  28125,-0.0004882
-00001ff0: 3831 3235 2922 3e0a 2020 203c 7061 7468  8125)">.   <path
-00002000: 2064 3d22 4d20 3334 362c 3435 3720 4320   d="M 346,457 C 
-00002010: 3237 332c 3435 3720 3230 392c 3438 3320  273,457 209,483 
-00002020: 3135 352c 3533 3520 3130 312c 3538 3620  155,535 101,586 
-00002030: 3734 2c36 3439 2037 342c 3732 3320 3734  74,649 74,723 74
-00002040: 2c37 3936 2031 3031 2c38 3539 2031 3535  ,796 101,859 155
-00002050: 2c39 3131 2032 3039 2c39 3633 2032 3733  ,911 209,963 273
-00002060: 2c39 3839 2033 3436 2c39 3839 2034 3139  ,989 346,989 419
-00002070: 2c39 3839 2034 3830 2c39 3633 2035 3331  ,989 480,963 531
-00002080: 2c39 3130 2035 3832 2c38 3539 2036 3038  ,910 582,859 608
-00002090: 2c37 3936 2036 3038 2c37 3233 2036 3038  ,796 608,723 608
-000020a0: 2c36 3438 2035 3833 2c35 3836 2035 3332  ,648 583,586 532
-000020b0: 2c35 3335 2034 3832 2c34 3833 2034 3230  ,535 482,483 420
-000020c0: 2c34 3537 2033 3436 2c34 3537 205a 222f  ,457 346,457 Z"/
-000020d0: 3e0a 2020 3c2f 673e 0a20 203c 6720 6964  >.  </g>.  <g id
-000020e0: 3d22 6275 6c6c 6574 2d63 6861 722d 7465  ="bullet-char-te
-000020f0: 6d70 6c61 7465 2d38 3231 3122 2074 7261  mplate-8211" tra
-00002100: 6e73 666f 726d 3d22 7363 616c 6528 302e  nsform="scale(0.
-00002110: 3030 3034 3838 3238 3132 352c 2d30 2e30  00048828125,-0.0
-00002120: 3030 3438 3832 3831 3235 2922 3e0a 2020  0048828125)">.  
-00002130: 203c 7061 7468 2064 3d22 4d20 2d34 2c34   <path d="M -4,4
-00002140: 3539 204c 2031 3133 352c 3435 3920 3131  59 L 1135,459 11
-00002150: 3335 2c36 3036 202d 342c 3630 3620 2d34  35,606 -4,606 -4
-00002160: 2c34 3539 205a 222f 3e0a 2020 3c2f 673e  ,459 Z"/>.  </g>
-00002170: 0a20 203c 6720 6964 3d22 6275 6c6c 6574  .  <g id="bullet
-00002180: 2d63 6861 722d 7465 6d70 6c61 7465 2d36  -char-template-6
-00002190: 3135 3438 2220 7472 616e 7366 6f72 6d3d  1548" transform=
-000021a0: 2273 6361 6c65 2830 2e30 3030 3438 3832  "scale(0.0004882
-000021b0: 3831 3235 2c2d 302e 3030 3034 3838 3238  8125,-0.00048828
-000021c0: 3132 3529 223e 0a20 2020 3c70 6174 6820  125)">.   <path 
-000021d0: 643d 224d 2031 3733 2c37 3430 2043 2031  d="M 173,740 C 1
-000021e0: 3733 2c39 3033 2032 3331 2c31 3034 3320  73,903 231,1043 
-000021f0: 3334 362c 3131 3539 2034 3632 2c31 3237  346,1159 462,127
-00002200: 3420 3630 312c 3133 3332 2037 3635 2c31  4 601,1332 765,1
-00002210: 3333 3220 3932 382c 3133 3332 2031 3036  332 928,1332 106
-00002220: 372c 3132 3734 2031 3138 332c 3131 3539  7,1274 1183,1159
-00002230: 2031 3239 392c 3130 3433 2031 3335 372c   1299,1043 1357,
-00002240: 3930 3320 3133 3537 2c37 3430 2031 3335  903 1357,740 135
-00002250: 372c 3537 3720 3132 3939 2c34 3337 2031  7,577 1299,437 1
-00002260: 3138 332c 3332 3220 3130 3637 2c32 3036  183,322 1067,206
-00002270: 2039 3238 2c31 3438 2037 3635 2c31 3438   928,148 765,148
-00002280: 2036 3031 2c31 3438 2034 3632 2c32 3036   601,148 462,206
-00002290: 2033 3436 2c33 3232 2032 3331 2c34 3337   346,322 231,437
-000022a0: 2031 3733 2c35 3737 2031 3733 2c37 3430   173,577 173,740
-000022b0: 205a 222f 3e0a 2020 3c2f 673e 0a20 3c2f   Z"/>.  </g>. </
-000022c0: 6465 6673 3e0a 203c 6720 636c 6173 733d  defs>. <g class=
-000022d0: 2250 6167 6522 3e0a 2020 3c67 2063 6c61  "Page">.  <g cla
-000022e0: 7373 3d22 636f 6d2e 7375 6e2e 7374 6172  ss="com.sun.star
-000022f0: 2e64 7261 7769 6e67 2e43 7573 746f 6d53  .drawing.CustomS
-00002300: 6861 7065 223e 0a20 2020 3c67 2069 643d  hape">.   <g id=
-00002310: 2269 6433 223e 0a20 2020 203c 7265 6374  "id3">.    <rect
-00002320: 2063 6c61 7373 3d22 426f 756e 6469 6e67   class="Bounding
-00002330: 426f 7822 2073 7472 6f6b 653d 226e 6f6e  Box" stroke="non
-00002340: 6522 2066 696c 6c3d 226e 6f6e 6522 2078  e" fill="none" x
-00002350: 3d22 3130 3030 2220 793d 2231 3030 3022  ="1000" y="1000"
-00002360: 2077 6964 7468 3d22 3132 3030 3122 2068   width="12001" h
-00002370: 6569 6768 743d 2231 3030 3122 2f3e 0a20  eight="1001"/>. 
-00002380: 2020 203c 7061 7468 2066 696c 6c3d 2272     <path fill="r
-00002390: 6762 2831 3030 2c31 3439 2c32 3337 2922  gb(100,149,237)"
-000023a0: 2073 7472 6f6b 653d 226e 6f6e 6522 2064   stroke="none" d
-000023b0: 3d22 4d20 3730 3030 2c32 3030 3020 4c20  ="M 7000,2000 L 
-000023c0: 3130 3030 2c32 3030 3020 3130 3030 2c31  1000,2000 1000,1
-000023d0: 3030 3020 3133 3030 302c 3130 3030 2031  000 13000,1000 1
-000023e0: 3330 3030 2c32 3030 3020 3730 3030 2c32  3000,2000 7000,2
-000023f0: 3030 3020 5a22 2f3e 0a20 2020 203c 7465  000 Z"/>.    <te
-00002400: 7874 2063 6c61 7373 3d22 5356 4754 6578  xt class="SVGTex
-00002410: 7453 6861 7065 223e 3c74 7370 616e 2063  tShape"><tspan c
-00002420: 6c61 7373 3d22 5465 7874 5061 7261 6772  lass="TextParagr
-00002430: 6170 6822 2066 6f6e 742d 6661 6d69 6c79  aph" font-family
-00002440: 3d22 4c69 6265 7261 7469 6f6e 2053 616e  ="Liberation San
-00002450: 732c 2073 616e 732d 7365 7269 6622 2066  s, sans-serif" f
-00002460: 6f6e 742d 7369 7a65 3d22 3633 3570 7822  ont-size="635px"
-00002470: 2066 6f6e 742d 7765 6967 6874 3d22 3430   font-weight="40
-00002480: 3022 3e3c 7473 7061 6e20 636c 6173 733d  0"><tspan class=
-00002490: 2254 6578 7450 6f73 6974 696f 6e22 2078  "TextPosition" x
-000024a0: 3d22 3531 3335 2220 793d 2231 3732 3122  ="5135" y="1721"
-000024b0: 3e3c 7473 7061 6e20 6669 6c6c 3d22 7267  ><tspan fill="rg
-000024c0: 6228 302c 302c 3029 2220 7374 726f 6b65  b(0,0,0)" stroke
-000024d0: 3d22 6e6f 6e65 2220 7374 796c 653d 2277  ="none" style="w
-000024e0: 6869 7465 2d73 7061 6365 3a20 7072 6522  hite-space: pre"
-000024f0: 3e53 6571 7565 6e63 6520 2331 3c2f 7473  >Sequence #1</ts
-00002500: 7061 6e3e 3c2f 7473 7061 6e3e 3c2f 7473  pan></tspan></ts
-00002510: 7061 6e3e 3c2f 7465 7874 3e0a 2020 203c  pan></text>.   <
-00002520: 2f67 3e0a 2020 3c2f 673e 0a20 203c 6720  /g>.  </g>.  <g 
-00002530: 636c 6173 733d 2263 6f6d 2e73 756e 2e73  class="com.sun.s
-00002540: 7461 722e 6472 6177 696e 672e 4c69 6e65  tar.drawing.Line
-00002550: 5368 6170 6522 3e0a 2020 203c 6720 6964  Shape">.   <g id
-00002560: 3d22 6964 3422 3e0a 2020 2020 3c72 6563  ="id4">.    <rec
-00002570: 7420 636c 6173 733d 2242 6f75 6e64 696e  t class="Boundin
-00002580: 6742 6f78 2220 7374 726f 6b65 3d22 6e6f  gBox" stroke="no
-00002590: 6e65 2220 6669 6c6c 3d22 6e6f 6e65 2220  ne" fill="none" 
-000025a0: 783d 2231 3030 3022 2079 3d22 3237 3530  x="1000" y="2750
-000025b0: 2220 7769 6474 683d 2234 3030 3122 2068  " width="4001" h
-000025c0: 6569 6768 743d 2235 3031 222f 3e0a 2020  eight="501"/>.  
-000025d0: 2020 3c70 6174 6820 6669 6c6c 3d22 6e6f    <path fill="no
-000025e0: 6e65 2220 7374 726f 6b65 3d22 7267 6228  ne" stroke="rgb(
-000025f0: 302c 302c 3029 2220 7374 726f 6b65 2d77  0,0,0)" stroke-w
-00002600: 6964 7468 3d22 3533 2220 7374 726f 6b65  idth="53" stroke
-00002610: 2d6c 696e 656a 6f69 6e3d 2272 6f75 6e64  -linejoin="round
-00002620: 2220 7374 726f 6b65 2d6c 696e 6563 6170  " stroke-linecap
-00002630: 3d22 7371 7561 7265 2220 643d 224d 2031  ="square" d="M 1
-00002640: 3033 322c 3330 3030 204c 2034 3936 382c  032,3000 L 4968,
-00002650: 3330 3030 222f 3e0a 2020 2020 3c70 6174  3000"/>.    <pat
-00002660: 6820 6669 6c6c 3d22 7267 6228 302c 302c  h fill="rgb(0,0,
-00002670: 3029 2220 7374 726f 6b65 3d22 6e6f 6e65  0)" stroke="none
-00002680: 2220 643d 224d 2031 3030 302c 3332 3530  " d="M 1000,3250
-00002690: 204c 2031 3030 302c 3330 3834 2031 3030   L 1000,3084 100
-000026a0: 302c 3239 3137 2031 3030 302c 3237 3530  0,2917 1000,2750
-000026b0: 2031 3032 322c 3237 3530 2031 3034 332c   1022,2750 1043,
-000026c0: 3237 3530 2031 3036 362c 3237 3530 2031  2750 1066,2750 1
-000026d0: 3036 362c 3239 3136 2031 3036 362c 3330  066,2916 1066,30
-000026e0: 3833 2031 3036 362c 3332 3530 2031 3034  83 1066,3250 104
-000026f0: 342c 3332 3530 2031 3032 332c 3332 3530  4,3250 1023,3250
-00002700: 2031 3030 302c 3332 3530 205a 222f 3e0a   1000,3250 Z"/>.
-00002710: 2020 2020 3c70 6174 6820 6669 6c6c 3d22      <path fill="
-00002720: 7267 6228 302c 302c 3029 2220 7374 726f  rgb(0,0,0)" stro
-00002730: 6b65 3d22 6e6f 6e65 2220 643d 224d 2035  ke="none" d="M 5
-00002740: 3030 302c 3237 3530 204c 2035 3030 302c  000,2750 L 5000,
-00002750: 3239 3136 2035 3030 302c 3330 3833 2035  2916 5000,3083 5
-00002760: 3030 302c 3332 3530 2034 3937 382c 3332  000,3250 4978,32
-00002770: 3530 2034 3935 372c 3332 3530 2034 3933  50 4957,3250 493
-00002780: 342c 3332 3530 2034 3933 342c 3330 3834  4,3250 4934,3084
-00002790: 2034 3933 342c 3239 3137 2034 3933 342c   4934,2917 4934,
-000027a0: 3237 3530 2034 3935 362c 3237 3530 2034  2750 4956,2750 4
-000027b0: 3937 372c 3237 3530 2035 3030 302c 3237  977,2750 5000,27
-000027c0: 3530 205a 222f 3e0a 2020 203c 2f67 3e0a  50 Z"/>.   </g>.
-000027d0: 2020 3c2f 673e 0a20 203c 6720 636c 6173    </g>.  <g clas
-000027e0: 733d 2263 6f6d 2e73 756e 2e73 7461 722e  s="com.sun.star.
-000027f0: 6472 6177 696e 672e 4c69 6e65 5368 6170  drawing.LineShap
-00002800: 6522 3e0a 2020 203c 6720 6964 3d22 6964  e">.   <g id="id
-00002810: 3522 3e0a 2020 2020 3c72 6563 7420 636c  5">.    <rect cl
-00002820: 6173 733d 2242 6f75 6e64 696e 6742 6f78  ass="BoundingBox
-00002830: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00002840: 6669 6c6c 3d22 6e6f 6e65 2220 783d 2239  fill="none" x="9
-00002850: 3030 3022 2079 3d22 3237 3530 2220 7769  000" y="2750" wi
-00002860: 6474 683d 2234 3030 3122 2068 6569 6768  dth="4001" heigh
-00002870: 743d 2235 3031 222f 3e0a 2020 2020 3c70  t="501"/>.    <p
-00002880: 6174 6820 6669 6c6c 3d22 6e6f 6e65 2220  ath fill="none" 
-00002890: 7374 726f 6b65 3d22 7267 6228 302c 302c  stroke="rgb(0,0,
-000028a0: 3029 2220 7374 726f 6b65 2d77 6964 7468  0)" stroke-width
-000028b0: 3d22 3533 2220 7374 726f 6b65 2d6c 696e  ="53" stroke-lin
-000028c0: 656a 6f69 6e3d 2272 6f75 6e64 2220 7374  ejoin="round" st
-000028d0: 726f 6b65 2d6c 696e 6563 6170 3d22 7371  roke-linecap="sq
-000028e0: 7561 7265 2220 643d 224d 2039 3033 322c  uare" d="M 9032,
-000028f0: 3330 3030 204c 2031 3239 3638 2c33 3030  3000 L 12968,300
-00002900: 3022 2f3e 0a20 2020 203c 7061 7468 2066  0"/>.    <path f
-00002910: 696c 6c3d 2272 6762 2830 2c30 2c30 2922  ill="rgb(0,0,0)"
-00002920: 2073 7472 6f6b 653d 226e 6f6e 6522 2064   stroke="none" d
-00002930: 3d22 4d20 3930 3030 2c33 3235 3020 4c20  ="M 9000,3250 L 
-00002940: 3930 3030 2c33 3038 3420 3930 3030 2c32  9000,3084 9000,2
-00002950: 3931 3720 3930 3030 2c32 3735 3020 3930  917 9000,2750 90
-00002960: 3232 2c32 3735 3020 3930 3433 2c32 3735  22,2750 9043,275
-00002970: 3020 3930 3636 2c32 3735 3020 3930 3636  0 9066,2750 9066
-00002980: 2c32 3931 3620 3930 3636 2c33 3038 3320  ,2916 9066,3083 
-00002990: 3930 3636 2c33 3235 3020 3930 3434 2c33  9066,3250 9044,3
-000029a0: 3235 3020 3930 3233 2c33 3235 3020 3930  250 9023,3250 90
-000029b0: 3030 2c33 3235 3020 5a22 2f3e 0a20 2020  00,3250 Z"/>.   
-000029c0: 203c 7061 7468 2066 696c 6c3d 2272 6762   <path fill="rgb
-000029d0: 2830 2c30 2c30 2922 2073 7472 6f6b 653d  (0,0,0)" stroke=
-000029e0: 226e 6f6e 6522 2064 3d22 4d20 3133 3030  "none" d="M 1300
-000029f0: 302c 3237 3530 204c 2031 3330 3030 2c32  0,2750 L 13000,2
-00002a00: 3931 3620 3133 3030 302c 3330 3833 2031  916 13000,3083 1
-00002a10: 3330 3030 2c33 3235 3020 3132 3937 382c  3000,3250 12978,
-00002a20: 3332 3530 2031 3239 3537 2c33 3235 3020  3250 12957,3250 
-00002a30: 3132 3933 342c 3332 3530 2031 3239 3334  12934,3250 12934
-00002a40: 2c33 3038 3420 3132 3933 342c 3239 3137  ,3084 12934,2917
-00002a50: 2031 3239 3334 2c32 3735 3020 3132 3935   12934,2750 1295
-00002a60: 362c 3237 3530 2031 3239 3737 2c32 3735  6,2750 12977,275
-00002a70: 3020 3133 3030 302c 3237 3530 205a 222f  0 13000,2750 Z"/
-00002a80: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
-00002a90: 0a20 203c 6720 636c 6173 733d 2263 6f6d  .  <g class="com
-00002aa0: 2e73 756e 2e73 7461 722e 6472 6177 696e  .sun.star.drawin
-00002ab0: 672e 4375 7374 6f6d 5368 6170 6522 3e0a  g.CustomShape">.
-00002ac0: 2020 203c 6720 6964 3d22 6964 3622 3e0a     <g id="id6">.
-00002ad0: 2020 2020 3c72 6563 7420 636c 6173 733d      <rect class=
-00002ae0: 2242 6f75 6e64 696e 6742 6f78 2220 7374  "BoundingBox" st
-00002af0: 726f 6b65 3d22 6e6f 6e65 2220 6669 6c6c  roke="none" fill
-00002b00: 3d22 6e6f 6e65 2220 783d 2235 3030 3022  ="none" x="5000"
-00002b10: 2079 3d22 3235 3030 2220 7769 6474 683d   y="2500" width=
-00002b20: 2231 3030 3122 2068 6569 6768 743d 2231  "1001" height="1
-00002b30: 3030 3122 2f3e 0a20 2020 203c 7061 7468  001"/>.    <path
-00002b40: 2066 696c 6c3d 2272 6762 2831 3932 2c31   fill="rgb(192,1
-00002b50: 3932 2c31 3932 2922 2073 7472 6f6b 653d  92,192)" stroke=
-00002b60: 226e 6f6e 6522 2064 3d22 4d20 3535 3030  "none" d="M 5500
-00002b70: 2c33 3530 3020 4c20 3530 3030 2c33 3530  ,3500 L 5000,350
-00002b80: 3020 3530 3030 2c32 3530 3020 3630 3030  0 5000,2500 6000
-00002b90: 2c32 3530 3020 3630 3030 2c33 3530 3020  ,2500 6000,3500 
-00002ba0: 3535 3030 2c33 3530 3020 5a22 2f3e 0a20  5500,3500 Z"/>. 
-00002bb0: 2020 3c2f 673e 0a20 203c 2f67 3e0a 2020    </g>.  </g>.  
-00002bc0: 3c67 2063 6c61 7373 3d22 636f 6d2e 7375  <g class="com.su
-00002bd0: 6e2e 7374 6172 2e64 7261 7769 6e67 2e43  n.star.drawing.C
-00002be0: 7573 746f 6d53 6861 7065 223e 0a20 2020  ustomShape">.   
-00002bf0: 3c67 2069 643d 2269 6437 223e 0a20 2020  <g id="id7">.   
-00002c00: 203c 7265 6374 2063 6c61 7373 3d22 426f   <rect class="Bo
-00002c10: 756e 6469 6e67 426f 7822 2073 7472 6f6b  undingBox" strok
-00002c20: 653d 226e 6f6e 6522 2066 696c 6c3d 226e  e="none" fill="n
-00002c30: 6f6e 6522 2078 3d22 3830 3030 2220 793d  one" x="8000" y=
-00002c40: 2232 3530 3022 2077 6964 7468 3d22 3130  "2500" width="10
-00002c50: 3031 2220 6865 6967 6874 3d22 3130 3031  01" height="1001
-00002c60: 222f 3e0a 2020 2020 3c70 6174 6820 6669  "/>.    <path fi
-00002c70: 6c6c 3d22 7267 6228 3139 322c 3139 322c  ll="rgb(192,192,
-00002c80: 3139 3229 2220 7374 726f 6b65 3d22 6e6f  192)" stroke="no
-00002c90: 6e65 2220 643d 224d 2038 3530 302c 3335  ne" d="M 8500,35
-00002ca0: 3030 204c 2038 3030 302c 3335 3030 2038  00 L 8000,3500 8
-00002cb0: 3030 302c 3235 3030 2039 3030 302c 3235  000,2500 9000,25
-00002cc0: 3030 2039 3030 302c 3335 3030 2038 3530  00 9000,3500 850
-00002cd0: 302c 3335 3030 205a 222f 3e0a 2020 203c  0,3500 Z"/>.   <
-00002ce0: 2f67 3e0a 2020 3c2f 673e 0a20 203c 6720  /g>.  </g>.  <g 
-00002cf0: 636c 6173 733d 2263 6f6d 2e73 756e 2e73  class="com.sun.s
-00002d00: 7461 722e 6472 6177 696e 672e 4375 7374  tar.drawing.Cust
-00002d10: 6f6d 5368 6170 6522 3e0a 2020 203c 6720  omShape">.   <g 
-00002d20: 6964 3d22 6964 3822 3e0a 2020 2020 3c72  id="id8">.    <r
-00002d30: 6563 7420 636c 6173 733d 2242 6f75 6e64  ect class="Bound
-00002d40: 696e 6742 6f78 2220 7374 726f 6b65 3d22  ingBox" stroke="
-00002d50: 6e6f 6e65 2220 6669 6c6c 3d22 6e6f 6e65  none" fill="none
-00002d60: 2220 783d 2231 3030 3022 2079 3d22 3430  " x="1000" y="40
-00002d70: 3030 2220 7769 6474 683d 2238 3030 3122  00" width="8001"
-00002d80: 2068 6569 6768 743d 2231 3030 3122 2f3e   height="1001"/>
-00002d90: 0a20 2020 203c 7061 7468 2066 696c 6c3d  .    <path fill=
-00002da0: 2272 6762 2831 3030 2c31 3439 2c32 3337  "rgb(100,149,237
-00002db0: 2922 2073 7472 6f6b 653d 226e 6f6e 6522  )" stroke="none"
-00002dc0: 2064 3d22 4d20 3530 3030 2c35 3030 3020   d="M 5000,5000 
-00002dd0: 4c20 3130 3030 2c35 3030 3020 3130 3030  L 1000,5000 1000
-00002de0: 2c34 3030 3020 3930 3030 2c34 3030 3020  ,4000 9000,4000 
-00002df0: 3930 3030 2c35 3030 3020 3530 3030 2c35  9000,5000 5000,5
-00002e00: 3030 3020 5a22 2f3e 0a20 2020 203c 7465  000 Z"/>.    <te
-00002e10: 7874 2063 6c61 7373 3d22 5356 4754 6578  xt class="SVGTex
-00002e20: 7453 6861 7065 223e 3c74 7370 616e 2063  tShape"><tspan c
-00002e30: 6c61 7373 3d22 5465 7874 5061 7261 6772  lass="TextParagr
-00002e40: 6170 6822 2066 6f6e 742d 6661 6d69 6c79  aph" font-family
-00002e50: 3d22 4c69 6265 7261 7469 6f6e 2053 616e  ="Liberation San
-00002e60: 732c 2073 616e 732d 7365 7269 6622 2066  s, sans-serif" f
-00002e70: 6f6e 742d 7369 7a65 3d22 3633 3570 7822  ont-size="635px"
-00002e80: 2066 6f6e 742d 7765 6967 6874 3d22 3430   font-weight="40
-00002e90: 3022 3e3c 7473 7061 6e20 636c 6173 733d  0"><tspan class=
-00002ea0: 2254 6578 7450 6f73 6974 696f 6e22 2078  "TextPosition" x
-00002eb0: 3d22 3331 3335 2220 793d 2234 3732 3122  ="3135" y="4721"
-00002ec0: 3e3c 7473 7061 6e20 6669 6c6c 3d22 7267  ><tspan fill="rg
-00002ed0: 6228 302c 302c 3029 2220 7374 726f 6b65  b(0,0,0)" stroke
-00002ee0: 3d22 6e6f 6e65 2220 7374 796c 653d 2277  ="none" style="w
-00002ef0: 6869 7465 2d73 7061 6365 3a20 7072 6522  hite-space: pre"
-00002f00: 3e53 6571 7565 6e63 6520 2332 3c2f 7473  >Sequence #2</ts
-00002f10: 7061 6e3e 3c2f 7473 7061 6e3e 3c2f 7473  pan></tspan></ts
-00002f20: 7061 6e3e 3c2f 7465 7874 3e0a 2020 203c  pan></text>.   <
-00002f30: 2f67 3e0a 2020 3c2f 673e 0a20 203c 6720  /g>.  </g>.  <g 
-00002f40: 636c 6173 733d 2263 6f6d 2e73 756e 2e73  class="com.sun.s
-00002f50: 7461 722e 6472 6177 696e 672e 4c69 6e65  tar.drawing.Line
-00002f60: 5368 6170 6522 3e0a 2020 203c 6720 6964  Shape">.   <g id
-00002f70: 3d22 6964 3922 3e0a 2020 2020 3c72 6563  ="id9">.    <rec
-00002f80: 7420 636c 6173 733d 2242 6f75 6e64 696e  t class="Boundin
-00002f90: 6742 6f78 2220 7374 726f 6b65 3d22 6e6f  gBox" stroke="no
-00002fa0: 6e65 2220 6669 6c6c 3d22 6e6f 6e65 2220  ne" fill="none" 
-00002fb0: 783d 2231 3030 3022 2079 3d22 3537 3530  x="1000" y="5750
-00002fc0: 2220 7769 6474 683d 2233 3030 3122 2068  " width="3001" h
-00002fd0: 6569 6768 743d 2235 3031 222f 3e0a 2020  eight="501"/>.  
-00002fe0: 2020 3c70 6174 6820 6669 6c6c 3d22 6e6f    <path fill="no
-00002ff0: 6e65 2220 7374 726f 6b65 3d22 7267 6228  ne" stroke="rgb(
-00003000: 302c 302c 3029 2220 7374 726f 6b65 2d77  0,0,0)" stroke-w
-00003010: 6964 7468 3d22 3533 2220 7374 726f 6b65  idth="53" stroke
-00003020: 2d6c 696e 656a 6f69 6e3d 2272 6f75 6e64  -linejoin="round
-00003030: 2220 7374 726f 6b65 2d6c 696e 6563 6170  " stroke-linecap
-00003040: 3d22 7371 7561 7265 2220 643d 224d 2031  ="square" d="M 1
-00003050: 3033 322c 3630 3030 204c 2033 3936 382c  032,6000 L 3968,
-00003060: 3630 3030 222f 3e0a 2020 2020 3c70 6174  6000"/>.    <pat
-00003070: 6820 6669 6c6c 3d22 7267 6228 302c 302c  h fill="rgb(0,0,
-00003080: 3029 2220 7374 726f 6b65 3d22 6e6f 6e65  0)" stroke="none
-00003090: 2220 643d 224d 2031 3030 302c 3632 3530  " d="M 1000,6250
-000030a0: 204c 2031 3030 302c 3630 3834 2031 3030   L 1000,6084 100
-000030b0: 302c 3539 3137 2031 3030 302c 3537 3530  0,5917 1000,5750
-000030c0: 2031 3032 322c 3537 3530 2031 3034 332c   1022,5750 1043,
-000030d0: 3537 3530 2031 3036 362c 3537 3530 2031  5750 1066,5750 1
-000030e0: 3036 362c 3539 3136 2031 3036 362c 3630  066,5916 1066,60
-000030f0: 3833 2031 3036 362c 3632 3530 2031 3034  83 1066,6250 104
-00003100: 342c 3632 3530 2031 3032 332c 3632 3530  4,6250 1023,6250
-00003110: 2031 3030 302c 3632 3530 205a 222f 3e0a   1000,6250 Z"/>.
-00003120: 2020 2020 3c70 6174 6820 6669 6c6c 3d22      <path fill="
-00003130: 7267 6228 302c 302c 3029 2220 7374 726f  rgb(0,0,0)" stro
-00003140: 6b65 3d22 6e6f 6e65 2220 643d 224d 2034  ke="none" d="M 4
-00003150: 3030 302c 3537 3530 204c 2034 3030 302c  000,5750 L 4000,
-00003160: 3539 3136 2034 3030 302c 3630 3833 2034  5916 4000,6083 4
-00003170: 3030 302c 3632 3530 2033 3937 382c 3632  000,6250 3978,62
-00003180: 3530 2033 3935 372c 3632 3530 2033 3933  50 3957,6250 393
-00003190: 342c 3632 3530 2033 3933 342c 3630 3834  4,6250 3934,6084
-000031a0: 2033 3933 342c 3539 3137 2033 3933 342c   3934,5917 3934,
-000031b0: 3537 3530 2033 3935 362c 3537 3530 2033  5750 3956,5750 3
-000031c0: 3937 372c 3537 3530 2034 3030 302c 3537  977,5750 4000,57
-000031d0: 3530 205a 222f 3e0a 2020 203c 2f67 3e0a  50 Z"/>.   </g>.
-000031e0: 2020 3c2f 673e 0a20 203c 6720 636c 6173    </g>.  <g clas
-000031f0: 733d 2263 6f6d 2e73 756e 2e73 7461 722e  s="com.sun.star.
-00003200: 6472 6177 696e 672e 4375 7374 6f6d 5368  drawing.CustomSh
-00003210: 6170 6522 3e0a 2020 203c 6720 6964 3d22  ape">.   <g id="
-00003220: 6964 3130 223e 0a20 2020 203c 7265 6374  id10">.    <rect
-00003230: 2063 6c61 7373 3d22 426f 756e 6469 6e67   class="Bounding
-00003240: 426f 7822 2073 7472 6f6b 653d 226e 6f6e  Box" stroke="non
-00003250: 6522 2066 696c 6c3d 226e 6f6e 6522 2078  e" fill="none" x
-00003260: 3d22 3430 3030 2220 793d 2235 3530 3022  ="4000" y="5500"
-00003270: 2077 6964 7468 3d22 3130 3031 2220 6865   width="1001" he
-00003280: 6967 6874 3d22 3130 3031 222f 3e0a 2020  ight="1001"/>.  
-00003290: 2020 3c70 6174 6820 6669 6c6c 3d22 7267    <path fill="rg
-000032a0: 6228 3139 322c 3139 322c 3139 3229 2220  b(192,192,192)" 
-000032b0: 7374 726f 6b65 3d22 6e6f 6e65 2220 643d  stroke="none" d=
-000032c0: 224d 2034 3530 302c 3635 3030 204c 2034  "M 4500,6500 L 4
-000032d0: 3030 302c 3635 3030 2034 3030 302c 3535  000,6500 4000,55
-000032e0: 3030 2035 3030 302c 3535 3030 2035 3030  00 5000,5500 500
-000032f0: 302c 3635 3030 2034 3530 302c 3635 3030  0,6500 4500,6500
-00003300: 205a 222f 3e0a 2020 203c 2f67 3e0a 2020   Z"/>.   </g>.  
-00003310: 3c2f 673e 0a20 203c 6720 636c 6173 733d  </g>.  <g class=
-00003320: 2263 6f6d 2e73 756e 2e73 7461 722e 6472  "com.sun.star.dr
-00003330: 6177 696e 672e 4375 7374 6f6d 5368 6170  awing.CustomShap
-00003340: 6522 3e0a 2020 203c 6720 6964 3d22 6964  e">.   <g id="id
-00003350: 3131 223e 0a20 2020 203c 7265 6374 2063  11">.    <rect c
-00003360: 6c61 7373 3d22 426f 756e 6469 6e67 426f  lass="BoundingBo
-00003370: 7822 2073 7472 6f6b 653d 226e 6f6e 6522  x" stroke="none"
-00003380: 2066 696c 6c3d 226e 6f6e 6522 2078 3d22   fill="none" x="
-00003390: 3530 3030 2220 793d 2235 3530 3022 2077  5000" y="5500" w
-000033a0: 6964 7468 3d22 3130 3031 2220 6865 6967  idth="1001" heig
-000033b0: 6874 3d22 3130 3031 222f 3e0a 2020 2020  ht="1001"/>.    
-000033c0: 3c70 6174 6820 6669 6c6c 3d22 7267 6228  <path fill="rgb(
-000033d0: 3139 322c 3139 322c 3139 3229 2220 7374  192,192,192)" st
-000033e0: 726f 6b65 3d22 6e6f 6e65 2220 643d 224d  roke="none" d="M
-000033f0: 2035 3530 302c 3635 3030 204c 2035 3030   5500,6500 L 500
-00003400: 302c 3635 3030 2035 3030 302c 3535 3030  0,6500 5000,5500
-00003410: 2036 3030 302c 3535 3030 2036 3030 302c   6000,5500 6000,
-00003420: 3635 3030 2035 3530 302c 3635 3030 205a  6500 5500,6500 Z
-00003430: 222f 3e0a 2020 203c 2f67 3e0a 2020 3c2f  "/>.   </g>.  </
-00003440: 673e 0a20 203c 6720 636c 6173 733d 2263  g>.  <g class="c
-00003450: 6f6d 2e73 756e 2e73 7461 722e 6472 6177  om.sun.star.draw
-00003460: 696e 672e 4375 7374 6f6d 5368 6170 6522  ing.CustomShape"
-00003470: 3e0a 2020 203c 6720 6964 3d22 6964 3132  >.   <g id="id12
-00003480: 223e 0a20 2020 203c 7265 6374 2063 6c61  ">.    <rect cla
-00003490: 7373 3d22 426f 756e 6469 6e67 426f 7822  ss="BoundingBox"
-000034a0: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
-000034b0: 696c 6c3d 226e 6f6e 6522 2078 3d22 3131  ill="none" x="11
-000034c0: 3530 3022 2079 3d22 3430 3030 2220 7769  500" y="4000" wi
-000034d0: 6474 683d 2231 3530 3122 2068 6569 6768  dth="1501" heigh
-000034e0: 743d 2231 3030 3122 2f3e 0a20 2020 203c  t="1001"/>.    <
-000034f0: 7061 7468 2066 696c 6c3d 2272 6762 2831  path fill="rgb(1
-00003500: 3030 2c31 3439 2c32 3337 2922 2073 7472  00,149,237)" str
-00003510: 6f6b 653d 226e 6f6e 6522 2064 3d22 4d20  oke="none" d="M 
-00003520: 3132 3235 302c 3530 3030 204c 2031 3135  12250,5000 L 115
-00003530: 3030 2c35 3030 3020 3131 3530 302c 3430  00,5000 11500,40
-00003540: 3030 2031 3330 3030 2c34 3030 3020 3133  00 13000,4000 13
-00003550: 3030 302c 3530 3030 2031 3232 3530 2c35  000,5000 12250,5
-00003560: 3030 3020 5a22 2f3e 0a20 2020 203c 7465  000 Z"/>.    <te
-00003570: 7874 2063 6c61 7373 3d22 5356 4754 6578  xt class="SVGTex
-00003580: 7453 6861 7065 223e 3c74 7370 616e 2063  tShape"><tspan c
-00003590: 6c61 7373 3d22 5465 7874 5061 7261 6772  lass="TextParagr
-000035a0: 6170 6822 2066 6f6e 742d 6661 6d69 6c79  aph" font-family
-000035b0: 3d22 4c69 6265 7261 7469 6f6e 2053 616e  ="Liberation San
-000035c0: 732c 2073 616e 732d 7365 7269 6622 2066  s, sans-serif" f
-000035d0: 6f6e 742d 7369 7a65 3d22 3633 3570 7822  ont-size="635px"
-000035e0: 2066 6f6e 742d 7765 6967 6874 3d22 3430   font-weight="40
-000035f0: 3022 3e3c 7473 7061 6e20 636c 6173 733d  0"><tspan class=
-00003600: 2254 6578 7450 6f73 6974 696f 6e22 2078  "TextPosition" x
-00003610: 3d22 3131 3839 3922 2079 3d22 3437 3231  ="11899" y="4721
-00003620: 223e 3c74 7370 616e 2066 696c 6c3d 2272  "><tspan fill="r
-00003630: 6762 2830 2c30 2c30 2922 2073 7472 6f6b  gb(0,0,0)" strok
-00003640: 653d 226e 6f6e 6522 2073 7479 6c65 3d22  e="none" style="
-00003650: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
-00003660: 223e 2333 3c2f 7473 7061 6e3e 3c2f 7473  ">#3</tspan></ts
-00003670: 7061 6e3e 3c2f 7473 7061 6e3e 3c2f 7465  pan></tspan></te
-00003680: 7874 3e0a 2020 203c 2f67 3e0a 2020 3c2f  xt>.   </g>.  </
-00003690: 673e 0a20 203c 6720 636c 6173 733d 2263  g>.  <g class="c
-000036a0: 6f6d 2e73 756e 2e73 7461 722e 6472 6177  om.sun.star.draw
-000036b0: 696e 672e 4375 7374 6f6d 5368 6170 6522  ing.CustomShape"
-000036c0: 3e0a 2020 203c 6720 6964 3d22 6964 3133  >.   <g id="id13
-000036d0: 223e 0a20 2020 203c 7265 6374 2063 6c61  ">.    <rect cla
-000036e0: 7373 3d22 426f 756e 6469 6e67 426f 7822  ss="BoundingBox"
-000036f0: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
-00003700: 696c 6c3d 226e 6f6e 6522 2078 3d22 3131  ill="none" x="11
-00003710: 3530 3022 2079 3d22 3535 3030 2220 7769  500" y="5500" wi
-00003720: 6474 683d 2231 3530 3122 2068 6569 6768  dth="1501" heigh
-00003730: 743d 2231 3030 3122 2f3e 0a20 2020 203c  t="1001"/>.    <
-00003740: 7061 7468 2066 696c 6c3d 2272 6762 2831  path fill="rgb(1
-00003750: 3932 2c31 3932 2c31 3932 2922 2073 7472  92,192,192)" str
-00003760: 6f6b 653d 226e 6f6e 6522 2064 3d22 4d20  oke="none" d="M 
-00003770: 3132 3235 302c 3635 3030 204c 2031 3135  12250,6500 L 115
-00003780: 3030 2c36 3530 3020 3131 3530 302c 3535  00,6500 11500,55
-00003790: 3030 2031 3330 3030 2c35 3530 3020 3133  00 13000,5500 13
-000037a0: 3030 302c 3635 3030 2031 3232 3530 2c36  000,6500 12250,6
-000037b0: 3530 3020 5a22 2f3e 0a20 2020 3c2f 673e  500 Z"/>.   </g>
-000037c0: 0a20 203c 2f67 3e0a 2020 3c67 2063 6c61  .  </g>.  <g cla
-000037d0: 7373 3d22 636f 6d2e 7375 6e2e 7374 6172  ss="com.sun.star
-000037e0: 2e64 7261 7769 6e67 2e4c 696e 6553 6861  .drawing.LineSha
-000037f0: 7065 223e 0a20 2020 3c67 2069 643d 2269  pe">.   <g id="i
-00003800: 6431 3422 3e0a 2020 2020 3c72 6563 7420  d14">.    <rect 
-00003810: 636c 6173 733d 2242 6f75 6e64 696e 6742  class="BoundingB
-00003820: 6f78 2220 7374 726f 6b65 3d22 6e6f 6e65  ox" stroke="none
-00003830: 2220 6669 6c6c 3d22 6e6f 6e65 2220 783d  " fill="none" x=
-00003840: 2236 3030 3022 2079 3d22 3537 3530 2220  "6000" y="5750" 
-00003850: 7769 6474 683d 2233 3030 3122 2068 6569  width="3001" hei
-00003860: 6768 743d 2235 3031 222f 3e0a 2020 2020  ght="501"/>.    
-00003870: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-00003880: 2220 7374 726f 6b65 3d22 7267 6228 302c  " stroke="rgb(0,
-00003890: 302c 3029 2220 7374 726f 6b65 2d77 6964  0,0)" stroke-wid
-000038a0: 7468 3d22 3533 2220 7374 726f 6b65 2d6c  th="53" stroke-l
-000038b0: 696e 656a 6f69 6e3d 2272 6f75 6e64 2220  inejoin="round" 
-000038c0: 7374 726f 6b65 2d6c 696e 6563 6170 3d22  stroke-linecap="
-000038d0: 7371 7561 7265 2220 643d 224d 2036 3033  square" d="M 603
-000038e0: 322c 3630 3030 204c 2038 3936 382c 3630  2,6000 L 8968,60
-000038f0: 3030 222f 3e0a 2020 2020 3c70 6174 6820  00"/>.    <path 
-00003900: 6669 6c6c 3d22 7267 6228 302c 302c 3029  fill="rgb(0,0,0)
-00003910: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00003920: 643d 224d 2036 3030 302c 3632 3530 204c  d="M 6000,6250 L
-00003930: 2036 3030 302c 3630 3834 2036 3030 302c   6000,6084 6000,
-00003940: 3539 3137 2036 3030 302c 3537 3530 2036  5917 6000,5750 6
-00003950: 3032 322c 3537 3530 2036 3034 332c 3537  022,5750 6043,57
-00003960: 3530 2036 3036 362c 3537 3530 2036 3036  50 6066,5750 606
-00003970: 362c 3539 3136 2036 3036 362c 3630 3833  6,5916 6066,6083
-00003980: 2036 3036 362c 3632 3530 2036 3034 342c   6066,6250 6044,
-00003990: 3632 3530 2036 3032 332c 3632 3530 2036  6250 6023,6250 6
-000039a0: 3030 302c 3632 3530 205a 222f 3e0a 2020  000,6250 Z"/>.  
-000039b0: 2020 3c70 6174 6820 6669 6c6c 3d22 7267    <path fill="rg
-000039c0: 6228 302c 302c 3029 2220 7374 726f 6b65  b(0,0,0)" stroke
-000039d0: 3d22 6e6f 6e65 2220 643d 224d 2039 3030  ="none" d="M 900
-000039e0: 302c 3537 3530 204c 2039 3030 302c 3539  0,5750 L 9000,59
-000039f0: 3136 2039 3030 302c 3630 3833 2039 3030  16 9000,6083 900
-00003a00: 302c 3632 3530 2038 3937 382c 3632 3530  0,6250 8978,6250
-00003a10: 2038 3935 372c 3632 3530 2038 3933 342c   8957,6250 8934,
-00003a20: 3632 3530 2038 3933 342c 3630 3834 2038  6250 8934,6084 8
-00003a30: 3933 342c 3539 3137 2038 3933 342c 3537  934,5917 8934,57
-00003a40: 3530 2038 3935 362c 3537 3530 2038 3937  50 8956,5750 897
-00003a50: 372c 3537 3530 2039 3030 302c 3537 3530  7,5750 9000,5750
-00003a60: 205a 222f 3e0a 2020 203c 2f67 3e0a 2020   Z"/>.   </g>.  
-00003a70: 3c2f 673e 0a20 3c2f 673e 0a3c 2f73 7667  </g>. </g>.</svg
-00003a80: 3e                                       >
+000000a0: 7468 3d22 3132 302e 3034 6d6d 2220 6865  th="120.04mm" he
+000000b0: 6967 6874 3d22 3830 2e30 326d 6d22 2076  ight="80.02mm" v
+000000c0: 6965 7742 6f78 3d22 3939 3920 3130 3030  iewBox="999 1000
+000000d0: 2031 3230 3034 2038 3030 3222 2070 7265   12004 8002" pre
+000000e0: 7365 7276 6541 7370 6563 7452 6174 696f  serveAspectRatio
+000000f0: 3d22 784d 6964 594d 6964 2220 6669 6c6c  ="xMidYMid" fill
+00000100: 2d72 756c 653d 2265 7665 6e6f 6464 2220  -rule="evenodd" 
+00000110: 7374 726f 6b65 2d77 6964 7468 3d22 3238  stroke-width="28
+00000120: 2e32 3232 2220 7374 726f 6b65 2d6c 696e  .222" stroke-lin
+00000130: 656a 6f69 6e3d 2272 6f75 6e64 2220 786d  ejoin="round" xm
+00000140: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00000150: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
+00000160: 2078 6d6c 6e73 3a6f 6f6f 3d22 6874 7470   xmlns:ooo="http
+00000170: 3a2f 2f78 6d6c 2e6f 7065 6e6f 6666 6963  ://xml.openoffic
+00000180: 652e 6f72 672f 7376 672f 6578 706f 7274  e.org/svg/export
+00000190: 2220 786d 6c6e 733a 786c 696e 6b3d 2268  " xmlns:xlink="h
+000001a0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+000001b0: 2f31 3939 392f 786c 696e 6b22 2078 6d6c  /1999/xlink" xml
+000001c0: 6e73 3a70 7265 7365 6e74 6174 696f 6e3d  ns:presentation=
+000001d0: 2268 7474 703a 2f2f 7375 6e2e 636f 6d2f  "http://sun.com/
+000001e0: 786d 6c6e 732f 7374 6172 6f66 6669 6365  xmlns/staroffice
+000001f0: 2f70 7265 7365 6e74 6174 696f 6e22 2078  /presentation" x
+00000200: 6d6c 6e73 3a73 6d69 6c3d 2268 7474 703a  mlns:smil="http:
+00000210: 2f2f 7777 772e 7733 2e6f 7267 2f32 3030  //www.w3.org/200
+00000220: 312f 534d 494c 3230 2f22 2078 6d6c 6e73  1/SMIL20/" xmlns
+00000230: 3a61 6e69 6d3d 2275 726e 3a6f 6173 6973  :anim="urn:oasis
+00000240: 3a6e 616d 6573 3a74 633a 6f70 656e 646f  :names:tc:opendo
+00000250: 6375 6d65 6e74 3a78 6d6c 6e73 3a61 6e69  cument:xmlns:ani
+00000260: 6d61 7469 6f6e 3a31 2e30 2220 786d 6c3a  mation:1.0" xml:
+00000270: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
+00000280: 3e0a 203c 6465 6673 3e0a 2020 3c66 6f6e  >. <defs>.  <fon
+00000290: 7420 6964 3d22 456d 6265 6464 6564 466f  t id="EmbeddedFo
+000002a0: 6e74 5f31 2220 686f 7269 7a2d 6164 762d  nt_1" horiz-adv-
+000002b0: 783d 2232 3034 3822 3e0a 2020 203c 666f  x="2048">.   <fo
+000002c0: 6e74 2d66 6163 6520 666f 6e74 2d66 616d  nt-face font-fam
+000002d0: 696c 793d 224c 6962 6572 6174 696f 6e20  ily="Liberation 
+000002e0: 5361 6e73 2065 6d62 6564 6465 6422 2075  Sans embedded" u
+000002f0: 6e69 7473 2d70 6572 2d65 6d3d 2232 3034  nits-per-em="204
+00000300: 3822 2066 6f6e 742d 7765 6967 6874 3d22  8" font-weight="
+00000310: 6e6f 726d 616c 2220 666f 6e74 2d73 7479  normal" font-sty
+00000320: 6c65 3d22 6e6f 726d 616c 2220 6173 6365  le="normal" asce
+00000330: 6e74 3d22 3138 3532 2220 6465 7363 656e  nt="1852" descen
+00000340: 743d 2234 3233 222f 3e0a 2020 203c 6d69  t="423"/>.   <mi
+00000350: 7373 696e 672d 676c 7970 6820 686f 7269  ssing-glyph hori
+00000360: 7a2d 6164 762d 783d 2232 3034 3822 2064  z-adv-x="2048" d
+00000370: 3d22 4d20 302c 3020 4c20 3230 3437 2c30  ="M 0,0 L 2047,0
+00000380: 2032 3034 372c 3230 3437 2030 2c32 3034   2047,2047 0,204
+00000390: 3720 302c 3020 5a22 2f3e 0a20 2020 3c67  7 0,0 Z"/>.   <g
+000003a0: 6c79 7068 2075 6e69 636f 6465 3d22 7522  lyph unicode="u"
+000003b0: 2068 6f72 697a 2d61 6476 2d78 3d22 3837   horiz-adv-x="87
+000003c0: 3422 2064 3d22 4d20 3331 342c 3130 3832  4" d="M 314,1082
+000003d0: 204c 2033 3134 2c33 3936 2043 2033 3134   L 314,396 C 314
+000003e0: 2c33 3235 2033 3231 2c32 3639 2033 3335  ,325 321,269 335
+000003f0: 2c32 3330 2033 3439 2c31 3931 2033 3731  ,230 349,191 371
+00000400: 2c31 3632 2034 3032 2c31 3435 2034 3333  ,162 402,145 433
+00000410: 2c31 3238 2034 3738 2c31 3139 2035 3337  ,128 478,119 537
+00000420: 2c31 3139 2036 3234 2c31 3139 2036 3932  ,119 624,119 692
+00000430: 2c31 3439 2037 3432 2c32 3038 2037 3932  ,149 742,208 792
+00000440: 2c32 3637 2038 3137 2c33 3530 2038 3137  ,267 817,350 817
+00000450: 2c34 3535 204c 2038 3137 2c31 3038 3220  ,455 L 817,1082 
+00000460: 3939 372c 3130 3832 2039 3937 2c32 3331  997,1082 997,231
+00000470: 2043 2039 3937 2c31 3035 2039 3939 2c32   C 997,105 999,2
+00000480: 3820 3130 3033 2c30 204c 2038 3333 2c30  8 1003,0 L 833,0
+00000490: 2043 2038 3332 2c33 2038 3332 2c31 3220   C 832,3 832,12 
+000004a0: 3833 312c 3237 2038 3330 2c34 3220 3833  831,27 830,42 83
+000004b0: 302c 3539 2038 3239 2c37 3820 3832 382c  0,59 829,78 828,
+000004c0: 3937 2038 3236 2c31 3332 2038 3235 2c31  97 826,132 825,1
+000004d0: 3835 204c 2038 3232 2c31 3835 2043 2037  85 L 822,185 C 7
+000004e0: 3831 2c31 3130 2037 3333 2c35 3820 3637  81,110 733,58 67
+000004f0: 392c 3237 2036 3234 2c2d 3420 3535 372c  9,27 624,-4 557,
+00000500: 2d32 3020 3437 362c 2d32 3020 3335 372c  -20 476,-20 357,
+00000510: 2d32 3020 3237 312c 3130 2032 3136 2c36  -20 271,10 216,6
+00000520: 3920 3136 312c 3132 3820 3133 332c 3232  9 161,128 133,22
+00000530: 3520 3133 332c 3336 3120 4c20 3133 332c  5 133,361 L 133,
+00000540: 3130 3832 2033 3134 2c31 3038 3220 5a22  1082 314,1082 Z"
+00000550: 2f3e 0a20 2020 3c67 6c79 7068 2075 6e69  />.   <glyph uni
+00000560: 636f 6465 3d22 7122 2068 6f72 697a 2d61  code="q" horiz-a
+00000570: 6476 2d78 3d22 3932 3722 2064 3d22 4d20  dv-x="927" d="M 
+00000580: 3438 342c 2d32 3020 4320 3334 372c 2d32  484,-20 C 347,-2
+00000590: 3020 3234 362c 3236 2031 3832 2c31 3139  0 246,26 182,119
+000005a0: 2031 3138 2c32 3132 2038 362c 3335 3120   118,212 86,351 
+000005b0: 3836 2c35 3336 2038 362c 3931 3320 3231  86,536 86,913 21
+000005c0: 392c 3131 3032 2034 3834 2c31 3130 3220  9,1102 484,1102 
+000005d0: 3536 362c 3131 3032 2036 3334 2c31 3038  566,1102 634,108
+000005e0: 3820 3638 372c 3130 3539 2037 3430 2c31  8 687,1059 740,1
+000005f0: 3033 3020 3738 352c 3938 3120 3832 312c  030 785,981 821,
+00000600: 3931 3420 4c20 3832 332c 3931 3420 4320  914 L 823,914 C 
+00000610: 3832 332c 3933 3420 3832 342c 3936 3920  823,934 824,969 
+00000620: 3832 372c 3130 3138 2038 3330 2c31 3036  827,1018 830,106
+00000630: 3720 3833 322c 3130 3933 2038 3335 2c31  7 832,1093 835,1
+00000640: 3039 3620 4c20 3130 3038 2c31 3039 3620  096 L 1008,1096 
+00000650: 4320 3130 3033 2c31 3035 3720 3130 3031  C 1003,1057 1001
+00000660: 2c39 3538 2031 3030 312c 3830 3120 4c20  ,958 1001,801 L 
+00000670: 3130 3031 2c2d 3432 3520 3832 312c 2d34  1001,-425 821,-4
+00000680: 3235 2038 3231 2c31 3420 3832 352c 3137  25 821,14 825,17
+00000690: 3820 3832 332c 3137 3820 4320 3738 372c  8 823,178 C 787,
+000006a0: 3130 3720 3734 332c 3536 2036 3930 2c32  107 743,56 690,2
+000006b0: 3620 3633 372c 2d35 2035 3639 2c2d 3230  6 637,-5 569,-20
+000006c0: 2034 3834 2c2d 3230 205a 204d 2038 3231   484,-20 Z M 821
+000006d0: 2c35 3534 2043 2038 3231 2c36 3935 2037  ,554 C 821,695 7
+000006e0: 3938 2c37 3939 2037 3532 2c38 3637 2037  98,799 752,867 7
+000006f0: 3036 2c39 3335 2036 3333 2c39 3639 2035  06,935 633,969 5
+00000700: 3332 2c39 3639 2034 3431 2c39 3639 2033  32,969 441,969 3
+00000710: 3735 2c39 3335 2033 3335 2c38 3637 2032  75,935 335,867 2
+00000720: 3935 2c37 3939 2032 3735 2c36 3931 2032  95,799 275,691 2
+00000730: 3735 2c35 3432 2032 3735 2c33 3931 2032  75,542 275,391 2
+00000740: 3935 2c32 3832 2033 3336 2c32 3137 2033  95,282 336,217 3
+00000750: 3736 2c31 3532 2034 3431 2c31 3139 2035  76,152 441,119 5
+00000760: 3330 2c31 3139 2036 3332 2c31 3139 2037  30,119 632,119 7
+00000770: 3036 2c31 3535 2037 3532 2c32 3238 2037  06,155 752,228 7
+00000780: 3938 2c33 3031 2038 3231 2c34 3039 2038  98,301 821,409 8
+00000790: 3231 2c35 3534 205a 222f 3e0a 2020 203c  21,554 Z"/>.   <
+000007a0: 676c 7970 6820 756e 6963 6f64 653d 226e  glyph unicode="n
+000007b0: 2220 686f 7269 7a2d 6164 762d 783d 2238  " horiz-adv-x="8
+000007c0: 3734 2220 643d 224d 2038 3235 2c30 204c  74" d="M 825,0 L
+000007d0: 2038 3235 2c36 3836 2043 2038 3235 2c37   825,686 C 825,7
+000007e0: 3537 2038 3138 2c38 3133 2038 3034 2c38  57 818,813 804,8
+000007f0: 3532 2037 3930 2c38 3931 2037 3638 2c39  52 790,891 768,9
+00000800: 3230 2037 3337 2c39 3337 2037 3036 2c39  20 737,937 706,9
+00000810: 3534 2036 3631 2c39 3633 2036 3032 2c39  54 661,963 602,9
+00000820: 3633 2035 3135 2c39 3633 2034 3437 2c39  63 515,963 447,9
+00000830: 3333 2033 3937 2c38 3734 2033 3437 2c38  33 397,874 347,8
+00000840: 3135 2033 3232 2c37 3332 2033 3232 2c36  15 322,732 322,6
+00000850: 3237 204c 2033 3232 2c30 2031 3432 2c30  27 L 322,0 142,0
+00000860: 2031 3432 2c38 3531 2043 2031 3432 2c39   142,851 C 142,9
+00000870: 3737 2031 3430 2c31 3035 3420 3133 362c  77 140,1054 136,
+00000880: 3130 3832 204c 2033 3036 2c31 3038 3220  1082 L 306,1082 
+00000890: 4320 3330 372c 3130 3739 2033 3037 2c31  C 307,1079 307,1
+000008a0: 3037 3020 3330 382c 3130 3535 2033 3039  070 308,1055 309
+000008b0: 2c31 3034 3020 3331 302c 3130 3234 2033  ,1040 310,1024 3
+000008c0: 3131 2c31 3030 3520 3331 322c 3938 3620  11,1005 312,986 
+000008d0: 3331 332c 3935 3020 3331 342c 3839 3720  313,950 314,897 
+000008e0: 4c20 3331 372c 3839 3720 4320 3335 382c  L 317,897 C 358,
+000008f0: 3937 3220 3430 362c 3130 3235 2034 3631  972 406,1025 461
+00000900: 2c31 3035 3620 3531 352c 3130 3837 2035  ,1056 515,1087 5
+00000910: 3832 2c31 3130 3220 3636 332c 3131 3032  82,1102 663,1102
+00000920: 2037 3832 2c31 3130 3220 3836 392c 3130   782,1102 869,10
+00000930: 3733 2039 3234 2c31 3031 3420 3937 392c  73 924,1014 979,
+00000940: 3935 3520 3130 3036 2c38 3537 2031 3030  955 1006,857 100
+00000950: 362c 3732 3120 4c20 3130 3036 2c30 2038  6,721 L 1006,0 8
+00000960: 3235 2c30 205a 222f 3e0a 2020 203c 676c  25,0 Z"/>.   <gl
+00000970: 7970 6820 756e 6963 6f64 653d 2265 2220  yph unicode="e" 
+00000980: 686f 7269 7a2d 6164 762d 783d 2239 3830  horiz-adv-x="980
+00000990: 2220 643d 224d 2032 3736 2c35 3033 2043  " d="M 276,503 C
+000009a0: 2032 3736 2c33 3739 2033 3032 2c32 3833   276,379 302,283
+000009b0: 2033 3533 2c32 3136 2034 3034 2c31 3439   353,216 404,149
+000009c0: 2034 3739 2c31 3135 2035 3738 2c31 3135   479,115 578,115
+000009d0: 2036 3536 2c31 3135 2037 3139 2c31 3331   656,115 719,131
+000009e0: 2037 3636 2c31 3632 2038 3133 2c31 3933   766,162 813,193
+000009f0: 2038 3434 2c32 3333 2038 3631 2c32 3831   844,233 861,281
+00000a00: 204c 2031 3031 392c 3233 3620 4320 3935   L 1019,236 C 95
+00000a10: 342c 3635 2038 3037 2c2d 3230 2035 3738  4,65 807,-20 578
+00000a20: 2c2d 3230 2034 3138 2c2d 3230 2032 3936  ,-20 418,-20 296
+00000a30: 2c32 3820 3231 332c 3132 3320 3132 392c  ,28 213,123 129,
+00000a40: 3231 3820 3837 2c33 3630 2038 372c 3534  218 87,360 87,54
+00000a50: 3820 3837 2c37 3237 2031 3239 2c38 3634  8 87,727 129,864
+00000a60: 2032 3133 2c39 3539 2032 3936 2c31 3035   213,959 296,105
+00000a70: 3420 3431 362c 3131 3032 2035 3731 2c31  4 416,1102 571,1
+00000a80: 3130 3220 3838 392c 3131 3032 2031 3034  102 889,1102 104
+00000a90: 382c 3931 3020 3130 3438 2c35 3237 204c  8,910 1048,527 L
+00000aa0: 2031 3034 382c 3530 3320 3237 362c 3530   1048,503 276,50
+00000ab0: 3320 5a20 4d20 3836 322c 3634 3120 4320  3 Z M 862,641 C 
+00000ac0: 3835 322c 3735 3520 3832 332c 3833 3820  852,755 823,838 
+00000ad0: 3737 352c 3839 3120 3732 372c 3934 3320  775,891 727,943 
+00000ae0: 3635 382c 3936 3920 3536 382c 3936 3920  658,969 568,969 
+00000af0: 3438 312c 3936 3920 3431 322c 3934 3020  481,969 412,940 
+00000b00: 3336 312c 3838 3220 3331 302c 3832 3320  361,882 310,823 
+00000b10: 3238 322c 3734 3320 3237 382c 3634 3120  282,743 278,641 
+00000b20: 4c20 3836 322c 3634 3120 5a22 2f3e 0a20  L 862,641 Z"/>. 
+00000b30: 2020 3c67 6c79 7068 2075 6e69 636f 6465    <glyph unicode
+00000b40: 3d22 6322 2068 6f72 697a 2d61 6476 2d78  ="c" horiz-adv-x
+00000b50: 3d22 3930 3122 2064 3d22 4d20 3237 352c  ="901" d="M 275,
+00000b60: 3534 3620 4320 3237 352c 3430 3220 3239  546 C 275,402 29
+00000b70: 382c 3239 3520 3334 332c 3232 3620 3338  8,295 343,226 38
+00000b80: 382c 3135 3720 3435 372c 3132 3220 3534  8,157 457,122 54
+00000b90: 382c 3132 3220 3631 322c 3132 3220 3636  8,122 612,122 66
+00000ba0: 362c 3133 3920 3730 392c 3137 3420 3735  6,139 709,174 75
+00000bb0: 322c 3230 3920 3737 382c 3236 3220 3738  2,209 778,262 78
+00000bc0: 382c 3333 3420 4c20 3937 302c 3332 3220  8,334 L 970,322 
+00000bd0: 4320 3935 362c 3231 3820 3931 322c 3133  C 956,218 912,13
+00000be0: 3520 3833 372c 3733 2037 3632 2c31 3120  5 837,73 762,11 
+00000bf0: 3636 382c 2d32 3020 3535 332c 2d32 3020  668,-20 553,-20 
+00000c00: 3430 322c 2d32 3020 3238 362c 3238 2032  402,-20 286,28 2
+00000c10: 3037 2c31 3234 2031 3237 2c32 3139 2038  07,124 127,219 8
+00000c20: 372c 3335 3920 3837 2c35 3432 2038 372c  7,359 87,542 87,
+00000c30: 3732 3420 3132 372c 3836 3320 3230 372c  724 127,863 207,
+00000c40: 3935 3920 3238 372c 3130 3534 2034 3032  959 287,1054 402
+00000c50: 2c31 3130 3220 3535 312c 3131 3032 2036  ,1102 551,1102 6
+00000c60: 3632 2c31 3130 3220 3735 342c 3130 3733  62,1102 754,1073
+00000c70: 2038 3237 2c31 3031 3620 3930 302c 3935   827,1016 900,95
+00000c80: 3920 3934 352c 3838 3020 3936 342c 3737  9 945,880 964,77
+00000c90: 3920 4c20 3737 392c 3736 3520 4320 3737  9 L 779,765 C 77
+00000ca0: 302c 3832 3520 3734 362c 3837 3320 3730  0,825 746,873 70
+00000cb0: 382c 3930 3820 3637 302c 3934 3320 3631  8,908 670,943 61
+00000cc0: 362c 3936 3120 3534 362c 3936 3120 3435  6,961 546,961 45
+00000cd0: 312c 3936 3120 3338 322c 3932 3920 3333  1,961 382,929 33
+00000ce0: 392c 3836 3620 3239 362c 3830 3320 3237  9,866 296,803 27
+00000cf0: 352c 3639 3620 3237 352c 3534 3620 5a22  5,696 275,546 Z"
+00000d00: 2f3e 0a20 2020 3c67 6c79 7068 2075 6e69  />.   <glyph uni
+00000d10: 636f 6465 3d22 5322 2068 6f72 697a 2d61  code="S" horiz-a
+00000d20: 6476 2d78 3d22 3131 3932 2220 643d 224d  dv-x="1192" d="M
+00000d30: 2031 3237 322c 3338 3920 4320 3132 3732   1272,389 C 1272
+00000d40: 2c32 3539 2031 3232 312c 3135 3820 3131  ,259 1221,158 11
+00000d50: 3230 2c38 3720 3130 3138 2c31 3620 3837  20,87 1018,16 87
+00000d60: 352c 2d32 3020 3639 302c 2d32 3020 3334  5,-20 690,-20 34
+00000d70: 372c 2d32 3020 3134 382c 3939 2039 332c  7,-20 148,99 93,
+00000d80: 3333 3820 4c20 3237 382c 3337 3520 4320  338 L 278,375 C 
+00000d90: 3239 392c 3239 3020 3334 352c 3232 3820  299,290 345,228 
+00000da0: 3431 342c 3138 3920 3438 332c 3134 3920  414,189 483,149 
+00000db0: 3537 382c 3132 3920 3639 372c 3132 3920  578,129 697,129 
+00000dc0: 3832 302c 3132 3920 3931 362c 3135 3020  820,129 916,150 
+00000dd0: 3938 332c 3139 3320 3130 3530 2c32 3335  983,193 1050,235
+00000de0: 2031 3038 332c 3239 3720 3130 3833 2c33   1083,297 1083,3
+00000df0: 3739 2031 3038 332c 3432 3520 3130 3733  79 1083,425 1073
+00000e00: 2c34 3632 2031 3035 322c 3439 3120 3130  ,462 1052,491 10
+00000e10: 3331 2c35 3230 2031 3030 312c 3534 3320  31,520 1001,543 
+00000e20: 3936 332c 3536 3220 3932 352c 3538 3120  963,562 925,581 
+00000e30: 3838 302c 3539 3620 3832 372c 3630 3920  880,596 827,609 
+00000e40: 3737 342c 3632 3220 3731 362c 3633 3520  774,622 716,635 
+00000e50: 3635 322c 3635 3020 3534 312c 3637 3520  652,650 541,675 
+00000e60: 3435 362c 3639 3920 3339 392c 3732 3420  456,699 399,724 
+00000e70: 3334 312c 3734 3920 3239 352c 3737 3620  341,749 295,776 
+00000e80: 3236 322c 3830 3720 3232 392c 3833 3720  262,807 229,837 
+00000e90: 3230 332c 3837 3220 3138 362c 3931 3320  203,872 186,913 
+00000ea0: 3136 382c 3935 3420 3135 392c 3130 3030  168,954 159,1000
+00000eb0: 2031 3539 2c31 3035 3320 3135 392c 3131   159,1053 159,11
+00000ec0: 3734 2032 3035 2c31 3236 3720 3239 382c  74 205,1267 298,
+00000ed0: 3133 3332 2033 3930 2c31 3339 3720 3532  1332 390,1397 52
+00000ee0: 322c 3134 3330 2036 3934 2c31 3433 3020  2,1430 694,1430 
+00000ef0: 3835 342c 3134 3330 2039 3736 2c31 3430  854,1430 976,140
+00000f00: 3620 3130 3631 2c31 3335 3720 3131 3436  6 1061,1357 1146
+00000f10: 2c31 3330 3820 3132 3035 2c31 3232 3420  ,1308 1205,1224 
+00000f20: 3132 3339 2c31 3130 3620 4c20 3130 3531  1239,1106 L 1051
+00000f30: 2c31 3037 3320 4320 3130 3330 2c31 3134  ,1073 C 1030,114
+00000f40: 3820 3939 312c 3132 3032 2039 3333 2c31  8 991,1202 933,1
+00000f50: 3233 3620 3837 352c 3132 3639 2037 3935  236 875,1269 795
+00000f60: 2c31 3238 3620 3639 322c 3132 3836 2035  ,1286 692,1286 5
+00000f70: 3739 2c31 3238 3620 3439 332c 3132 3637  79,1286 493,1267
+00000f80: 2034 3334 2c31 3233 3020 3337 352c 3131   434,1230 375,11
+00000f90: 3933 2033 3435 2c31 3133 3720 3334 352c  93 345,1137 345,
+00000fa0: 3130 3633 2033 3435 2c31 3032 3020 3335  1063 345,1020 35
+00000fb0: 372c 3938 3420 3338 302c 3935 3620 3430  7,984 380,956 40
+00000fc0: 332c 3932 3720 3433 362c 3930 3320 3437  3,927 436,903 47
+00000fd0: 392c 3838 3420 3532 322c 3836 3420 3630  9,884 522,864 60
+00000fe0: 392c 3834 3020 3733 382c 3831 3120 3738  9,840 738,811 78
+00000ff0: 312c 3830 3120 3832 352c 3739 3120 3836  1,801 825,791 86
+00001000: 382c 3738 3120 3931 312c 3737 3020 3935  8,781 911,770 95
+00001010: 322c 3735 3820 3939 312c 3734 3420 3130  2,758 991,744 10
+00001020: 3330 2c37 3239 2031 3036 372c 3731 3220  30,729 1067,712 
+00001030: 3131 3032 2c36 3933 2031 3133 362c 3637  1102,693 1136,67
+00001040: 3420 3131 3636 2c36 3530 2031 3139 312c  4 1166,650 1191,
+00001050: 3632 3220 3132 3136 2c35 3934 2031 3233  622 1216,594 123
+00001060: 362c 3536 3120 3132 3531 2c35 3233 2031  6,561 1251,523 1
+00001070: 3236 352c 3438 3520 3132 3732 2c34 3430  265,485 1272,440
+00001080: 2031 3237 322c 3338 3920 5a22 2f3e 0a20   1272,389 Z"/>. 
+00001090: 2020 3c67 6c79 7068 2075 6e69 636f 6465    <glyph unicode
+000010a0: 3d22 5222 2068 6f72 697a 2d61 6476 2d78  ="R" horiz-adv-x
+000010b0: 3d22 3132 3434 2220 643d 224d 2031 3136  ="1244" d="M 116
+000010c0: 342c 3020 4c20 3739 382c 3538 3520 3335  4,0 L 798,585 35
+000010d0: 392c 3538 3520 3335 392c 3020 3136 382c  9,585 359,0 168,
+000010e0: 3020 3136 382c 3134 3039 2038 3331 2c31  0 168,1409 831,1
+000010f0: 3430 3920 4320 3939 302c 3134 3039 2031  409 C 990,1409 1
+00001100: 3131 322c 3133 3734 2031 3139 392c 3133  112,1374 1199,13
+00001110: 3033 2031 3238 352c 3132 3332 2031 3332  03 1285,1232 132
+00001120: 382c 3131 3333 2031 3332 382c 3130 3036  8,1133 1328,1006
+00001130: 2031 3332 382c 3930 3120 3132 3938 2c38   1328,901 1298,8
+00001140: 3133 2031 3233 372c 3734 3220 3131 3736  13 1237,742 1176
+00001150: 2c36 3731 2031 3039 312c 3632 3620 3938  ,671 1091,626 98
+00001160: 342c 3630 3720 4c20 3133 3834 2c30 2031  4,607 L 1384,0 1
+00001170: 3136 342c 3020 5a20 4d20 3131 3336 2c31  164,0 Z M 1136,1
+00001180: 3030 3420 4320 3131 3336 2c31 3038 3620  004 C 1136,1086 
+00001190: 3131 3038 2c31 3134 3920 3130 3533 2c31  1108,1149 1053,1
+000011a0: 3139 3220 3939 372c 3132 3335 2039 3137  192 997,1235 917
+000011b0: 2c31 3235 3620 3831 322c 3132 3536 204c  ,1256 812,1256 L
+000011c0: 2033 3539 2c31 3235 3620 3335 392c 3733   359,1256 359,73
+000011d0: 3620 3832 302c 3733 3620 4320 3932 312c  6 820,736 C 921,
+000011e0: 3733 3620 3939 392c 3736 3020 3130 3534  736 999,760 1054
+000011f0: 2c38 3037 2031 3130 392c 3835 3420 3131  ,807 1109,854 11
+00001200: 3336 2c39 3139 2031 3133 362c 3130 3034  36,919 1136,1004
+00001210: 205a 222f 3e0a 2020 203c 676c 7970 6820   Z"/>.   <glyph 
+00001220: 756e 6963 6f64 653d 2234 2220 686f 7269  unicode="4" hori
+00001230: 7a2d 6164 762d 783d 2231 3036 3022 2064  z-adv-x="1060" d
+00001240: 3d22 4d20 3838 312c 3331 3920 4c20 3838  ="M 881,319 L 88
+00001250: 312c 3020 3731 312c 3020 3731 312c 3331  1,0 711,0 711,31
+00001260: 3920 3437 2c33 3139 2034 372c 3435 3920  9 47,319 47,459 
+00001270: 3639 322c 3134 3039 2038 3831 2c31 3430  692,1409 881,140
+00001280: 3920 3838 312c 3436 3120 3130 3739 2c34  9 881,461 1079,4
+00001290: 3631 2031 3037 392c 3331 3920 3838 312c  61 1079,319 881,
+000012a0: 3331 3920 5a20 4d20 3731 312c 3132 3036  319 Z M 711,1206
+000012b0: 2043 2037 3130 2c31 3230 3220 3730 302c   C 710,1202 700,
+000012c0: 3131 3834 2036 3833 2c31 3135 3320 3636  1184 683,1153 66
+000012d0: 362c 3131 3232 2036 3533 2c31 3130 3020  6,1122 653,1100 
+000012e0: 3634 342c 3130 3837 204c 2032 3833 2c35  644,1087 L 283,5
+000012f0: 3535 2032 3239 2c34 3831 2032 3133 2c34  55 229,481 213,4
+00001300: 3631 2037 3131 2c34 3631 2037 3131 2c31  61 711,461 711,1
+00001310: 3230 3620 5a22 2f3e 0a20 2020 3c67 6c79  206 Z"/>.   <gly
+00001320: 7068 2075 6e69 636f 6465 3d22 3322 2068  ph unicode="3" h
+00001330: 6f72 697a 2d61 6476 2d78 3d22 3130 3036  oriz-adv-x="1006
+00001340: 2220 643d 224d 2031 3034 392c 3338 3920  " d="M 1049,389 
+00001350: 4320 3130 3439 2c32 3539 2031 3030 382c  C 1049,259 1008,
+00001360: 3135 3820 3932 352c 3837 2038 3432 2c31  158 925,87 842,1
+00001370: 3620 3732 342c 2d32 3020 3537 312c 2d32  6 724,-20 571,-2
+00001380: 3020 3432 382c 2d32 3020 3331 352c 3132  0 428,-20 315,12
+00001390: 2032 3330 2c37 3720 3134 352c 3134 3120   230,77 145,141 
+000013a0: 3934 2c32 3336 2037 382c 3336 3220 4c20  94,236 78,362 L 
+000013b0: 3236 342c 3337 3920 4320 3238 382c 3231  264,379 C 288,21
+000013c0: 3220 3339 302c 3132 3920 3537 312c 3132  2 390,129 571,12
+000013d0: 3920 3636 322c 3132 3920 3733 332c 3135  9 662,129 733,15
+000013e0: 3120 3738 352c 3139 3620 3833 362c 3234  1 785,196 836,24
+000013f0: 3120 3836 322c 3330 3720 3836 322c 3339  1 862,307 862,39
+00001400: 3520 3836 322c 3437 3220 3833 332c 3533  5 862,472 833,53
+00001410: 3220 3737 342c 3537 3520 3731 352c 3631  2 774,575 715,61
+00001420: 3820 3632 392c 3633 3920 3531 382c 3633  8 629,639 518,63
+00001430: 3920 4c20 3431 362c 3633 3920 3431 362c  9 L 416,639 416,
+00001440: 3739 3520 3531 342c 3739 3520 4320 3631  795 514,795 C 61
+00001450: 332c 3739 3520 3638 392c 3831 3720 3734  3,795 689,817 74
+00001460: 342c 3836 3020 3739 382c 3930 3320 3832  4,860 798,903 82
+00001470: 352c 3936 3220 3832 352c 3130 3338 2038  5,962 825,1038 8
+00001480: 3235 2c31 3131 3320 3830 332c 3131 3733  25,1113 803,1173
+00001490: 2037 3539 2c31 3231 3720 3731 342c 3132   759,1217 714,12
+000014a0: 3630 2036 3438 2c31 3238 3220 3536 312c  60 648,1282 561,
+000014b0: 3132 3832 2034 3832 2c31 3238 3220 3431  1282 482,1282 41
+000014c0: 382c 3132 3632 2033 3639 2c31 3232 3120  8,1262 369,1221 
+000014d0: 3332 302c 3131 3830 2032 3931 2c31 3132  320,1180 291,112
+000014e0: 3320 3238 332c 3130 3439 204c 2031 3032  3 283,1049 L 102
+000014f0: 2c31 3036 3320 4320 3131 352c 3131 3738  ,1063 C 115,1178
+00001500: 2031 3633 2c31 3236 3820 3234 362c 3133   163,1268 246,13
+00001510: 3333 2033 3238 2c31 3339 3820 3433 342c  33 328,1398 434,
+00001520: 3134 3330 2035 3633 2c31 3433 3020 3730  1430 563,1430 70
+00001530: 342c 3134 3330 2038 3134 2c31 3339 3720  4,1430 814,1397 
+00001540: 3839 332c 3133 3332 2039 3731 2c31 3236  893,1332 971,126
+00001550: 3620 3130 3130 2c31 3137 3420 3130 3130  6 1010,1174 1010
+00001560: 2c31 3035 3720 3130 3130 2c39 3637 2039  ,1057 1010,967 9
+00001570: 3835 2c38 3934 2039 3335 2c38 3338 2038  85,894 935,838 8
+00001580: 3834 2c37 3831 2038 3131 2c37 3433 2037  84,781 811,743 7
+00001590: 3135 2c37 3233 204c 2037 3135 2c37 3139  15,723 L 715,719
+000015a0: 2043 2038 3230 2c37 3038 2039 3032 2c36   C 820,708 902,6
+000015b0: 3732 2039 3631 2c36 3133 2031 3032 302c  72 961,613 1020,
+000015c0: 3535 3420 3130 3439 2c34 3739 2031 3034  554 1049,479 104
+000015d0: 392c 3338 3920 5a22 2f3e 0a20 2020 3c67  9,389 Z"/>.   <g
+000015e0: 6c79 7068 2075 6e69 636f 6465 3d22 3222  lyph unicode="2"
+000015f0: 2068 6f72 697a 2d61 6476 2d78 3d22 3935   horiz-adv-x="95
+00001600: 3422 2064 3d22 4d20 3130 332c 3020 4c20  4" d="M 103,0 L 
+00001610: 3130 332c 3132 3720 4320 3133 372c 3230  103,127 C 137,20
+00001620: 3520 3137 392c 3237 3420 3232 382c 3333  5 179,274 228,33
+00001630: 3420 3237 372c 3339 3320 3332 382c 3434  4 277,393 328,44
+00001640: 3720 3338 322c 3439 3620 3433 362c 3534  7 382,496 436,54
+00001650: 3420 3439 302c 3538 3920 3534 332c 3633  4 490,589 543,63
+00001660: 3020 3539 362c 3637 3120 3634 332c 3731  0 596,671 643,71
+00001670: 3320 3638 362c 3735 3420 3732 392c 3739  3 686,754 729,79
+00001680: 3520 3736 332c 3833 3920 3739 302c 3838  5 763,839 790,88
+00001690: 3420 3831 362c 3932 3920 3832 392c 3938  4 816,929 829,98
+000016a0: 3120 3832 392c 3130 3338 2038 3239 2c31  1 829,1038 829,1
+000016b0: 3131 3520 3830 362c 3131 3735 2037 3631  115 806,1175 761
+000016c0: 2c31 3231 3820 3731 362c 3132 3631 2036  ,1218 716,1261 6
+000016d0: 3533 2c31 3238 3220 3537 322c 3132 3832  53,1282 572,1282
+000016e0: 2034 3935 2c31 3238 3220 3433 322c 3132   495,1282 432,12
+000016f0: 3631 2033 3833 2c31 3232 3020 3333 332c  61 383,1220 333,
+00001700: 3131 3738 2033 3034 2c31 3131 3920 3239  1178 304,1119 29
+00001710: 352c 3130 3434 204c 2031 3131 2c31 3036  5,1044 L 111,106
+00001720: 3120 4320 3132 342c 3131 3734 2031 3732  1 C 124,1174 172
+00001730: 2c31 3236 3320 3235 352c 3133 3330 2033  ,1263 255,1330 3
+00001740: 3337 2c31 3339 3720 3434 332c 3134 3330  37,1397 443,1430
+00001750: 2035 3732 2c31 3433 3020 3731 342c 3134   572,1430 714,14
+00001760: 3330 2038 3233 2c31 3339 3720 3930 302c  30 823,1397 900,
+00001770: 3133 3330 2039 3736 2c31 3236 3320 3130  1330 976,1263 10
+00001780: 3134 2c31 3136 3720 3130 3134 2c31 3034  14,1167 1014,104
+00001790: 3420 3130 3134 2c39 3839 2031 3030 322c  4 1014,989 1002,
+000017a0: 3933 3520 3937 372c 3838 3120 3935 322c  935 977,881 952,
+000017b0: 3832 3720 3931 342c 3737 3320 3836 352c  827 914,773 865,
+000017c0: 3731 3920 3831 362c 3636 3520 3732 312c  719 816,665 721,
+000017d0: 3538 3120 3538 322c 3436 3820 3530 352c  581 582,468 505,
+000017e0: 3430 3520 3434 342c 3334 3920 3339 392c  405 444,349 399,
+000017f0: 3239 3920 3335 342c 3234 3820 3332 312c  299 354,248 321,
+00001800: 3230 3020 3330 312c 3135 3320 4c20 3130  200 301,153 L 10
+00001810: 3336 2c31 3533 2031 3033 362c 3020 3130  36,153 1036,0 10
+00001820: 332c 3020 5a22 2f3e 0a20 2020 3c67 6c79  3,0 Z"/>.   <gly
+00001830: 7068 2075 6e69 636f 6465 3d22 3122 2068  ph unicode="1" h
+00001840: 6f72 697a 2d61 6476 2d78 3d22 3932 3722  oriz-adv-x="927"
+00001850: 2064 3d22 4d20 3135 362c 3020 4c20 3135   d="M 156,0 L 15
+00001860: 362c 3135 3320 3531 352c 3135 3320 3531  6,153 515,153 51
+00001870: 352c 3132 3337 2031 3937 2c31 3031 3020  5,1237 197,1010 
+00001880: 3139 372c 3131 3830 2035 3330 2c31 3430  197,1180 530,140
+00001890: 3920 3639 362c 3134 3039 2036 3936 2c31  9 696,1409 696,1
+000018a0: 3533 2031 3033 392c 3135 3320 3130 3339  53 1039,153 1039
+000018b0: 2c30 2031 3536 2c30 205a 222f 3e0a 2020  ,0 156,0 Z"/>.  
+000018c0: 203c 676c 7970 6820 756e 6963 6f64 653d   <glyph unicode=
+000018d0: 2223 2220 686f 7269 7a2d 6164 762d 783d  "#" horiz-adv-x=
+000018e0: 2231 3133 3922 2064 3d22 4d20 3839 362c  "1139" d="M 896,
+000018f0: 3838 3520 4c20 3831 382c 3531 3620 3130  885 L 818,516 10
+00001900: 3738 2c35 3136 2031 3037 382c 3430 3820  78,516 1078,408 
+00001910: 3739 352c 3430 3820 3730 372c 3020 3539  795,408 707,0 59
+00001920: 372c 3020 3638 332c 3430 3820 3332 302c  7,0 683,408 320,
+00001930: 3430 3820 3233 362c 3020 3132 362c 3020  408 236,0 126,0 
+00001940: 3231 302c 3430 3820 392c 3430 3820 392c  210,408 9,408 9,
+00001950: 3531 3620 3233 342c 3531 3620 3331 322c  516 234,516 312,
+00001960: 3838 3520 3630 2c38 3835 2036 302c 3939  885 60,885 60,99
+00001970: 3320 3333 342c 3939 3320 3432 332c 3134  3 334,993 423,14
+00001980: 3031 2035 3333 2c31 3430 3120 3434 352c  01 533,1401 445,
+00001990: 3939 3320 3830 382c 3939 3320 3839 362c  993 808,993 896,
+000019a0: 3134 3031 2031 3030 362c 3134 3031 2039  1401 1006,1401 9
+000019b0: 3138 2c39 3933 2031 3132 392c 3939 3320  18,993 1129,993 
+000019c0: 3131 3239 2c38 3835 2038 3936 2c38 3835  1129,885 896,885
+000019d0: 205a 204d 2034 3235 2c38 3835 204c 2033   Z M 425,885 L 3
+000019e0: 3435 2c35 3136 2037 3037 2c35 3136 2037  45,516 707,516 7
+000019f0: 3835 2c38 3835 2034 3235 2c38 3835 205a  85,885 425,885 Z
+00001a00: 222f 3e0a 2020 203c 676c 7970 6820 756e  "/>.   <glyph un
+00001a10: 6963 6f64 653d 2220 2220 686f 7269 7a2d  icode=" " horiz-
+00001a20: 6164 762d 783d 2235 3536 222f 3e0a 2020  adv-x="556"/>.  
+00001a30: 3c2f 666f 6e74 3e0a 203c 2f64 6566 733e  </font>. </defs>
+00001a40: 0a20 3c64 6566 7320 636c 6173 733d 2245  . <defs class="E
+00001a50: 6d62 6564 6465 6442 756c 6c65 7443 6861  mbeddedBulletCha
+00001a60: 7273 223e 0a20 203c 6720 6964 3d22 6275  rs">.  <g id="bu
+00001a70: 6c6c 6574 2d63 6861 722d 7465 6d70 6c61  llet-char-templa
+00001a80: 7465 2d35 3733 3536 2220 7472 616e 7366  te-57356" transf
+00001a90: 6f72 6d3d 2273 6361 6c65 2830 2e30 3030  orm="scale(0.000
+00001aa0: 3438 3832 3831 3235 2c2d 302e 3030 3034  48828125,-0.0004
+00001ab0: 3838 3238 3132 3529 223e 0a20 2020 3c70  8828125)">.   <p
+00001ac0: 6174 6820 643d 224d 2035 3830 2c31 3134  ath d="M 580,114
+00001ad0: 3120 4c20 3131 3633 2c35 3731 2035 3830  1 L 1163,571 580
+00001ae0: 2c30 202d 342c 3537 3120 3538 302c 3131  ,0 -4,571 580,11
+00001af0: 3431 205a 222f 3e0a 2020 3c2f 673e 0a20  41 Z"/>.  </g>. 
+00001b00: 203c 6720 6964 3d22 6275 6c6c 6574 2d63   <g id="bullet-c
+00001b10: 6861 722d 7465 6d70 6c61 7465 2d35 3733  har-template-573
+00001b20: 3534 2220 7472 616e 7366 6f72 6d3d 2273  54" transform="s
+00001b30: 6361 6c65 2830 2e30 3030 3438 3832 3831  cale(0.000488281
+00001b40: 3235 2c2d 302e 3030 3034 3838 3238 3132  25,-0.0004882812
+00001b50: 3529 223e 0a20 2020 3c70 6174 6820 643d  5)">.   <path d=
+00001b60: 224d 2038 2c31 3132 3820 4c20 3131 3337  "M 8,1128 L 1137
+00001b70: 2c31 3132 3820 3131 3337 2c30 2038 2c30  ,1128 1137,0 8,0
+00001b80: 2038 2c31 3132 3820 5a22 2f3e 0a20 203c   8,1128 Z"/>.  <
+00001b90: 2f67 3e0a 2020 3c67 2069 643d 2262 756c  /g>.  <g id="bul
+00001ba0: 6c65 742d 6368 6172 2d74 656d 706c 6174  let-char-templat
+00001bb0: 652d 3130 3134 3622 2074 7261 6e73 666f  e-10146" transfo
+00001bc0: 726d 3d22 7363 616c 6528 302e 3030 3034  rm="scale(0.0004
+00001bd0: 3838 3238 3132 352c 2d30 2e30 3030 3438  8828125,-0.00048
+00001be0: 3832 3831 3235 2922 3e0a 2020 203c 7061  828125)">.   <pa
+00001bf0: 7468 2064 3d22 4d20 3137 342c 3020 4c20  th d="M 174,0 L 
+00001c00: 3630 322c 3733 3920 3137 342c 3134 3831  602,739 174,1481
+00001c10: 2031 3435 362c 3733 3920 3137 342c 3020   1456,739 174,0 
+00001c20: 5a20 4d20 3133 3538 2c37 3339 204c 2033  Z M 1358,739 L 3
+00001c30: 3039 2c31 3334 3620 3635 392c 3733 3920  09,1346 659,739 
+00001c40: 3133 3538 2c37 3339 205a 222f 3e0a 2020  1358,739 Z"/>.  
+00001c50: 3c2f 673e 0a20 203c 6720 6964 3d22 6275  </g>.  <g id="bu
+00001c60: 6c6c 6574 2d63 6861 722d 7465 6d70 6c61  llet-char-templa
+00001c70: 7465 2d31 3031 3332 2220 7472 616e 7366  te-10132" transf
+00001c80: 6f72 6d3d 2273 6361 6c65 2830 2e30 3030  orm="scale(0.000
+00001c90: 3438 3832 3831 3235 2c2d 302e 3030 3034  48828125,-0.0004
+00001ca0: 3838 3238 3132 3529 223e 0a20 2020 3c70  8828125)">.   <p
+00001cb0: 6174 6820 643d 224d 2032 3031 352c 3733  ath d="M 2015,73
+00001cc0: 3920 4c20 3132 3736 2c30 2037 3137 2c30  9 L 1276,0 717,0
+00001cd0: 2031 3236 302c 3534 3320 3137 342c 3534   1260,543 174,54
+00001ce0: 3320 3137 342c 3933 3620 3132 3630 2c39  3 174,936 1260,9
+00001cf0: 3336 2037 3137 2c31 3438 3120 3132 3734  36 717,1481 1274
+00001d00: 2c31 3438 3120 3230 3135 2c37 3339 205a  ,1481 2015,739 Z
+00001d10: 222f 3e0a 2020 3c2f 673e 0a20 203c 6720  "/>.  </g>.  <g 
+00001d20: 6964 3d22 6275 6c6c 6574 2d63 6861 722d  id="bullet-char-
+00001d30: 7465 6d70 6c61 7465 2d31 3030 3037 2220  template-10007" 
+00001d40: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
+00001d50: 2830 2e30 3030 3438 3832 3831 3235 2c2d  (0.00048828125,-
+00001d60: 302e 3030 3034 3838 3238 3132 3529 223e  0.00048828125)">
+00001d70: 0a20 2020 3c70 6174 6820 643d 224d 2030  .   <path d="M 0
+00001d80: 2c2d 3220 4320 2d37 2c31 3420 2d31 362c  ,-2 C -7,14 -16,
+00001d90: 3237 202d 3235 2c33 3720 4c20 3335 362c  27 -25,37 L 356,
+00001da0: 3536 3720 4320 3236 322c 3832 3320 3231  567 C 262,823 21
+00001db0: 352c 3935 3220 3231 352c 3935 3420 3231  5,952 215,954 21
+00001dc0: 352c 3937 3920 3232 382c 3939 3220 3235  5,979 228,992 25
+00001dd0: 352c 3939 3220 3236 342c 3939 3220 3237  5,992 264,992 27
+00001de0: 362c 3939 3020 3238 392c 3938 3720 3331  6,990 289,987 31
+00001df0: 302c 3939 3120 3333 312c 3939 3920 3335  0,991 331,999 35
+00001e00: 342c 3130 3132 204c 2033 3831 2c39 3939  4,1012 L 381,999
+00001e10: 2034 3932 2c37 3438 2037 3732 2c31 3034   492,748 772,104
+00001e20: 3920 3833 362c 3130 3234 2038 3630 2c31  9 836,1024 860,1
+00001e30: 3034 3920 4320 3838 312c 3130 3339 2039  049 C 881,1039 9
+00001e40: 3031 2c31 3032 3520 3932 322c 3130 3036  01,1025 922,1006
+00001e50: 2038 3836 2c39 3337 2038 3335 2c38 3633   886,937 835,863
+00001e60: 2037 3730 2c37 3834 2037 3639 2c37 3833   770,784 769,783
+00001e70: 2037 3130 2c37 3136 2035 3934 2c35 3834   710,716 594,584
+00001e80: 204c 2037 3734 2c32 3233 2043 2037 3734   L 774,223 C 774
+00001e90: 2c31 3936 2037 3533 2c31 3638 2037 3131  ,196 753,168 711
+00001ea0: 2c31 3339 204c 2037 3237 2c31 3139 2043  ,139 L 727,119 C
+00001eb0: 2037 3137 2c39 3020 3639 392c 3736 2036   717,90 699,76 6
+00001ec0: 3732 2c37 3620 3634 312c 3736 2035 3730  72,76 641,76 570
+00001ed0: 2c31 3738 2034 3537 2c33 3831 204c 2031  ,178 457,381 L 1
+00001ee0: 3634 2c2d 3736 2043 2031 3432 2c2d 3131  64,-76 C 142,-11
+00001ef0: 3020 3131 312c 2d31 3237 2037 322c 2d31  0 111,-127 72,-1
+00001f00: 3237 2033 302c 2d31 3237 2039 2c2d 3131  27 30,-127 9,-11
+00001f10: 3020 382c 2d37 3620 312c 2d36 3720 2d32  0 8,-76 1,-67 -2
+00001f20: 2c2d 3532 202d 322c 2d33 3220 2d32 2c2d  ,-52 -2,-32 -2,-
+00001f30: 3233 202d 312c 2d31 3320 302c 2d32 205a  23 -1,-13 0,-2 Z
+00001f40: 222f 3e0a 2020 3c2f 673e 0a20 203c 6720  "/>.  </g>.  <g 
+00001f50: 6964 3d22 6275 6c6c 6574 2d63 6861 722d  id="bullet-char-
+00001f60: 7465 6d70 6c61 7465 2d31 3030 3034 2220  template-10004" 
+00001f70: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
+00001f80: 2830 2e30 3030 3438 3832 3831 3235 2c2d  (0.00048828125,-
+00001f90: 302e 3030 3034 3838 3238 3132 3529 223e  0.00048828125)">
+00001fa0: 0a20 2020 3c70 6174 6820 643d 224d 2032  .   <path d="M 2
+00001fb0: 3835 2c2d 3333 2043 2031 3832 2c2d 3333  85,-33 C 182,-33
+00001fc0: 2031 3131 2c33 3020 3734 2c31 3536 2035   111,30 74,156 5
+00001fd0: 322c 3232 3820 3431 2c33 3333 2034 312c  2,228 41,333 41,
+00001fe0: 3437 3120 3431 2c35 3439 2035 352c 3631  471 41,549 55,61
+00001ff0: 3620 3832 2c36 3732 2031 3136 2c37 3433  6 82,672 116,743
+00002000: 2031 3639 2c37 3738 2032 3430 2c37 3738   169,778 240,778
+00002010: 2032 3933 2c37 3738 2033 3238 2c37 3437   293,778 328,747
+00002020: 2033 3436 2c36 3834 204c 2033 3639 2c35   346,684 L 369,5
+00002030: 3038 2043 2033 3737 2c34 3434 2033 3937  08 C 377,444 397
+00002040: 2c34 3131 2034 3238 2c34 3130 204c 2031  ,411 428,410 L 1
+00002050: 3136 332c 3131 3136 2043 2031 3137 342c  163,1116 C 1174,
+00002060: 3131 3237 2031 3139 362c 3131 3333 2031  1127 1196,1133 1
+00002070: 3232 392c 3131 3333 2031 3237 312c 3131  229,1133 1271,11
+00002080: 3333 2031 3239 322c 3131 3138 2031 3239  33 1292,1118 129
+00002090: 322c 3130 3837 204c 2031 3239 322c 3936  2,1087 L 1292,96
+000020a0: 3520 4320 3132 3932 2c39 3239 2031 3238  5 C 1292,929 128
+000020b0: 322c 3930 3120 3132 3632 2c38 3831 204c  2,901 1262,881 L
+000020c0: 2034 3432 2c34 3720 4320 3339 302c 2d36   442,47 C 390,-6
+000020d0: 2033 3338 2c2d 3333 2032 3835 2c2d 3333   338,-33 285,-33
+000020e0: 205a 222f 3e0a 2020 3c2f 673e 0a20 203c   Z"/>.  </g>.  <
+000020f0: 6720 6964 3d22 6275 6c6c 6574 2d63 6861  g id="bullet-cha
+00002100: 722d 7465 6d70 6c61 7465 2d39 3637 3922  r-template-9679"
+00002110: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
+00002120: 6528 302e 3030 3034 3838 3238 3132 352c  e(0.00048828125,
+00002130: 2d30 2e30 3030 3438 3832 3831 3235 2922  -0.00048828125)"
+00002140: 3e0a 2020 203c 7061 7468 2064 3d22 4d20  >.   <path d="M 
+00002150: 3831 332c 3020 4320 3633 322c 3020 3438  813,0 C 632,0 48
+00002160: 392c 3534 2033 3833 2c31 3631 2032 3736  9,54 383,161 276
+00002170: 2c32 3638 2032 3233 2c34 3131 2032 3233  ,268 223,411 223
+00002180: 2c35 3932 2032 3233 2c37 3733 2032 3736  ,592 223,773 276
+00002190: 2c39 3136 2033 3833 2c31 3032 3320 3438  ,916 383,1023 48
+000021a0: 392c 3131 3330 2036 3332 2c31 3138 3420  9,1130 632,1184 
+000021b0: 3831 332c 3131 3834 2039 3932 2c31 3138  813,1184 992,118
+000021c0: 3420 3131 3336 2c31 3133 3020 3132 3435  4 1136,1130 1245
+000021d0: 2c31 3032 3320 3133 3533 2c39 3136 2031  ,1023 1353,916 1
+000021e0: 3430 372c 3737 3220 3134 3037 2c35 3932  407,772 1407,592
+000021f0: 2031 3430 372c 3431 3220 3133 3533 2c32   1407,412 1353,2
+00002200: 3638 2031 3234 352c 3136 3120 3131 3336  68 1245,161 1136
+00002210: 2c35 3420 3939 322c 3020 3831 332c 3020  ,54 992,0 813,0 
+00002220: 5a22 2f3e 0a20 203c 2f67 3e0a 2020 3c67  Z"/>.  </g>.  <g
+00002230: 2069 643d 2262 756c 6c65 742d 6368 6172   id="bullet-char
+00002240: 2d74 656d 706c 6174 652d 3832 3236 2220  -template-8226" 
+00002250: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
+00002260: 2830 2e30 3030 3438 3832 3831 3235 2c2d  (0.00048828125,-
+00002270: 302e 3030 3034 3838 3238 3132 3529 223e  0.00048828125)">
+00002280: 0a20 2020 3c70 6174 6820 643d 224d 2033  .   <path d="M 3
+00002290: 3436 2c34 3537 2043 2032 3733 2c34 3537  46,457 C 273,457
+000022a0: 2032 3039 2c34 3833 2031 3535 2c35 3335   209,483 155,535
+000022b0: 2031 3031 2c35 3836 2037 342c 3634 3920   101,586 74,649 
+000022c0: 3734 2c37 3233 2037 342c 3739 3620 3130  74,723 74,796 10
+000022d0: 312c 3835 3920 3135 352c 3931 3120 3230  1,859 155,911 20
+000022e0: 392c 3936 3320 3237 332c 3938 3920 3334  9,963 273,989 34
+000022f0: 362c 3938 3920 3431 392c 3938 3920 3438  6,989 419,989 48
+00002300: 302c 3936 3320 3533 312c 3931 3020 3538  0,963 531,910 58
+00002310: 322c 3835 3920 3630 382c 3739 3620 3630  2,859 608,796 60
+00002320: 382c 3732 3320 3630 382c 3634 3820 3538  8,723 608,648 58
+00002330: 332c 3538 3620 3533 322c 3533 3520 3438  3,586 532,535 48
+00002340: 322c 3438 3320 3432 302c 3435 3720 3334  2,483 420,457 34
+00002350: 362c 3435 3720 5a22 2f3e 0a20 203c 2f67  6,457 Z"/>.  </g
+00002360: 3e0a 2020 3c67 2069 643d 2262 756c 6c65  >.  <g id="bulle
+00002370: 742d 6368 6172 2d74 656d 706c 6174 652d  t-char-template-
+00002380: 3832 3131 2220 7472 616e 7366 6f72 6d3d  8211" transform=
+00002390: 2273 6361 6c65 2830 2e30 3030 3438 3832  "scale(0.0004882
+000023a0: 3831 3235 2c2d 302e 3030 3034 3838 3238  8125,-0.00048828
+000023b0: 3132 3529 223e 0a20 2020 3c70 6174 6820  125)">.   <path 
+000023c0: 643d 224d 202d 342c 3435 3920 4c20 3131  d="M -4,459 L 11
+000023d0: 3335 2c34 3539 2031 3133 352c 3630 3620  35,459 1135,606 
+000023e0: 2d34 2c36 3036 202d 342c 3435 3920 5a22  -4,606 -4,459 Z"
+000023f0: 2f3e 0a20 203c 2f67 3e0a 2020 3c67 2069  />.  </g>.  <g i
+00002400: 643d 2262 756c 6c65 742d 6368 6172 2d74  d="bullet-char-t
+00002410: 656d 706c 6174 652d 3631 3534 3822 2074  emplate-61548" t
+00002420: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
+00002430: 302e 3030 3034 3838 3238 3132 352c 2d30  0.00048828125,-0
+00002440: 2e30 3030 3438 3832 3831 3235 2922 3e0a  .00048828125)">.
+00002450: 2020 203c 7061 7468 2064 3d22 4d20 3137     <path d="M 17
+00002460: 332c 3734 3020 4320 3137 332c 3930 3320  3,740 C 173,903 
+00002470: 3233 312c 3130 3433 2033 3436 2c31 3135  231,1043 346,115
+00002480: 3920 3436 322c 3132 3734 2036 3031 2c31  9 462,1274 601,1
+00002490: 3333 3220 3736 352c 3133 3332 2039 3238  332 765,1332 928
+000024a0: 2c31 3333 3220 3130 3637 2c31 3237 3420  ,1332 1067,1274 
+000024b0: 3131 3833 2c31 3135 3920 3132 3939 2c31  1183,1159 1299,1
+000024c0: 3034 3320 3133 3537 2c39 3033 2031 3335  043 1357,903 135
+000024d0: 372c 3734 3020 3133 3537 2c35 3737 2031  7,740 1357,577 1
+000024e0: 3239 392c 3433 3720 3131 3833 2c33 3232  299,437 1183,322
+000024f0: 2031 3036 372c 3230 3620 3932 382c 3134   1067,206 928,14
+00002500: 3820 3736 352c 3134 3820 3630 312c 3134  8 765,148 601,14
+00002510: 3820 3436 322c 3230 3620 3334 362c 3332  8 462,206 346,32
+00002520: 3220 3233 312c 3433 3720 3137 332c 3537  2 231,437 173,57
+00002530: 3720 3137 332c 3734 3020 5a22 2f3e 0a20  7 173,740 Z"/>. 
+00002540: 203c 2f67 3e0a 203c 2f64 6566 733e 0a20   </g>. </defs>. 
+00002550: 3c67 2063 6c61 7373 3d22 5061 6765 223e  <g class="Page">
+00002560: 0a20 203c 6720 636c 6173 733d 2263 6f6d  .  <g class="com
+00002570: 2e73 756e 2e73 7461 722e 6472 6177 696e  .sun.star.drawin
+00002580: 672e 4375 7374 6f6d 5368 6170 6522 3e0a  g.CustomShape">.
+00002590: 2020 203c 6720 6964 3d22 6964 3322 3e0a     <g id="id3">.
+000025a0: 2020 2020 3c72 6563 7420 636c 6173 733d      <rect class=
+000025b0: 2242 6f75 6e64 696e 6742 6f78 2220 7374  "BoundingBox" st
+000025c0: 726f 6b65 3d22 6e6f 6e65 2220 6669 6c6c  roke="none" fill
+000025d0: 3d22 6e6f 6e65 2220 783d 2231 3030 3022  ="none" x="1000"
+000025e0: 2079 3d22 3130 3030 2220 7769 6474 683d   y="1000" width=
+000025f0: 2231 3230 3031 2220 6865 6967 6874 3d22  "12001" height="
+00002600: 3130 3031 222f 3e0a 2020 2020 3c70 6174  1001"/>.    <pat
+00002610: 6820 6669 6c6c 3d22 7267 6228 3130 302c  h fill="rgb(100,
+00002620: 3134 392c 3233 3729 2220 7374 726f 6b65  149,237)" stroke
+00002630: 3d22 6e6f 6e65 2220 643d 224d 2037 3030  ="none" d="M 700
+00002640: 302c 3230 3030 204c 2031 3030 302c 3230  0,2000 L 1000,20
+00002650: 3030 2031 3030 302c 3130 3030 2031 3330  00 1000,1000 130
+00002660: 3030 2c31 3030 3020 3133 3030 302c 3230  00,1000 13000,20
+00002670: 3030 2037 3030 302c 3230 3030 205a 222f  00 7000,2000 Z"/
+00002680: 3e0a 2020 2020 3c74 6578 7420 636c 6173  >.    <text clas
+00002690: 733d 2253 5647 5465 7874 5368 6170 6522  s="SVGTextShape"
+000026a0: 3e3c 7473 7061 6e20 636c 6173 733d 2254  ><tspan class="T
+000026b0: 6578 7450 6172 6167 7261 7068 2220 666f  extParagraph" fo
+000026c0: 6e74 2d66 616d 696c 793d 224c 6962 6572  nt-family="Liber
+000026d0: 6174 696f 6e20 5361 6e73 2c20 7361 6e73  ation Sans, sans
+000026e0: 2d73 6572 6966 2220 666f 6e74 2d73 697a  -serif" font-siz
+000026f0: 653d 2236 3335 7078 2220 666f 6e74 2d77  e="635px" font-w
+00002700: 6569 6768 743d 2234 3030 223e 3c74 7370  eight="400"><tsp
+00002710: 616e 2063 6c61 7373 3d22 5465 7874 506f  an class="TextPo
+00002720: 7369 7469 6f6e 2220 783d 2235 3133 3522  sition" x="5135"
+00002730: 2079 3d22 3137 3231 223e 3c74 7370 616e   y="1721"><tspan
+00002740: 2066 696c 6c3d 2272 6762 2830 2c30 2c30   fill="rgb(0,0,0
+00002750: 2922 2073 7472 6f6b 653d 226e 6f6e 6522  )" stroke="none"
+00002760: 2073 7479 6c65 3d22 7768 6974 652d 7370   style="white-sp
+00002770: 6163 653a 2070 7265 223e 5365 7175 656e  ace: pre">Sequen
+00002780: 6365 2023 313c 2f74 7370 616e 3e3c 2f74  ce #1</tspan></t
+00002790: 7370 616e 3e3c 2f74 7370 616e 3e3c 2f74  span></tspan></t
+000027a0: 6578 743e 0a20 2020 3c2f 673e 0a20 203c  ext>.   </g>.  <
+000027b0: 2f67 3e0a 2020 3c67 2063 6c61 7373 3d22  /g>.  <g class="
+000027c0: 636f 6d2e 7375 6e2e 7374 6172 2e64 7261  com.sun.star.dra
+000027d0: 7769 6e67 2e4c 696e 6553 6861 7065 223e  wing.LineShape">
+000027e0: 0a20 2020 3c67 2069 643d 2269 6434 223e  .   <g id="id4">
+000027f0: 0a20 2020 203c 7265 6374 2063 6c61 7373  .    <rect class
+00002800: 3d22 426f 756e 6469 6e67 426f 7822 2073  ="BoundingBox" s
+00002810: 7472 6f6b 653d 226e 6f6e 6522 2066 696c  troke="none" fil
+00002820: 6c3d 226e 6f6e 6522 2078 3d22 3130 3030  l="none" x="1000
+00002830: 2220 793d 2232 3735 3022 2077 6964 7468  " y="2750" width
+00002840: 3d22 3430 3031 2220 6865 6967 6874 3d22  ="4001" height="
+00002850: 3530 3122 2f3e 0a20 2020 203c 7061 7468  501"/>.    <path
+00002860: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+00002870: 6f6b 653d 2272 6762 2830 2c30 2c30 2922  oke="rgb(0,0,0)"
+00002880: 2073 7472 6f6b 652d 7769 6474 683d 2235   stroke-width="5
+00002890: 3322 2073 7472 6f6b 652d 6c69 6e65 6a6f  3" stroke-linejo
+000028a0: 696e 3d22 726f 756e 6422 2073 7472 6f6b  in="round" strok
+000028b0: 652d 6c69 6e65 6361 703d 2273 7175 6172  e-linecap="squar
+000028c0: 6522 2064 3d22 4d20 3130 3332 2c33 3030  e" d="M 1032,300
+000028d0: 3020 4c20 3439 3638 2c33 3030 3022 2f3e  0 L 4968,3000"/>
+000028e0: 0a20 2020 203c 7061 7468 2066 696c 6c3d  .    <path fill=
+000028f0: 2272 6762 2830 2c30 2c30 2922 2073 7472  "rgb(0,0,0)" str
+00002900: 6f6b 653d 226e 6f6e 6522 2064 3d22 4d20  oke="none" d="M 
+00002910: 3130 3030 2c33 3235 3020 4c20 3130 3030  1000,3250 L 1000
+00002920: 2c33 3038 3420 3130 3030 2c32 3931 3720  ,3084 1000,2917 
+00002930: 3130 3030 2c32 3735 3020 3130 3232 2c32  1000,2750 1022,2
+00002940: 3735 3020 3130 3433 2c32 3735 3020 3130  750 1043,2750 10
+00002950: 3636 2c32 3735 3020 3130 3636 2c32 3931  66,2750 1066,291
+00002960: 3620 3130 3636 2c33 3038 3320 3130 3636  6 1066,3083 1066
+00002970: 2c33 3235 3020 3130 3434 2c33 3235 3020  ,3250 1044,3250 
+00002980: 3130 3233 2c33 3235 3020 3130 3030 2c33  1023,3250 1000,3
+00002990: 3235 3020 5a22 2f3e 0a20 2020 203c 7061  250 Z"/>.    <pa
+000029a0: 7468 2066 696c 6c3d 2272 6762 2830 2c30  th fill="rgb(0,0
+000029b0: 2c30 2922 2073 7472 6f6b 653d 226e 6f6e  ,0)" stroke="non
+000029c0: 6522 2064 3d22 4d20 3530 3030 2c32 3735  e" d="M 5000,275
+000029d0: 3020 4c20 3530 3030 2c32 3931 3620 3530  0 L 5000,2916 50
+000029e0: 3030 2c33 3038 3320 3530 3030 2c33 3235  00,3083 5000,325
+000029f0: 3020 3439 3738 2c33 3235 3020 3439 3537  0 4978,3250 4957
+00002a00: 2c33 3235 3020 3439 3334 2c33 3235 3020  ,3250 4934,3250 
+00002a10: 3439 3334 2c33 3038 3420 3439 3334 2c32  4934,3084 4934,2
+00002a20: 3931 3720 3439 3334 2c32 3735 3020 3439  917 4934,2750 49
+00002a30: 3536 2c32 3735 3020 3439 3737 2c32 3735  56,2750 4977,275
+00002a40: 3020 3530 3030 2c32 3735 3020 5a22 2f3e  0 5000,2750 Z"/>
+00002a50: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
+00002a60: 2020 3c67 2063 6c61 7373 3d22 636f 6d2e    <g class="com.
+00002a70: 7375 6e2e 7374 6172 2e64 7261 7769 6e67  sun.star.drawing
+00002a80: 2e4c 696e 6553 6861 7065 223e 0a20 2020  .LineShape">.   
+00002a90: 3c67 2069 643d 2269 6435 223e 0a20 2020  <g id="id5">.   
+00002aa0: 203c 7265 6374 2063 6c61 7373 3d22 426f   <rect class="Bo
+00002ab0: 756e 6469 6e67 426f 7822 2073 7472 6f6b  undingBox" strok
+00002ac0: 653d 226e 6f6e 6522 2066 696c 6c3d 226e  e="none" fill="n
+00002ad0: 6f6e 6522 2078 3d22 3930 3030 2220 793d  one" x="9000" y=
+00002ae0: 2232 3735 3022 2077 6964 7468 3d22 3430  "2750" width="40
+00002af0: 3031 2220 6865 6967 6874 3d22 3530 3122  01" height="501"
+00002b00: 2f3e 0a20 2020 203c 7061 7468 2066 696c  />.    <path fil
+00002b10: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00002b20: 2272 6762 2830 2c30 2c30 2922 2073 7472  "rgb(0,0,0)" str
+00002b30: 6f6b 652d 7769 6474 683d 2235 3322 2073  oke-width="53" s
+00002b40: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3d22  troke-linejoin="
+00002b50: 726f 756e 6422 2073 7472 6f6b 652d 6c69  round" stroke-li
+00002b60: 6e65 6361 703d 2273 7175 6172 6522 2064  necap="square" d
+00002b70: 3d22 4d20 3930 3332 2c33 3030 3020 4c20  ="M 9032,3000 L 
+00002b80: 3132 3936 382c 3330 3030 222f 3e0a 2020  12968,3000"/>.  
+00002b90: 2020 3c70 6174 6820 6669 6c6c 3d22 7267    <path fill="rg
+00002ba0: 6228 302c 302c 3029 2220 7374 726f 6b65  b(0,0,0)" stroke
+00002bb0: 3d22 6e6f 6e65 2220 643d 224d 2039 3030  ="none" d="M 900
+00002bc0: 302c 3332 3530 204c 2039 3030 302c 3330  0,3250 L 9000,30
+00002bd0: 3834 2039 3030 302c 3239 3137 2039 3030  84 9000,2917 900
+00002be0: 302c 3237 3530 2039 3032 322c 3237 3530  0,2750 9022,2750
+00002bf0: 2039 3034 332c 3237 3530 2039 3036 362c   9043,2750 9066,
+00002c00: 3237 3530 2039 3036 362c 3239 3136 2039  2750 9066,2916 9
+00002c10: 3036 362c 3330 3833 2039 3036 362c 3332  066,3083 9066,32
+00002c20: 3530 2039 3034 342c 3332 3530 2039 3032  50 9044,3250 902
+00002c30: 332c 3332 3530 2039 3030 302c 3332 3530  3,3250 9000,3250
+00002c40: 205a 222f 3e0a 2020 2020 3c70 6174 6820   Z"/>.    <path 
+00002c50: 6669 6c6c 3d22 7267 6228 302c 302c 3029  fill="rgb(0,0,0)
+00002c60: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+00002c70: 643d 224d 2031 3330 3030 2c32 3735 3020  d="M 13000,2750 
+00002c80: 4c20 3133 3030 302c 3239 3136 2031 3330  L 13000,2916 130
+00002c90: 3030 2c33 3038 3320 3133 3030 302c 3332  00,3083 13000,32
+00002ca0: 3530 2031 3239 3738 2c33 3235 3020 3132  50 12978,3250 12
+00002cb0: 3935 372c 3332 3530 2031 3239 3334 2c33  957,3250 12934,3
+00002cc0: 3235 3020 3132 3933 342c 3330 3834 2031  250 12934,3084 1
+00002cd0: 3239 3334 2c32 3931 3720 3132 3933 342c  2934,2917 12934,
+00002ce0: 3237 3530 2031 3239 3536 2c32 3735 3020  2750 12956,2750 
+00002cf0: 3132 3937 372c 3237 3530 2031 3330 3030  12977,2750 13000
+00002d00: 2c32 3735 3020 5a22 2f3e 0a20 2020 3c2f  ,2750 Z"/>.   </
+00002d10: 673e 0a20 203c 2f67 3e0a 2020 3c67 2063  g>.  </g>.  <g c
+00002d20: 6c61 7373 3d22 636f 6d2e 7375 6e2e 7374  lass="com.sun.st
+00002d30: 6172 2e64 7261 7769 6e67 2e43 7573 746f  ar.drawing.Custo
+00002d40: 6d53 6861 7065 223e 0a20 2020 3c67 2069  mShape">.   <g i
+00002d50: 643d 2269 6436 223e 0a20 2020 203c 7265  d="id6">.    <re
+00002d60: 6374 2063 6c61 7373 3d22 426f 756e 6469  ct class="Boundi
+00002d70: 6e67 426f 7822 2073 7472 6f6b 653d 226e  ngBox" stroke="n
+00002d80: 6f6e 6522 2066 696c 6c3d 226e 6f6e 6522  one" fill="none"
+00002d90: 2078 3d22 3530 3030 2220 793d 2232 3530   x="5000" y="250
+00002da0: 3022 2077 6964 7468 3d22 3130 3031 2220  0" width="1001" 
+00002db0: 6865 6967 6874 3d22 3130 3031 222f 3e0a  height="1001"/>.
+00002dc0: 2020 2020 3c70 6174 6820 6669 6c6c 3d22      <path fill="
+00002dd0: 7267 6228 3139 322c 3139 322c 3139 3229  rgb(192,192,192)
+00002de0: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+00002df0: 643d 224d 2035 3530 302c 3335 3030 204c  d="M 5500,3500 L
+00002e00: 2035 3030 302c 3335 3030 2035 3030 302c   5000,3500 5000,
+00002e10: 3235 3030 2036 3030 302c 3235 3030 2036  2500 6000,2500 6
+00002e20: 3030 302c 3335 3030 2035 3530 302c 3335  000,3500 5500,35
+00002e30: 3030 205a 222f 3e0a 2020 203c 2f67 3e0a  00 Z"/>.   </g>.
+00002e40: 2020 3c2f 673e 0a20 203c 6720 636c 6173    </g>.  <g clas
+00002e50: 733d 2263 6f6d 2e73 756e 2e73 7461 722e  s="com.sun.star.
+00002e60: 6472 6177 696e 672e 4375 7374 6f6d 5368  drawing.CustomSh
+00002e70: 6170 6522 3e0a 2020 203c 6720 6964 3d22  ape">.   <g id="
+00002e80: 6964 3722 3e0a 2020 2020 3c72 6563 7420  id7">.    <rect 
+00002e90: 636c 6173 733d 2242 6f75 6e64 696e 6742  class="BoundingB
+00002ea0: 6f78 2220 7374 726f 6b65 3d22 6e6f 6e65  ox" stroke="none
+00002eb0: 2220 6669 6c6c 3d22 6e6f 6e65 2220 783d  " fill="none" x=
+00002ec0: 2238 3030 3022 2079 3d22 3235 3030 2220  "8000" y="2500" 
+00002ed0: 7769 6474 683d 2231 3030 3122 2068 6569  width="1001" hei
+00002ee0: 6768 743d 2231 3030 3122 2f3e 0a20 2020  ght="1001"/>.   
+00002ef0: 203c 7061 7468 2066 696c 6c3d 2272 6762   <path fill="rgb
+00002f00: 2831 3932 2c31 3932 2c31 3932 2922 2073  (192,192,192)" s
+00002f10: 7472 6f6b 653d 226e 6f6e 6522 2064 3d22  troke="none" d="
+00002f20: 4d20 3835 3030 2c33 3530 3020 4c20 3830  M 8500,3500 L 80
+00002f30: 3030 2c33 3530 3020 3830 3030 2c32 3530  00,3500 8000,250
+00002f40: 3020 3930 3030 2c32 3530 3020 3930 3030  0 9000,2500 9000
+00002f50: 2c33 3530 3020 3835 3030 2c33 3530 3020  ,3500 8500,3500 
+00002f60: 5a22 2f3e 0a20 2020 3c2f 673e 0a20 203c  Z"/>.   </g>.  <
+00002f70: 2f67 3e0a 2020 3c67 2063 6c61 7373 3d22  /g>.  <g class="
+00002f80: 636f 6d2e 7375 6e2e 7374 6172 2e64 7261  com.sun.star.dra
+00002f90: 7769 6e67 2e43 7573 746f 6d53 6861 7065  wing.CustomShape
+00002fa0: 223e 0a20 2020 3c67 2069 643d 2269 6438  ">.   <g id="id8
+00002fb0: 223e 0a20 2020 203c 7265 6374 2063 6c61  ">.    <rect cla
+00002fc0: 7373 3d22 426f 756e 6469 6e67 426f 7822  ss="BoundingBox"
+00002fd0: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
+00002fe0: 696c 6c3d 226e 6f6e 6522 2078 3d22 3130  ill="none" x="10
+00002ff0: 3030 2220 793d 2234 3030 3022 2077 6964  00" y="4000" wid
+00003000: 7468 3d22 3830 3031 2220 6865 6967 6874  th="8001" height
+00003010: 3d22 3130 3031 222f 3e0a 2020 2020 3c70  ="1001"/>.    <p
+00003020: 6174 6820 6669 6c6c 3d22 7267 6228 3130  ath fill="rgb(10
+00003030: 302c 3134 392c 3233 3729 2220 7374 726f  0,149,237)" stro
+00003040: 6b65 3d22 6e6f 6e65 2220 643d 224d 2035  ke="none" d="M 5
+00003050: 3030 302c 3530 3030 204c 2031 3030 302c  000,5000 L 1000,
+00003060: 3530 3030 2031 3030 302c 3430 3030 2039  5000 1000,4000 9
+00003070: 3030 302c 3430 3030 2039 3030 302c 3530  000,4000 9000,50
+00003080: 3030 2035 3030 302c 3530 3030 205a 222f  00 5000,5000 Z"/
+00003090: 3e0a 2020 2020 3c74 6578 7420 636c 6173  >.    <text clas
+000030a0: 733d 2253 5647 5465 7874 5368 6170 6522  s="SVGTextShape"
+000030b0: 3e3c 7473 7061 6e20 636c 6173 733d 2254  ><tspan class="T
+000030c0: 6578 7450 6172 6167 7261 7068 2220 666f  extParagraph" fo
+000030d0: 6e74 2d66 616d 696c 793d 224c 6962 6572  nt-family="Liber
+000030e0: 6174 696f 6e20 5361 6e73 2c20 7361 6e73  ation Sans, sans
+000030f0: 2d73 6572 6966 2220 666f 6e74 2d73 697a  -serif" font-siz
+00003100: 653d 2236 3335 7078 2220 666f 6e74 2d77  e="635px" font-w
+00003110: 6569 6768 743d 2234 3030 223e 3c74 7370  eight="400"><tsp
+00003120: 616e 2063 6c61 7373 3d22 5465 7874 506f  an class="TextPo
+00003130: 7369 7469 6f6e 2220 783d 2233 3133 3522  sition" x="3135"
+00003140: 2079 3d22 3437 3231 223e 3c74 7370 616e   y="4721"><tspan
+00003150: 2066 696c 6c3d 2272 6762 2830 2c30 2c30   fill="rgb(0,0,0
+00003160: 2922 2073 7472 6f6b 653d 226e 6f6e 6522  )" stroke="none"
+00003170: 2073 7479 6c65 3d22 7768 6974 652d 7370   style="white-sp
+00003180: 6163 653a 2070 7265 223e 5365 7175 656e  ace: pre">Sequen
+00003190: 6365 2023 323c 2f74 7370 616e 3e3c 2f74  ce #2</tspan></t
+000031a0: 7370 616e 3e3c 2f74 7370 616e 3e3c 2f74  span></tspan></t
+000031b0: 6578 743e 0a20 2020 3c2f 673e 0a20 203c  ext>.   </g>.  <
+000031c0: 2f67 3e0a 2020 3c67 2063 6c61 7373 3d22  /g>.  <g class="
+000031d0: 636f 6d2e 7375 6e2e 7374 6172 2e64 7261  com.sun.star.dra
+000031e0: 7769 6e67 2e4c 696e 6553 6861 7065 223e  wing.LineShape">
+000031f0: 0a20 2020 3c67 2069 643d 2269 6439 223e  .   <g id="id9">
+00003200: 0a20 2020 203c 7265 6374 2063 6c61 7373  .    <rect class
+00003210: 3d22 426f 756e 6469 6e67 426f 7822 2073  ="BoundingBox" s
+00003220: 7472 6f6b 653d 226e 6f6e 6522 2066 696c  troke="none" fil
+00003230: 6c3d 226e 6f6e 6522 2078 3d22 3130 3030  l="none" x="1000
+00003240: 2220 793d 2235 3735 3022 2077 6964 7468  " y="5750" width
+00003250: 3d22 3330 3031 2220 6865 6967 6874 3d22  ="3001" height="
+00003260: 3530 3122 2f3e 0a20 2020 203c 7061 7468  501"/>.    <path
+00003270: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+00003280: 6f6b 653d 2272 6762 2830 2c30 2c30 2922  oke="rgb(0,0,0)"
+00003290: 2073 7472 6f6b 652d 7769 6474 683d 2235   stroke-width="5
+000032a0: 3322 2073 7472 6f6b 652d 6c69 6e65 6a6f  3" stroke-linejo
+000032b0: 696e 3d22 726f 756e 6422 2073 7472 6f6b  in="round" strok
+000032c0: 652d 6c69 6e65 6361 703d 2273 7175 6172  e-linecap="squar
+000032d0: 6522 2064 3d22 4d20 3130 3332 2c36 3030  e" d="M 1032,600
+000032e0: 3020 4c20 3339 3638 2c36 3030 3022 2f3e  0 L 3968,6000"/>
+000032f0: 0a20 2020 203c 7061 7468 2066 696c 6c3d  .    <path fill=
+00003300: 2272 6762 2830 2c30 2c30 2922 2073 7472  "rgb(0,0,0)" str
+00003310: 6f6b 653d 226e 6f6e 6522 2064 3d22 4d20  oke="none" d="M 
+00003320: 3130 3030 2c36 3235 3020 4c20 3130 3030  1000,6250 L 1000
+00003330: 2c36 3038 3420 3130 3030 2c35 3931 3720  ,6084 1000,5917 
+00003340: 3130 3030 2c35 3735 3020 3130 3232 2c35  1000,5750 1022,5
+00003350: 3735 3020 3130 3433 2c35 3735 3020 3130  750 1043,5750 10
+00003360: 3636 2c35 3735 3020 3130 3636 2c35 3931  66,5750 1066,591
+00003370: 3620 3130 3636 2c36 3038 3320 3130 3636  6 1066,6083 1066
+00003380: 2c36 3235 3020 3130 3434 2c36 3235 3020  ,6250 1044,6250 
+00003390: 3130 3233 2c36 3235 3020 3130 3030 2c36  1023,6250 1000,6
+000033a0: 3235 3020 5a22 2f3e 0a20 2020 203c 7061  250 Z"/>.    <pa
+000033b0: 7468 2066 696c 6c3d 2272 6762 2830 2c30  th fill="rgb(0,0
+000033c0: 2c30 2922 2073 7472 6f6b 653d 226e 6f6e  ,0)" stroke="non
+000033d0: 6522 2064 3d22 4d20 3430 3030 2c35 3735  e" d="M 4000,575
+000033e0: 3020 4c20 3430 3030 2c35 3931 3620 3430  0 L 4000,5916 40
+000033f0: 3030 2c36 3038 3320 3430 3030 2c36 3235  00,6083 4000,625
+00003400: 3020 3339 3738 2c36 3235 3020 3339 3537  0 3978,6250 3957
+00003410: 2c36 3235 3020 3339 3334 2c36 3235 3020  ,6250 3934,6250 
+00003420: 3339 3334 2c36 3038 3420 3339 3334 2c35  3934,6084 3934,5
+00003430: 3931 3720 3339 3334 2c35 3735 3020 3339  917 3934,5750 39
+00003440: 3536 2c35 3735 3020 3339 3737 2c35 3735  56,5750 3977,575
+00003450: 3020 3430 3030 2c35 3735 3020 5a22 2f3e  0 4000,5750 Z"/>
+00003460: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
+00003470: 2020 3c67 2063 6c61 7373 3d22 636f 6d2e    <g class="com.
+00003480: 7375 6e2e 7374 6172 2e64 7261 7769 6e67  sun.star.drawing
+00003490: 2e43 7573 746f 6d53 6861 7065 223e 0a20  .CustomShape">. 
+000034a0: 2020 3c67 2069 643d 2269 6431 3022 3e0a    <g id="id10">.
+000034b0: 2020 2020 3c72 6563 7420 636c 6173 733d      <rect class=
+000034c0: 2242 6f75 6e64 696e 6742 6f78 2220 7374  "BoundingBox" st
+000034d0: 726f 6b65 3d22 6e6f 6e65 2220 6669 6c6c  roke="none" fill
+000034e0: 3d22 6e6f 6e65 2220 783d 2234 3030 3022  ="none" x="4000"
+000034f0: 2079 3d22 3535 3030 2220 7769 6474 683d   y="5500" width=
+00003500: 2231 3030 3122 2068 6569 6768 743d 2231  "1001" height="1
+00003510: 3030 3122 2f3e 0a20 2020 203c 7061 7468  001"/>.    <path
+00003520: 2066 696c 6c3d 2272 6762 2831 3932 2c31   fill="rgb(192,1
+00003530: 3932 2c31 3932 2922 2073 7472 6f6b 653d  92,192)" stroke=
+00003540: 226e 6f6e 6522 2064 3d22 4d20 3435 3030  "none" d="M 4500
+00003550: 2c36 3530 3020 4c20 3430 3030 2c36 3530  ,6500 L 4000,650
+00003560: 3020 3430 3030 2c35 3530 3020 3530 3030  0 4000,5500 5000
+00003570: 2c35 3530 3020 3530 3030 2c36 3530 3020  ,5500 5000,6500 
+00003580: 3435 3030 2c36 3530 3020 5a22 2f3e 0a20  4500,6500 Z"/>. 
+00003590: 2020 3c2f 673e 0a20 203c 2f67 3e0a 2020    </g>.  </g>.  
+000035a0: 3c67 2063 6c61 7373 3d22 636f 6d2e 7375  <g class="com.su
+000035b0: 6e2e 7374 6172 2e64 7261 7769 6e67 2e43  n.star.drawing.C
+000035c0: 7573 746f 6d53 6861 7065 223e 0a20 2020  ustomShape">.   
+000035d0: 3c67 2069 643d 2269 6431 3122 3e0a 2020  <g id="id11">.  
+000035e0: 2020 3c72 6563 7420 636c 6173 733d 2242    <rect class="B
+000035f0: 6f75 6e64 696e 6742 6f78 2220 7374 726f  oundingBox" stro
+00003600: 6b65 3d22 6e6f 6e65 2220 6669 6c6c 3d22  ke="none" fill="
+00003610: 6e6f 6e65 2220 783d 2235 3030 3022 2079  none" x="5000" y
+00003620: 3d22 3535 3030 2220 7769 6474 683d 2231  ="5500" width="1
+00003630: 3030 3122 2068 6569 6768 743d 2231 3030  001" height="100
+00003640: 3122 2f3e 0a20 2020 203c 7061 7468 2066  1"/>.    <path f
+00003650: 696c 6c3d 2272 6762 2831 3932 2c31 3932  ill="rgb(192,192
+00003660: 2c31 3932 2922 2073 7472 6f6b 653d 226e  ,192)" stroke="n
+00003670: 6f6e 6522 2064 3d22 4d20 3535 3030 2c36  one" d="M 5500,6
+00003680: 3530 3020 4c20 3530 3030 2c36 3530 3020  500 L 5000,6500 
+00003690: 3530 3030 2c35 3530 3020 3630 3030 2c35  5000,5500 6000,5
+000036a0: 3530 3020 3630 3030 2c36 3530 3020 3535  500 6000,6500 55
+000036b0: 3030 2c36 3530 3020 5a22 2f3e 0a20 2020  00,6500 Z"/>.   
+000036c0: 3c2f 673e 0a20 203c 2f67 3e0a 2020 3c67  </g>.  </g>.  <g
+000036d0: 2063 6c61 7373 3d22 636f 6d2e 7375 6e2e   class="com.sun.
+000036e0: 7374 6172 2e64 7261 7769 6e67 2e43 7573  star.drawing.Cus
+000036f0: 746f 6d53 6861 7065 223e 0a20 2020 3c67  tomShape">.   <g
+00003700: 2069 643d 2269 6431 3222 3e0a 2020 2020   id="id12">.    
+00003710: 3c72 6563 7420 636c 6173 733d 2242 6f75  <rect class="Bou
+00003720: 6e64 696e 6742 6f78 2220 7374 726f 6b65  ndingBox" stroke
+00003730: 3d22 6e6f 6e65 2220 6669 6c6c 3d22 6e6f  ="none" fill="no
+00003740: 6e65 2220 783d 2231 3135 3030 2220 793d  ne" x="11500" y=
+00003750: 2234 3030 3022 2077 6964 7468 3d22 3135  "4000" width="15
+00003760: 3031 2220 6865 6967 6874 3d22 3130 3031  01" height="1001
+00003770: 222f 3e0a 2020 2020 3c70 6174 6820 6669  "/>.    <path fi
+00003780: 6c6c 3d22 7267 6228 3130 302c 3134 392c  ll="rgb(100,149,
+00003790: 3233 3729 2220 7374 726f 6b65 3d22 6e6f  237)" stroke="no
+000037a0: 6e65 2220 643d 224d 2031 3232 3530 2c35  ne" d="M 12250,5
+000037b0: 3030 3020 4c20 3131 3530 302c 3530 3030  000 L 11500,5000
+000037c0: 2031 3135 3030 2c34 3030 3020 3133 3030   11500,4000 1300
+000037d0: 302c 3430 3030 2031 3330 3030 2c35 3030  0,4000 13000,500
+000037e0: 3020 3132 3235 302c 3530 3030 205a 222f  0 12250,5000 Z"/
+000037f0: 3e0a 2020 2020 3c74 6578 7420 636c 6173  >.    <text clas
+00003800: 733d 2253 5647 5465 7874 5368 6170 6522  s="SVGTextShape"
+00003810: 3e3c 7473 7061 6e20 636c 6173 733d 2254  ><tspan class="T
+00003820: 6578 7450 6172 6167 7261 7068 2220 666f  extParagraph" fo
+00003830: 6e74 2d66 616d 696c 793d 224c 6962 6572  nt-family="Liber
+00003840: 6174 696f 6e20 5361 6e73 2c20 7361 6e73  ation Sans, sans
+00003850: 2d73 6572 6966 2220 666f 6e74 2d73 697a  -serif" font-siz
+00003860: 653d 2236 3335 7078 2220 666f 6e74 2d77  e="635px" font-w
+00003870: 6569 6768 743d 2234 3030 223e 3c74 7370  eight="400"><tsp
+00003880: 616e 2063 6c61 7373 3d22 5465 7874 506f  an class="TextPo
+00003890: 7369 7469 6f6e 2220 783d 2231 3138 3939  sition" x="11899
+000038a0: 2220 793d 2234 3732 3122 3e3c 7473 7061  " y="4721"><tspa
+000038b0: 6e20 6669 6c6c 3d22 7267 6228 302c 302c  n fill="rgb(0,0,
+000038c0: 3029 2220 7374 726f 6b65 3d22 6e6f 6e65  0)" stroke="none
+000038d0: 2220 7374 796c 653d 2277 6869 7465 2d73  " style="white-s
+000038e0: 7061 6365 3a20 7072 6522 3e23 333c 2f74  pace: pre">#3</t
+000038f0: 7370 616e 3e3c 2f74 7370 616e 3e3c 2f74  span></tspan></t
+00003900: 7370 616e 3e3c 2f74 6578 743e 0a20 2020  span></text>.   
+00003910: 3c2f 673e 0a20 203c 2f67 3e0a 2020 3c67  </g>.  </g>.  <g
+00003920: 2063 6c61 7373 3d22 636f 6d2e 7375 6e2e   class="com.sun.
+00003930: 7374 6172 2e64 7261 7769 6e67 2e43 7573  star.drawing.Cus
+00003940: 746f 6d53 6861 7065 223e 0a20 2020 3c67  tomShape">.   <g
+00003950: 2069 643d 2269 6431 3322 3e0a 2020 2020   id="id13">.    
+00003960: 3c72 6563 7420 636c 6173 733d 2242 6f75  <rect class="Bou
+00003970: 6e64 696e 6742 6f78 2220 7374 726f 6b65  ndingBox" stroke
+00003980: 3d22 6e6f 6e65 2220 6669 6c6c 3d22 6e6f  ="none" fill="no
+00003990: 6e65 2220 783d 2231 3135 3030 2220 793d  ne" x="11500" y=
+000039a0: 2235 3530 3022 2077 6964 7468 3d22 3135  "5500" width="15
+000039b0: 3031 2220 6865 6967 6874 3d22 3130 3031  01" height="1001
+000039c0: 222f 3e0a 2020 2020 3c70 6174 6820 6669  "/>.    <path fi
+000039d0: 6c6c 3d22 7267 6228 3139 322c 3139 322c  ll="rgb(192,192,
+000039e0: 3139 3229 2220 7374 726f 6b65 3d22 6e6f  192)" stroke="no
+000039f0: 6e65 2220 643d 224d 2031 3232 3530 2c36  ne" d="M 12250,6
+00003a00: 3530 3020 4c20 3131 3530 302c 3635 3030  500 L 11500,6500
+00003a10: 2031 3135 3030 2c35 3530 3020 3133 3030   11500,5500 1300
+00003a20: 302c 3535 3030 2031 3330 3030 2c36 3530  0,5500 13000,650
+00003a30: 3020 3132 3235 302c 3635 3030 205a 222f  0 12250,6500 Z"/
+00003a40: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
+00003a50: 0a20 203c 6720 636c 6173 733d 2263 6f6d  .  <g class="com
+00003a60: 2e73 756e 2e73 7461 722e 6472 6177 696e  .sun.star.drawin
+00003a70: 672e 4c69 6e65 5368 6170 6522 3e0a 2020  g.LineShape">.  
+00003a80: 203c 6720 6964 3d22 6964 3134 223e 0a20   <g id="id14">. 
+00003a90: 2020 203c 7265 6374 2063 6c61 7373 3d22     <rect class="
+00003aa0: 426f 756e 6469 6e67 426f 7822 2073 7472  BoundingBox" str
+00003ab0: 6f6b 653d 226e 6f6e 6522 2066 696c 6c3d  oke="none" fill=
+00003ac0: 226e 6f6e 6522 2078 3d22 3630 3030 2220  "none" x="6000" 
+00003ad0: 793d 2235 3735 3022 2077 6964 7468 3d22  y="5750" width="
+00003ae0: 3330 3031 2220 6865 6967 6874 3d22 3530  3001" height="50
+00003af0: 3122 2f3e 0a20 2020 203c 7061 7468 2066  1"/>.    <path f
+00003b00: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+00003b10: 653d 2272 6762 2830 2c30 2c30 2922 2073  e="rgb(0,0,0)" s
+00003b20: 7472 6f6b 652d 7769 6474 683d 2235 3322  troke-width="53"
+00003b30: 2073 7472 6f6b 652d 6c69 6e65 6a6f 696e   stroke-linejoin
+00003b40: 3d22 726f 756e 6422 2073 7472 6f6b 652d  ="round" stroke-
+00003b50: 6c69 6e65 6361 703d 2273 7175 6172 6522  linecap="square"
+00003b60: 2064 3d22 4d20 3630 3332 2c36 3030 3020   d="M 6032,6000 
+00003b70: 4c20 3839 3638 2c36 3030 3022 2f3e 0a20  L 8968,6000"/>. 
+00003b80: 2020 203c 7061 7468 2066 696c 6c3d 2272     <path fill="r
+00003b90: 6762 2830 2c30 2c30 2922 2073 7472 6f6b  gb(0,0,0)" strok
+00003ba0: 653d 226e 6f6e 6522 2064 3d22 4d20 3630  e="none" d="M 60
+00003bb0: 3030 2c36 3235 3020 4c20 3630 3030 2c36  00,6250 L 6000,6
+00003bc0: 3038 3420 3630 3030 2c35 3931 3720 3630  084 6000,5917 60
+00003bd0: 3030 2c35 3735 3020 3630 3232 2c35 3735  00,5750 6022,575
+00003be0: 3020 3630 3433 2c35 3735 3020 3630 3636  0 6043,5750 6066
+00003bf0: 2c35 3735 3020 3630 3636 2c35 3931 3620  ,5750 6066,5916 
+00003c00: 3630 3636 2c36 3038 3320 3630 3636 2c36  6066,6083 6066,6
+00003c10: 3235 3020 3630 3434 2c36 3235 3020 3630  250 6044,6250 60
+00003c20: 3233 2c36 3235 3020 3630 3030 2c36 3235  23,6250 6000,625
+00003c30: 3020 5a22 2f3e 0a20 2020 203c 7061 7468  0 Z"/>.    <path
+00003c40: 2066 696c 6c3d 2272 6762 2830 2c30 2c30   fill="rgb(0,0,0
+00003c50: 2922 2073 7472 6f6b 653d 226e 6f6e 6522  )" stroke="none"
+00003c60: 2064 3d22 4d20 3930 3030 2c35 3735 3020   d="M 9000,5750 
+00003c70: 4c20 3930 3030 2c35 3931 3620 3930 3030  L 9000,5916 9000
+00003c80: 2c36 3038 3320 3930 3030 2c36 3235 3020  ,6083 9000,6250 
+00003c90: 3839 3738 2c36 3235 3020 3839 3537 2c36  8978,6250 8957,6
+00003ca0: 3235 3020 3839 3334 2c36 3235 3020 3839  250 8934,6250 89
+00003cb0: 3334 2c36 3038 3420 3839 3334 2c35 3931  34,6084 8934,591
+00003cc0: 3720 3839 3334 2c35 3735 3020 3839 3536  7 8934,5750 8956
+00003cd0: 2c35 3735 3020 3839 3737 2c35 3735 3020  ,5750 8977,5750 
+00003ce0: 3930 3030 2c35 3735 3020 5a22 2f3e 0a20  9000,5750 Z"/>. 
+00003cf0: 2020 3c2f 673e 0a20 203c 2f67 3e0a 2020    </g>.  </g>.  
+00003d00: 3c67 2063 6c61 7373 3d22 636f 6d2e 7375  <g class="com.su
+00003d10: 6e2e 7374 6172 2e64 7261 7769 6e67 2e43  n.star.drawing.C
+00003d20: 7573 746f 6d53 6861 7065 223e 0a20 2020  ustomShape">.   
+00003d30: 3c67 2069 643d 2269 6431 3522 3e0a 2020  <g id="id15">.  
+00003d40: 2020 3c72 6563 7420 636c 6173 733d 2242    <rect class="B
+00003d50: 6f75 6e64 696e 6742 6f78 2220 7374 726f  oundingBox" stro
+00003d60: 6b65 3d22 6e6f 6e65 2220 6669 6c6c 3d22  ke="none" fill="
+00003d70: 6e6f 6e65 2220 783d 2235 3439 3922 2079  none" x="5499" y
+00003d80: 3d22 3830 3030 2220 7769 6474 683d 2237  ="8000" width="7
+00003d90: 3530 3322 2068 6569 6768 743d 2231 3030  503" height="100
+00003da0: 3222 2f3e 0a20 2020 203c 7061 7468 2066  2"/>.    <path f
+00003db0: 696c 6c3d 2272 6762 2831 3030 2c31 3439  ill="rgb(100,149
+00003dc0: 2c32 3337 2922 2073 7472 6f6b 653d 226e  ,237)" stroke="n
+00003dd0: 6f6e 6522 2064 3d22 4d20 3133 3030 312c  one" d="M 13001,
+00003de0: 3830 3030 204c 2035 3937 362c 3830 3030  8000 L 5976,8000
+00003df0: 2035 3937 362c 3830 3030 2035 3530 302c   5976,8000 5500,
+00003e00: 3835 3030 2035 3937 362c 3930 3031 2035  8500 5976,9001 5
+00003e10: 3937 362c 3930 3031 2031 3330 3031 2c39  976,9001 13001,9
+00003e20: 3030 3120 3133 3030 312c 3830 3030 205a  001 13001,8000 Z
+00003e30: 222f 3e0a 2020 2020 3c74 6578 7420 636c  "/>.    <text cl
+00003e40: 6173 733d 2253 5647 5465 7874 5368 6170  ass="SVGTextShap
+00003e50: 6522 3e3c 7473 7061 6e20 636c 6173 733d  e"><tspan class=
+00003e60: 2254 6578 7450 6172 6167 7261 7068 2220  "TextParagraph" 
+00003e70: 666f 6e74 2d66 616d 696c 793d 224c 6962  font-family="Lib
+00003e80: 6572 6174 696f 6e20 5361 6e73 2c20 7361  eration Sans, sa
+00003e90: 6e73 2d73 6572 6966 2220 666f 6e74 2d73  ns-serif" font-s
+00003ea0: 697a 653d 2236 3335 7078 2220 666f 6e74  ize="635px" font
+00003eb0: 2d77 6569 6768 743d 2234 3030 223e 3c74  -weight="400"><t
+00003ec0: 7370 616e 2063 6c61 7373 3d22 5465 7874  span class="Text
+00003ed0: 506f 7369 7469 6f6e 2220 783d 2237 3133  Position" x="713
+00003ee0: 3122 2079 3d22 3837 3231 223e 3c74 7370  1" y="8721"><tsp
+00003ef0: 616e 2066 696c 6c3d 2272 6762 2830 2c30  an fill="rgb(0,0
+00003f00: 2c30 2922 2073 7472 6f6b 653d 226e 6f6e  ,0)" stroke="non
+00003f10: 6522 2073 7479 6c65 3d22 7768 6974 652d  e" style="white-
+00003f20: 7370 6163 653a 2070 7265 223e 5365 7175  space: pre">Sequ
+00003f30: 656e 6365 2023 3420 5232 3c2f 7473 7061  ence #4 R2</tspa
+00003f40: 6e3e 3c2f 7473 7061 6e3e 3c2f 7473 7061  n></tspan></tspa
+00003f50: 6e3e 3c2f 7465 7874 3e0a 2020 203c 2f67  n></text>.   </g
+00003f60: 3e0a 2020 3c2f 673e 0a20 203c 6720 636c  >.  </g>.  <g cl
+00003f70: 6173 733d 2263 6f6d 2e73 756e 2e73 7461  ass="com.sun.sta
+00003f80: 722e 6472 6177 696e 672e 4375 7374 6f6d  r.drawing.Custom
+00003f90: 5368 6170 6522 3e0a 2020 203c 6720 6964  Shape">.   <g id
+00003fa0: 3d22 6964 3136 223e 0a20 2020 203c 7265  ="id16">.    <re
+00003fb0: 6374 2063 6c61 7373 3d22 426f 756e 6469  ct class="Boundi
+00003fc0: 6e67 426f 7822 2073 7472 6f6b 653d 226e  ngBox" stroke="n
+00003fd0: 6f6e 6522 2066 696c 6c3d 226e 6f6e 6522  one" fill="none"
+00003fe0: 2078 3d22 3131 3530 3022 2079 3d22 3730   x="11500" y="70
+00003ff0: 3030 2220 7769 6474 683d 2231 3530 3322  00" width="1503"
+00004000: 2068 6569 6768 743d 2231 3030 3222 2f3e   height="1002"/>
+00004010: 0a20 2020 203c 7061 7468 2066 696c 6c3d  .    <path fill=
+00004020: 2272 6762 2831 3932 2c31 3932 2c31 3932  "rgb(192,192,192
+00004030: 2922 2073 7472 6f6b 653d 226e 6f6e 6522  )" stroke="none"
+00004040: 2064 3d22 4d20 3133 3030 312c 3730 3030   d="M 13001,7000
+00004050: 204c 2031 3138 3237 2c37 3030 3020 3131   L 11827,7000 11
+00004060: 3832 372c 3730 3030 2031 3135 3030 2c37  827,7000 11500,7
+00004070: 3530 3020 3131 3832 372c 3830 3031 2031  500 11827,8001 1
+00004080: 3138 3237 2c38 3030 3120 3133 3030 312c  1827,8001 13001,
+00004090: 3830 3031 2031 3330 3031 2c37 3030 3020  8001 13001,7000 
+000040a0: 5a22 2f3e 0a20 2020 3c2f 673e 0a20 203c  Z"/>.   </g>.  <
+000040b0: 2f67 3e0a 2020 3c67 2063 6c61 7373 3d22  /g>.  <g class="
+000040c0: 636f 6d2e 7375 6e2e 7374 6172 2e64 7261  com.sun.star.dra
+000040d0: 7769 6e67 2e43 7573 746f 6d53 6861 7065  wing.CustomShape
+000040e0: 223e 0a20 2020 3c67 2069 643d 2269 6431  ">.   <g id="id1
+000040f0: 3722 3e0a 2020 2020 3c72 6563 7420 636c  7">.    <rect cl
+00004100: 6173 733d 2242 6f75 6e64 696e 6742 6f78  ass="BoundingBox
+00004110: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+00004120: 6669 6c6c 3d22 6e6f 6e65 2220 783d 2239  fill="none" x="9
+00004130: 3939 2220 793d 2237 3939 3922 2077 6964  99" y="7999" wid
+00004140: 7468 3d22 3135 3032 2220 6865 6967 6874  th="1502" height
+00004150: 3d22 3130 3032 222f 3e0a 2020 2020 3c70  ="1002"/>.    <p
+00004160: 6174 6820 6669 6c6c 3d22 7267 6228 3139  ath fill="rgb(19
+00004170: 322c 3139 322c 3139 3229 2220 7374 726f  2,192,192)" stro
+00004180: 6b65 3d22 6e6f 6e65 2220 643d 224d 2039  ke="none" d="M 9
+00004190: 3939 2c39 3030 3020 4c20 3231 3733 2c39  99,9000 L 2173,9
+000041a0: 3030 3020 3231 3733 2c39 3030 3020 3235  000 2173,9000 25
+000041b0: 3030 2c38 3530 3020 3231 3733 2c37 3939  00,8500 2173,799
+000041c0: 3920 3231 3733 2c37 3939 3920 3939 392c  9 2173,7999 999,
+000041d0: 3739 3939 2039 3939 2c39 3030 3020 5a22  7999 999,9000 Z"
+000041e0: 2f3e 0a20 2020 3c2f 673e 0a20 203c 2f67  />.   </g>.  </g
+000041f0: 3e0a 2020 3c67 2063 6c61 7373 3d22 636f  >.  <g class="co
+00004200: 6d2e 7375 6e2e 7374 6172 2e64 7261 7769  m.sun.star.drawi
+00004210: 6e67 2e43 7573 746f 6d53 6861 7065 223e  ng.CustomShape">
+00004220: 0a20 2020 3c67 2069 643d 2269 6431 3822  .   <g id="id18"
+00004230: 3e0a 2020 2020 3c72 6563 7420 636c 6173  >.    <rect clas
+00004240: 733d 2242 6f75 6e64 696e 6742 6f78 2220  s="BoundingBox" 
+00004250: 7374 726f 6b65 3d22 6e6f 6e65 2220 6669  stroke="none" fi
+00004260: 6c6c 3d22 6e6f 6e65 2220 783d 2239 3939  ll="none" x="999
+00004270: 2220 793d 2237 3030 3022 2077 6964 7468  " y="7000" width
+00004280: 3d22 3730 3032 2220 6865 6967 6874 3d22  ="7002" height="
+00004290: 3130 3032 222f 3e0a 2020 2020 3c70 6174  1002"/>.    <pat
+000042a0: 6820 6669 6c6c 3d22 7267 6228 3130 302c  h fill="rgb(100,
+000042b0: 3134 392c 3233 3729 2220 7374 726f 6b65  149,237)" stroke
+000042c0: 3d22 6e6f 6e65 2220 643d 224d 2039 3939  ="none" d="M 999
+000042d0: 2c37 3030 3020 4c20 3735 3536 2c37 3030  ,7000 L 7556,700
+000042e0: 3020 3735 3536 2c37 3030 3020 3830 3030  0 7556,7000 8000
+000042f0: 2c37 3530 3020 3735 3536 2c38 3030 3120  ,7500 7556,8001 
+00004300: 3735 3536 2c38 3030 3120 3939 392c 3830  7556,8001 999,80
+00004310: 3031 2039 3939 2c37 3030 3020 5a22 2f3e  01 999,7000 Z"/>
+00004320: 0a20 2020 203c 7465 7874 2063 6c61 7373  .    <text class
+00004330: 3d22 5356 4754 6578 7453 6861 7065 223e  ="SVGTextShape">
+00004340: 3c74 7370 616e 2063 6c61 7373 3d22 5465  <tspan class="Te
+00004350: 7874 5061 7261 6772 6170 6822 2066 6f6e  xtParagraph" fon
+00004360: 742d 6661 6d69 6c79 3d22 4c69 6265 7261  t-family="Libera
+00004370: 7469 6f6e 2053 616e 732c 2073 616e 732d  tion Sans, sans-
+00004380: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00004390: 3d22 3633 3570 7822 2066 6f6e 742d 7765  ="635px" font-we
+000043a0: 6967 6874 3d22 3430 3022 3e3c 7473 7061  ight="400"><tspa
+000043b0: 6e20 636c 6173 733d 2254 6578 7450 6f73  n class="TextPos
+000043c0: 6974 696f 6e22 2078 3d22 3139 3230 2220  ition" x="1920" 
+000043d0: 793d 2237 3732 3122 3e3c 7473 7061 6e20  y="7721"><tspan 
+000043e0: 6669 6c6c 3d22 7267 6228 302c 302c 3029  fill="rgb(0,0,0)
+000043f0: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+00004400: 7374 796c 653d 2277 6869 7465 2d73 7061  style="white-spa
+00004410: 6365 3a20 7072 6522 3e53 6571 7565 6e63  ce: pre">Sequenc
+00004420: 6520 2334 2052 313c 2f74 7370 616e 3e3c  e #4 R1</tspan><
+00004430: 2f74 7370 616e 3e3c 2f74 7370 616e 3e3c  /tspan></tspan><
+00004440: 2f74 6578 743e 0a20 2020 3c2f 673e 0a20  /text>.   </g>. 
+00004450: 203c 2f67 3e0a 203c 2f67 3e0a 3c2f 7376   </g>. </g>.</sv
+00004460: 673e                                     g>
```

### Comparing `sequali-0.7.1/docs/_static/images/overrepresented_sampling.fodg` & `sequali-0.8.0/docs/_static/images/overrepresented_sampling.fodg`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/docs/_static/images/overrepresented_sampling.svg` & `sequali-0.8.0/docs/_static/images/overrepresented_sampling.svg`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/docs/conf.py` & `sequali-0.8.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,10 +24,13 @@
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
 html_static_path = ['_static']
 
+# Add reports to the root so they can be referenced
+html_extra_path = ['reports']
+
 html_theme_options = dict(
     display_version=True,
 )
```

### Comparing `sequali-0.7.1/docs/includes/CHANGELOG.rst` & `sequali-0.8.0/docs/includes/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 ==========
 
 .. Newest changes should be on top.
 
 .. This document is user facing. Please word the changes in such a way
 .. that users understand how the changes affect the new version.
 
+version 0.8.0
+-----------------
++ A citation file was added to the repository.
++ Calculate insert sizes and used adapters based on overlap between the
+  read pairs.
++ Both reads from paired-end reads are taken into consideration when
+  evaluating the duplication rate.
++ Support for paired-end reads added.
++ Minor performance improvement by providing a non-temporal cache hint in the
+  QCMetrics module.
+
 version 0.7.1
 -----------------
 + Fix a small visual bug in the report sidebar.
 + PyGAL report htmls are now fully HTML5 compliant. HTML5 validation has been
   made a part of the integration testing.
 
 version 0.7.0
```

### Comparing `sequali-0.7.1/docs/includes/README.rst` & `sequali-0.8.0/docs/includes/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-.. image:: https://img.shields.io/pypi/v/sequali.svg
+.. |python-version-shield| image:: https://img.shields.io/pypi/v/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/conda/v/bioconda/sequali.svg
+.. |conda-version-shield| image:: https://img.shields.io/conda/v/bioconda/sequali.svg
   :target: https://bioconda.github.io/recipes/sequali/README.html
   :alt:
 
-.. image:: https://img.shields.io/pypi/pyversions/sequali.svg
+.. |python-install-version-shield| image:: https://img.shields.io/pypi/pyversions/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/pypi/l/sequali.svg
+.. |license-shield| image:: https://img.shields.io/pypi/l/sequali.svg
   :target: https://github.com/rhpvorderman/sequali/blob/main/LICENSE
   :alt:
 
-.. image:: https://readthedocs.org/projects/sequali/badge/?version=latest
+.. |docs-shield| image:: https://readthedocs.org/projects/sequali/badge/?version=latest
   :target: https://sequali.readthedocs.io/en/latest/?badge=latest
   :alt:
 
-.. image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
+.. |coverage-shield| image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
   :target: https://codecov.io/gh/rhpvorderman/sequali
   :alt:
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
+.. |zenodo-shield| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
   :target: https://doi.org/10.5281/zenodo.10854010
   :alt:
 
+|python-version-shield| |conda-version-shield| |python-install-version-shield|
+|license-shield| |docs-shield| |coverage-shield| |zenodo-shield|
+
 ========
 Sequali
 ========
 
 .. introduction start
 
 Sequence quality metrics for FASTQ and uBAM files.
@@ -40,22 +43,25 @@
 + Informative graphs that allow for judging the quality of a sequence at
   a quick glance.
 + Overrepresentation analysis using 21 bp sequence fragments. Overrepresented
   sequences are checked against the NCBI univec database.
 + Estimate duplication rate using a `fingerprint subsampling technique which is
   also used in filesystem duplication estimation
   <https://www.usenix.org/system/files/conference/atc13/atc13-xie.pdf>`_.
-+ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences.
++ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences
+  for single read data.
++ Determines adapters by overlap analysis for paired read data.
++ Insert size metrics for paired read data.
 + Per tile quality plots for illumina reads.
 + Channel and other plots for nanopore reads.
 + FASTQ and unaligned BAM are supported. See "Supported formats".
 
 Example reports:
 
-+ `GM24385_1.fastq.gz <https://github.com/rhpvorderman/sequali/files/14725146/GM24385_1.fastq.gz.html.zip>`_;
++ `GM24385_1.fastq.gz <https://sequali.readthedocs.io/en/latest/GM24385_1.fastq.gz.html>`_;
   HG002 (Genome In A Bottle) on ultra-long Nanopore Sequencing. `Sequence file download <https://ftp-trace.ncbi.nlm.nih.gov/ReferenceSamples/giab/data/AshkenazimTrio/HG002_NA24385_son/UCSC_Ultralong_OxfordNanopore_Promethion/GM24385_1.fastq.gz>`_.
 
 .. introduction end
 
 For more information check `the documentation <https://sequali.readthedocs.io>`_.
 
 Supported formats
@@ -63,19 +69,19 @@
 
 .. formats start
 
 - FASTQ. Only the Sanger variation with a phred offset of 33 and the error rate
   calculation of 10 ^ (-phred/10) is supported. All sequencers use this
   format today.
 
+  - Paired end sequencing data is supported.
   - For sequences called by illumina base callers an additional plot with the
     per tile quality will be provided.
   - For sequences called by guppy additional plots for nanopore specific
     data will be provided.
-
 - unaligned BAM. Any alignment flags are currently ignored.
 
   - For uBAM data as delivered by dorado additional nanopore plots will be
     provided.
 
 .. formats end
```

### Comparing `sequali-0.7.1/docs/index.rst` & `sequali-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/docs/module_options.rst` & `sequali-0.8.0/docs/module_options.rst`

 * *Files 3% similar despite different names*

```diff
@@ -104,23 +104,27 @@
 such this can provide a reasonable estimate, which is good enough for detecting
 problematic libraries.
 
 Sequali's fingerprints by collecting a small sample from the front and back
 of the sequence. To avoid adapter sequences, the samples are taken at an
 offset. If the sequence is small, the offsets are sunk proportionally. If the
 sequence is smaller than the sample sequence lenghts, its entire length
-is sampled.
+is sampled. Paired sequences are sampled at the beginning of both its sequences
+without an offset, since adapter sequences for illumina sequences are closer
+to the end.
 
 .. figure:: _static/images/fingerprint.svg
 
     Sequali fingerprinting. Small samples are taken from the front and back
     of the sequence at an offset. Sequence #1 shows the common situation where
     the sequence is long. Sequence #2 is smaller than the combined length of
     the offsets and the samples, so the offsets are shrunk proportionally.
     Sequence #3 is smaller than the sample length, so its sampled entirely.
+    Sequence #4 is paired, so samples are taken from the beginning of R1 and
+    R2.
 
 The sampled sequences are then combined into one and hashed. The hash
 seed is determined by the sequence length integer divided by 64. The resulting
 hash is the fingerprint.
 
 Since not all fingerprints can be counted due to memory constraints, `a hash
 subsampling technique from the file storage world
@@ -144,11 +148,13 @@
 
 + ``--duplication-max-stored-fingerprints``: The maximum amount of stored
   fingerprints. More fingerprints lead to more accurate estimates but also more
   memory usage.
 
 These options can be used to control how the fingerprint is taken
 
-+ ``--fingerprint-front-length``
-+ ``--fingerprint-back-length``
-+ ``--fingerprint-front-offset``
-+ ``--fingerprint-back-offset``
++ ``--fingerprint-front-length``.
++ ``--fingerprint-back-length``.  For paired-end sequencing this is the length
+  of the sample from from the beginning for R2.
++ ``--fingerprint-front-offset``.
++ ``--fingerprint-back-offset``. For paired-end sequencing this is the offset
+  the sample from the beginning for R2.
```

### Comparing `sequali-0.7.1/pyproject.toml` & `sequali-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "setuptools-scm>=8.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="sequali"
-description="Fast sequencing quality metrics"
+description="Sequali is a QC tool that generates useful graphs for both short and long-read data."
 authors = [
     {name = "Ruben Vorderman", email = "r.h.p.vorderman@lumc.nl"}
 ]
 keywords=[
     "FASTQ",
     "sequencing quality",
     "uBAM",
```

### Comparing `sequali-0.7.1/setup.py` & `sequali-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/__init__.py` & `sequali-0.8.0/src/sequali/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with Sequali.  If not, see <https://www.gnu.org/licenses/
 
 from ._qc import A, C, G, N, T
-from ._qc import AdapterCounter, BamParser, FastqParser, FastqRecordView, \
-    PerTileQuality, QCMetrics, SequenceDuplication
+from ._qc import (
+    AdapterCounter, BamParser, FastqParser, FastqRecordArrayView,
+    FastqRecordView, PerTileQuality, QCMetrics, SequenceDuplication
+)
 from ._qc import NUMBER_OF_NUCS, NUMBER_OF_PHREDS, PHRED_MAX, TABLE_SIZE
 from ._version import __version__
 
 
 __all__ = [
     "A", "C", "G", "N", "T",
     "AdapterCounter",
     "BamParser",
     "FastqParser",
     "FastqRecordView",
+    "FastqRecordArrayView",
     "PerTileQuality",
     "QCMetrics",
     "SequenceDuplication",
     "NUMBER_OF_NUCS",
     "NUMBER_OF_PHREDS",
     "PHRED_MAX",
     "TABLE_SIZE",
```

### Comparing `sequali-0.7.1/src/sequali/__main__.py` & `sequali-0.8.0/src/sequali/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,53 +11,58 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with Sequali.  If not, see <https://www.gnu.org/licenses/
 
 import argparse
+import contextlib
 import json
 import os
 import sys
 
-import xopen
 
 from ._qc import (
     AdapterCounter,
-    BamParser,
     DEFAULT_DEDUP_MAX_STORED_FINGERPRINTS,
     DEFAULT_FINGERPRINT_BACK_SEQUENCE_LENGTH,
     DEFAULT_FINGERPRINT_BACK_SEQUENCE_OFFSET,
     DEFAULT_FINGERPRINT_FRONT_SEQUENCE_LENGTH,
     DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET,
     DEFAULT_FRAGMENT_LENGTH,
     DEFAULT_MAX_UNIQUE_FRAGMENTS,
     DEFAULT_UNIQUE_SAMPLE_EVERY,
     DedupEstimator,
-    FastqParser,
+    InsertSizeMetrics,
     NanoStats,
     PerTileQuality,
     QCMetrics,
     SequenceDuplication
 )
 from ._version import __version__
 from .adapters import DEFAULT_ADAPTER_FILE, adapters_from_file
 from .report_modules import (calculate_stats, dict_to_report_modules,
                              report_modules_to_dict, write_html_report)
-from .util import (ProgressUpdater, guess_sequencing_technology_from_bam_header,
-                   guess_sequencing_technology_from_file)
+from .util import NGSFile, sequence_names_match
+
+DEFAULT_FINGERPRINT_BACK_SEQUENCE_PAIRED_OFFSET = 0
+DEFAULT_FINGERPRINT_FRONT_SEQUENCE_PAIRED_OFFSET = 0
 
 
 def argument_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description="Create a quality metrics report for sequencing data.")
     parser.add_argument("input", metavar="INPUT",
                         help="Input FASTQ or uBAM file. "
                              "The format is autodetected and compressed "
                              "formats are supported.")
+    parser.add_argument("input_reverse", metavar="INPUT_REVERSE",
+                        nargs="?",
+                        help="Second FASTQ file for Illumina paired-end reads."
+                        )
     parser.add_argument("--json",
                         help="JSON output file. default: '<input>.json'.")
     parser.add_argument("--html",
                         help="HTML output file. default: '<input>.html'.")
     parser.add_argument("--outdir", "--dir", metavar="OUTDIR",
                         help="Output directory for the report files. default: "
                              "current working directory.",
@@ -134,100 +139,171 @@
                         default=DEFAULT_FINGERPRINT_BACK_SEQUENCE_LENGTH,
                         metavar="LENGTH",
                         help=f"Set the number of bases to be taken for the "
                              f"deduplication fingerprint from the back of "
                              f"the sequence. "
                              f"Default: {DEFAULT_FINGERPRINT_BACK_SEQUENCE_LENGTH}.")
     parser.add_argument("--fingerprint-front-offset", type=int,
-                        default=DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET,
                         metavar="LENGTH",
                         help=f"Set the offset for the front part of the "
                              f"deduplication fingerprint. Useful for avoiding "
                              f"adapter sequences. "
-                             f"Default: {DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET}.")
+                             f"Default: {DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET} "
+                             f"for single end, "
+                             f"{DEFAULT_FINGERPRINT_FRONT_SEQUENCE_PAIRED_OFFSET} "
+                             f"for paired sequences.")
     parser.add_argument("--fingerprint-back-offset", type=int,
-                        default=DEFAULT_FINGERPRINT_BACK_SEQUENCE_OFFSET,
                         metavar="LENGTH",
                         help=f"Set the offset for the back part of the "
                              f"deduplication fingerprint. Useful for avoiding "
                              f"adapter sequences. "
-                             f"Default: {DEFAULT_FINGERPRINT_BACK_SEQUENCE_OFFSET}.")
+                             f"Default: {DEFAULT_FINGERPRINT_BACK_SEQUENCE_OFFSET} "
+                             f"for single end, "
+                             f"{DEFAULT_FINGERPRINT_BACK_SEQUENCE_PAIRED_OFFSET} "
+                             f"for paired sequences.")
     parser.add_argument("-t", "--threads", type=int, default=2,
                         help="Number of threads to use. If greater than one "
                              "an additional thread for gzip "
                              "decompression will be used. Default: 2.")
     parser.add_argument("--version", action="version",
                         version=__version__)
     return parser
 
 
 def main() -> None:
     args = argument_parser().parse_args()
+    threads = args.threads
+    if threads < 1:
+        raise ValueError(f"Threads must be greater than 1, got {threads}.")
+
     fraction_threshold = args.overrepresentation_threshold_fraction
     max_threshold = args.overrepresentation_max_threshold
     # if max_threshold is set it needs to be lower than min threshold
     min_threshold = min(args.overrepresentation_min_threshold, max_threshold)
+    paired = bool(args.input_reverse)
 
-    metrics = QCMetrics()
-    per_tile_quality = PerTileQuality()
-    sequence_duplication = SequenceDuplication(
+    metrics1 = QCMetrics()
+    per_tile_quality1 = PerTileQuality()
+    nanostats1 = NanoStats()
+    sequence_duplication1 = SequenceDuplication(
         max_unique_fragments=args.overrepresentation_max_unique_fragments,
         fragment_length=args.overrepresentation_fragment_length,
         sample_every=args.overrepresentation_sample_every
     )
+    if paired:
+        if args.fingerprint_front_offset is None:
+            args.fingerprint_front_offset = (
+                DEFAULT_FINGERPRINT_FRONT_SEQUENCE_PAIRED_OFFSET)
+        if args.fingerprint_back_offset is None:
+            args.fingerprint_back_offset = (
+                DEFAULT_FINGERPRINT_BACK_SEQUENCE_PAIRED_OFFSET)
+    else:
+        if args.fingerprint_front_offset is None:
+            args.fingerprint_front_offset = (
+                DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET)
+        if args.fingerprint_back_offset is None:
+            args.fingerprint_back_offset = (
+                DEFAULT_FINGERPRINT_BACK_SEQUENCE_PAIRED_OFFSET)
     dedup_estimator = DedupEstimator(
         max_stored_fingerprints=args.duplication_max_stored_fingerprints,
         front_sequence_length=args.fingerprint_front_length,
         front_sequence_offset=args.fingerprint_front_offset,
         back_sequence_length=args.fingerprint_back_length,
         back_sequence_offset=args.fingerprint_back_offset,
     )
-    nanostats = NanoStats()
-    filename: str = args.input
-    threads = args.threads
-    if threads < 1:
-        raise ValueError(f"Threads must be greater than 1, got {threads}.")
-    with open(filename, "rb") as raw:
-        progress = ProgressUpdater(raw)
-        with xopen.xopen(raw, "rb", threads=threads - 1) as file:
-            if filename.endswith(".bam") or (
-                    hasattr(file, "peek") and file.peek(4)[:4] == b"BAM\1"):
-                reader = BamParser(file)
-                seqtech = guess_sequencing_technology_from_bam_header(reader.header)
+
+    if paired:
+        insert_size_metrics = InsertSizeMetrics()
+        metrics2 = QCMetrics()
+        per_tile_quality2 = PerTileQuality()
+        sequence_duplication2 = SequenceDuplication(
+            max_unique_fragments=args.overrepresentation_max_unique_fragments,
+            fragment_length=args.overrepresentation_fragment_length,
+            sample_every=args.overrepresentation_sample_every
+        )
+    else:
+        metrics2 = None
+        per_tile_quality2 = None
+        sequence_duplication2 = None
+        insert_size_metrics = None
+    with contextlib.ExitStack() as exit_stack:
+        reader1 = NGSFile(args.input, threads - 1)
+        exit_stack.enter_context(reader1)
+        seqtech = reader1.sequencing_technology
+        if paired:
+            reader2 = NGSFile(args.input_reverse, threads - 1)
+            exit_stack.enter_context(reader2)
+            if reader1.sequencing_technology != reader2.sequencing_technology:
+                raise RuntimeError(
+                    f"Mismatching sequencing technologies:\n"
+                    f"{reader1.filepath}: {reader1.sequencing_technology}\n"
+                    f"{reader2.filepath}: {reader2.sequencing_technology}\n")
+            if not (reader1.format == "FASTQ" and reader2.format == "FASTQ"):
+                raise RuntimeError("Paired end mode is only supported for "
+                                   "FASTQ files.")
+            seqtech = "illumina"  # Paired end is always illumina
+            adapter_counter1 = None
+        adapters = list(adapters_from_file(args.adapter_file, seqtech))
+        if not paired:
+            adapter_counter1 = AdapterCounter(
+                adapter.sequence for adapter in adapters)
+        for record_array1 in reader1:
+            metrics1.add_record_array(record_array1)
+            per_tile_quality1.add_record_array(record_array1)
+            sequence_duplication1.add_record_array(record_array1)
+            nanostats1.add_record_array(record_array1)
+            if paired:
+                record_array2 = reader2.read(len(record_array1))
+                if len(record_array1) != len(record_array2):
+                    raise RuntimeError(
+                        f"FASTQ Files out of sync {args.input} has more "
+                        f"FASTQ records than {args.input_reverse}.")
+                if not (record_array1.is_mate(record_array2)):
+                    for r1, r2 in zip(iter(record_array1),
+                                      iter(record_array2)):
+                        if not sequence_names_match(r1.name(),
+                                                    r2.name()):
+                            raise RuntimeError(
+                                f"Mismatching names found! {r1.name()} "
+                                f"{r2.name()}")
+                    raise RuntimeError("Mismatching names found!")
+                dedup_estimator.add_record_array_pair(record_array1, record_array2)
+                insert_size_metrics.add_record_array_pair(record_array1, record_array2)  # type: ignore  # noqa: E501
+                metrics2.add_record_array(record_array2)  # type: ignore  # noqa: E501
+                per_tile_quality2.add_record_array(record_array2)  # type: ignore  # noqa: E501
+                sequence_duplication2.add_record_array(record_array2)  # type: ignore  # noqa: E501
             else:
-                reader = FastqParser(file)  # type: ignore
-                seqtech = guess_sequencing_technology_from_file(file)  # type: ignore
-            adapters = list(adapters_from_file(args.adapter_file, seqtech))
-            adapter_counter = AdapterCounter(adapter.sequence for adapter in adapters)
-            with progress:
-                for record_array in reader:
-                    metrics.add_record_array(record_array)
-                    per_tile_quality.add_record_array(record_array)
-                    adapter_counter.add_record_array(record_array)
-                    sequence_duplication.add_record_array(record_array)
-                    nanostats.add_record_array(record_array)
-                    dedup_estimator.add_record_array(record_array)
-                    progress.update(record_array)
+                adapter_counter1.add_record_array(record_array1)   # type: ignore  # noqa: E501
+                dedup_estimator.add_record_array(record_array1)
+        if paired and len(reader2.read(1)) > 0:
+            raise RuntimeError(
+                f"FASTQ Files out of sync {args.input_reverse} has "
+                f"more FASTQ records than {args.input}.")
     report_modules = calculate_stats(
-        filename,
-        metrics,
-        adapter_counter,
-        per_tile_quality,
-        sequence_duplication,
-        dedup_estimator,
-        nanostats,
+        filename=args.input,
+        metrics=metrics1,
+        adapter_counter=adapter_counter1,
+        per_tile_quality=per_tile_quality1,
+        sequence_duplication=sequence_duplication1,
+        dedup_estimator=dedup_estimator,
+        nanostats=nanostats1,
+        insert_size_metrics=insert_size_metrics,
+        filename_reverse=args.input_reverse,
+        metrics_reverse=metrics2,
+        per_tile_quality_reverse=per_tile_quality2,
+        sequence_duplication_reverse=sequence_duplication2,
         adapters=adapters,
         fraction_threshold=fraction_threshold,
         min_threshold=min_threshold,
         max_threshold=max_threshold)
+    os.makedirs(args.outdir, exist_ok=True)
     if args.json is None:
-        args.json = os.path.basename(filename) + ".json"
+        args.json = os.path.basename(args.input) + ".json"
     if args.html is None:
-        args.html = os.path.basename(filename) + ".html"
-    os.makedirs(args.outdir, exist_ok=True)
+        args.html = os.path.basename(args.input) + ".html"
     if not os.path.isabs(args.json):
         args.json = os.path.join(args.outdir, args.json)
     if not os.path.isabs(args.html):
         args.html = os.path.join(args.outdir, args.html)
     with open(args.json, "wt") as json_file:
         json_dict = report_modules_to_dict(report_modules)
         # Indent=0 is ~40% smaller than indent=2 while still human-readable
```

### Comparing `sequali-0.7.1/src/sequali/_qc.pyi` & `sequali-0.8.0/src/sequali/_qc.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -32,33 +32,36 @@
 DEFAULT_DEDUP_MAX_STORED_FINGERPRINTS: int
 DEFAULT_FRAGMENT_LENGTH: int
 DEFAULT_UNIQUE_SAMPLE_EVERY: int
 DEFAULT_FINGERPRINT_FRONT_SEQUENCE_LENGTH: int
 DEFAULT_FINGERPRINT_BACK_SEQUENCE_LENGTH: int
 DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET: int
 DEFAULT_FINGERPRINT_BACK_SEQUENCE_OFFSET: int
+INSERT_SIZE_MAX_ADAPTER_STORE_SIZE: int
 
 
 class FastqRecordView:
     obj: bytes
     def __init__(self, __name, __sequence, __qualities) -> None: ...
     def name(self) -> str: ...
     def sequence(self) -> str: ...
     def qualities(self) -> str: ...
 
 class FastqRecordArrayView:
     obj: bytes
     def __init__(self, view_items: Iterable[FastqRecordView]) -> None: ...
     def __getitem__(self, index: SupportsIndex) -> FastqRecordView: ...
-    def __len__(self) -> int: ... 
+    def __len__(self) -> int: ...
+    def is_mate(self, other: FastqRecordArrayView): ...
 
 class FastqParser:
     def __init__(self, fileobj, initial_buffersize = 128 * 1024): ...
     def __iter__(self) -> FastqParser: ...
     def __next__(self) -> FastqRecordArrayView: ...
+    def read(self, number_of_records: int) -> FastqRecordArrayView: ...
 
 class BamParser:
     header: bytes
     def __init__(self, fileobj, initial_buffersize = 96 * 1024): ...
     def __iter__(self) -> BamParser: ...
     def __next__(self) -> FastqRecordArrayView: ...
 
@@ -128,15 +131,20 @@
             *,
             front_sequence_length: int = DEFAULT_FINGERPRINT_FRONT_SEQUENCE_LENGTH,
             back_sequence_length: int = DEFAULT_FINGERPRINT_BACK_SEQUENCE_LENGTH,
             front_sequence_offset: int = DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET,
             back_sequence_offset: int = DEFAULT_FINGERPRINT_BACK_SEQUENCE_OFFSET,
     ): ...
     def add_sequence(self, __sequence: str) -> None: ...
+    def add_sequence_pair(self, __sequence1: str, __sequence2: str) -> None: ...
     def add_record_array(self, __record_array: FastqRecordArrayView) -> None: ...
+    def add_record_array_pair(self, 
+                              __record_array1: FastqRecordArrayView,
+                              __record_array2: FastqRecordArrayView,
+                              ) -> None: ...
     def duplication_counts(self) -> array.ArrayType: ...
 
 class NanoporeReadInfo:
     start_time: int
     channel_id: int
     length: int
     cumulative_error_rate: float
@@ -146,7 +154,23 @@
     number_of_reads: int
     skipped_reason: Optional[str]
     minimum_time: int
     maximum_time: int
     def add_read(self, __read: FastqRecordView) -> None: ...
     def add_record_array(self, __record_array: FastqRecordArrayView) -> None: ...
     def nano_info_iterator(self) -> Iterator[NanoporeReadInfo]: ...
+
+
+class InsertSizeMetrics:
+    total_reads: int
+    number_of_adapters_read1: int
+    number_of_adapters_read2: int
+
+    def __init__(self): ...
+    def add_sequence_pair(self, __sequence1: str, __sequence2: str) -> None: ...
+    def add_record_array_pair(self,
+                              __record_array1: FastqRecordArrayView,
+                              __record_array2: FastqRecordArrayView,
+                              ) -> None: ...
+    def insert_sizes(self) -> array.ArrayType: ...
+    def adapters_read1(self) -> List[Tuple[str, int]]: ...
+    def adapters_read2(self) -> List[Tuple[str, int]]: ...
```

### Comparing `sequali-0.7.1/src/sequali/_qcmodule.c` & `sequali-0.8.0/src/sequali/_qcmodule.c`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,24 @@
 #define PHRED_MAX 93
 
 
 /*********
  * Utils *
  *********/
 
+static inline void non_temporal_prefetch(void *address)
+{
+    #ifdef __SSE2__
+    _mm_prefetch(address, _MM_HINT_NTA);
+    #else 
+    /* no-op for non-x86 architectures*/
+    return;
+    #endif
+}
+
 static PyObject *
 PythonArray_FromBuffer(char typecode, void *buffer, size_t buffersize) 
 {
     PyObject *array = PyObject_CallFunction((PyObject *)PythonArray, "C", typecode);
     if (array == NULL) {
         return NULL;
     } 
@@ -577,14 +587,15 @@
     PyObject *obj = PyBytes_FromStringAndSize(NULL, total_memory_size);
     if (obj == NULL) {
         return PyErr_NoMemory();
     }
     FastqRecordArrayView *record_array = 
         (FastqRecordArrayView *)
         FastqRecordArrayView_FromPointerSizeAndObject(NULL, number_of_items, obj);
+    Py_DECREF(obj);  // Reference count increased by 1 by previous function.
     if (record_array == NULL) {
         Py_DECREF(obj); 
         return NULL;
     }
     char *record_ptr = PyBytes_AS_STRING(obj);
     struct FastqMeta *metas = record_array->records;
     for (Py_ssize_t i=0; i < number_of_items; i++) {
@@ -631,14 +642,105 @@
 }
 
 static inline int 
 FastqRecordArrayView_CheckExact(void *obj) {
     return Py_TYPE(obj) == &FastqRecordArrayView_Type;
 }
 
+/**
+ * @brief Compare two FASTQ record names to see if they are mates.
+ * 
+ * They are mates if their IDs are the same. The ID is the part before the 
+ * first whitespace. If the last symbol of both IDs is a '1' or '2' it is 
+ * ignored to allow 'record/1' and 'record/2' to match.
+ * 
+ * @param name1 Pointer to the first name
+ * @param name2 Pointer to the second name
+ * @param name2_length The length of the second name
+ */
+static inline bool 
+fastq_names_are_mates(const char *name1, const char *name2, size_t name2_length) {
+    /* strcspn will return the length of the string if none of the complement 
+       characters is found, so name1_length is not necessary as a parameter.*/
+    size_t id_length = strcspn(name1, " \t\n");
+    if (name2_length < id_length) {
+        return false;
+    }  
+    if (name2_length > id_length) {
+        char id2_sep = name2[id_length];
+        if (!(id2_sep == ' ' || id2_sep == '\t' || id2_sep == '\n')) {
+            return false;
+        }
+    }
+    /* Make sure /1 and /2 endings are ignored. */
+    char id1_last_char = name1[id_length - 1];
+    if (id1_last_char == '1' || id1_last_char == '2') {
+        char id2_last_char = name2[id_length -1];
+        if (id2_last_char == '1' || id2_last_char == '2') {
+            id_length -= 1;
+        }
+    }
+    return memcmp(name1, name2, id_length) == 0;
+}
+
+PyDoc_STRVAR(FastqRecordArrayView_is_mate__doc__,
+"is_mate($self, other, /)\n"
+"--\n"
+"\n"
+"Check if the record IDs in this array view match with those in other.\n"
+"\n"
+"  other\n"
+"    Another FastqRecordArrayView object.\n"
+);
+
+#define FastqRecordArrayView_is_mate_method METH_O
+static PyObject *
+FastqRecordArrayView_is_mate(FastqRecordArrayView *self, PyObject *other_obj)
+{
+    if (!FastqRecordArrayView_CheckExact(other_obj)) {
+        PyErr_Format(
+            PyExc_TypeError,
+            "other must be of type FastqRecordArrayView, got %s",
+            Py_TYPE(other_obj)->tp_name
+        );
+        return NULL;
+    }
+    FastqRecordArrayView *other = (FastqRecordArrayView *)other_obj;
+    Py_ssize_t length = Py_SIZE(self);
+    if (length != Py_SIZE(other)) {
+        PyErr_Format(
+            PyExc_ValueError,
+            "other is not the same length as this record array view. "
+            "This length: %zd, other length: %zd",
+            length, 
+            Py_SIZE(other)
+        );
+        return NULL;
+    }
+    struct FastqMeta *self_records = self->records;
+    struct FastqMeta *other_records = other->records;
+    for (Py_ssize_t i=0; i<length; i++) {
+        struct FastqMeta *record1 = self_records + i;
+        struct FastqMeta *record2 = other_records + i;
+        char *name1 = (char *)record1->record_start + 1;
+        char *name2 = (char *)record2->record_start + 1;
+        size_t name2_length = record2->name_length;
+        if (!fastq_names_are_mates(name1, name2, name2_length)) {
+            Py_RETURN_FALSE;
+        }
+    }
+    Py_RETURN_TRUE;
+}
+
+static PyMethodDef FastqRecordArrayView_methods[] = {
+    {"is_mate", (PyCFunction)FastqRecordArrayView_is_mate, 
+     FastqRecordArrayView_is_mate_method, FastqRecordArrayView_is_mate__doc__},
+    {NULL},
+};
+
 static PySequenceMethods FastqRecordArrayView_sequence_methods = {
     .sq_item = (ssizeargfunc)FastqRecordArrayView__get_item__,
     .sq_length = (lenfunc)FastqRecordArrayView__length__,
 };
 
 static PyMemberDef FastqRecordArrayView_members[] = {
     {"obj", T_OBJECT, offsetof(FastqRecordArrayView, obj), READONLY,
@@ -650,14 +752,15 @@
     .tp_name = "_qc.FastqRecordArrayView",
     .tp_dealloc = (destructor)FastqRecordArrayView_dealloc,
     .tp_basicsize = sizeof(FastqRecordArrayView),
     .tp_itemsize = sizeof(struct FastqMeta),
     .tp_as_sequence = &FastqRecordArrayView_sequence_methods,
     .tp_new = FastqRecordArrayView__new__,
     .tp_members = FastqRecordArrayView_members,
+    .tp_methods = FastqRecordArrayView_methods,
 };
 
 
 /****************
  * FASTQ PARSER *
  ****************/
 
@@ -721,47 +824,81 @@
 static PyObject *
 FastqParser__iter__(PyObject *self)
 {
     Py_INCREF(self);
     return self;
 }
 
+static inline bool 
+buffer_contains_fastq(const uint8_t *buffer, size_t buffer_size)
+{
+    const uint8_t *buffer_end = buffer + buffer_size;
+    const uint8_t *buffer_pos = buffer;
+    /* Four newlines should be present in a FASTQ record. */
+    for (size_t i=0; i<4;i++) { 
+        buffer_pos = memchr(buffer_pos, '\n', buffer_end - buffer_pos);
+        if (buffer_pos == NULL) {
+            return false;
+        }
+        /* Skip the found newline */
+        buffer_pos += 1;
+    }
+    return true;
+}
+
 static PyObject *
-FastqParser__next__(FastqParser *self) 
+FastqParser_create_record_array(FastqParser *self, size_t min_records, size_t max_records)
 {
     uint8_t *record_start = self->record_start;
     uint8_t *buffer_end = self->buffer_end;
     size_t parsed_records = 0;
     PyObject *new_buffer_obj = NULL;
-    while (parsed_records == 0) {
+    while (parsed_records < min_records) {
         size_t leftover_size = buffer_end - record_start;
         size_t read_in_size;
-        if (leftover_size >= self->read_in_size) {
-        	// A FASTQ record does not fit, enlarge the buffer
-            read_in_size = self->read_in_size;
-        } else {
-        	// Fill up the buffer up to read_in_size
-        	read_in_size = self->read_in_size - leftover_size;
-        }
-        Py_ssize_t new_buffer_size = leftover_size + read_in_size;
+        size_t read_in_offset;
+        Py_ssize_t new_buffer_size;
+        size_t record_start_offset;
         if (new_buffer_obj == NULL) {
+            /* On the first loop create a new buffer and initialize it with 
+               the leftover from the last run of the function. */
+            new_buffer_size = self->read_in_size;
             new_buffer_obj = PyBytes_FromStringAndSize(NULL, new_buffer_size);
             if (new_buffer_obj == NULL) {
                 return NULL;
             }
             memcpy(PyBytes_AS_STRING(new_buffer_obj), record_start, leftover_size);
+        	read_in_size = new_buffer_size - leftover_size;
+            read_in_offset = leftover_size;
+            record_start_offset = 0;
         } else {
+            /* On subsequent loops, enlarge the buffer until the minimum 
+               amount of records fits. */
+            uint8_t *old_start = (uint8_t *)PyBytes_AS_STRING(new_buffer_obj);
+            record_start_offset = record_start - old_start;
+            size_t old_size = buffer_end - old_start;
+            new_buffer_size = old_size + self->read_in_size;
             if (_PyBytes_Resize(&new_buffer_obj, new_buffer_size) == -1) {
                 return NULL;
             }
+            /* Change the already parsed records to point to the new buffer. */
+            uint8_t *new_start = (uint8_t *)PyBytes_AS_STRING(new_buffer_obj);
+            struct FastqMeta *meta_buffer = self->meta_buffer;
+            for (size_t i=0; i < parsed_records; i++) {
+                struct FastqMeta *record = meta_buffer + i;
+                intptr_t record_offset = record->record_start - old_start;
+                record->record_start = new_start + record_offset;
+            }
+            read_in_size = self->read_in_size;
+            read_in_offset = old_size; 
         }
         uint8_t *new_buffer = (uint8_t *)PyBytes_AS_STRING(new_buffer_obj);
 
         PyObject *remaining_space_view = PyMemoryView_FromMemory(
-            (char *)new_buffer + leftover_size, read_in_size, PyBUF_WRITE);
+            (char *)new_buffer + read_in_offset, read_in_size, PyBUF_WRITE);
         if (remaining_space_view == NULL) {
             return NULL;
         }
         PyObject *read_bytes_obj = PyObject_CallMethod(
             self->file_obj, "readinto", "O", remaining_space_view);
         Py_DECREF(remaining_space_view);
         if (read_bytes_obj == NULL) {
@@ -770,55 +907,62 @@
         }
         Py_ssize_t read_bytes = PyLong_AsSsize_t(read_bytes_obj);
         if (read_bytes == -1) {
             Py_DECREF(new_buffer_obj);
             return NULL;
         }
         Py_DECREF(read_bytes_obj);
-        Py_ssize_t actual_buffer_size = leftover_size + read_bytes;
+        Py_ssize_t actual_buffer_size = read_in_offset + read_bytes;
         if (actual_buffer_size < new_buffer_size) {
             if (_PyBytes_Resize(&new_buffer_obj, actual_buffer_size) == -1) {
                 return NULL;
             }
         }
         new_buffer = (uint8_t *)PyBytes_AS_STRING(new_buffer_obj);
         new_buffer_size = actual_buffer_size;
-        if (!string_is_ascii((char *)new_buffer + leftover_size, read_bytes)) {
+        if (!string_is_ascii((char *)new_buffer + read_in_offset, read_bytes)) {
             Py_ssize_t pos;
-            for (pos=leftover_size; pos<new_buffer_size; pos+=1) {
+            for (pos=read_in_offset; pos<new_buffer_size; pos+=1) {
                 if (new_buffer[pos] & ASCII_MASK_1BYTE) {
                     break;
                 }
             }
             PyErr_Format(
                 PyExc_ValueError, 
                 "Found non-ASCII character in file: %c", new_buffer[pos]
             );
             Py_DECREF(new_buffer_obj);
             return NULL;
         }
 
         if (new_buffer_size == 0) {
-            // Entire file is read
-            PyErr_SetNone(PyExc_StopIteration);
-            Py_DECREF(new_buffer_obj);
-            return NULL;
+            // Entire file is read.
+            break;
         } else if (read_bytes == 0) {
-            // Incomplete record at the end of file;
-            PyErr_Format(
-                PyExc_EOFError,
-                "Incomplete record at the end of file %s", 
-                new_buffer);
-            Py_DECREF(new_buffer_obj);
-            return NULL;
+            if (!buffer_contains_fastq(new_buffer, new_buffer_size)) {
+                // Incomplete record at the end of file;
+                PyErr_Format(
+                    PyExc_EOFError,
+                    "Incomplete record at the end of file %s", 
+                    new_buffer);
+                Py_DECREF(new_buffer_obj);
+                return NULL;
+            }
+            if (parsed_records) {
+                /* min_records not yet reached, but file contains no more
+                   records */
+                break;
+            }
+            /* At this point, there are still valid FASTQ records in the buffer 
+               but these have not been parsed yet.*/
         }
-        record_start = new_buffer;
-        buffer_end = record_start + new_buffer_size;
+        record_start = new_buffer + record_start_offset;
+        buffer_end = new_buffer + new_buffer_size;
 
-        while (1) {
+        while (parsed_records < max_records) {
             if (record_start + 2 >= buffer_end) {
                 break;
             }
             if (record_start[0] != '@') {
                 PyErr_Format(
                     PyExc_ValueError,
                     "Record does not start with @ but with %c", 
@@ -892,30 +1036,80 @@
             meta->accumulated_error_rate = 0.0;
             meta->channel=-1;
             meta->duration=0.0;
             meta->start_time=0;
             record_start = qualities_end + 1;
         }
     }
+    /* Save the current buffer object so any leftovers can be reused at the 
+       next invocation. */
     PyObject *tmp = self->buffer_obj;
     self->buffer_obj = new_buffer_obj;
     Py_DECREF(tmp);
+    /* Save record start and buffer end for next invocation. */
     self->record_start = record_start;
     self->buffer_end = buffer_end;
     return FastqRecordArrayView_FromPointerSizeAndObject(
         self->meta_buffer, parsed_records, new_buffer_obj);
 }
 
+static PyObject * 
+FastqParser__next__(FastqParser *self)
+{
+    PyObject *ret = FastqParser_create_record_array(self, 1, SIZE_MAX);
+    if ((ret != NULL) && (Py_SIZE(ret) == 0)) {
+        PyErr_SetNone(PyExc_StopIteration);
+        Py_DECREF(ret);
+        return NULL;
+    }
+    return ret;
+}
+
+
+PyDoc_STRVAR(FastqParser_read__doc__,
+"read($self, number_of_records, /)\n"
+"--\n"
+"\n"
+"Read a number of records into a count array.\n"
+"\n"
+"  Number_of_records\n"
+"    Number_of_records that should be attempted to read.\n"
+);
+
+#define FastqParser_read_method METH_O
+
+static PyObject *
+FastqParser_read(FastqParser *self, PyObject *number_of_records_obj) 
+{
+    Py_ssize_t number_of_records = PyLong_AsSsize_t(number_of_records_obj);
+    if (number_of_records < 1) {
+        PyErr_Format(
+            PyExc_ValueError,
+            "number_of_records should be greater than 1, got %zd",
+            number_of_records
+        );
+        return NULL; 
+    }
+    return FastqParser_create_record_array(self, number_of_records, number_of_records);
+}
+
+static PyMethodDef FastqParser_methods[] = {
+    {"read", (PyCFunction)FastqParser_read, FastqParser_read_method, 
+     FastqParser_read__doc__},
+    {NULL},
+};
+
 PyTypeObject FastqParser_Type = {
     .tp_name = "_qc.FastqParser",
     .tp_basicsize = sizeof(FastqParser),
     .tp_dealloc = (destructor)FastqParser_dealloc,
     .tp_new = FastqParser__new__,
     .tp_iter = (iternextfunc)FastqParser__iter__,
     .tp_iternext = (iternextfunc)FastqParser__next__,
+    .tp_methods = FastqParser_methods,
 };
 
 /**************
  * BAM PARSER *
  * ************/
 
 typedef struct _BamParserStruct {
@@ -1467,24 +1661,33 @@
 QCMetrics_flush_staging(QCMetrics *self) {
     if (self->staging_count == 0) {
         return;
     }
     uint64_t *base_counts = (uint64_t *)self->base_counts;
     uint16_t *staging_base_counts = (uint16_t *)self->staging_base_counts;
     size_t number_of_base_slots = self->max_length * NUC_TABLE_SIZE;
+    /* base counts is only updated once every 65535 times. So make sure it 
+       does not pollute the cache and use non temporal prefetching. The 
+       same goes for phred counts.
+    */
+    non_temporal_prefetch(base_counts);
     for (size_t i=0; i < number_of_base_slots; i++) {
         base_counts[i] += staging_base_counts[i];
+        /* Fetch the next 64 byte cache line non-temporal. */
+        non_temporal_prefetch(base_counts + i + 8);
     }
     memset(staging_base_counts, 0, number_of_base_slots * sizeof(uint16_t));
 
     uint64_t *phred_counts = (uint64_t *)self->phred_counts;
     uint16_t *staging_phred_counts = (uint16_t *)self->staging_phred_counts;
     size_t number_of_phred_slots = self->max_length * PHRED_TABLE_SIZE;
+    non_temporal_prefetch(phred_counts);
     for (size_t i=0; i < number_of_phred_slots; i++) {
         phred_counts[i] += staging_phred_counts[i];
+        non_temporal_prefetch(phred_counts + i + 8);
     }
     memset(staging_phred_counts, 0, number_of_phred_slots * sizeof(uint16_t));
 
     self->staging_count = 0;
 }
 
 #ifdef __SSE2__
@@ -3602,39 +3805,20 @@
     self->hash_table = new_hash_table;
     self->modulo_bits = next_modulo_bits;
     self->stored_entries = new_stored_entries;
     PyMem_Free(tmp);
     return 0;
 }
 
-static int 
-DedupEstimator_add_sequence_ptr(DedupEstimator *self, 
-                               uint8_t *sequence, size_t sequence_length) 
+static int DedupEstimator_add_fingerprint(DedupEstimator *self, 
+                                          uint8_t *fingerprint, 
+                                          size_t fingerprint_length, 
+                                          uint64_t seed) 
 {
-
-    uint64_t hash;
-    size_t front_sequence_length = self->front_sequence_length;
-    size_t back_sequence_length = self->back_sequence_length;
-    size_t front_sequence_offset = self->front_sequence_offset;
-    size_t back_sequence_offset = self->back_sequence_offset;
-    size_t fingerprint_length = front_sequence_length + back_sequence_length;
-    uint8_t *fingerprint = self->fingerprint_store;
-    if (sequence_length <= fingerprint_length) {
-        hash = MurmurHash3_x64_64(sequence, sequence_length, 0);
-    } else {
-        uint64_t seed = sequence_length >> 6;
-        size_t remainder = sequence_length - fingerprint_length;
-        size_t front_offset = Py_MIN(remainder / 2, front_sequence_offset);
-        size_t back_offset = Py_MIN(remainder / 2, back_sequence_offset);
-        memcpy(fingerprint, sequence + front_offset, front_sequence_length);
-        memcpy(fingerprint + front_sequence_length, 
-               sequence + sequence_length - (back_offset + back_sequence_length), 
-               back_sequence_length);
-        hash = MurmurHash3_x64_64(fingerprint, fingerprint_length, seed);
-    }
+    uint64_t hash = MurmurHash3_x64_64(fingerprint, fingerprint_length, seed);
     size_t modulo_bits = self->modulo_bits;
     size_t ignore_mask = (1ULL << modulo_bits) - 1;
     if (hash & ignore_mask) {
         return 0;
     }
     size_t hash_table_size = self->hash_table_size;
     if (self->stored_entries >= self->max_stored_entries) {
@@ -3659,14 +3843,72 @@
         }
         index += 1; 
         index &= index_mask;
     }
     return 0;
 }
 
+static int 
+DedupEstimator_add_sequence_ptr(DedupEstimator *self, 
+                               uint8_t *sequence, size_t sequence_length) 
+{
+    size_t front_sequence_length = self->front_sequence_length;
+    size_t back_sequence_length = self->back_sequence_length;
+    size_t front_sequence_offset = self->front_sequence_offset;
+    size_t back_sequence_offset = self->back_sequence_offset;
+    size_t fingerprint_length = front_sequence_length + back_sequence_length;
+    uint8_t *fingerprint = self->fingerprint_store;
+    if (sequence_length <= fingerprint_length) {
+        return DedupEstimator_add_fingerprint(self, sequence, sequence_length, 0);
+    } 
+    uint64_t seed = sequence_length >> 6;
+    size_t remainder = sequence_length - fingerprint_length;
+    size_t front_offset = Py_MIN(remainder / 2, front_sequence_offset);
+    size_t back_offset = Py_MIN(remainder / 2, back_sequence_offset);
+    memcpy(fingerprint, sequence + front_offset, front_sequence_length);
+    memcpy(fingerprint + front_sequence_length, 
+            sequence + sequence_length - (back_offset + back_sequence_length), 
+            back_sequence_length);
+    return DedupEstimator_add_fingerprint(self, fingerprint, fingerprint_length, seed);
+}
+
+static int 
+DedupEstimator_add_sequence_pair_ptr(
+    DedupEstimator *self, 
+    uint8_t *sequence1, 
+    Py_ssize_t sequence_length1,
+    uint8_t *sequence2, 
+    Py_ssize_t sequence_length2
+) 
+{
+    Py_ssize_t front_sequence_length = self->front_sequence_length;
+    Py_ssize_t back_sequence_length = self->back_sequence_length;
+    Py_ssize_t front_sequence_offset = self->front_sequence_offset;
+    Py_ssize_t back_sequence_offset = self->back_sequence_offset;
+    Py_ssize_t fingerprint_length = front_sequence_length + back_sequence_length;
+    uint8_t *fingerprint = self->fingerprint_store;
+    uint64_t seed = (sequence_length1 + sequence_length2) >> 6;
+    
+    // Ensure not more sequence is taken than available. 
+    front_sequence_length = Py_MIN(front_sequence_length, sequence_length1);
+    // Ensure that the offset is not beyond the length of the sequence.
+    Py_ssize_t front_offset = Py_MIN(
+        front_sequence_offset, (sequence_length1 - front_sequence_length));
+    // Same guarantees for sequence 2.
+    back_sequence_length = Py_MIN(back_sequence_length, sequence_length2);
+    Py_ssize_t back_offset = Py_MIN(
+        back_sequence_offset, (sequence_length2 - back_sequence_length));
+    
+    memcpy(fingerprint, sequence1 + front_offset, front_sequence_length);
+    memcpy(fingerprint + front_sequence_length, sequence2 + back_offset, 
+           back_sequence_length);
+    return DedupEstimator_add_fingerprint(self, fingerprint, fingerprint_length, seed);
+}
+
+
 PyDoc_STRVAR(DedupEstimator_add_record_array__doc__,
 "add_record_array($self, record_array, /)\n"
 "--\n"
 "\n"
 "Add a record_array to the deduplication estimator. \n"
 "\n"
 "  record_array\n"
@@ -3693,14 +3935,83 @@
         if (DedupEstimator_add_sequence_ptr(self, sequence, sequence_length) != 0) {
             return NULL;
         }
     }
     Py_RETURN_NONE;
 }
 
+
+PyDoc_STRVAR(DedupEstimator_add_record_array_pair__doc__,
+"add_record_array_pair($self, record_array1, record_array2 /)\n"
+"--\n"
+"\n"
+"Add a pair of record arrays to the deduplication estimator. \n"
+"\n"
+"  record_array1\n"
+"    A FastqRecordArrayView object. First of read pair.\n"
+"  record_array2\n"
+"    A FastqRecordArrayView object. Second of read pair.\n"
+);
+
+#define DedupEstimator_add_record_array_pair_method METH_FASTCALL
+
+static PyObject *
+DedupEstimator_add_record_array_pair(DedupEstimator *self, PyObject *const *args, Py_ssize_t nargs) 
+{
+    if (nargs != 2) {
+        PyErr_Format(PyExc_TypeError, 
+                     "Dedupestimatorr.add_record_array_pair() "
+                     "takes exactly two arguments (%zd given)", 
+                     nargs);
+    }
+    FastqRecordArrayView *record_array1 = (FastqRecordArrayView *)args[0];
+    FastqRecordArrayView *record_array2 = (FastqRecordArrayView *)args[1];
+    if (!FastqRecordArrayView_CheckExact(record_array1)) {
+        PyErr_Format(
+            PyExc_TypeError, 
+            "record_array1 should be a FastqRecordArrayView object, got %s", 
+            Py_TYPE(record_array1)->tp_name
+        );
+        return NULL;
+    }    
+    if (!FastqRecordArrayView_CheckExact(record_array2)) {
+        PyErr_Format(
+            PyExc_TypeError, 
+            "record_array2 should be a FastqRecordArrayView object, got %s", 
+            Py_TYPE(record_array2)->tp_name
+        );
+        return NULL;
+    }
+    Py_ssize_t number_of_records = Py_SIZE(record_array1);
+    if (Py_SIZE(record_array2) != number_of_records) {
+        PyErr_Format(
+            PyExc_ValueError, 
+            "record_array1 and record_array2 must be of the same size. "
+            "Got %zd and %zd respectively.", 
+            number_of_records, Py_SIZE(record_array2)
+        );
+    }
+    struct FastqMeta *records1 = record_array1->records;
+    struct FastqMeta *records2 = record_array2->records;
+    for (Py_ssize_t i=0; i < number_of_records; i++) {
+        struct FastqMeta *meta1 = records1 + i;
+        struct FastqMeta *meta2 = records2 + i; 
+        uint8_t *sequence1 = meta1->record_start + meta1->sequence_offset;
+        uint8_t *sequence2 = meta2->record_start + meta2->sequence_offset;
+        size_t sequence_length1 = meta1->sequence_length; 
+        size_t sequence_length2 = meta2->sequence_length; 
+        int ret = DedupEstimator_add_sequence_pair_ptr(
+            self, sequence1, sequence_length1, sequence2, sequence_length2);
+        if (ret != 0) {
+            return NULL;
+        }
+    }
+    Py_RETURN_NONE;
+}
+
 PyDoc_STRVAR(DedupEstimator_add_sequence__doc__,
 "add_sequence($self, sequence, /)\n"
 "--\n"
 "\n"
 "Add a sequence to the deduplication estimator. \n"
 "\n"
 "  sequence\n"
@@ -3728,14 +4039,59 @@
             self, PyUnicode_DATA(sequence), PyUnicode_GET_LENGTH(sequence)) != 0) {
         return NULL;
     }
     Py_RETURN_NONE;
 }
 
 
+PyDoc_STRVAR(DedupEstimator_add_sequence_pair__doc__,
+"add__paired_sequence($self, sequence1, sequence2, /)\n"
+"--\n"
+"\n"
+"Add a paired sequence to the deduplication estimator. \n"
+"\n"
+"  sequence1\n"
+"    An ASCII string.\n"
+"  sequence2\n"
+"    An ASCII string.\n"
+);
+
+#define DedupEstimator_add_sequence_pair_method METH_VARARGS
+
+static PyObject *
+DedupEstimator_add_sequence_pair(DedupEstimator *self, PyObject *args) 
+{
+    PyObject *sequence1_obj = NULL; 
+    PyObject *sequence2_obj = NULL; 
+    if (!PyArg_ParseTuple(args, "UU|:add_sequence_pair", &sequence1_obj, &sequence2_obj)) {
+        return NULL;
+    }
+    if (!PyUnicode_IS_COMPACT_ASCII(sequence1_obj)) {
+        PyErr_SetString(
+            PyExc_ValueError, 
+            "sequence should consist only of ASCII characters.");
+        return NULL;
+    }
+    if (!PyUnicode_IS_COMPACT_ASCII(sequence2_obj)) {
+        PyErr_SetString(
+            PyExc_ValueError, 
+            "sequence should consist only of ASCII characters.");
+        return NULL;
+    }
+    uint8_t *sequence1 = PyUnicode_DATA(sequence1_obj);
+    uint8_t *sequence2 = PyUnicode_DATA(sequence2_obj);
+    Py_ssize_t sequence1_length = PyUnicode_GET_LENGTH(sequence1_obj);
+    Py_ssize_t sequence2_length = PyUnicode_GET_LENGTH(sequence2_obj);
+    if (DedupEstimator_add_sequence_pair_ptr(
+        self, sequence1, sequence1_length, sequence2, sequence2_length) != 0) {
+            return NULL;
+        }
+    Py_RETURN_NONE;
+}
+
 PyDoc_STRVAR(DedupEstimator_duplication_counts__doc__,
 "duplication_counts($self)\n"
 "--\n"
 "\n"
 "Return a array.array with only the counts. \n"
 );
 
@@ -3765,16 +4121,22 @@
     PyMem_Free(counts);
     return result;
 } 
 
 static PyMethodDef DedupEstimator_methods[] = {
     {"add_record_array", (PyCFunction)DedupEstimator_add_record_array, 
      DedupEstimator_add_record_array_method, DedupEstimator_add_record_array__doc__},
+    {"add_record_array_pair", (PyCFunction)DedupEstimator_add_record_array_pair, 
+     DedupEstimator_add_record_array_pair_method, 
+     DedupEstimator_add_record_array_pair__doc__},
     {"add_sequence", (PyCFunction)DedupEstimator_add_sequence, 
      DedupEstimator_add_sequence_method, DedupEstimator_add_sequence__doc__},
+    {"add_sequence_pair", (PyCFunction)DedupEstimator_add_sequence_pair, 
+     DedupEstimator_add_sequence_pair_method, 
+     DedupEstimator_add_sequence_pair__doc__},
     {"duplication_counts", (PyCFunction)DedupEstimator_duplication_counts, 
      DedupEstimator_duplication_counts_method, DedupEstimator_duplication_counts__doc__},
     {NULL},
 };
 
 static PyMemberDef DedupEstimator_members[] = {
     {"_modulo_bits", T_ULONGLONG, offsetof(DedupEstimator, modulo_bits), 
@@ -4186,14 +4548,525 @@
     .tp_basicsize = sizeof(NanoStats),
     .tp_dealloc = (destructor)NanoStats_dealloc,
     .tp_new = (newfunc)NanoStats__new__, 
     .tp_methods = NanoStats_methods,
     .tp_members = NanoStats_members,
 };
 
+/***********************
+ * INSERT SIZE METRICS * 
+ ***********************/
+
+#define INSERT_SIZE_MAX_ADAPTERS 10000
+#define INSERT_SIZE_MAX_ADAPTER_STORE_SIZE 31
+
+struct AdapterTableEntry {
+    uint64_t hash;
+    uint64_t adapter_count; 
+    uint8_t adapter_length; 
+    uint8_t adapter[INSERT_SIZE_MAX_ADAPTER_STORE_SIZE];
+};
+
+typedef struct _InsertSizeMetricsStruct {
+    PyObject_HEAD 
+    uint64_t *insert_sizes;
+    uint64_t total_reads;
+    uint64_t number_of_adapters_read1;
+    uint64_t number_of_adapters_read2;
+    struct AdapterTableEntry *hash_table_read1;
+    struct AdapterTableEntry *hash_table_read2; 
+    size_t max_adapters;
+    size_t hash_table_size;
+    size_t hash_table_read1_entries;
+    size_t hash_table_read2_entries;
+    size_t max_insert_size; 
+} InsertSizeMetrics;
+
+static void
+InsertSizeMetrics_dealloc(InsertSizeMetrics *self) {
+    PyMem_Free(self->hash_table_read1);
+    PyMem_Free(self->hash_table_read2); 
+    PyMem_Free(self->insert_sizes);
+    Py_TYPE(self)->tp_free(self);
+}
+
+static PyMemberDef InsertSizeMetrics_members[] = {
+    {"total_reads", T_ULONGLONG, offsetof(InsertSizeMetrics, total_reads), 
+     READONLY, "the total number of reads"},
+    {"number_of_adapters_read1", T_ULONGLONG, 
+      offsetof(InsertSizeMetrics, number_of_adapters_read1), READONLY, 
+      "The number off reads in read 1 with an adapter."},
+    {"number_of_adapters_read2", T_ULONGLONG, 
+      offsetof(InsertSizeMetrics, number_of_adapters_read2), READONLY, 
+      "The number off reads in read 2 with an adapter."},
+    {NULL},
+};
+
+static PyObject *
+InsertSizeMetrics__new__(PyTypeObject *type, PyObject *args, PyObject *kwargs) 
+{
+    Py_ssize_t max_adapters = INSERT_SIZE_MAX_ADAPTERS;
+    static char *format = "|n:InsertSizeMetrics.__new__";
+    static char *keywords[] = {"max_adapters", NULL};
+    if (!PyArg_ParseTupleAndKeywords(
+        args, kwargs, format, keywords, &max_adapters
+    )) {
+        return NULL;
+    }
+
+    if (max_adapters < 1) {
+        PyErr_Format(
+            PyExc_ValueError,
+            "max_adapters must be at least 1, got %zd", 
+            max_adapters
+        );
+        return NULL;
+    }
+
+    InsertSizeMetrics *self = PyObject_New(InsertSizeMetrics, type);
+    if (self == NULL) {
+        return PyErr_NoMemory();
+    }
+    size_t hash_table_bits = (size_t)(log2(max_adapters * 1.5) + 1);
+
+    self->max_adapters = max_adapters;
+    self->max_insert_size = 300;
+    self->hash_table_read1_entries = 0;
+    self->hash_table_read2_entries = 0;
+    self->hash_table_size = 1 << hash_table_bits; 
+    self->hash_table_read1 = PyMem_Calloc(self->hash_table_size, 
+                                          sizeof(struct AdapterTableEntry));
+    self->hash_table_read2 = PyMem_Calloc(self->hash_table_size, 
+                                          sizeof(struct AdapterTableEntry));
+    self->insert_sizes = PyMem_Calloc(self->max_insert_size + 1, sizeof(uint64_t));
+    self->total_reads = 0;
+    self->number_of_adapters_read1 = 0;
+    self->number_of_adapters_read2 = 0;
+
+    if (self->hash_table_read1 == NULL || self->hash_table_read2 == NULL || 
+            self->insert_sizes == NULL) {
+        /* Memory gets freed in the dealloc method. */
+        Py_DECREF(self);
+        return PyErr_NoMemory();
+    }
+    return (PyObject *)self;
+}
+
+static int 
+InsertSizeMetrics_resize(InsertSizeMetrics *self, size_t new_size)
+{
+    if (new_size <= self->max_insert_size) {
+        return 0;
+    }
+    size_t old_size = self->max_insert_size;
+    size_t new_raw_size = sizeof(uint64_t) * (new_size + 1);
+    uint64_t *tmp = PyMem_Realloc(self->insert_sizes, new_raw_size);
+    if (tmp == NULL) {
+        PyErr_NoMemory();
+        return -1;
+    }
+    memset(tmp + old_size, 0, (new_size - old_size) * sizeof(uint64_t));
+    self->max_insert_size = new_size;
+    self->insert_sizes = tmp;
+    return 0;
+}
+
+static inline void 
+InsertSizeMetrics_add_adapter(
+    InsertSizeMetrics *self, const uint8_t *adapter, size_t adapter_length, bool read2)
+{
+    assert(adapter_length <= INSERT_SIZE_MAX_ADAPTER_STORE_SIZE);
+    uint64_t hash = MurmurHash3_x64_64(adapter, adapter_length, 0);
+    size_t hash_table_size = self->hash_table_size;
+    struct AdapterTableEntry *hash_table = self->hash_table_read1;
+    size_t *current_entries = &self->hash_table_read1_entries;
+    if (read2) {
+        hash_table = self->hash_table_read2;
+        current_entries = &self->hash_table_read2_entries;
+    }
+    bool hash_table_full = *current_entries == self->max_adapters;  
+
+    size_t hash_to_index_int = hash_table_size - 1;  // Works because size is a power of 2.
+    size_t index = hash & hash_to_index_int;
+    while (true) {
+        struct AdapterTableEntry *entry = hash_table + index; 
+        uint64_t current_hash = entry->hash; 
+        if (current_hash == hash) {
+            if (adapter_length == entry->adapter_length && 
+                memcmp(adapter, entry->adapter, adapter_length) == 0) {
+                entry->adapter_count += 1;
+                return;
+            }
+        }
+        else if (entry->adapter_count == 0) {
+            if (!hash_table_full) {
+                entry->hash = hash;
+                entry->adapter_length = adapter_length;
+                memcpy(entry->adapter, adapter, adapter_length);
+                entry->adapter_count = 1;
+                current_entries[0] += 1;
+            }
+            return;
+        } 
+        index += 1;
+        index &= hash_to_index_int;
+    }
+}
+
+static const uint8_t NUCLEOTIDE_COMPLEMENT[128] = {
+// All non-ACGT become 0 so they don't match with N.
+// Control characters
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+// Interpunction numbers etc
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+//      A,  B,  C,  D, E, F,  G,  H, I, J, K, L, M, N, O,
+    0, 'T', 0, 'G', 0, 0, 0, 'C', 0, 0, 0, 0, 0, 0, 0, 0,
+//  P, Q, R, S,  T,  U,  V, W, X, Y, Z,  
+    0, 0, 0, 0, 'A', 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+//      a,  b,  c,  d, e, f,  g,  h, i, j, k, l, m, n, o,
+    0, 'T', 0, 'G', 0, 0, 0, 'C', 0, 0, 0, 0, 0, 0, 0, 0,
+//  p, q, r, s,  t,  u,  v, w, x, y, z, 
+    0, 0, 0, 0, 'A', 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 
+};
+
+static inline void 
+reverse_complement(uint8_t *restrict dest, const uint8_t *restrict src, size_t length) 
+{
+    size_t dest_index = length;
+    for (size_t src_index=0; src_index<length; src_index++) {
+        dest_index -= 1; 
+        dest[dest_index] = NUCLEOTIDE_COMPLEMENT[src[src_index]];
+    }
+}
+
+static inline size_t 
+hamming_distance(const uint8_t *restrict sequence1, 
+                 const uint8_t *restrict sequence2, 
+                 size_t length)
+{
+    size_t distance = 0;
+    for (size_t i=0; i<length; i++) {
+        if (sequence1[i] != sequence2[i]) {
+            distance += 1;
+        }
+    }
+    return distance;
+}
+
+/* Everything set except the bit for 32. This is the difference in ASCII 
+   between lowercase and uppercase. */
+
+#define UPPER_MASK 0xDFDFDFDFDFDFDFDFULL
+
+/**
+ * @brief Determine insert size between sequences by calculating the overlap.
+ * 
+ * @return Py_ssize_t 0, when no overlap could be determined.
+ */
+static size_t 
+calculate_insert_size(const uint8_t *restrict sequence1, 
+                      size_t sequence1_length,
+                      const uint8_t *restrict sequence2, 
+                      size_t sequence2_length) 
+{
+    /* The needle size is 16. One error is allowed. By hardcoding is it can 
+       be optimized by looking for 2 64-bit integers instead. At least one of 
+       the 64-bit integers must find a match at a position if there is only one 
+       error. This is the pigeon hole principle. This way the sequence can be
+       searched quickly, while allowing errors. */
+ 
+    if (sequence2_length < 16 || sequence1_length < 16) {
+        return 0;
+    }
+    uint8_t seq_store[32];
+    uint8_t *start_seq = seq_store;
+    uint8_t *end_seq = ((uint8_t *)seq_store) + 16;
+    reverse_complement(start_seq, sequence2, 16);
+    reverse_complement(end_seq, sequence2 + sequence2_length - 16, 16);
+
+    uint64_t start1 = ((uint64_t *)start_seq)[0];
+    uint64_t start2 = ((uint64_t *)start_seq)[1];
+    uint64_t end1 = ((uint64_t *)end_seq)[0];
+    uint64_t end2 = ((uint64_t *)end_seq)[1];
+
+    size_t run_length = sequence1_length - 15;
+    for(size_t i=0; i<run_length; i++) {
+        uint64_t word1 = ((uint64_t *)(sequence1 + i))[0] & UPPER_MASK;
+        uint64_t word2 = ((uint64_t *)(sequence1 + i))[1] & UPPER_MASK;
+        if (start1 == word1 || start2 == word2) {
+            if (hamming_distance(sequence1 + i, start_seq, 16) <= 1) {
+                return i + 16;
+            }
+        }
+        if (end1 == word1 || end2 == word2) {
+            if (hamming_distance(sequence1 + i, end_seq, 16) <= 1) {
+                return i + sequence2_length;
+            }
+        }
+    }
+    return 0;  // No matches found.
+}
+
+static int InsertSizeMetrics_add_sequence_pair_ptr(
+    InsertSizeMetrics *self, const uint8_t *sequence1, size_t sequence1_length, 
+    const uint8_t *sequence2, size_t sequence2_length)
+{
+    
+    size_t insert_size = calculate_insert_size(sequence1, sequence1_length, 
+                                               sequence2, sequence2_length);
+    if (insert_size > self->max_insert_size) {
+        if (InsertSizeMetrics_resize(self, insert_size) != 0) {
+            return -1;
+        };
+    }
+    self->total_reads += 1;
+    self->insert_sizes[insert_size] += 1;
+    /* Don't store adapters when no overlap is detected. */
+    if ((insert_size) == 0) {
+        return 0;
+    }
+    Py_ssize_t remainder1 = (Py_ssize_t)sequence1_length - (Py_ssize_t)insert_size;
+    if (remainder1 > 0) {
+        self->number_of_adapters_read1 += 1;
+        InsertSizeMetrics_add_adapter(
+            self, sequence1 + insert_size, 
+            Py_MIN(remainder1, INSERT_SIZE_MAX_ADAPTER_STORE_SIZE), false);
+    }
+    Py_ssize_t remainder2 = (Py_ssize_t)sequence2_length - (Py_ssize_t)insert_size;
+    if (remainder2 > 0) {
+        self->number_of_adapters_read2 += 1;
+        InsertSizeMetrics_add_adapter(
+            self, sequence2 + insert_size, 
+            Py_MIN(remainder2, INSERT_SIZE_MAX_ADAPTER_STORE_SIZE), true);
+    }
+    return 0;
+}
+
+PyDoc_STRVAR(InsertSizeMetrics_add_sequence_pair__doc__,
+"add_sequence_pair($self, sequence1, sequence2, /)\n"
+"--\n"
+"\n"
+"Add a paired sequence to the insert size metrics. \n"
+"\n"
+"  sequence1\n"
+"    An ASCII string.\n"
+"  sequence2\n"
+"    An ASCII string.\n"
+);
+
+#define InsertSizeMetrics_add_sequence_pair_method METH_VARARGS
+
+static PyObject *
+InsertSizeMetrics_add_sequence_pair(InsertSizeMetrics *self, PyObject *args)
+{
+    PyObject *sequence1_obj = NULL;
+    PyObject *sequence2_obj = NULL;
+    if (!PyArg_ParseTuple(
+        args, "UU|:InsertSizeMetrics.add_sequence_pair", 
+        &sequence1_obj, &sequence2_obj)) {
+            return NULL;
+        }
+    if (!PyUnicode_IS_COMPACT_ASCII(sequence1_obj) || 
+        !PyUnicode_IS_COMPACT_ASCII(sequence2_obj)) {
+        PyErr_SetString(
+            PyExc_ValueError, "Both sequences must be ASCII strings.");
+        return NULL;
+    }
+    int ret = InsertSizeMetrics_add_sequence_pair_ptr(
+        self, 
+        PyUnicode_DATA(sequence1_obj),
+        PyUnicode_GET_LENGTH(sequence1_obj),
+        PyUnicode_DATA(sequence2_obj), 
+        PyUnicode_GET_LENGTH(sequence2_obj)
+    );
+    if (ret != 0) {
+        return NULL;
+    }
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(InsertSizeMetrics_add_record_array_pair__doc__,
+"add_record_array_pair($self, record_array1, record_array2 /)\n"
+"--\n"
+"\n"
+"Add a pair of record arrays to the insert size metrics. \n"
+"\n"
+"  record_array1\n"
+"    A FastqRecordArrayView object. First of read pair.\n"
+"  record_array2\n"
+"    A FastqRecordArrayView object. Second of read pair.\n"
+);
+
+#define InsertSizeMetrics_add_record_array_pair_method METH_FASTCALL
+
+static PyObject *
+InsertSizeMetrics_add_record_array_pair(
+    InsertSizeMetrics *self, PyObject *const *args, Py_ssize_t nargs) 
+{
+    if (nargs != 2) {
+        PyErr_Format(PyExc_TypeError, 
+                     "InsertSizeMetrics.add_record_array_pair() "
+                     "takes exactly two arguments, got %zd", 
+                      nargs);
+    }
+    FastqRecordArrayView *record_array1 = (FastqRecordArrayView *)args[0];
+    FastqRecordArrayView *record_array2 = (FastqRecordArrayView *)args[1];
+    if (!FastqRecordArrayView_CheckExact(record_array1)) {
+        PyErr_Format(
+            PyExc_TypeError, 
+            "record_array1 should be a FastqRecordArrayView object, got %s", 
+            Py_TYPE(record_array1)->tp_name
+        );
+        return NULL;
+    }    
+    if (!FastqRecordArrayView_CheckExact(record_array2)) {
+        PyErr_Format(
+            PyExc_TypeError, 
+            "record_array2 should be a FastqRecordArrayView object, got %s", 
+            Py_TYPE(record_array2)->tp_name
+        );
+        return NULL;
+    }
+    Py_ssize_t number_of_records = Py_SIZE(record_array1);
+    if (Py_SIZE(record_array2) != number_of_records) {
+        PyErr_Format(
+            PyExc_ValueError, 
+            "record_array1 and record_array2 must be of the same size. "
+            "Got %zd and %zd respectively.", 
+            number_of_records, Py_SIZE(record_array2)
+        );
+    }
+    struct FastqMeta *records1 = record_array1->records;
+    struct FastqMeta *records2 = record_array2->records;
+    for (Py_ssize_t i=0; i < number_of_records; i++) {
+        struct FastqMeta *meta1 = records1 + i;
+        struct FastqMeta *meta2 = records2 + i; 
+        uint8_t *sequence1 = meta1->record_start + meta1->sequence_offset;
+        uint8_t *sequence2 = meta2->record_start + meta2->sequence_offset;
+        size_t sequence_length1 = meta1->sequence_length; 
+        size_t sequence_length2 = meta2->sequence_length; 
+        int ret = InsertSizeMetrics_add_sequence_pair_ptr(
+            self, sequence1, sequence_length1, sequence2, sequence_length2);
+        if (ret != 0) {
+            return NULL;
+        }
+    }
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(InsertSizeMetrics_insert_sizes__doc__,
+"insert_sizes($self)\n"
+"--\n"
+"\n"
+"Retrieve an array of the insert sizes.\n"
+);
+
+#define InsertSizeMetrics_insert_sizes_method METH_NOARGS
+
+static PyObject *
+InsertSizeMetrics_insert_sizes(InsertSizeMetrics *self, PyObject *Py_UNUSED(ignore))
+{
+    return PythonArray_FromBuffer('Q', self->insert_sizes, 
+        (self->max_insert_size + 1) * sizeof(uint64_t));
+}
+
+static PyObject *adapter_hash_table_to_python_list(
+    struct AdapterTableEntry *hash_table, size_t hash_table_size)
+{
+    PyObject *adapter_list = PyList_New(0);
+    struct AdapterTableEntry *entries = hash_table;
+    for (size_t i=0; i<hash_table_size; i++) {
+        struct AdapterTableEntry *entry = entries + i; 
+        uint64_t adapter_count = entry->adapter_count;
+        if (adapter_count) {
+            PyObject *adapter_tuple = Py_BuildValue(
+                "(s#K)", 
+                entry->adapter, 
+                (Py_ssize_t)entry->adapter_length,
+                adapter_count
+            );
+            if (adapter_tuple == NULL) {
+                Py_DECREF(adapter_list);
+                return NULL;
+            }
+            if (PyList_Append(adapter_list, adapter_tuple) != 0) {
+                return NULL;
+            }
+            Py_DECREF(adapter_tuple);
+        }
+    }
+    return adapter_list;
+}
+
+PyDoc_STRVAR(InsertSizeMetrics_adapters_read1__doc__,
+"adapters_read1($self)\n"
+"--\n"
+"\n"
+"Retrieve a list of adapters for read 1 with their counts.\n"
+);
+
+#define InsertSizeMetrics_adapters_read1_method METH_NOARGS
+
+static PyObject *
+InsertSizeMetrics_adapters_read1(InsertSizeMetrics *self, PyObject *Py_UNUSED(ignore))
+{
+    return adapter_hash_table_to_python_list(
+        self->hash_table_read1, self->hash_table_size);
+}
+
+PyDoc_STRVAR(InsertSizeMetrics_adapters_read2__doc__,
+"adapters_read2($self)\n"
+"--\n"
+"\n"
+"Retrieve a list of adapters for read 2 with their counts.\n"
+);
+
+#define InsertSizeMetrics_adapters_read2_method METH_NOARGS
+
+static PyObject *
+InsertSizeMetrics_adapters_read2(InsertSizeMetrics *self, PyObject *Py_UNUSED(ignore))
+{
+    return adapter_hash_table_to_python_list(
+        self->hash_table_read2, self->hash_table_size);
+}
+
+static PyMethodDef InsertSizeMetrics_methods[] = {
+    {"add_sequence_pair", (PyCFunction)InsertSizeMetrics_add_sequence_pair, 
+     InsertSizeMetrics_add_sequence_pair_method, 
+     InsertSizeMetrics_add_sequence_pair__doc__},
+    {"add_record_array_pair", 
+     (PyCFunction)InsertSizeMetrics_add_record_array_pair,
+     InsertSizeMetrics_add_record_array_pair_method,
+     InsertSizeMetrics_add_record_array_pair__doc__,
+    },
+    {"insert_sizes", (PyCFunction)InsertSizeMetrics_insert_sizes, 
+     InsertSizeMetrics_insert_sizes_method, 
+     InsertSizeMetrics_insert_sizes__doc__},
+    {"adapters_read1", (PyCFunction)InsertSizeMetrics_adapters_read1,
+     InsertSizeMetrics_adapters_read1_method, 
+     InsertSizeMetrics_adapters_read1__doc__},
+    {"adapters_read2", (PyCFunction)InsertSizeMetrics_adapters_read2,
+     InsertSizeMetrics_adapters_read2_method, 
+     InsertSizeMetrics_adapters_read2__doc__},
+
+    {NULL},
+};
+
+static PyTypeObject InsertSizeMetrics_Type = {
+    .tp_name = "_qc.InsertSizeMetrics",
+    .tp_basicsize = sizeof(InsertSizeMetrics),
+    .tp_dealloc = (destructor)InsertSizeMetrics_dealloc,
+    .tp_flags= Py_TPFLAGS_DEFAULT,
+    .tp_new = InsertSizeMetrics__new__,
+    .tp_methods = InsertSizeMetrics_methods,
+    .tp_members = InsertSizeMetrics_members,
+};
+
 /*************************
  * MODULE INITIALIZATION *
  *************************/
 
 
 static struct PyModuleDef _qc_module = {
     PyModuleDef_HEAD_INIT,
@@ -4292,14 +5165,17 @@
     if (python_module_add_type(m, &NanoStats_Type) != 0) {
         return NULL;
     }
     if (python_module_add_type(m, &NanoStatsIterator_Type) != 0) {
         return NULL;
     }
 
+    if (python_module_add_type(m, &InsertSizeMetrics_Type) != 0) {
+        return NULL;
+    }
     PyModule_AddIntConstant(m, "NUMBER_OF_NUCS", NUC_TABLE_SIZE);
     PyModule_AddIntConstant(m, "NUMBER_OF_PHREDS", PHRED_TABLE_SIZE);
     PyModule_AddIntConstant(m, "TABLE_SIZE", PHRED_TABLE_SIZE * NUC_TABLE_SIZE);
     PyModule_AddIntMacro(m, A);
     PyModule_AddIntMacro(m, C);
     PyModule_AddIntMacro(m, G);
     PyModule_AddIntMacro(m, T);
@@ -4310,9 +5186,10 @@
     PyModule_AddIntMacro(m, DEFAULT_DEDUP_MAX_STORED_FINGERPRINTS);
     PyModule_AddIntMacro(m, DEFAULT_FRAGMENT_LENGTH);
     PyModule_AddIntMacro(m, DEFAULT_UNIQUE_SAMPLE_EVERY);
     PyModule_AddIntMacro(m, DEFAULT_FINGERPRINT_FRONT_SEQUENCE_LENGTH);
     PyModule_AddIntMacro(m, DEFAULT_FINGERPRINT_BACK_SEQUENCE_LENGTH);
     PyModule_AddIntMacro(m, DEFAULT_FINGERPRINT_FRONT_SEQUENCE_OFFSET);
     PyModule_AddIntMacro(m, DEFAULT_FINGERPRINT_BACK_SEQUENCE_OFFSET);
+    PyModule_AddIntMacro(m, INSERT_SIZE_MAX_ADAPTER_STORE_SIZE);
     return m;
 }
```

### Comparing `sequali-0.7.1/src/sequali/adapters/adapter_list.tsv` & `sequali-0.8.0/src/sequali/adapters/adapter_list.tsv`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/adapters.py` & `sequali-0.8.0/src/sequali/adapters.py`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/contaminants/README` & `sequali-0.8.0/src/sequali/contaminants/README`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/contaminants/UniVec.fasta` & `sequali-0.8.0/src/sequali/contaminants/UniVec.fasta`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/contaminants/oxford_nanopore.fasta` & `sequali-0.8.0/src/sequali/contaminants/oxford_nanopore.fasta`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/contaminants/oxford_nanopore_barcodes.fasta` & `sequali-0.8.0/src/sequali/contaminants/oxford_nanopore_barcodes.fasta`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/debug_vectors.h` & `sequali-0.8.0/src/sequali/debug_vectors.h`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/function_dispatch.h` & `sequali-0.8.0/src/sequali/function_dispatch.h`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/murmur3.h` & `sequali-0.8.0/src/sequali/murmur3.h`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/pygal.js/2.0.x/pygal-tooltips.js` & `sequali-0.8.0/src/sequali/pygal.js/2.0.x/pygal-tooltips.js`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/pygal.js/2.0.x/pygal-tooltips.min.js` & `sequali-0.8.0/src/sequali/pygal.js/2.0.x/pygal-tooltips.min.js`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/pygal.js/README.md` & `sequali-0.8.0/src/sequali/pygal.js/README.md`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/report_modules.py` & `sequali-0.8.0/src/sequali/report_modules.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 from typing import (Any, Dict, Iterable, Iterator, List, Optional, Sequence,
                     Set, Tuple, Type)
 
 import pygal  # type: ignore
 import pygal.style  # type: ignore
 
 from ._qc import A, C, G, N, T
-from ._qc import (AdapterCounter, DedupEstimator, NanoStats, PerTileQuality,
-                  QCMetrics, SequenceDuplication)
+from ._qc import (AdapterCounter, DedupEstimator,
+                  INSERT_SIZE_MAX_ADAPTER_STORE_SIZE, InsertSizeMetrics,
+                  NanoStats, PerTileQuality, QCMetrics, SequenceDuplication)
 from ._qc import NUMBER_OF_NUCS, NUMBER_OF_PHREDS, PHRED_MAX
 from ._version import __version__
 from .adapters import Adapter
-from .sequence_identification import DEFAULT_CONTAMINANTS_FILES, DEFAULT_K, \
-    create_sequence_index, identify_sequence, reverse_complement
-from .util import fasta_parser
+from .sequence_identification import (identify_sequence_builtin,
+                                      reverse_complement)
 
 SEQUALI_REPORT_CSS = Path(__file__).parent / "static" / "sequali_report.css"
 SEQUALI_REPORT_CSS_CONTENT = SEQUALI_REPORT_CSS.read_text(encoding="utf-8")
 SEQUALI_REPORT_JS = (Path(__file__).parent / "pygal.js" / "2.0.x" /
                      "pygal-tooltips.min.js")
 SEQUALI_DOWNLOAD_SVG_JS = (Path(__file__).parent / "static" /
                            "svg_to_download_link.js")
@@ -109,16 +109,22 @@
     truncate_label=-1,
     width=1250,
     height=700,
     disable_xml_declaration=True,
     js=[],  # Script is globally downloaded once
 )
 
+READ1 = "Read 1"
+READ2 = "Read 2"
+NOT_OF_PAIR = None
 
-def html_header(header: str, level: int):
+
+def html_header(header: str, level: int, prefix: Optional[str] = None):
+    if prefix is not None:
+        header = f"{prefix}: {header}"
     html_id = header.lower().replace(" ", "-")
     return f"""
         <h{level} id="{html_id}">
             <a class="headerlink" href="#{html_id}">{header}</a>
         </h{level}>
     """
 
@@ -335,54 +341,82 @@
 
 @dataclasses.dataclass
 class Meta(ReportModule):
     sequali_version: str
     report_generated: str
     filename: str
     filesize: int
+    filename_read2: Optional[str]
+    filesize_read2: Optional[int]
 
     @classmethod
-    def from_filepath(cls, filepath):
+    def from_filepath(cls, filepath: str, filepath_read2: Optional[str] = None):
         filename = os.path.basename(filepath)
         try:
-            filesize = os.stat(filepath).st_size
+            filesize = os.path.getsize(filepath)
         except OSError:
             filesize = 0
+        if filepath_read2:
+            filename_read2 = os.path.basename(filepath_read2)
+            try:
+                filesize_read2 = os.path.getsize(filepath_read2)
+            except OSError:
+                filesize_read2 = 0
+        else:
+            filename_read2 = None
+            filesize_read2 = None
         timestamp = time.time()
         time_struct = time.localtime(timestamp)
         report_generated = time.strftime("%Y-%m-%d %H:%M:%S%z", time_struct)
-        return cls(__version__, report_generated, filename, filesize)
+        return cls(__version__, report_generated, filename, filesize,
+                   filename_read2, filesize_read2)
 
     def to_html(self) -> str:
-        return f"""
-        {html_header("Metadata", 1)}
-        <table>
+        content = io.StringIO()
+        content.write(html_header("Metadata", 1))
+        content.write(f"""
+            <table>
             <tr><td>Filename</td><td><code>{self.filename}</code></td></tr>
             <tr><td>Filesize</td><td>{self.filesize / (1024 ** 3):.2f} GiB</td></tr>
+        """)
+        if self.filename_read2 is not None and self.filesize_read2 is not None:
+            content.write(f"""
+                <tr>
+                    <td>Filename read 2</td>
+                    <td><code>{self.filename_read2}</code></td>
+                </tr>
+                <tr>
+                    <td>Filesize read 2</td>
+                    <td>{self.filesize_read2 / (1024 ** 3):.2f} GiB</td>
+                </tr>
+            """)
+        content.write(f"""
             <tr><td>Sequali version</td><td>{self.sequali_version}</td></tr>
             <tr><td>Report generated on</td><td>{self.report_generated}</td></tr>
-        </table>
-        """
+            </table>
+        """)
+        return content.getvalue()
 
 
 @dataclasses.dataclass
 class Summary(ReportModule):
     mean_length: float
     minimum_length: int
     maximum_length: int
     total_reads: int
     q20_reads: int
     total_bases: int
     q20_bases: int
     total_gc_bases: int
     total_n_bases: int
+    read_pair_info: Optional[str] = None
 
     def to_html(self) -> str:
         return f"""
-            {html_header("Summary", 1)}
+            {html_header("Summary", 1, self.read_pair_info)}
             <table>
             <tr><td>Mean length</td><td style="text-align:right;">
                 {self.mean_length:,.2f}</td><td></td></tr>
             <tr><td>Length range (min-max)</td><td style="text-align:right;">
                 {self.minimum_length:,}</td>
                 <td style="text-align:right;">{self.maximum_length:,}</td></tr>
             <tr>
@@ -430,14 +464,15 @@
     q10: int
     q25: int
     q50: int
     q75: int
     q90: int
     q95: int
     q99: int
+    read_pair_info: Optional[str] = None
 
     def plot(self) -> pygal.Graph:
         plot = pygal.Bar(
             title="Sequence length distribution",
             x_title="sequence length",
             y_title="number of reads",
             style=ONE_SERIE_STYLE,
@@ -463,24 +498,26 @@
                 <tr><td>N95</td><td style="text-align:right;">{self.q95:,}</td></tr>
                 <tr><td>N99</td><td style="text-align:right;">{self.q99:,}</td></tr>
             </table>
         """
 
     def to_html(self):
         return f"""
-            {html_header("Sequence length distribution", 1)}
+            {html_header("Sequence length distribution", 1,
+                         self.read_pair_info)}
             {self.distribution_table()}
             {figurize_plot(self.plot())}
         """
 
     @classmethod
     def from_base_count_tables(cls,
                                base_count_tables: array.ArrayType,
                                total_sequences: int,
-                               data_ranges: Sequence[Tuple[int, int]]):
+                               data_ranges: Sequence[Tuple[int, int]],
+                               read_pair_info: Optional[str] = None):
         max_length = len(base_count_tables) // NUMBER_OF_NUCS
         # use bytes constructor to initialize to 0
         sequence_lengths = array.array("Q", bytes(8 * (max_length + 1)))
         base_counts = array.array("Q", bytes(8 * (max_length + 1)))
         base_counts[0] = total_sequences  # all reads have at least 0 bases
         for i, table in enumerate(table_iterator(base_count_tables, NUMBER_OF_NUCS)):
             base_counts[i + 1] = sum(table)
@@ -515,21 +552,22 @@
                     continue
                 break
             accumulated_count += count
             if done:
                 break
 
         return cls(["0"] + x_labels, [sequence_lengths[0]] + lengths,
-                   *percentile_lengths)
+                   *percentile_lengths, read_pair_info=read_pair_info)  # type: ignore
 
 
 @dataclasses.dataclass
 class PerPositionMeanQualityAndSpread(ReportModule):
     x_labels: List[str]
     percentiles: List[Tuple[str, List[float]]]
+    read_pair_info: Optional[str] = None
 
     def plot(self) -> pygal.Graph:
         plot = pygal.Line(
             title="Per position quality percentiles",
             show_dots=False,
             x_title="position",
             y_title="phred score",
@@ -553,25 +591,29 @@
                  stroke_style={"dasharray": '3,3'})
         plot.add("bottom 1%", label_values(percentiles["bottom 1%"], self.x_labels),
                  stroke_style={"dasharray": '1,2'})
         return plot
 
     def to_html(self):
         return f"""
-            {html_header("Per position quality percentiles", 1)}
+            {html_header("Per position quality percentiles", 1,
+                         self.read_pair_info)}
             <p class="explanation">Shows the mean for all bases and the means
             of the lowest and
             highest percentiles to indicate the spread. Since the graph is
             based on the sampled categories, rather than exact phreds, it is
             an approximation.</p>
             {figurize_plot(self.plot())}
         """
 
     @classmethod
-    def from_phred_table_and_labels(cls, phred_tables: array.ArrayType, x_labels):
+    def from_phred_table_and_labels(cls,
+                                    phred_tables: array.ArrayType,
+                                    x_labels,
+                                    read_pair_info: Optional[str] = None):
         percentiles = [1, 5, 10, 25, 50, 75, 90, 95, 99]
         percentile_fractions = [i / 100 for i in percentiles]
         total_tables = len(phred_tables) // NUMBER_OF_PHREDS
         percentile_tables = [[0.0 for _ in range(total_tables)]
                              for _ in percentiles]
         reversed_percentile_tables = [[0.0 for _ in range(total_tables)]
                                       for _ in percentiles]
@@ -629,26 +671,30 @@
             ("top 25%", reversed_percentile_tables[-4]),
             ("top 10%", reversed_percentile_tables[-3]),
             ("top 5%", reversed_percentile_tables[-2]),
             ("top 1%", reversed_percentile_tables[-1]),
         ]
         return cls(
             x_labels=x_labels,
-            percentiles=graph_series
+            percentiles=graph_series,
+            read_pair_info=read_pair_info,
             )
 
 
 @dataclasses.dataclass
 class PerBaseQualityScoreDistribution(ReportModule):
     x_labels: Sequence[str]
     series: Sequence[Sequence[float]]
+    read_pair_info: Optional[str] = None
 
     @classmethod
     def from_phred_count_table_and_labels(
-            cls, phred_tables: array.ArrayType, x_labels: Sequence[str]):
+            cls, phred_tables: array.ArrayType, x_labels: Sequence[str],
+            read_pair_info: Optional[str] = None
+    ):
         total_tables = len(x_labels)
         quality_distribution = [
             [0.0 for _ in range(total_tables)]
             for _ in range(NUMBER_OF_PHREDS)
         ]
         for cat_index, table in enumerate(
                 table_iterator(phred_tables, NUMBER_OF_PHREDS)):
@@ -656,15 +702,15 @@
             if total_nucs == 0:
                 continue
             for offset, phred_count in enumerate(table):
                 if phred_count == 0:
                     continue
                 nuc_fraction = phred_count / total_nucs
                 quality_distribution[offset][cat_index] = nuc_fraction
-        return cls(x_labels, quality_distribution)
+        return cls(x_labels, quality_distribution, read_pair_info=read_pair_info)
 
     def plot(self) -> pygal.Graph:
         plot = pygal.StackedBar(
             title="Per base quality distribution",
             style=QUALITY_DISTRIBUTION_STYLE,
             dots_size=1,
             y_labels=[i / 10 for i in range(11)],
@@ -678,23 +724,25 @@
             serie_filled = sum(serie) > 0.0
             plot.add(name, label_values(serie, self.x_labels),
                      show_dots=serie_filled)
         return plot
 
     def to_html(self):
         return f"""
-            {html_header("Per position quality score distribution", 1)}
+            {html_header("Per position quality score distribution",
+                         1, self.read_pair_info)}
             {figurize_plot(self.plot())}
         """
 
 
 @dataclasses.dataclass
 class PerSequenceAverageQualityScores(ReportModule):
     average_quality_counts: Sequence[int]
     x_labels: Tuple[str, ...] = tuple(str(x) for x in range(PHRED_MAX + 1))
+    read_pair_info: Optional[str] = None
 
     def plot(self) -> pygal.Graph:
         maximum_score = 0
         for i, count in enumerate(self.average_quality_counts):
             if count > 0:
                 maximum_score = i
         maximum_score = max(maximum_score + 2, 40)
@@ -716,15 +764,16 @@
                                  for score in self.average_quality_counts]
 
         plot.add("", percentage_scores[:maximum_score])
         return plot
 
     def to_html(self) -> str:
         return f"""
-            {html_header("Per sequence average quality scores", 1)}
+            {html_header("Per sequence average quality scores", 1,
+                         self.read_pair_info)}
             {self.quality_scores_table()}
             {figurize_plot(self.plot())}
         """
 
     def quality_scores_table(self) -> str:
         table = io.StringIO()
         total = max(sum(self.average_quality_counts), 1)
@@ -744,25 +793,27 @@
                 </tr>
                 """
             )
         table.write("</table>")
         return table.getvalue()
 
     @classmethod
-    def from_qc_metrics(cls, metrics: QCMetrics):
-        return cls(list(metrics.phred_scores()))
+    def from_qc_metrics(cls, metrics: QCMetrics,
+                        read_pair_info: Optional[str] = None):
+        return cls(list(metrics.phred_scores()), read_pair_info=read_pair_info)
 
 
 @dataclasses.dataclass
 class PerPositionBaseContent(ReportModule):
     x_labels: Sequence[str]
     A: Sequence[float]
     C: Sequence[float]
     G: Sequence[float]
     T: Sequence[float]
+    read_pair_info: Optional[str] = None
 
     def plot(self) -> pygal.Graph:
         style_class = pygal.style.Style
         green = COLOR_GREEN
         dark_green = "#228B22"  # ForestGreen
         blue = "#00BFFF"  # DeepSkyBlue
         dark_blue = "#1E90FF"  # DodgerBlue
@@ -786,22 +837,25 @@
         plot.add("C", label_values(self.C, self.x_labels))
         plot.add("A", label_values(self.A, self.x_labels))
         plot.add("T", label_values(self.T, self.x_labels))
         return plot
 
     def to_html(self) -> str:
         return f"""
-             {html_header("Per position base content", 1)}
+             {html_header("Per position base content", 1,
+                          self.read_pair_info)}
              {figurize_plot(self.plot())}
         """
 
     @classmethod
     def from_base_count_tables_and_labels(cls,
                                           base_count_tables: array.ArrayType,
-                                          labels: Sequence[str]):
+                                          labels: Sequence[str],
+                                          read_pair_info: Optional[str] = None,
+                                          ):
         total_tables = len(base_count_tables) // NUMBER_OF_NUCS
         base_fractions = [
             [0.0 for _ in range(total_tables)]
             for _ in range(NUMBER_OF_NUCS)
         ]
         for index, table in enumerate(
                 table_iterator(base_count_tables, NUMBER_OF_NUCS)):
@@ -815,37 +869,42 @@
             base_fractions[G][index] = table[G] / named_total
             base_fractions[T][index] = table[T] / named_total
         return cls(
             labels,
             A=base_fractions[A],
             C=base_fractions[C],
             G=base_fractions[G],
-            T=base_fractions[T]
+            T=base_fractions[T],
+            read_pair_info=read_pair_info,
         )
 
 
 @dataclasses.dataclass
 class PerPositionNContent(ReportModule):
     x_labels: Sequence[str]
     n_content: Sequence[float]
+    read_pair_info: Optional[str] = None
 
     @classmethod
     def from_base_count_tables_and_labels(
-            cls, base_count_tables: array.ArrayType, labels: Sequence[str]):
+            cls, base_count_tables: array.ArrayType, labels: Sequence[str],
+            read_pair_info: Optional[str] = None,
+    ):
         total_tables = len(base_count_tables) // NUMBER_OF_NUCS
         n_fractions = [0.0 for _ in range(total_tables)]
         for index, table in enumerate(
                 table_iterator(base_count_tables, NUMBER_OF_NUCS)):
             total_bases = sum(table)
             if total_bases == 0:
                 continue
             n_fractions[index] = table[N] / total_bases
         return cls(
             labels,
-            n_fractions
+            n_fractions,
+            read_pair_info,
         )
 
     def plot(self) -> pygal.Graph:
         plot = pygal.Bar(
             title="Per position N content",
             dots_size=1,
             y_labels=[i / 10 for i in range(11)],
@@ -857,25 +916,27 @@
             **COMMON_GRAPH_OPTIONS,
         )
         plot.add("N", label_values(self.n_content, self.x_labels))
         return plot
 
     def to_html(self) -> str:
         return f"""
-            {html_header("Per position N content", 1)}
+            {html_header("Per position N content", 1,
+                         self.read_pair_info)}
             {figurize_plot(self.plot())}
         """
 
 
 @dataclasses.dataclass
 class PerSequenceGCContent(ReportModule):
     gc_content_counts: Sequence[int]
     smoothened_gc_content_counts: Sequence[int]
     x_labels: Sequence[str] = tuple(str(x) for x in range(101))
     smoothened_x_labels: Sequence[str] = tuple(str(x) for x in range(0, 101, 2))
+    read_pair_info: Optional[str] = None
 
     def plot(self) -> pygal.Graph:
         plot = pygal.Bar(
             title="Per sequence GC content",
             x_labels=self.x_labels,
             x_labels_major_every=3,
             show_minor_x_labels=False,
@@ -900,44 +961,46 @@
             **COMMON_GRAPH_OPTIONS,
         )
         plot.add("", self.smoothened_gc_content_counts)
         return plot
 
     def to_html(self) -> str:
         return f"""
-            {html_header("Per sequence GC content", 1)}
+            {html_header("Per sequence GC content", 1,
+                         self.read_pair_info)}
             <p class="explanation">
             For short reads with fixed size (i.e. Illumina) the plot will
             look very spiky due to the GC content calculation: GC bases / all
             bases. For read lengths of 151, both 75 and 76 GC bases lead to a
             percentage of 50% (rounded) and 72 and 73 GC bases leads to 48%
             (rounded). Only 74 GC bases leads to 49%. As a result the
             even categories will be twice as high, which creates a spike. The
             smoothened plot is provided to give a clearer picture in this case.
             </p>
             {figurize_plot(self.plot())}
             {figurize_plot(self.smoothened_plot())}
         """
 
     @classmethod
-    def from_qc_metrics(cls, metrics: QCMetrics):
+    def from_qc_metrics(cls, metrics: QCMetrics, read_pair_info: Optional[str] = None):
         gc_content = list(metrics.gc_content())
         smoothened_gc_content = []
         gc_content_iter = iter(gc_content)
         for i in range(50):
             smoothened_gc_content.append(next(gc_content_iter) + next(gc_content_iter))
         # Append the last 100% category.
         smoothened_gc_content.append(next(gc_content_iter))
-        return cls(gc_content, smoothened_gc_content)
+        return cls(gc_content, smoothened_gc_content, read_pair_info=read_pair_info)
 
 
 @dataclasses.dataclass
 class AdapterContent(ReportModule):
     x_labels: Sequence[str]
     adapter_content: Sequence[Tuple[str, Sequence[float]]]
+    read_pair_info: Optional[str] = None
 
     def plot(self) -> pygal.Graph:
         plot = pygal.Line(
             title="Adapter content (%)",
             range=(0.0, 100.0),
             x_title="position",
             y_title="%",
@@ -954,15 +1017,15 @@
                              reverse=True)
         for label, content in adapter_content:
             plot.add(label, label_values(content, self.x_labels))
         return plot
 
     def to_html(self):
         return f"""
-            {html_header("Adapter content", 1)}
+            {html_header("Adapter content", 1, self.read_pair_info)}
             <p class="explanation">Only adapters that are present more than 0.1%
             are shown. Given the 12&#8239;bp
             length of the sequences used to estimate the content, values below this
             threshold are problably false positives. The legend is sorted from
             most frequent to least frequent.</p>
             <p class="explanation">For nanopore the the adapter mix (AMX) and
             ligation kit have overlapping adapter sequences and are therefore
@@ -975,15 +1038,17 @@
             the last 11 base pairs.</p>
             {figurize_plot(self.plot())}
         """  # noqa: E501
 
     @classmethod
     def from_adapter_counter_adapters_and_ranges(
             cls, adapter_counter: AdapterCounter, adapters: Sequence[Adapter],
-            data_ranges: Sequence[Tuple[int, int]]):
+            data_ranges: Sequence[Tuple[int, int]],
+            read_pair_info: Optional[str] = None,
+    ):
 
         def accumulate_counts(counts: Iterable[int]) -> List[int]:
             total = 0
             accumulated_counts = []
             for count in counts:
                 total += count
                 accumulated_counts.append(total)
@@ -1003,40 +1068,47 @@
                 # Reverse the counts, accumulate them and reverse again for
                 # adapters at the front.
                 accumulated_counts = list(reversed(
                     accumulate_counts(reversed(adapter_counts))))
             all_adapters.append([count * 100 / total_sequences
                                  for count in accumulated_counts])
         return cls(stringify_ranges(data_ranges),
-                   list(zip(adapter_names, all_adapters)))
+                   list(zip(adapter_names, all_adapters)),
+                   read_pair_info=read_pair_info)
 
 
 @dataclasses.dataclass
 class PerTileQualityReport(ReportModule):
     x_labels: Sequence[str]
     normalized_per_tile_averages: Sequence[Tuple[str, Sequence[float]]]
     tiles_2x_errors: Sequence[str]
     tiles_10x_errors: Sequence[str]
     skipped_reason: Optional[str]
+    read_pair_info: Optional[str] = None
 
     @classmethod
     def from_per_tile_quality_and_ranges(
-            cls, ptq: PerTileQuality, data_ranges: Sequence[Tuple[int, int]]):
+            cls, ptq: PerTileQuality, data_ranges: Sequence[Tuple[int, int]],
+            read_pair_info: Optional[str] = None,
+    ):
         if ptq.skipped_reason:
             return cls([], [], [], [], ptq.skipped_reason)
         average_phreds = []
         per_category_totals = [0.0 for i in range(len(data_ranges))]
         tile_counts = ptq.get_tile_counts()
         for tile, summed_errors, counts in tile_counts:
             range_averages = [
-                sum(summed_errors[start:stop]) / sum(counts[start:stop])
+                sum(summed_errors[start:stop]) / max(sum(counts[start:stop]), 1)
                 for start, stop in data_ranges]
             range_phreds = []
             for i, average in enumerate(range_averages):
-                phred = -10 * math.log10(average)
+                if average != 0:
+                    phred = -10 * math.log10(average)
+                else:
+                    phred = 0
                 range_phreds.append(phred)
                 # Averaging phreds takes geometric mean.
                 per_category_totals[i] += phred
             average_phreds.append((tile, range_phreds))
         number_of_tiles = len(tile_counts)
         averages_per_category = [total / number_of_tiles
                                  for total in per_category_totals]
@@ -1059,14 +1131,15 @@
             normalized_averages.append((str(tile), normalized_tile_phreds))
         return cls(
             x_labels=stringify_ranges(data_ranges),
             normalized_per_tile_averages=normalized_averages,
             tiles_2x_errors=tiles_2x_errors,
             tiles_10x_errors=tiles_10x_errors,
             skipped_reason=ptq.skipped_reason,
+            read_pair_info=read_pair_info,
         )
 
     def plot(self) -> pygal.Graph:
         style_colors = MULTIPLE_SERIES_STYLE.colors
         red = "#FF0000"
         yellow = "#FFD700"  # actually 'Gold' which is darker and more visible.
         style = pygal.style.Style(
@@ -1105,15 +1178,15 @@
                               for phred, label in
                               zip(tile_phreds, self.x_labels)]
             scatter_plot.add(str(tile), cleaned_phreds)
 
         return scatter_plot
 
     def to_html(self) -> str:
-        header = html_header("Per tile quality", 1)
+        header = html_header("Per tile quality", 1, self.read_pair_info)
         if self.skipped_reason:
             return header + (f"Per tile quality skipped. Reason: "
                              f"{self.skipped_reason}.")
         return header + f"""
             <p class="explanation">
             This graph shows the deviation of each tile on each position from
             the geometric mean of all tiles at that position. The scale is
@@ -1286,40 +1359,44 @@
     max_unique_fragments: int
     collected_fragments: int
     sample_every: int
     sequence_length: int
     total_fragments: int
     total_sequences: int
     sampled_sequences: int
+    read_pair_info: Optional[str] = None
 
     def to_dict(self) -> Dict[str, Any]:
         return {"overrepresented_sequences":
                 [x._asdict() for x in self.overrepresented_sequences],
                 "max_unique_fragments": self.max_unique_fragments,
                 "sample_every": self.sample_every,
                 "collected_fragments": self.collected_fragments,
                 "sequence_length": self.sequence_length,
                 "total_fragments": self.total_fragments,
                 "total_sequences": self.total_sequences,
-                "sampled_sequences": self.sampled_sequences}
+                "sampled_sequences": self.sampled_sequences,
+                "read_pair_info": self.read_pair_info}
 
     def from_dict(cls, d: Dict[str, List[Dict[str, Any]]]):
         overrepresented_sequences = d["overrepresented_sequences"]
         return cls([OverRepresentedSequence(**d)
                    for d in overrepresented_sequences],
                    max_unique_fragments=d["max_unique_fragments"],
                    collected_fragments=d["collected_fragments"],
                    sample_every=d["sample_every"],
                    sequence_length=d["sequence_length"],
                    total_fragments=d["total_fragments"],
                    total_sequences=d["total_sequences"],
-                   sampled_sequences=d["sampled_sequences"])  # type: ignore
+                   sampled_sequences=d["sampled_sequences"],
+                   read_pair_info=d["read_pair_info"])  # type: ignore
 
     def to_html(self) -> str:
-        header = html_header("Overrepresented sequences", 1)
+        header = html_header("Overrepresented sequences", 1,
+                             self.read_pair_info)
         if len(self.overrepresented_sequences) == 0:
             return header + "No overrepresented sequences."
         content = io.StringIO()
         content.write(header)
         content.write(
             f"""
             <p class="explanation">A subsample of the sequences is analysed
@@ -1394,43 +1471,37 @@
     @classmethod
     def from_sequence_duplication(
             cls,
             seqdup: SequenceDuplication,
             fraction_threshold: float = DEFAULT_FRACTION_THRESHOLD,
             min_threshold: int = DEFAULT_MIN_THRESHOLD,
             max_threshold: int = DEFAULT_MAX_THRESHOLD,
+            read_pair_info: Optional[str] = None,
     ):
         overrepresented_sequences = seqdup.overrepresented_sequences(
             fraction_threshold,
             min_threshold,
             max_threshold
         )
-        if overrepresented_sequences:
-            def contaminant_iterator():
-                for file in DEFAULT_CONTAMINANTS_FILES:
-                    yield from fasta_parser(file)
-
-            sequence_index = create_sequence_index(contaminant_iterator(),
-                                                   DEFAULT_K)
-        else:  # Only spend time creating sequence index when its worth it.
-            sequence_index = {}
+
         overrepresented_with_identification = [
             OverRepresentedSequence(
                 count, fraction, sequence, reverse_complement(sequence),
-                *identify_sequence(sequence, sequence_index))
+                *identify_sequence_builtin(sequence))
             for count, fraction, sequence in overrepresented_sequences
         ]
         return cls(overrepresented_with_identification,
                    seqdup.max_unique_fragments,
                    seqdup.collected_unique_fragments,
                    seqdup.sample_every,
                    seqdup.fragment_length,
                    seqdup.total_fragments,
                    seqdup.number_of_sequences,
-                   seqdup.sampled_sequences)
+                   seqdup.sampled_sequences,
+                   read_pair_info=read_pair_info)
 
 
 @dataclasses.dataclass
 class NanoStatsReport(ReportModule):
     x_labels: List[str]
     time_bases: List[int]
     time_reads: List[int]
@@ -1665,14 +1736,194 @@
         {figurize_plot(self.time_quality_distribution_plot())}
         {html_header("Per channel base yield versus quality", 2)}
         {figurize_plot(self.channel_plot())}
         {self.translocation_section()}
         """
 
 
+@dataclasses.dataclass
+class InsertSizeMetricsReport(ReportModule):
+
+    insert_sizes: Sequence[int]
+
+    @classmethod
+    def from_insert_size_metrics(cls, metrics: InsertSizeMetrics):
+        return cls(
+            insert_sizes=metrics.insert_sizes().tolist(),
+        )
+
+    def insert_sizes_plot(self):
+        insert_sizes_copy = list(self.insert_sizes)
+        insert_sizes_copy[0] = 0
+        plot = pygal.Bar(
+            title="Insert Sizes",
+            x_title="Insert size",
+            y_title="Number of reads",
+            style=ONE_SERIE_STYLE,
+            x_labels=list(range(len(insert_sizes_copy))),
+            x_labels_major_every=10,
+            show_minor_x_labels=False,
+            **COMMON_GRAPH_OPTIONS
+        )
+        plot.add("", insert_sizes_copy)
+        return plot
+
+    def to_html(self) -> str:
+        total_reads = sum(self.insert_sizes)
+        no_overlap_reads = self.insert_sizes[0]
+        return f"""
+            {html_header("Insert Sizes", 1)}
+            <p class="explanation">
+            Insert sizes are calculated by taking the first and last
+            16&#8239;bp from read 2. These are searched for in read 1 while
+            allowing at most 1 error. This method is very fast and reasonably
+            accurate, but does not account for long poly-G cycles.
+            </p>
+            <table>
+            <tr>
+                <td>Total reads</td>
+                <td style="text-align:right;">{total_reads:,}</td>
+            </tr>
+            <tr>
+                <td>Reads without overlap</td>
+                <td style="text-align:right;">{no_overlap_reads:,}</td>
+                <td style="text-align:right;">
+                    {no_overlap_reads / max(total_reads, 1):.2%}
+                </td>
+            </tr>
+            </table>
+            {figurize_plot(self.insert_sizes_plot())}
+        """
+
+
+@dataclasses.dataclass
+class AdapterFromOverlapReport(ReportModule):
+    total_reads: int
+    number_of_adapters_read1: int
+    number_of_adapters_read2: int
+    adapters_read1: Sequence[Tuple[str, int]]
+    adapters_read2: Sequence[Tuple[str, int]]
+    longest_adapter_read1: str
+    longest_adapter_read2: str
+    longest_adapter_read1_match: str
+    longest_adapter_read2_match: str
+
+    @staticmethod
+    def select_relevant_adapters(adapter_list: Sequence[Tuple[str, int]]):
+        """
+        Get the most prevalent adapters for each length. Sort the resulting
+        list on length.
+        """
+        # Sort list on count
+        sorted_list = sorted(adapter_list, reverse=True, key=lambda x: (x[1]))
+        new_list = []
+        lengths_to_get = set(range(1, INSERT_SIZE_MAX_ADAPTER_STORE_SIZE + 1))
+        for adapter, count in sorted_list:
+            if len(adapter) in lengths_to_get:
+                lengths_to_get.remove(len(adapter))
+                new_list.append((adapter, count))
+        new_list.sort(key=lambda x: len(x[0]))
+        return new_list
+
+    @classmethod
+    def from_insert_size_metrics(cls, metrics: InsertSizeMetrics):
+        adapters_read1 = AdapterFromOverlapReport.select_relevant_adapters(
+                metrics.adapters_read1())
+        adapters_read2 = AdapterFromOverlapReport.select_relevant_adapters(
+            metrics.adapters_read2())
+        longest_adapter_read1 = adapters_read1[-1][0]
+        longest_adapter_read2 = adapters_read2[-1][0]
+        longest_adapter_read1_match = identify_sequence_builtin(
+            longest_adapter_read1)[2]
+        longest_adapter_read2_match = identify_sequence_builtin(
+            longest_adapter_read2)[2]
+        return cls(
+            total_reads=metrics.total_reads,
+            number_of_adapters_read1=metrics.number_of_adapters_read1,
+            number_of_adapters_read2=metrics.number_of_adapters_read2,
+            adapters_read1=adapters_read1,
+            adapters_read2=adapters_read2,
+            longest_adapter_read1=longest_adapter_read1,
+            longest_adapter_read2=longest_adapter_read2,
+            longest_adapter_read1_match=longest_adapter_read1_match,
+            longest_adapter_read2_match=longest_adapter_read2_match,
+        )
+
+    def to_html(self) -> str:
+        report = io.StringIO()
+        report.write(f"""
+            {html_header("Adapter Content", 1)}
+            <p class="explanation">
+                By calculating the overlap between reads it is possible to
+                determine where the adapter is.
+            </p>
+            <table>
+            <tr>
+                <td>Total reads</td>
+                <td style="text-align:right;">{self.total_reads:,}</td>
+                <td style="text-align:right;">
+                    {self.total_reads / max(self.total_reads, 1):.2%}
+                </td>
+            </tr>
+            <tr>
+                <td>Adapters in read 1</td>
+                <td style="text-align:right;">{self.number_of_adapters_read1:,}</td>
+                <td style="text-align:right;">
+                    {self.number_of_adapters_read1 / max(self.total_reads, 1):.2%}
+                </td>
+            </tr>
+            <tr>
+                <td>Adapters in read 2</td>
+                <td style="text-align:right;">{self.number_of_adapters_read2:,}</td>
+                <td style="text-align:right;">
+                    {self.number_of_adapters_read2 / max(self.total_reads, 1):.2%}
+                </td>
+            </tr>
+            </table>
+            <table><tr><th>Longest most frequent adapter</th>
+            <th>Adapter Sequence</th><th>Best match</th></tr>
+            <tr>
+                <td>Read 1</td>
+                <td>{self.longest_adapter_read1}</td>
+                <td>{self.longest_adapter_read1_match}</td>
+            </tr>
+            <tr>
+                <td>Read 2</td>
+                <td>{self.longest_adapter_read2}</td>
+                <td>{self.longest_adapter_read2_match}</td>
+            </tr>
+            </table>
+        """)
+
+        report.write(html_header("Adapters read 1", 2))
+        report.write("<table>")
+        report.write("<tr><th>Adapter</th><th>Count</th></tr>")
+        for adapter, count in self.adapters_read1:
+            report.write(
+                f"""<tr>
+                        <td>{adapter}</td>
+                        <td style="text-align:right;">{count}</td>
+                    </tr>
+                """)
+        report.write("</table>")
+
+        report.write(html_header("Adapters read 2", 2))
+        report.write("<table>")
+        report.write("<tr><th>Adapter</th><th>Count</th></tr>")
+        for adapter, count in self.adapters_read2:
+            report.write(
+                f"""<tr>
+                        <td>{adapter}</td>
+                        <td style="text-align:right;">{count}</td>
+                    </tr>
+                """)
+        report.write("</table>")
+        return report.getvalue()
+
+
 NAME_TO_CLASS: Dict[str, Type[ReportModule]] = {
     "meta": Meta,
     "summary": Summary,
     "per_position_mean_quality_and_spread": PerPositionMeanQualityAndSpread,
     "per_position_quality_distribution": PerBaseQualityScoreDistribution,
     "sequence_length_distribution": SequenceLengthDistribution,
     "per_position_base_content": PerPositionBaseContent,
@@ -1680,30 +1931,38 @@
     "per_sequence_gc_content": PerSequenceGCContent,
     "per_sequence_quality_scores": PerSequenceAverageQualityScores,
     "adapter_content": AdapterContent,
     "per_tile_quality": PerTileQualityReport,
     "duplication_fractions": DuplicationCounts,
     "overrepresented_sequences": OverRepresentedSequences,
     "nanopore_metrics": NanoStatsReport,
+    "adapter_content_from_overlap": AdapterFromOverlapReport,
+    "insert_size_metrics": InsertSizeMetricsReport,
 }
 
 CLASS_TO_NAME: Dict[Type[ReportModule], str] = {
     value: key for key, value in NAME_TO_CLASS.items()}
 
 
 def report_modules_to_dict(report_modules: Iterable[ReportModule]):
+    def get_name(module: ReportModule) -> str:
+        class_name = CLASS_TO_NAME[type(module)]
+        if hasattr(module, "read_pair_info"):
+            if module.read_pair_info == READ2:
+                class_name += "_read2"
+        return class_name
     return {
-        CLASS_TO_NAME[type(module)]: module.to_dict()
+        get_name(module): module.to_dict()
         for module in report_modules
     }
 
 
 def dict_to_report_modules(d: Dict[str, Dict[str, Any]]) -> List[ReportModule]:
-    return [NAME_TO_CLASS[name].from_dict(
-                NAME_TO_CLASS[name], class_dict)  # type: ignore
+    return [NAME_TO_CLASS[name.replace("_read2", "")].from_dict(
+                NAME_TO_CLASS[name.replace("_read2", "")], class_dict)  # type: ignore
             for name, class_dict in d.items()]
 
 
 def write_html_report(report_modules: Iterable[ReportModule],
                       html: str):
     for mod in report_modules:
         if isinstance(mod, Meta):
@@ -1757,15 +2016,16 @@
         """)
         html_file.write('</div>')
         html_file.write(content)
         html_file.write("</body></html>")
 
 
 def qc_metrics_modules(metrics: QCMetrics,
-                       data_ranges: Sequence[Tuple[int, int]]
+                       data_ranges: Sequence[Tuple[int, int]],
+                       read_pair_info: Optional[str] = None,
                        ) -> List[ReportModule]:
     base_count_tables = metrics.base_count_table()
     phred_count_table = metrics.phred_count_table()
     x_labels = stringify_ranges(data_ranges)
     aggregrated_base_matrix = aggregate_count_matrix(
         base_count_tables, data_ranges, NUMBER_OF_NUCS)
     aggregated_phred_matrix = aggregate_count_matrix(
@@ -1792,58 +2052,112 @@
             minimum_length=minimum_length,
             maximum_length=metrics.max_length,
             total_reads=total_reads,
             total_bases=total_bases,
             q20_bases=sum(summary_phreds[5:]),
             q20_reads=q20_reads,
             total_gc_bases=total_gc_bases,
-            total_n_bases=summary_bases[N]),
+            total_n_bases=summary_bases[N],
+            read_pair_info=read_pair_info),
         SequenceLengthDistribution.from_base_count_tables(
-            base_count_tables, total_reads, data_ranges),
+            base_count_tables, total_reads, data_ranges,
+            read_pair_info=read_pair_info),
         PerBaseQualityScoreDistribution.from_phred_count_table_and_labels(
-            aggregated_phred_matrix, x_labels),
+            aggregated_phred_matrix, x_labels, read_pair_info=read_pair_info),
         PerPositionMeanQualityAndSpread.from_phred_table_and_labels(
-           aggregated_phred_matrix, x_labels),
-        PerSequenceAverageQualityScores.from_qc_metrics(metrics),
+           aggregated_phred_matrix, x_labels, read_pair_info=read_pair_info),
+        PerSequenceAverageQualityScores.from_qc_metrics(
+            metrics, read_pair_info=read_pair_info),
         PerPositionBaseContent.from_base_count_tables_and_labels(
-            aggregrated_base_matrix, x_labels),
+            aggregrated_base_matrix, x_labels, read_pair_info=read_pair_info),
         PerPositionNContent.from_base_count_tables_and_labels(
-            aggregrated_base_matrix, x_labels),
-        PerSequenceGCContent.from_qc_metrics(metrics),
+            aggregrated_base_matrix, x_labels, read_pair_info=read_pair_info),
+        PerSequenceGCContent.from_qc_metrics(
+            metrics, read_pair_info=read_pair_info),
     ]
 
 
 def calculate_stats(
         filename: str,
         metrics: QCMetrics,
-        adapter_counter: AdapterCounter,
         per_tile_quality: PerTileQuality,
         sequence_duplication: SequenceDuplication,
         dedup_estimator: DedupEstimator,
         nanostats: NanoStats,
         adapters: List[Adapter],
+        adapter_counter: Optional[AdapterCounter] = None,
+        filename_reverse: Optional[str] = None,
+        insert_size_metrics: Optional[InsertSizeMetrics] = None,
+        metrics_reverse: Optional[QCMetrics] = None,
+        per_tile_quality_reverse: Optional[PerTileQuality] = None,
+        sequence_duplication_reverse: Optional[SequenceDuplication] = None,
         graph_resolution: int = 200,
         fraction_threshold: float = DEFAULT_FRACTION_THRESHOLD,
         min_threshold: int = DEFAULT_MIN_THRESHOLD,
         max_threshold: int = DEFAULT_MAX_THRESHOLD,
 ) -> List[ReportModule]:
+    read_pair_info1 = READ1 if filename_reverse else None
     max_length = metrics.max_length
     if max_length > 500:
         data_ranges = list(logarithmic_ranges(max_length))
     else:
         data_ranges = list(equidistant_ranges(max_length, graph_resolution))
-    return [
-        Meta.from_filepath(filename),
-        *qc_metrics_modules(metrics, data_ranges),
-        AdapterContent.from_adapter_counter_adapters_and_ranges(
-            adapter_counter, adapters, data_ranges),
-        PerTileQualityReport.from_per_tile_quality_and_ranges(
-            per_tile_quality, data_ranges),
-        DuplicationCounts.from_dedup_estimator(dedup_estimator),
+    modules = [
+        Meta.from_filepath(filename, filename_reverse),
+    ]
+    # Generic modules for both read1 and read2 come first.
+    if insert_size_metrics:
+        modules.append(
+            AdapterFromOverlapReport.from_insert_size_metrics(insert_size_metrics))
+        modules.append(
+            InsertSizeMetricsReport.from_insert_size_metrics(insert_size_metrics))
+    if filename_reverse:
+        modules.append(
+            DuplicationCounts.from_dedup_estimator(dedup_estimator),
+        )
+    modules.extend(qc_metrics_modules(metrics, data_ranges,
+                                      read_pair_info=read_pair_info1))
+    if adapter_counter:
+        modules.append(
+            AdapterContent.from_adapter_counter_adapters_and_ranges(
+                adapter_counter, adapters, data_ranges, read_pair_info=read_pair_info1)
+        )
+    modules.append(PerTileQualityReport.from_per_tile_quality_and_ranges(
+        per_tile_quality, data_ranges, read_pair_info=read_pair_info1),)
+    if not filename_reverse:
+        modules.append(
+            DuplicationCounts.from_dedup_estimator(dedup_estimator)
+        )
+    modules.append(
         OverRepresentedSequences.from_sequence_duplication(
             sequence_duplication,
             fraction_threshold=fraction_threshold,
             min_threshold=min_threshold,
-            max_threshold=max_threshold
-        ),
-        NanoStatsReport.from_nanostats(nanostats)
-    ]
+            max_threshold=max_threshold,
+            read_pair_info=read_pair_info1,
+        )
+    )
+
+    if (metrics_reverse and per_tile_quality_reverse and
+            sequence_duplication_reverse):
+        max_length_reverse = metrics_reverse.max_length
+        if max_length_reverse > 500:
+            data_ranges_reverse = list(logarithmic_ranges(max_length_reverse))
+        else:
+            data_ranges_reverse = list(
+                equidistant_ranges(max_length_reverse, graph_resolution))
+
+        modules.extend(qc_metrics_modules(metrics_reverse, data_ranges_reverse,
+                                          read_pair_info=READ2))
+        modules.append(PerTileQualityReport.from_per_tile_quality_and_ranges(
+            per_tile_quality_reverse, data_ranges_reverse,
+            read_pair_info=READ2))
+        modules.append(OverRepresentedSequences.from_sequence_duplication(
+            sequence_duplication_reverse,
+            fraction_threshold=fraction_threshold,
+            min_threshold=min_threshold,
+            max_threshold=max_threshold,
+            read_pair_info=READ2,
+        ))
+
+    modules.append(NanoStatsReport.from_nanostats(nanostats))
+    return modules
```

### Comparing `sequali-0.7.1/src/sequali/score_to_error_rate.h` & `sequali-0.8.0/src/sequali/score_to_error_rate.h`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/sequence_identification.py` & `sequali-0.8.0/src/sequali/sequence_identification.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,25 +10,33 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with Sequali.  If not, see <https://www.gnu.org/licenses/
 import collections
+import functools
 import os
 import typing
-from typing import Dict, Iterable, List, Tuple, Union
+from typing import Dict, Iterable, Iterator, List, Tuple, Union
+
+from .util import fasta_parser
 
 DEFAULT_K = 13
 
 CONTAMINANTS_DIR = os.path.join(os.path.dirname(__file__), "contaminants")
 DEFAULT_CONTAMINANTS_FILES = [f.path for f in os.scandir(CONTAMINANTS_DIR)
                               if f.name != "README"]
 
 
+def default_contaminant_iterator() -> Iterator[Tuple[str, str]]:
+    for file in DEFAULT_CONTAMINANTS_FILES:
+        yield from fasta_parser(file)
+
+
 def create_upper_table():
     upper_table = bytearray(b"N" * 256)
     for c in "acgtACGT":
         upper_table[ord(c)] = ord(c.upper())
     return bytes(upper_table)
 
 
@@ -89,14 +97,20 @@
                 else:
                     sequence_index[kmer] = [name, prev_entry]
             else:
                 sequence_index[kmer] = name
     return sequence_index
 
 
+@functools.lru_cache
+def create_default_sequence_index(k: int = DEFAULT_K
+                                  ) -> Dict[str, Union[List[str], str]]:
+    return create_sequence_index(default_contaminant_iterator(), k)
+
+
 def identify_sequence(
         sequence: str,
         sequence_index: Dict[str, Union[List[str], str]],
         k: int = DEFAULT_K) -> Tuple[int, int, str]:
     kmers = canonical_kmers(sequence, k)
     counted_seqs: typing.Counter[str] = collections.Counter()
     for kmer in kmers:
@@ -107,7 +121,17 @@
             counted_seqs.update([matched])
     most_matches = 0
     best_match = "No match"
     matches = sorted(counted_seqs.items(), key=lambda tup: tup[1], reverse=True)
     if matches:
         best_match, most_matches = matches[0]
     return most_matches, len(kmers), best_match
+
+
+def identify_sequence_builtin(sequence: str, k: int = DEFAULT_K):
+    """
+    Identify a sequence using the builtin sequence libraries.
+    :return: A tuple of kmer matches, the max matches and a string containing
+             the best match.
+    """
+    sequence_index = create_default_sequence_index(k)
+    return identify_sequence(sequence, sequence_index, k)
```

### Comparing `sequali-0.7.1/src/sequali/static/sequali_report.css` & `sequali-0.8.0/src/sequali/static/sequali_report.css`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/static/svg_to_download_link.js` & `sequali-0.8.0/src/sequali/static/svg_to_download_link.js`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali/wanghash.h` & `sequali-0.8.0/src/sequali/wanghash.h`

 * *Files identical despite different names*

### Comparing `sequali-0.7.1/src/sequali.egg-info/PKG-INFO` & `sequali-0.8.0/src/sequali.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sequali
-Version: 0.7.1
-Summary: Fast sequencing quality metrics
+Version: 0.8.0
+Summary: Sequali is a QC tool that generates useful graphs for both short and long-read data.
 Author-email: Ruben Vorderman <r.h.p.vorderman@lumc.nl>
 License: AGPL-v3.0
 Project-URL: Documentation, https://sequali.readthedocs.io
 Project-URL: Homepage, https://github.com/rhpvorderman/sequali
 Project-URL: Issue tracker, https://github.com/rhpvorderman/sequali/issues
 Keywords: FASTQ,sequencing quality,uBAM,QC,nanopore,illumina
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,42 +21,45 @@
 Requires-Python: >3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: xopen>=2.0.0
 Requires-Dist: pygal>=3.0.4
 Requires-Dist: tqdm
 
-.. image:: https://img.shields.io/pypi/v/sequali.svg
+.. |python-version-shield| image:: https://img.shields.io/pypi/v/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/conda/v/bioconda/sequali.svg
+.. |conda-version-shield| image:: https://img.shields.io/conda/v/bioconda/sequali.svg
   :target: https://bioconda.github.io/recipes/sequali/README.html
   :alt:
 
-.. image:: https://img.shields.io/pypi/pyversions/sequali.svg
+.. |python-install-version-shield| image:: https://img.shields.io/pypi/pyversions/sequali.svg
   :target: https://pypi.org/project/sequali/
   :alt:
 
-.. image:: https://img.shields.io/pypi/l/sequali.svg
+.. |license-shield| image:: https://img.shields.io/pypi/l/sequali.svg
   :target: https://github.com/rhpvorderman/sequali/blob/main/LICENSE
   :alt:
 
-.. image:: https://readthedocs.org/projects/sequali/badge/?version=latest
+.. |docs-shield| image:: https://readthedocs.org/projects/sequali/badge/?version=latest
   :target: https://sequali.readthedocs.io/en/latest/?badge=latest
   :alt:
 
-.. image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
+.. |coverage-shield| image:: https://codecov.io/gh/rhpvorderman/sequali/graph/badge.svg?token=MSR1A6BEGC
   :target: https://codecov.io/gh/rhpvorderman/sequali
   :alt:
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
+.. |zenodo-shield| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10854010.svg
   :target: https://doi.org/10.5281/zenodo.10854010
   :alt:
 
+|python-version-shield| |conda-version-shield| |python-install-version-shield|
+|license-shield| |docs-shield| |coverage-shield| |zenodo-shield|
+
 ========
 Sequali
 ========
 
 .. introduction start
 
 Sequence quality metrics for FASTQ and uBAM files.
@@ -67,22 +70,25 @@
 + Informative graphs that allow for judging the quality of a sequence at
   a quick glance.
 + Overrepresentation analysis using 21 bp sequence fragments. Overrepresented
   sequences are checked against the NCBI univec database.
 + Estimate duplication rate using a `fingerprint subsampling technique which is
   also used in filesystem duplication estimation
   <https://www.usenix.org/system/files/conference/atc13/atc13-xie.pdf>`_.
-+ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences.
++ Checks for 6 illumina adapter sequences and 17 nanopore adapter sequences
+  for single read data.
++ Determines adapters by overlap analysis for paired read data.
++ Insert size metrics for paired read data.
 + Per tile quality plots for illumina reads.
 + Channel and other plots for nanopore reads.
 + FASTQ and unaligned BAM are supported. See "Supported formats".
 
 Example reports:
 
-+ `GM24385_1.fastq.gz <https://github.com/rhpvorderman/sequali/files/14725146/GM24385_1.fastq.gz.html.zip>`_;
++ `GM24385_1.fastq.gz <https://sequali.readthedocs.io/en/latest/GM24385_1.fastq.gz.html>`_;
   HG002 (Genome In A Bottle) on ultra-long Nanopore Sequencing. `Sequence file download <https://ftp-trace.ncbi.nlm.nih.gov/ReferenceSamples/giab/data/AshkenazimTrio/HG002_NA24385_son/UCSC_Ultralong_OxfordNanopore_Promethion/GM24385_1.fastq.gz>`_.
 
 .. introduction end
 
 For more information check `the documentation <https://sequali.readthedocs.io>`_.
 
 Supported formats
@@ -90,19 +96,19 @@
 
 .. formats start
 
 - FASTQ. Only the Sanger variation with a phred offset of 33 and the error rate
   calculation of 10 ^ (-phred/10) is supported. All sequencers use this
   format today.
 
+  - Paired end sequencing data is supported.
   - For sequences called by illumina base callers an additional plot with the
     per tile quality will be provided.
   - For sequences called by guppy additional plots for nanopore specific
     data will be provided.
-
 - unaligned BAM. Any alignment flags are currently ignored.
 
   - For uBAM data as delivered by dorado additional nanopore plots will be
     provided.
 
 .. formats end
```

### Comparing `sequali-0.7.1/src/sequali.egg-info/SOURCES.txt` & `sequali-0.8.0/src/sequali.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .readthedocs.yml
 CHANGELOG.rst
+CITATION.cff
 LICENSE
 MANIFEST.in
 README.rst
 codecov.yml
 pyproject.toml
 setup.py
 docs/conf.py
@@ -12,14 +13,15 @@
 docs/requirements-docs.txt
 docs/_static/images/fingerprint.fodg
 docs/_static/images/fingerprint.svg
 docs/_static/images/overrepresented_sampling.fodg
 docs/_static/images/overrepresented_sampling.svg
 docs/includes/CHANGELOG.rst
 docs/includes/README.rst
+docs/reports/GM24385_1.fastq.gz.html
 src/sequali/__init__.py
 src/sequali/__main__.py
 src/sequali/_qc.pyi
 src/sequali/_qcmodule.c
 src/sequali/_version.py
 src/sequali/adapters.py
 src/sequali/debug_vectors.h
```


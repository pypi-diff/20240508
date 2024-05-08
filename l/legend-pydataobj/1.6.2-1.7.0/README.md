# Comparing `tmp/legend_pydataobj-1.6.2.tar.gz` & `tmp/legend_pydataobj-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pydataobj-1.6.2.tar", last modified: Wed May  1 12:28:06 2024, max compression
+gzip compressed data, was "legend_pydataobj-1.7.0.tar", last modified: Wed May  8 12:14:21 2024, max compression
```

## Comparing `legend_pydataobj-1.6.2.tar` & `legend_pydataobj-1.7.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.516618 legend_pydataobj-1.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.520618 legend_pydataobj-1.6.2/src/lgdo/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/lgdo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.520618 legend_pydataobj-1.6.2/src/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/radware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/varlen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lgdo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/vector_of_vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/vector_of_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/src/lgdo/types/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (127)    15293 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/lgdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    17153 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/vovutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/waveformtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/compression/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/compression/sigcompress/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/sigcompress/special-wf-clipped.dat
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    48214 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_radware_sigcompress.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_str2wfcodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_uleb128_zigzag_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/lh5/
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/test_lgdo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/tests/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_table_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_vovutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_waveformtable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.582988 legend_pydataobj-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-08 12:14:21.582988 legend_pydataobj-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:14:21.582988 legend_pydataobj-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.562988 legend_pydataobj-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.582988 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.566988 legend_pydataobj-1.7.0/src/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 12:14:21.000000 legend_pydataobj-1.7.0/src/lgdo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.570988 legend_pydataobj-1.7.0/src/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/compression/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/compression/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/compression/radware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/compression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/compression/varlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lgdo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.570988 legend_pydataobj-1.7.0/src/lgdo/lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.570988 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.570988 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/vector_of_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.574988 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/vector_of_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.574988 legend_pydataobj-1.7.0/src/lgdo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15293 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/lgdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17936 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/vovutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/types/waveformtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/src/lgdo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.574988 legend_pydataobj-1.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.578988 legend_pydataobj-1.7.0/tests/compression/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/compression/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.578988 legend_pydataobj-1.7.0/tests/compression/sigcompress/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/compression/sigcompress/special-wf-clipped.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/compression/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48214 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/compression/test_radware_sigcompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/compression/test_str2wfcodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/compression/test_uleb128_zigzag_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.578988 legend_pydataobj-1.7.0/tests/lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/test_lh5_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/test_lh5_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/test_lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/test_lh5_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/test_lh5_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/lh5/test_lh5_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/test_lgdo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:14:21.582988 legend_pydataobj-1.7.0/tests/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_table_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_vovutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-08 12:14:17.000000 legend_pydataobj-1.7.0/tests/types/test_waveformtable.py
```

### Comparing `legend_pydataobj-1.6.2/LICENSE` & `legend_pydataobj-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/PKG-INFO` & `legend_pydataobj-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pydataobj
-Version: 1.6.2
+Version: 1.7.0
 Summary: LEGEND Python Data Objects
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pydataobj-1.6.2/README.md` & `legend_pydataobj-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/pyproject.toml` & `legend_pydataobj-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/PKG-INFO` & `legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pydataobj
-Version: 1.6.2
+Version: 1.7.0
 Summary: LEGEND Python Data Objects
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/SOURCES.txt` & `legend_pydataobj-1.7.0/src/legend_pydataobj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/__init__.py` & `legend_pydataobj-1.7.0/src/lgdo/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/cli.py` & `legend_pydataobj-1.7.0/src/lgdo/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,40 @@
     parser.add_argument(
         "--depth",
         "-d",
         type=int,
         default=None,
         help="""Maximum tree depth of groups to print""",
     )
+    parser.add_argument(
+        "--detail",
+        action="store_true",
+        help="""Print details about datasets""",
+    )
 
     args = parser.parse_args(args)
 
     if args.verbose:
         lgdogging.setup(logging.DEBUG)
     elif args.debug:
         lgdogging.setup(logging.DEBUG, logging.root)
     else:
         lgdogging.setup()
 
     if args.version:
         print(__version__)  # noqa: T201
         sys.exit()
 
-    lh5.show(args.lh5_file, args.lh5_group, attrs=args.attributes, depth=args.depth)
+    lh5.show(
+        args.lh5_file,
+        args.lh5_group,
+        attrs=args.attributes,
+        depth=args.depth,
+        detail=args.detail,
+    )
 
 
 def lh5concat(args=None):
     """Command line interface for concatenating array-like LGDOs in LH5 files."""
     parser = argparse.ArgumentParser(
         prog="lh5concat",
         description="""
```

### Comparing `legend_pydataobj-1.6.2/src/lgdo/compression/__init__.py` & `legend_pydataobj-1.7.0/src/lgdo/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/compression/base.py` & `legend_pydataobj-1.7.0/src/lgdo/compression/base.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/compression/generic.py` & `legend_pydataobj-1.7.0/src/lgdo/compression/generic.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/compression/radware.py` & `legend_pydataobj-1.7.0/src/lgdo/compression/radware.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/compression/utils.py` & `legend_pydataobj-1.7.0/src/lgdo/compression/utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/compression/varlen.py` & `legend_pydataobj-1.7.0/src/lgdo/compression/varlen.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lgdo_utils.py` & `legend_pydataobj-1.7.0/src/lgdo/lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/__init__.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/__init__.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/array.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/composite.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/composite.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/encoded.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/ndarray.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/ndarray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/scalar.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/vector_of_vectors.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/read/vector_of_vectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/array.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 
 from .... import types
 from ...exceptions import LH5EncodeError
 
 log = logging.getLogger(__name__)
 
-DEFAULT_HDF5_SETTINGS: dict[str, ...] = {"shuffle": True, "compression": "lzf"}
+DEFAULT_HDF5_SETTINGS: dict[str, ...] = {"shuffle": True, "compression": "gzip"}
 
 
 def _h5_write_array(
     obj,
     name,
     lh5_file,
     group="/",
```

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/composite.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/composite.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/scalar.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/vector_of_vectors.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/_serializers/write/vector_of_vectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/core.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/core.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/datatype.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/datatype.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/exceptions.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/exceptions.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/iterator.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/iterator.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/store.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/store.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/tools.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 def show(
     lh5_file: str | h5py.Group,
     lh5_group: str = "/",
     attrs: bool = False,
     indent: str = "",
     header: bool = True,
     depth: int | None = None,
+    detail: bool = False,
 ) -> None:
     """Print a tree of LH5 file contents with LGDO datatype.
 
     Parameters
     ----------
     lh5_file
         the LH5 file.
@@ -100,14 +101,16 @@
         print the HDF5 attributes too.
     indent
         indent the diagram with this string.
     header
         print `lh5_group` at the top of the diagram.
     depth
         maximum tree depth of groups to print
+    detail
+        whether to print additional information about how the data is stored
 
     Examples
     --------
     >>> from lgdo import show
     >>> show("file.lh5", "/geds/raw")
     /geds/raw
     ├── channel · array<1>{real}
@@ -167,22 +170,43 @@
             char = "└──"
             killme = True  # we'll have to kill this loop later
         else:
             char = "├──"
 
         print(f"{indent}{char} \033[1m{key}\033[0m · {dtype} {_attrs}")  # noqa: T201
 
+        if detail and isinstance(val, h5py.Dataset):
+            char = "|       "
+            if killme:
+                char = "        "
+            toprint = f"{indent}{char}"
+            try:
+                toprint += f"\033[3mdtype\033[0m={val.dtype}"
+                toprint += f", \033[3mshape\033[0m={val.shape}"
+                toprint += f", \033[3mnbytes\033[0m={utils.fmtbytes(val.nbytes)}"
+                if (chunkshape := val.chunks) is None:
+                    toprint += ", \033[3mnumchunks\033[0m=contiguous"
+                else:
+                    toprint += f", \033[3mnumchunks\033[0m={val.id.get_num_chunks()}"
+                    toprint += f", \033[3mchunkshape\033[0m={chunkshape}"
+                toprint += f", \033[3mcompression\033[0m={val.compression}"
+            except TypeError:
+                toprint += "(scalar)"
+
+            print(toprint)  # noqa: T201
+
         # if it's a group, call this function recursively
         if isinstance(val, h5py.Group):
             show(
                 val,
                 indent=indent + ("    " if killme else "│   "),
                 header=False,
                 attrs=attrs,
                 depth=depth - 1 if depth else None,
+                detail=detail,
             )
 
         # break or move to next key
         if killme:
             break
 
         key = k_new
```

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5/utils.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,7 +217,17 @@
         if len(paths) > 1:
             msg = f"found multiple paths matching {path}"
             raise FileNotFoundError(msg)
 
         return paths[0]
 
     return paths
+
+
+# https://stackoverflow.com/a/1094933
+def fmtbytes(num, suffix="B"):
+    """Returns formatted f-string for printing human-readable number of bytes."""
+    for unit in ("", "k", "M", "G", "T", "P", "E", "Z"):
+        if abs(num) < 1024.0:
+            return f"{num:3.1f} {unit}{suffix}"
+        num /= 1024.0
+    return f"{num:.1f} Y{suffix}"
```

### Comparing `legend_pydataobj-1.6.2/src/lgdo/lh5_store.py` & `legend_pydataobj-1.7.0/src/lgdo/lh5_store.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/logging.py` & `legend_pydataobj-1.7.0/src/lgdo/logging.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/__init__.py` & `legend_pydataobj-1.7.0/src/lgdo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/array.py` & `legend_pydataobj-1.7.0/src/lgdo/types/array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/arrayofequalsizedarrays.py` & `legend_pydataobj-1.7.0/src/lgdo/types/arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/encoded.py` & `legend_pydataobj-1.7.0/src/lgdo/types/encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/fixedsizearray.py` & `legend_pydataobj-1.7.0/src/lgdo/types/fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/lgdo.py` & `legend_pydataobj-1.7.0/src/lgdo/types/lgdo.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/scalar.py` & `legend_pydataobj-1.7.0/src/lgdo/types/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/struct.py` & `legend_pydataobj-1.7.0/src/lgdo/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,141 +1,128 @@
-"""
-Implements a LEGEND Data Object representing a struct and corresponding
-utilities.
-"""
+"""Implements utilities for LEGEND Data Objects."""
 
 from __future__ import annotations
 
 import logging
+import os
+from collections.abc import Iterator, MutableMapping
 from typing import Any
 
 import numpy as np
 
-from .lgdo import LGDO
-
 log = logging.getLogger(__name__)
 
 
-class Struct(LGDO, dict):
-    """A dictionary of LGDO's with an optional set of attributes.
+def get_element_type(obj: object) -> str:
+    """Get the LGDO element type of a scalar or array.
+
+    For use in LGDO datatype attributes.
+
+    Parameters
+    ----------
+    obj
+        if a ``str``, will automatically return ``string`` if the object has
+        a :class:`numpy.dtype`, that will be used for determining the element
+        type otherwise will attempt to case the type of the object to a
+        :class:`numpy.dtype`.
+
+    Returns
+    -------
+    element_type
+        A string stating the determined element type of the object.
+    """
 
-    After instantiation, add fields using :meth:`add_field` to keep the
-    datatype updated, or call :meth:`update_datatype` after adding.
+    # special handling for strings
+    if isinstance(obj, str):
+        return "string"
+
+    # the rest use dtypes
+    dt = obj.dtype if hasattr(obj, "dtype") else np.dtype(type(obj))
+    kind = dt.kind
+
+    if kind == "b":
+        return "bool"
+    if kind == "V":
+        return "blob"
+    if kind in ["i", "u", "f"]:
+        return "real"
+    if kind == "c":
+        return "complex"
+    if kind in ["S", "U"]:
+        return "string"
+
+    # couldn't figure it out
+    msg = "cannot determine lgdo element_type for object of type"
+    raise ValueError(msg, type(obj).__name__)
+
+
+def getenv_bool(name: str, default: bool = False) -> bool:
+    """Get environment value as a boolean, returning True for 1, t and true
+    (caps-insensitive), and False for any other value and default if undefined.
+    """
+    val = os.getenv(name)
+    if not val:
+        return default
+    return val.lower() in ("1", "t", "true")
+
+
+class NumbaDefaults(MutableMapping):
+    """Bare-bones class to store some Numba default options. Defaults values
+    are set from environment variables
+
+    Examples
+    --------
+    Set all default option values for a processor at once by expanding the
+    provided dictionary:
+
+    >>> from numba import guvectorize
+    >>> from lgdo.utils import numba_defaults_kwargs as nb_kwargs
+    >>> @guvectorize([], "", **nb_kwargs, nopython=True) # def proc(...): ...
+
+    Customize one argument but still set defaults for the others:
+
+    >>> from lgdo.utils import numba_defaults as nb_defaults
+    >>> @guvectorize([], "", **nb_defaults(cache=False) # def proc(...): ...
+
+    Override global options at runtime:
+
+    >>> from lgdo.utils import numba_defaults
+    >>> # must set options before explicitly importing lgdo modules!
+    >>> numba_defaults.cache = False
+    >>> numba_defaults.boundscheck = True
+    >>> from lgdo import compression # imports of numbified functions happen here
+    >>> compression.encode(...)
     """
 
-    def __init__(
-        self,
-        obj_dict: dict[str, LGDO] | None = None,
-        attrs: dict[str, Any] | None = None,
-    ) -> None:
-        """
-        Parameters
-        ----------
-        obj_dict
-            instantiate this Struct using the supplied named LGDO's.  Note: no
-            copy is performed, the objects are used directly.
-        attrs
-            a set of user attributes to be carried along with this LGDO.
-        """
-        if obj_dict is not None:
-            self.update(obj_dict)
-
-        super().__init__(attrs)
-
-    def datatype_name(self) -> str:
-        return "struct"
-
-    def form_datatype(self) -> str:
-        return (
-            self.datatype_name() + "{" + ",".join([str(k) for k in self.keys()]) + "}"
-        )
-
-    def update_datatype(self) -> None:
-        self.attrs["datatype"] = self.form_datatype()
-
-    def add_field(self, name: str | int, obj: LGDO) -> None:
-        """Add a field to the table."""
-        super().__setitem__(name, obj)
-        self.update_datatype()
-
-    def __setitem__(self, name: str, obj: LGDO) -> None:
-        return self.add_field(name, obj)
-
-    def __getattr__(self, name: str) -> LGDO:
-        if hasattr(super(), name):
-            return super().__getattr__(name)
-
-        if name in self.keys():
-            return super().__getitem__(name)
-
-        raise AttributeError(name)
-
-    def remove_field(self, name: str | int, delete: bool = False) -> None:
-        """Remove a field from the table.
-
-        Parameters
-        ----------
-        name
-            name of the field to be removed.
-        delete
-            if ``True``, delete the field object by calling :any:`del`.
-        """
-        if delete:
-            del self[name]
-        else:
-            self.pop(name)
-        self.update_datatype()
+    def __init__(self) -> None:
+        self.cache: bool = getenv_bool("LGDO_CACHE", default=True)
+        self.boundscheck: bool = getenv_bool("LGDO_BOUNDSCHECK", default=False)
 
-    def __str__(self) -> str:
-        """Convert to string (e.g. for printing)."""
+    def __getitem__(self, item: str) -> Any:
+        return self.__dict__[item]
 
-        thr_orig = np.get_printoptions()["threshold"]
-        np.set_printoptions(threshold=8)
+    def __setitem__(self, item: str, val: Any) -> None:
+        self.__dict__[item] = val
 
-        string = "{\n"
-        for k, v in self.items():
-            if "\n" in str(v):
-                rv = str(v).replace("\n", "\n    ")
-                string += f" '{k}':\n    {rv},\n"
-            else:
-                string += f" '{k}': {v},\n"
-        string += "}"
-
-        attrs = self.getattrs()
-        if attrs:
-            string += f" with attrs={attrs}"
+    def __delitem__(self, item: str) -> None:
+        del self.__dict__[item]
 
-        np.set_printoptions(threshold=thr_orig)
+    def __iter__(self) -> Iterator:
+        return self.__dict__.__iter__()
 
-        return string
+    def __len__(self) -> int:
+        return len(self.__dict__)
+
+    def __call__(self, **kwargs) -> dict:
+        mapping = self.__dict__.copy()
+        mapping.update(**kwargs)
+        return mapping
+
+    def __str__(self) -> str:
+        return str(self.__dict__)
 
     def __repr__(self) -> str:
-        npopt = np.get_printoptions()
-        np.set_printoptions(threshold=5, edgeitems=2, linewidth=100)
-        out = (
-            self.__class__.__name__
-            + "(dict="
-            + dict.__repr__(self)
-            + f", attrs={self.attrs!r})"
-        )
-        np.set_printoptions(**npopt)
-        return " ".join(out.replace("\n", " ").split())
-
-    def view_as(self) -> None:
-        r"""View the Struct data as a third-party format data structure.
-
-        Error
-        -----
-        Not implemented. Since Struct's fields can have different lengths,
-        converting to a NumPy, Pandas or Awkward is generally not possible.
-        Call :meth:`.LGDO.view_as` on the fields instead.
-
-        See Also
-        --------
-        .LGDO.view_as
-        """
-        msg = (
-            "Since Struct's fields can have different lengths, "
-            "converting to a NumPy, Pandas or Awkward is generally "
-            "not possible. Call view_as() on the fields instead."
-        )
-        raise NotImplementedError(msg)
+        return str(self.__dict__)
+
+
+numba_defaults = NumbaDefaults()
+numba_defaults_kwargs = numba_defaults
```

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/table.py` & `legend_pydataobj-1.7.0/src/lgdo/types/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,48 +38,57 @@
     If you write to a table and don't fill it up to its total size, be sure to
     resize it before passing to data processing functions, as they will call
     :meth:`__len__` to access valid data, which returns the ``size`` attribute.
     """
 
     def __init__(
         self,
+        col_dict: Mapping[str, LGDO] | pd.DataFrame | ak.Array | None = None,
         size: int | None = None,
-        col_dict: dict[str, LGDO] | None = None,
-        attrs: dict[str, Any] | None = None,
+        attrs: Mapping[str, Any] | None = None,
     ) -> None:
         r"""
         Parameters
         ----------
         size
             sets the number of rows in the table. :class:`.Array`\ s in
             `col_dict will be resized to match size if both are not ``None``.
             If `size` is left as ``None``, the number of table rows is
             determined from the length of the first array in `col_dict`. If
             neither is provided, a default length of 1024 is used.
         col_dict
-            instantiate this table using the supplied named array-like LGDO's.
-            Note 1: no copy is performed, the objects are used directly.
-            Note 2: if `size` is not ``None``, all arrays will be resized to
-            match it.  Note 3: if the arrays have different lengths, all will
-            be resized to match the length of the first array.
+            instantiate this table using the supplied mapping of column names
+            and array-like objects. Supported input types are: mapping of
+            strings to LGDOs, :class:`pd.DataFrame` and :class:`ak.Array`.
+            Note 1: no copy is performed, the objects are used directly (unless
+            :class:`ak.Array` is provided).  Note 2: if `size` is not ``None``,
+            all arrays will be resized to match it.  Note 3: if the arrays have
+            different lengths, all will be resized to match the length of the
+            first array.
         attrs
             A set of user attributes to be carried along with this LGDO.
 
         Notes
         -----
         the :attr:`loc` attribute is initialized to 0.
         """
+        if isinstance(col_dict, pd.DataFrame):
+            col_dict = {k: Array(v) for k, v in col_dict.items()}
+
+        if isinstance(col_dict, ak.Array):
+            col_dict = _ak_to_lgdo_or_col_dict(col_dict)
+
+        # call Struct constructor
         super().__init__(obj_dict=col_dict, attrs=attrs)
 
         # if col_dict is not empty, set size according to it
         # if size is also supplied, resize all fields to match it
         # otherwise, warn if the supplied fields have varying size
         if col_dict is not None and len(col_dict) > 0:
-            do_warn = size is None
-            self.resize(new_size=size, do_warn=do_warn)
+            self.resize(new_size=size, do_warn=(size is None))
 
         # if no col_dict, just set the size (default to 1024)
         else:
             self.size = size if size is not None else None
 
         # always start at loc=0
         self.loc = 0
@@ -475,7 +484,15 @@
             # NOTE: passing the Table directly (which inherits from a dict)
             # makes it somehow really slow. Not sure why, but this could be due
             # to extra LGDO fields (like "attrs")
             return ak.Array({col: self[col].view_as("ak") for col in cols})
 
         msg = f"{library!r} is not a supported third-party format."
         raise TypeError(msg)
+
+
+def _ak_to_lgdo_or_col_dict(array: ak.Array):
+    if isinstance(array.type.content, ak.types.RecordType):
+        return {field: _ak_to_lgdo_or_col_dict(array[field]) for field in array.fields}
+    if isinstance(array.type.content, ak.types.NumpyType):
+        return Array(ak.to_numpy(array))
+    return VectorOfVectors(array)
```

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/vectorofvectors.py` & `legend_pydataobj-1.7.0/src/lgdo/types/vectorofvectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,34 +298,31 @@
         >>> vov = VectorOfVectors([[1, 2], [3], [4, 5]])
         >>> vov.resize(2)
         >>> print(vov)
         [[1 2],
          [3],
         ]
         """
-        if self.ndim == 2:
-            vidx = self.cumulative_length
-            old_s = len(self)
-            dlen = new_size - old_s
-            csum = vidx[-1] if len(self) > 0 else 0
+        vidx = self.cumulative_length
+        old_s = len(self)
+        dlen = new_size - old_s
+        csum = vidx[-1] if len(self) > 0 else 0
 
-            # first resize the cumulative length
-            self.cumulative_length.resize(new_size)
+        # first resize the cumulative length
+        self.cumulative_length.resize(new_size)
 
-            # if new_size > size, new elements are filled with zeros, let's fix
-            # that
-            if dlen > 0:
-                self.cumulative_length[old_s:] = csum
+        # if new_size > size, new elements are filled with zeros, let's fix
+        # that
+        if dlen > 0:
+            self.cumulative_length[old_s:] = csum
 
-            # then resize the data array
-            # if dlen > 0 this has no effect
-            if len(self.cumulative_length) > 0:
-                self.flattened_data.resize(self.cumulative_length[-1])
-        else:
-            raise NotImplementedError
+        # then resize the data array
+        # if dlen > 0 this has no effect
+        if len(self.cumulative_length) > 0:
+            self.flattened_data.resize(self.cumulative_length[-1])
 
     def append(self, new: NDArray) -> None:
         """Append a 1D vector `new` at the end.
 
         Examples
         --------
         >>> vov = VectorOfVectors([[1, 2, 3], [4, 5]])
```

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/vovutils.py` & `legend_pydataobj-1.7.0/src/lgdo/types/vovutils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/src/lgdo/types/waveformtable.py` & `legend_pydataobj-1.7.0/src/lgdo/types/waveformtable.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat` & `legend_pydataobj-1.7.0/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/compression/sigcompress/special-wf-clipped.dat` & `legend_pydataobj-1.7.0/tests/compression/sigcompress/special-wf-clipped.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/compression/test_compression.py` & `legend_pydataobj-1.7.0/tests/compression/test_compression.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/compression/test_radware_sigcompress.py` & `legend_pydataobj-1.7.0/tests/compression/test_radware_sigcompress.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/compression/test_str2wfcodec.py` & `legend_pydataobj-1.7.0/tests/compression/test_str2wfcodec.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/compression/test_uleb128_zigzag_diff.py` & `legend_pydataobj-1.7.0/tests/compression/test_uleb128_zigzag_diff.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/conftest.py` & `legend_pydataobj-1.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/conftest.py` & `legend_pydataobj-1.7.0/tests/lh5/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/test_core.py` & `legend_pydataobj-1.7.0/tests/lh5/test_core.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/test_lh5_datatype.py` & `legend_pydataobj-1.7.0/tests/lh5/test_lh5_datatype.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/test_lh5_iterator.py` & `legend_pydataobj-1.7.0/tests/lh5/test_lh5_iterator.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/test_lh5_store.py` & `legend_pydataobj-1.7.0/tests/lh5/test_lh5_store.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/test_lh5_tools.py` & `legend_pydataobj-1.7.0/tests/lh5/test_lh5_tools.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/test_lh5_utils.py` & `legend_pydataobj-1.7.0/tests/lh5/test_lh5_utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/lh5/test_lh5_write.py` & `legend_pydataobj-1.7.0/tests/lh5/test_lh5_write.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/test_cli.py` & `legend_pydataobj-1.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_array.py` & `legend_pydataobj-1.7.0/tests/types/test_array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_arrayofequalsizedarrays.py` & `legend_pydataobj-1.7.0/tests/types/test_arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_encoded.py` & `legend_pydataobj-1.7.0/tests/types/test_encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_fixedsizearray.py` & `legend_pydataobj-1.7.0/tests/types/test_fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_representations.py` & `legend_pydataobj-1.7.0/tests/types/test_representations.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_scalar.py` & `legend_pydataobj-1.7.0/tests/types/test_scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_table.py` & `legend_pydataobj-1.7.0/tests/types/test_table.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,14 +27,56 @@
     tbl = Table(col_dict=col_dict)
     assert tbl.size == 4
 
     tbl = Table(size=3, col_dict=col_dict)
     assert tbl.size == 3
 
 
+def test_init_nested():
+    col_dict = {
+        "a": lgdo.Array(nda=np.array([1, 2, 3, 4])),
+        "b": lgdo.Array(nda=np.array([5, 6, 7, 8])),
+        "c": {
+            "f1": lgdo.Array([1, 2, 3, 4]),
+            "f2": lgdo.Array([1, 2, 3, 4]),
+        },
+    }
+
+    tbl = Table(col_dict=col_dict)
+    assert isinstance(tbl.c, Table)
+    assert isinstance(tbl.c.f1, lgdo.Array)
+    assert tbl.c.f1 == lgdo.Array([1, 2, 3, 4])
+
+
+def test_pandas_df_init():
+    df = pd.DataFrame({"a": [1, 2, 3, 4], "b": [5, 6, 7, 8]})
+    tbl = Table(col_dict=df)
+    assert sorted(tbl.keys()) == ["a", "b"]
+    assert isinstance(tbl.a, lgdo.Array)
+    assert isinstance(tbl.b, lgdo.Array)
+    assert tbl.a == lgdo.Array([1, 2, 3, 4])
+    assert tbl.b == lgdo.Array([5, 6, 7, 8])
+
+
+def test_ak_array_init():
+    array = ak.Array(
+        {
+            "a": [1, 2, 3, 4],
+            "b": [[1, 2], [3], [4], [5, 6, 7]],
+            "c": {"f1": [[], [5], [3, 7, 6], []], "f2": [5, 6, 7, 8]},
+        }
+    )
+    tbl = Table(array)
+    assert isinstance(tbl.a, lgdo.Array)
+    assert isinstance(tbl.b, lgdo.VectorOfVectors)
+    assert isinstance(tbl.c, Table)
+    assert isinstance(tbl.c.f1, lgdo.VectorOfVectors)
+    assert isinstance(tbl.c.f2, lgdo.Array)
+
+
 def test_datatype_name():
     tbl = Table()
     assert tbl.datatype_name() == "table"
 
 
 def test_push_row():
     tbl = Table()
@@ -91,15 +133,15 @@
     assert list(tbl1.keys()) == ["a", "b", "c", "d"]
 
     tbl2.join(tbl1, cols=("a"))
     assert list(tbl2.keys()) == ["c", "d", "a"]
 
 
 def test_view_as():
-    tbl = Table(3)
+    tbl = Table(size=3)
     tbl.add_column("a", lgdo.Array(np.array([1, 2, 3]), attrs={"units": "m"}))
     tbl.add_column("b", lgdo.Array(np.array([[0, 1, 2], [3, 4, 5], [6, 7, 8]])))
     tbl.add_column(
         "c",
         lgdo.VectorOfVectors(
             flattened_data=lgdo.Array(np.array([0, 1, 2, 3, 4, 5, 6])),
             cumulative_length=lgdo.Array(np.array([3, 4, 7])),
```

### Comparing `legend_pydataobj-1.6.2/tests/types/test_table_eval.py` & `legend_pydataobj-1.7.0/tests/types/test_table_eval.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_vectorofvectors.py` & `legend_pydataobj-1.7.0/tests/types/test_vectorofvectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,28 +170,45 @@
     assert np.array_equal(testvov[-2], desired[-2])
 
     v = VectorOfVectors([[1, 2]], dtype="uint32")
     assert np.array_equal(v[-1], [1, 2])
 
 
 def test_resize(testvov):
-    testvov = testvov.v2d
+    vov = testvov.v2d
 
-    testvov.resize(3)
-    assert ak.is_valid(testvov.view_as("ak"))
-    assert len(testvov.cumulative_length) == 3
-    assert len(testvov.flattened_data) == testvov.cumulative_length[-1]
-    assert testvov == VectorOfVectors([[1, 2], [3, 4, 5], [2]])
-
-    testvov.resize(5)
-    assert ak.is_valid(testvov.view_as("ak"))
-    assert len(testvov) == 5
-    assert len(testvov[3]) == 0
-    assert len(testvov[4]) == 0
-    assert testvov == VectorOfVectors([[1, 2], [3, 4, 5], [2], [], []])
+    vov.resize(3)
+    assert ak.is_valid(vov.view_as("ak"))
+    assert len(vov.cumulative_length) == 3
+    assert len(vov.flattened_data) == vov.cumulative_length[-1]
+    assert vov == VectorOfVectors([[1, 2], [3, 4, 5], [2]])
+
+    vov.resize(5)
+    assert ak.is_valid(vov.view_as("ak"))
+    assert len(vov) == 5
+    assert len(vov[3]) == 0
+    assert len(vov[4]) == 0
+    assert vov == VectorOfVectors([[1, 2], [3, 4, 5], [2], [], []])
+
+    vov = testvov.v3d
+
+    vov.resize(3)
+    assert ak.is_valid(vov.view_as("ak"))
+    assert len(vov.cumulative_length) == 3
+    assert len(vov.flattened_data) == vov.cumulative_length[-1]
+    assert vov == VectorOfVectors(
+        [[[1, 2], [3, 4, 5]], [[2], [4, 8, 9, 7]], [[5, 3, 1]]]
+    )
+
+    vov.resize(5)
+    assert ak.is_valid(vov.view_as("ak"))
+    assert len(vov) == 5
+    assert vov == VectorOfVectors(
+        [[[1, 2], [3, 4, 5]], [[2], [4, 8, 9, 7]], [[5, 3, 1]], [], []]
+    )
 
     v = VectorOfVectors(dtype="i")
     v.resize(3)
     assert ak.is_valid(v.view_as("ak"))
     assert v == VectorOfVectors([[], [], []], dtype="i")
```

### Comparing `legend_pydataobj-1.6.2/tests/types/test_vovutils.py` & `legend_pydataobj-1.7.0/tests/types/test_vovutils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.2/tests/types/test_waveformtable.py` & `legend_pydataobj-1.7.0/tests/types/test_waveformtable.py`

 * *Files identical despite different names*


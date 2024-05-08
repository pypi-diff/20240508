# Comparing `tmp/satsure_core_test-0.0.1.tar.gz` & `tmp/satsure_core_test-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure_core_test-0.0.1.tar", last modified: Thu May  2 12:47:43 2024, max compression
+gzip compressed data, was "satsure_core_test-0.0.3.tar", last modified: Wed May  8 07:12:56 2024, max compression
```

## Comparing `satsure_core_test-0.0.1.tar` & `satsure_core_test-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,38 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-02 12:47:43.113031 satsure_core_test-0.0.1/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.0.1/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      308 2024-05-02 12:47:43.112828 satsure_core_test-0.0.1/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.0.1/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-02 12:47:43.110142 satsure_core_test-0.0.1/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-02 10:11:43.000000 satsure_core_test-0.0.1/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      629 2024-05-02 12:30:26.000000 satsure_core_test-0.0.1/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-02 12:47:43.111300 satsure_core_test-0.0.1/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      157 2024-05-02 12:36:28.000000 satsure_core_test-0.0.1/satelite/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2427 2024-05-02 09:49:02.000000 satsure_core_test-0.0.1/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-02 09:49:23.000000 satsure_core_test-0.0.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2994 2024-05-02 12:36:28.000000 satsure_core_test-0.0.1/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-02 12:47:43.112420 satsure_core_test-0.0.1/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      308 2024-05-02 12:47:43.000000 satsure_core_test-0.0.1/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      434 2024-05-02 12:47:43.000000 satsure_core_test-0.0.1/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-02 12:47:43.000000 satsure_core_test-0.0.1/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       54 2024-05-02 12:47:43.000000 satsure_core_test-0.0.1/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-02 12:47:43.000000 satsure_core_test-0.0.1/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-02 12:47:43.113080 satsure_core_test-0.0.1/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      351 2024-05-02 12:46:55.000000 satsure_core_test-0.0.1/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.614240 satsure_core_test-0.0.3/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.0.3/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      753 2024-05-08 07:12:56.614058 satsure_core_test-0.0.3/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.0.3/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.607600 satsure_core_test-0.0.3/qa_qc_check/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.609090 satsure_core_test-0.0.3/qa_qc_check/controller/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/controller/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4047 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/controller/checks.json
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4179 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/controller/meta_data.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3616 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/controller/meta_data_extractor.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1886 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/controller/meta_data_validator.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      887 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/controller/metadata_model.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1494 2024-05-08 07:07:59.000000 satsure_core_test-0.0.3/qa_qc_check/controller/qa_qc.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.609324 satsure_core_test-0.0.3/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.0.3/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      629 2024-05-07 12:57:11.000000 satsure_core_test-0.0.3/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.610596 satsure_core_test-0.0.3/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      157 2024-05-08 07:05:28.000000 satsure_core_test-0.0.3/satelite/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2427 2024-05-06 07:15:52.000000 satsure_core_test-0.0.3/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.0.3/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2994 2024-05-08 07:05:28.000000 satsure_core_test-0.0.3/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.611252 satsure_core_test-0.0.3/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:05:28.000000 satsure_core_test-0.0.3/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      747 2024-05-06 07:43:01.000000 satsure_core_test-0.0.3/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.612743 satsure_core_test-0.0.3/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:05:28.000000 satsure_core_test-0.0.3/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-06 07:43:01.000000 satsure_core_test-0.0.3/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.0.3/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1322 2024-05-06 07:34:13.000000 satsure_core_test-0.0.3/satelite/tests/sentinel2/test_get_tile.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-08 07:12:56.613716 satsure_core_test-0.0.3/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      753 2024-05-08 07:12:56.000000 satsure_core_test-0.0.3/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      981 2024-05-08 07:12:56.000000 satsure_core_test-0.0.3/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-08 07:12:56.000000 satsure_core_test-0.0.3/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      289 2024-05-08 07:12:56.000000 satsure_core_test-0.0.3/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       21 2024-05-08 07:12:56.000000 satsure_core_test-0.0.3/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-08 07:12:56.614289 satsure_core_test-0.0.3/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      845 2024-05-08 07:11:49.000000 satsure_core_test-0.0.3/setup.py
```

### Comparing `satsure_core_test-0.0.1/satelite/config.py` & `satsure_core_test-0.0.3/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.1/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure_core_test-0.0.3/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure_core_test-0.0.3/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.1/satelite/sentinel2/get_tiles.py` & `satsure_core_test-0.0.3/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*


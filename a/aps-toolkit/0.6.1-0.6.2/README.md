# Comparing `tmp/aps-toolkit-0.6.1.tar.gz` & `tmp/aps-toolkit-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.6.1.tar", last modified: Wed May  8 09:12:49 2024, max compression
+gzip compressed data, was "aps-toolkit-0.6.2.tar", last modified: Wed May  8 09:51:52 2024, max compression
```

## Comparing `aps-toolkit-0.6.1.tar` & `aps-toolkit-0.6.2.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.772856 aps-toolkit-0.6.1/
--rw-rw-rw-   0        0        0     1990 2024-05-08 09:12:49.771856 aps-toolkit-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 09:12:49.772856 aps-toolkit-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-05-08 09:12:17.000000 aps-toolkit-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.722872 aps-toolkit-0.6.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.752862 aps-toolkit-0.6.1/src/aps_toolkit/
--rw-rw-rw-   0        0        0    12938 2024-05-08 09:07:20.000000 aps-toolkit-0.6.1/src/aps_toolkit/Auth.py
--rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.6.1/src/aps_toolkit/AuthGoogleColab.py
--rw-rw-rw-   0        0        0    16333 2024-05-08 08:57:37.000000 aps-toolkit-0.6.1/src/aps_toolkit/BIM360.py
--rw-rw-rw-   0        0        0     9073 2024-05-08 09:08:48.000000 aps-toolkit-0.6.1/src/aps_toolkit/Bucket.py
--rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.6.1/src/aps_toolkit/DbReader.py
--rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.6.1/src/aps_toolkit/Derivative.py
--rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.6.1/src/aps_toolkit/Fragments.py
--rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/InputStream.py
--rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/ManifestItem.py
--rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/MaterialProperties.py
--rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/Materials.py
--rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/PackFileReader.py
--rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/PathInfo.py
--rw-rw-rw-   0        0        0     4591 2024-05-08 09:11:24.000000 aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderCad.py
--rw-rw-rw-   0        0        0     3602 2024-05-08 09:11:08.000000 aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderNavis.py
--rw-rw-rw-   0        0        0    21677 2024-05-08 09:01:33.000000 aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderRevit.py
--rw-rw-rw-   0        0        0    16114 2024-05-08 09:02:52.000000 aps-toolkit-0.6.1/src/aps_toolkit/PropReader.py
--rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.6.1/src/aps_toolkit/Resource.py
--rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFContent.py
--rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFGeometries.py
--rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFImage.py
--rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFLines.py
--rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFManifestType.py
--rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialGroup.py
--rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMap.py
--rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMapScale.py
--rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterials.py
--rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMesh.py
--rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMetadata.py
--rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFPoints.py
--rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFReader.py
--rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFTransform.py
--rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFUVMap.py
--rw-rw-rw-   0        0        0     1032 2024-05-08 09:09:27.000000 aps-toolkit-0.6.1/src/aps_toolkit/Token.py
--rw-rw-rw-   0        0        0      813 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/aps_toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.757869 aps-toolkit-0.6.1/src/aps_toolkit/units/
--rw-rw-rw-   0        0        0     1481 2024-05-08 09:12:04.000000 aps-toolkit-0.6.1/src/aps_toolkit/units/DisplayUnits.py
--rw-rw-rw-   0        0        0        0 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/aps_toolkit/units/__init__.py
--rw-rw-rw-   0        0        0    38555 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/aps_toolkit/units/units.json
-drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.755862 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1890 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.771856 aps-toolkit-0.6.1/src/test/
--rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.6.1/src/test/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/test/context.py
--rw-rw-rw-   0        0        0     2006 2024-05-08 07:26:15.000000 aps-toolkit-0.6.1/src/test/test_auth.py
--rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.6.1/src/test/test_auth_colab.py
--rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.6.1/src/test/test_bim360.py
--rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.6.1/src/test/test_bucket.py
--rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.6.1/src/test/test_db_reader.py
--rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.6.1/src/test/test_derivative.py
--rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_fragment.py
--rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_geometries.py
--rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_image.py
--rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_material.py
--rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_mesh.py
--rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_metadata.py
--rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.6.1/src/test/test_prop_reader.py
--rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_prop_reader_cad.py
--rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.6.1/src/test/test_prop_reader_navis.py
--rw-rw-rw-   0        0        0     3516 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/test/test_prop_reader_revit.py
--rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_svf_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:51:52.404227 aps-toolkit-0.6.2/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 09:51:52.403227 aps-toolkit-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 09:51:52.404227 aps-toolkit-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2024-05-08 09:51:45.000000 aps-toolkit-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:51:52.354263 aps-toolkit-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 09:51:52.384233 aps-toolkit-0.6.2/src/aps_toolkit/
+-rw-rw-rw-   0        0        0    12938 2024-05-08 09:41:59.000000 aps-toolkit-0.6.2/src/aps_toolkit/Auth.py
+-rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.6.2/src/aps_toolkit/AuthGoogleColab.py
+-rw-rw-rw-   0        0        0    16333 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/BIM360.py
+-rw-rw-rw-   0        0        0     9073 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/Bucket.py
+-rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.6.2/src/aps_toolkit/DbReader.py
+-rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.6.2/src/aps_toolkit/Derivative.py
+-rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.6.2/src/aps_toolkit/Fragments.py
+-rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/InputStream.py
+-rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/aps_toolkit/ManifestItem.py
+-rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/MaterialProperties.py
+-rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/Materials.py
+-rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/PackFileReader.py
+-rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/aps_toolkit/PathInfo.py
+-rw-rw-rw-   0        0        0     4591 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/ProDbReaderCad.py
+-rw-rw-rw-   0        0        0     3602 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/ProDbReaderNavis.py
+-rw-rw-rw-   0        0        0    21677 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/ProDbReaderRevit.py
+-rw-rw-rw-   0        0        0    16114 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/PropReader.py
+-rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.6.2/src/aps_toolkit/Resource.py
+-rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFContent.py
+-rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFGeometries.py
+-rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFImage.py
+-rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFLines.py
+-rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFManifestType.py
+-rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterialGroup.py
+-rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterialMap.py
+-rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterials.py
+-rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFMesh.py
+-rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFMetadata.py
+-rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFPoints.py
+-rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFReader.py
+-rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFTransform.py
+-rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/SVFUVMap.py
+-rw-rw-rw-   0        0        0     1032 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/Token.py
+-rw-rw-rw-   0        0        0     5076 2024-05-08 09:51:14.000000 aps-toolkit-0.6.2/src/aps_toolkit/Webhooks.py
+-rw-rw-rw-   0        0        0      845 2024-05-08 09:51:14.000000 aps-toolkit-0.6.2/src/aps_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:51:52.389227 aps-toolkit-0.6.2/src/aps_toolkit/units/
+-rw-rw-rw-   0        0        0     1481 2024-05-08 09:45:28.000000 aps-toolkit-0.6.2/src/aps_toolkit/units/DisplayUnits.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/units/__init__.py
+-rw-rw-rw-   0        0        0    38555 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/aps_toolkit/units/units.json
+drwxrwxrwx   0        0        0        0 2024-05-08 09:51:52.387225 aps-toolkit-0.6.2/src/aps_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 09:51:51.000000 aps-toolkit-0.6.2/src/aps_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1944 2024-05-08 09:51:51.000000 aps-toolkit-0.6.2/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 09:51:51.000000 aps-toolkit-0.6.2/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 09:51:51.000000 aps-toolkit-0.6.2/src/aps_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 09:51:51.000000 aps-toolkit-0.6.2/src/aps_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 09:51:52.402228 aps-toolkit-0.6.2/src/test/
+-rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.6.2/src/test/__init__.py
+-rw-rw-rw-   0        0        0     1093 2024-05-08 09:51:14.000000 aps-toolkit-0.6.2/src/test/context.py
+-rw-rw-rw-   0        0        0     1381 2024-05-08 09:51:14.000000 aps-toolkit-0.6.2/src/test/test_Webhooks.py
+-rw-rw-rw-   0        0        0     2006 2024-05-08 07:26:15.000000 aps-toolkit-0.6.2/src/test/test_auth.py
+-rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.6.2/src/test/test_auth_colab.py
+-rw-rw-rw-   0        0        0     2734 2024-05-08 09:40:51.000000 aps-toolkit-0.6.2/src/test/test_bim360.py
+-rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.6.2/src/test/test_bucket.py
+-rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.6.2/src/test/test_db_reader.py
+-rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.6.2/src/test/test_derivative.py
+-rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.6.2/src/test/test_fragment.py
+-rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.6.2/src/test/test_geometries.py
+-rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/test/test_image.py
+-rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.6.2/src/test/test_material.py
+-rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.6.2/src/test/test_mesh.py
+-rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/test/test_metadata.py
+-rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.6.2/src/test/test_prop_reader.py
+-rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/test/test_prop_reader_cad.py
+-rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.6.2/src/test/test_prop_reader_navis.py
+-rw-rw-rw-   0        0        0     3516 2024-05-08 09:41:50.000000 aps-toolkit-0.6.2/src/test/test_prop_reader_revit.py
+-rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.6.2/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.6.1/PKG-INFO` & `aps-toolkit-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.1/setup.py` & `aps-toolkit-0.6.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.6.1",
+    version="0.6.2",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
```

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/Auth.py` & `aps-toolkit-0.6.2/src/aps_toolkit/Auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/AuthGoogleColab.py` & `aps-toolkit-0.6.2/src/aps_toolkit/AuthGoogleColab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.6.2/src/aps_toolkit/BIM360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.6.2/src/aps_toolkit/Bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.6.2/src/aps_toolkit/DbReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.6.2/src/aps_toolkit/Derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.6.2/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.6.2/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.6.2/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.6.2/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/Materials.py` & `aps-toolkit-0.6.2/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.6.2/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.6.2/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.6.2/src/aps_toolkit/ProDbReaderCad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.6.2/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.6.2/src/aps_toolkit/ProDbReaderRevit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.6.2/src/aps_toolkit/PropReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/Resource.py` & `aps-toolkit-0.6.2/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.6.2/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/Token.py` & `aps-toolkit-0.6.2/src/aps_toolkit/Token.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/__init__.py` & `aps-toolkit-0.6.2/src/aps_toolkit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 from .Derivative import Derivative
 from .Fragments import Fragments
 from .SVFGeometries import SVFGeometries
 from .SVFMesh import SVFMesh
 from .SVFMaterials import SVFMaterials
 from .SVFImage import SVFImage
 from .SVFMetadata import SVFMetadata
+from .Webhooks import Webhooks
```

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/units/DisplayUnits.py` & `aps-toolkit-0.6.2/src/aps_toolkit/units/DisplayUnits.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit/units/units.json` & `aps-toolkit-0.6.2/src/aps_toolkit/units/units.json`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.6.2/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.1/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.6.2/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,25 +29,27 @@
 src/aps_toolkit/SVFMesh.py
 src/aps_toolkit/SVFMetadata.py
 src/aps_toolkit/SVFPoints.py
 src/aps_toolkit/SVFReader.py
 src/aps_toolkit/SVFTransform.py
 src/aps_toolkit/SVFUVMap.py
 src/aps_toolkit/Token.py
+src/aps_toolkit/Webhooks.py
 src/aps_toolkit/__init__.py
 src/aps_toolkit.egg-info/PKG-INFO
 src/aps_toolkit.egg-info/SOURCES.txt
 src/aps_toolkit.egg-info/dependency_links.txt
 src/aps_toolkit.egg-info/requires.txt
 src/aps_toolkit.egg-info/top_level.txt
 src/aps_toolkit/units/DisplayUnits.py
 src/aps_toolkit/units/__init__.py
 src/aps_toolkit/units/units.json
 src/test/__init__.py
 src/test/context.py
+src/test/test_Webhooks.py
 src/test/test_auth.py
 src/test/test_auth_colab.py
 src/test/test_bim360.py
 src/test/test_bucket.py
 src/test/test_db_reader.py
 src/test/test_derivative.py
 src/test/test_fragment.py
```

### Comparing `aps-toolkit-0.6.1/src/test/context.py` & `aps-toolkit-0.6.2/src/test/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 from aps_toolkit import Derivative
 from aps_toolkit import SVFReader
 from aps_toolkit import SVFMaterials
 from aps_toolkit import SVFImage
 from aps_toolkit import SVFMetadata
 from aps_toolkit import Bucket
 from aps_toolkit.units import DisplayUnits
+from aps_toolkit import Webhooks
 
 APS_CLIENT_ID = os.environ["APS_CLIENT_ID"]
 APS_CLIENT_SECRET = os.environ["APS_CLIENT_SECRET"]
```

### Comparing `aps-toolkit-0.6.1/src/test/test_auth.py` & `aps-toolkit-0.6.2/src/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_auth_colab.py` & `aps-toolkit-0.6.2/src/test/test_auth_colab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_bim360.py` & `aps-toolkit-0.6.2/src/test/test_bim360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_bucket.py` & `aps-toolkit-0.6.2/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_db_reader.py` & `aps-toolkit-0.6.2/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_derivative.py` & `aps-toolkit-0.6.2/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_fragment.py` & `aps-toolkit-0.6.2/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_geometries.py` & `aps-toolkit-0.6.2/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_image.py` & `aps-toolkit-0.6.2/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_material.py` & `aps-toolkit-0.6.2/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_mesh.py` & `aps-toolkit-0.6.2/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_prop_reader.py` & `aps-toolkit-0.6.2/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.6.2/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.6.2/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.6.2/src/test/test_prop_reader_revit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.1/src/test/test_svf_reader.py` & `aps-toolkit-0.6.2/src/test/test_svf_reader.py`

 * *Files identical despite different names*


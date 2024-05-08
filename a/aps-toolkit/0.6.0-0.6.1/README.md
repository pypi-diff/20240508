# Comparing `tmp/aps-toolkit-0.6.0.tar.gz` & `tmp/aps-toolkit-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.6.0.tar", last modified: Wed May  8 07:39:11 2024, max compression
+gzip compressed data, was "aps-toolkit-0.6.1.tar", last modified: Wed May  8 09:12:49 2024, max compression
```

## Comparing `aps-toolkit-0.6.0.tar` & `aps-toolkit-0.6.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.408698 aps-toolkit-0.6.0/
--rw-rw-rw-   0        0        0     1990 2024-05-08 07:39:11.407700 aps-toolkit-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 07:39:11.408698 aps-toolkit-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-05-08 07:38:56.000000 aps-toolkit-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.295759 aps-toolkit-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.373700 aps-toolkit-0.6.0/src/aps_toolkit/
--rw-rw-rw-   0        0        0    12872 2024-05-08 07:37:37.000000 aps-toolkit-0.6.0/src/aps_toolkit/Auth.py
--rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.6.0/src/aps_toolkit/AuthGoogleColab.py
--rw-rw-rw-   0        0        0    10333 2024-03-27 07:53:22.000000 aps-toolkit-0.6.0/src/aps_toolkit/BIM360.py
--rw-rw-rw-   0        0        0     9081 2024-04-01 02:00:06.000000 aps-toolkit-0.6.0/src/aps_toolkit/Bucket.py
--rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.6.0/src/aps_toolkit/DbReader.py
--rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.6.0/src/aps_toolkit/Derivative.py
--rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.6.0/src/aps_toolkit/Fragments.py
--rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/InputStream.py
--rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/ManifestItem.py
--rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/MaterialProperties.py
--rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/Materials.py
--rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/PackFileReader.py
--rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/PathInfo.py
--rw-rw-rw-   0        0        0     4586 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderCad.py
--rw-rw-rw-   0        0        0     3592 2024-03-25 01:46:50.000000 aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderNavis.py
--rw-rw-rw-   0        0        0    15835 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderRevit.py
--rw-rw-rw-   0        0        0    13956 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/PropReader.py
--rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.6.0/src/aps_toolkit/Resource.py
--rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFContent.py
--rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFGeometries.py
--rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFImage.py
--rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFLines.py
--rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFManifestType.py
--rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialGroup.py
--rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMap.py
--rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMapScale.py
--rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterials.py
--rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMesh.py
--rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMetadata.py
--rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFPoints.py
--rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFReader.py
--rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFTransform.py
--rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFUVMap.py
--rw-rw-rw-   0        0        0     1010 2024-04-01 02:00:06.000000 aps-toolkit-0.6.0/src/aps_toolkit/Token.py
--rw-rw-rw-   0        0        0      813 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.378699 aps-toolkit-0.6.0/src/aps_toolkit/units/
--rw-rw-rw-   0        0        0     1511 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/units/DisplayUnits.py
--rw-rw-rw-   0        0        0        0 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/units/__init__.py
--rw-rw-rw-   0        0        0    38555 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/units/units.json
-drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.376699 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1890 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.406698 aps-toolkit-0.6.0/src/test/
--rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.6.0/src/test/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/test/context.py
--rw-rw-rw-   0        0        0     2006 2024-05-08 07:26:15.000000 aps-toolkit-0.6.0/src/test/test_auth.py
--rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.6.0/src/test/test_auth_colab.py
--rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.6.0/src/test/test_bim360.py
--rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.6.0/src/test/test_bucket.py
--rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.6.0/src/test/test_db_reader.py
--rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.6.0/src/test/test_derivative.py
--rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_fragment.py
--rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_geometries.py
--rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_image.py
--rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_material.py
--rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_mesh.py
--rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_metadata.py
--rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.6.0/src/test/test_prop_reader.py
--rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_prop_reader_cad.py
--rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.6.0/src/test/test_prop_reader_navis.py
--rw-rw-rw-   0        0        0     3516 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/test/test_prop_reader_revit.py
--rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_svf_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.772856 aps-toolkit-0.6.1/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 09:12:49.771856 aps-toolkit-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 09:12:49.772856 aps-toolkit-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2024-05-08 09:12:17.000000 aps-toolkit-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.722872 aps-toolkit-0.6.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.752862 aps-toolkit-0.6.1/src/aps_toolkit/
+-rw-rw-rw-   0        0        0    12938 2024-05-08 09:07:20.000000 aps-toolkit-0.6.1/src/aps_toolkit/Auth.py
+-rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.6.1/src/aps_toolkit/AuthGoogleColab.py
+-rw-rw-rw-   0        0        0    16333 2024-05-08 08:57:37.000000 aps-toolkit-0.6.1/src/aps_toolkit/BIM360.py
+-rw-rw-rw-   0        0        0     9073 2024-05-08 09:08:48.000000 aps-toolkit-0.6.1/src/aps_toolkit/Bucket.py
+-rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.6.1/src/aps_toolkit/DbReader.py
+-rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.6.1/src/aps_toolkit/Derivative.py
+-rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.6.1/src/aps_toolkit/Fragments.py
+-rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/InputStream.py
+-rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/ManifestItem.py
+-rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/MaterialProperties.py
+-rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/Materials.py
+-rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/PackFileReader.py
+-rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/PathInfo.py
+-rw-rw-rw-   0        0        0     4591 2024-05-08 09:11:24.000000 aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderCad.py
+-rw-rw-rw-   0        0        0     3602 2024-05-08 09:11:08.000000 aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderNavis.py
+-rw-rw-rw-   0        0        0    21677 2024-05-08 09:01:33.000000 aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderRevit.py
+-rw-rw-rw-   0        0        0    16114 2024-05-08 09:02:52.000000 aps-toolkit-0.6.1/src/aps_toolkit/PropReader.py
+-rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.6.1/src/aps_toolkit/Resource.py
+-rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFContent.py
+-rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFGeometries.py
+-rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFImage.py
+-rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFLines.py
+-rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFManifestType.py
+-rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialGroup.py
+-rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMap.py
+-rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterials.py
+-rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMesh.py
+-rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFMetadata.py
+-rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFPoints.py
+-rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFReader.py
+-rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFTransform.py
+-rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.6.1/src/aps_toolkit/SVFUVMap.py
+-rw-rw-rw-   0        0        0     1032 2024-05-08 09:09:27.000000 aps-toolkit-0.6.1/src/aps_toolkit/Token.py
+-rw-rw-rw-   0        0        0      813 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/aps_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.757869 aps-toolkit-0.6.1/src/aps_toolkit/units/
+-rw-rw-rw-   0        0        0     1481 2024-05-08 09:12:04.000000 aps-toolkit-0.6.1/src/aps_toolkit/units/DisplayUnits.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/aps_toolkit/units/__init__.py
+-rw-rw-rw-   0        0        0    38555 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/aps_toolkit/units/units.json
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.755862 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 09:12:49.000000 aps-toolkit-0.6.1/src/aps_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:49.771856 aps-toolkit-0.6.1/src/test/
+-rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.6.1/src/test/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/test/context.py
+-rw-rw-rw-   0        0        0     2006 2024-05-08 07:26:15.000000 aps-toolkit-0.6.1/src/test/test_auth.py
+-rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.6.1/src/test/test_auth_colab.py
+-rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.6.1/src/test/test_bim360.py
+-rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.6.1/src/test/test_bucket.py
+-rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.6.1/src/test/test_db_reader.py
+-rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.6.1/src/test/test_derivative.py
+-rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_fragment.py
+-rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_geometries.py
+-rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_image.py
+-rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_material.py
+-rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.6.1/src/test/test_mesh.py
+-rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_metadata.py
+-rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.6.1/src/test/test_prop_reader.py
+-rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_prop_reader_cad.py
+-rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.6.1/src/test/test_prop_reader_navis.py
+-rw-rw-rw-   0        0        0     3516 2024-05-08 07:02:44.000000 aps-toolkit-0.6.1/src/test/test_prop_reader_revit.py
+-rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.6.1/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.6.0/PKG-INFO` & `aps-toolkit-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.0/setup.py` & `aps-toolkit-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.6.0",
+    version="0.6.1",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/Auth.py` & `aps-toolkit-0.6.1/src/aps_toolkit/Auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,15 @@
         self.refresh_token = content.get('refresh_token')
         result = Token(self.access_token, self.token_type, self.expires_in, self.refresh_token)
         return result
 
     def get_user_info(self) -> dict:
         """
         This method is used to get user information.
+        It requires OAuth 2.0 authentication with 3-legged flow.
         https://developer.api.autodesk.com/userprofile/v1/userinfo
         :return:  A dictionary containing user information.
         """
         if not self.access_token:
             raise Exception("Access token is required, please authenticate first. Use auth2leg or auth3leg method.")
         url = "https://api.userprofile.autodesk.com/userinfo"
         headers = {
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/AuthGoogleColab.py` & `aps-toolkit-0.6.1/src/aps_toolkit/AuthGoogleColab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.6.1/src/aps_toolkit/Bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             "policyKey": policy_key.value
         }
         response = requests.post(self.host, headers=headers, json=data)
         if response.status_code != 200:
             raise Exception(response.content)
         return response.json()
 
-    def delete_bucket(self, bucket_name: str) -> dict:
+    def delete_bucket(self, bucket_name: str):
         """
             Deletes a bucket in the Autodesk OSS API.
 
             This method sends a DELETE request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name is passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
 
             Args:
                 bucket_name (str): The name of the bucket to be deleted.
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.6.1/src/aps_toolkit/DbReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.6.1/src/aps_toolkit/Derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.6.1/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.6.1/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.6.1/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.6.1/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/Materials.py` & `aps-toolkit-0.6.1/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.6.1/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.6.1/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderCad.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 for child in childs:
                     properties = self.enumerate_properties(child)
                     for p in properties:
                         if p.name == "type":
                             db_categories[child] = p.value
         return db_categories
 
-    def get_data_by_category(self, category) -> pd.DataFrame:
+    def get_data_by_category(self, category: str) -> pd.DataFrame:
         """
         Get data by cad category : eg: MText, Line, Circle, ...
         :param category: the category name of cad file, e.g : MText, Line, Circle,Tables ...
         :return: pandas dataframe
         """
         db_categories = self.get_all_categories()
         category_ids = [k for k, v in db_categories.items() if v.lower() == category.lower()]
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.6.1/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,21 @@
         categories = []
         rg = re.compile(r'^__\w+__$')
         for i in range(1, len(self.attrs)):
             if self.attrs[i][1] not in categories and not rg.match(self.attrs[i][1]):
                 categories.append(self.attrs[i][1])
         return categories
 
-    def get_data_by_category(self, category) -> pd.DataFrame:
+    def get_data_by_category(self, category: str) -> pd.DataFrame:
         db_ids = [1]
         df = self._get_recursive_ids_by_category(db_ids, category)
         df = df.drop_duplicates(subset=df.columns.difference(['DbId']))
         return df
 
-    def _get_recursive_ids_by_category(self, db_ids: List[int], category) -> pd.DataFrame:
+    def _get_recursive_ids_by_category(self, db_ids: List[int], category: str) -> pd.DataFrame:
         dataframe = pd.DataFrame()
         props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
         if len(db_ids) == 0:
             return dataframe
         for id in db_ids:
             props = self.enumerate_properties(id)
             properties = {}
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.6.1/src/aps_toolkit/PropReader.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         derivative = Derivative(self.urn, self.token, self.region)
         manifest_items = derivative.read_svf_manifest_items()
         if len(manifest_items) > 0:
             self._read_metadata_item(derivative, manifest_items[0])
         else:
             raise Exception("No manifest item found")
 
-    def _read_metadata_item(self, derivative, manifest_item):
+    def _read_metadata_item(self, derivative: Derivative, manifest_item: ManifestItem):
         items = [
             "objects_attrs.json.gz",
             "objects_vals.json.gz",
             "objects_ids.json.gz",
             "objects_offs.json.gz",
             "objects_avs.json.gz",
             "objects_ids.json.gz"
@@ -78,14 +78,19 @@
         self.ids = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_ids.json.gz"]), 'utf-8'))
         self.offsets = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_offs.json.gz"]), 'utf-8'))
         self.avs = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_avs.json.gz"]), 'utf-8'))
         self.attrs = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_attrs.json.gz"]), 'utf-8'))
         self.vals = json.loads(codecs.decode(gzip.decompress(downloaded_files["objects_vals.json.gz"]), 'utf-8'))
 
     def enumerate_properties(self, id) -> list:
+        """
+        Get all properties of an object
+        :param id: database id storage in the manifest file
+        :return: list of properties
+        """
         properties = []
         if 0 < id < len(self.offsets):
             av_start = 2 * self.offsets[id]
             av_end = len(self.avs) if id == len(self.offsets) - 1 else 2 * self.offsets[id + 1]
             for i in range(av_start, av_end, 2):
                 attr_offset = self.avs[i]
                 val_offset = self.avs[i + 1]
@@ -111,32 +116,41 @@
         return properties
 
     """
     Get all properties exclude internal properties
     """
 
     def get_properties(self, id) -> dict:
+        """
+        Get all properties exclude internal properties
+        :param id:
+        :return:
+        """
         props = {}
         rg = re.compile(r'^__\w+__$')
         for prop in self.enumerate_properties(id):
             if prop.category and not rg.match(prop.category):
                 props[prop.name] = prop.value
         return props
 
-    """
-    Get all properties include internal properties
-    """
-
     def get_all_properties(self, id) -> dict:
+        """
+            Get all properties include internal properties
+        """
         props = {}
         for prop in self.enumerate_properties(id):
             props[prop.name] = prop.value
         return props
 
     def get_all_properties_display_unit(self, id) -> dict:
+        """
+        Get all properties include internal properties with display unit value
+        :param id: database id storage in the manifest file
+        :return: :class:`dict` of properties, key is property name, value is property value with display unit
+        """
         props = {}
         for prop in self.enumerate_properties(id):
             value = prop.value
             unit_type = prop.data_type_context
             if unit_type not in ["", None]:
                 unit = self.units.parse_symbol(unit_type)
                 props[prop.name] = f"{value} {unit}"
@@ -159,14 +173,19 @@
                         values = result.get(name, [])
                         if value not in values:
                             values.append(value)
                             result[name] = values
         return result
 
     def get_property_values_by_display_names(self, display_names: List[str]) -> dict:
+        """
+        Get property values by display names. e.g. : ["Name", "Category,"Comments"]
+        :param display_names: list of display names to get values
+        :return:
+        """
         result = {}
         for i in range(len(self.offsets)):
             av_start = 2 * self.offsets[i]
             av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
             for j in range(av_start, av_end, 2):
                 attr_offset = self.avs[j]
                 attr_obj = self.attrs[attr_offset]
@@ -178,14 +197,19 @@
                         if value not in values:
                             values.append(value)
                             result[display_name] = values
 
         return result
 
     def get_properties_group_by_category(self, id) -> dict:
+        """
+        Get all properties group by category Property.
+        :param id: database id storage in the manifest file
+        :return: :class:`dict` of properties, key is category name, value is list of properties
+        """
         properties = {}
         rg = re.compile(r'^__\w+__$')
         categories = []
 
         props = self.enumerate_properties(id)
         for prop in props:
             if prop.category:
@@ -200,28 +224,43 @@
                 prop_key = prop.name
                 prop_dictionary.append((prop_key, prop.value))
             properties[category] = prop_dictionary
 
         return properties
 
     def get_children(self, id) -> list:
+        """
+        Get all children of an object
+        :param id: database id storage in the manifest file
+        :return: list of children (database id)
+        """
         children = []
         for prop in self.enumerate_properties(id):
             if prop.category == "__child__":
                 children.append(int(prop.value))
         return children
 
     def get_parent(self, id) -> list:
+        """
+        Get all parent of an object
+        :param id: database id storage in the manifest file
+        :return: list of parent (database id)
+        """
         parent = []
         for prop in self.enumerate_properties(id):
             if prop.category == "__parent__":
                 parent.append(int(prop.value))
         return parent
 
     def get_instance(self, id) -> list:
+        """
+        Get all instance of an object
+        :param id:  database id storage in the manifest file
+        :return:  list of instance (database id)
+        """
         instance_of = []
         for prop in self.enumerate_properties(id):
             if prop.category == "__instanceof__":
                 instance_of.append(int(prop.value))
         return instance_of
 
     def get_internal_ref(self, id) -> list:
@@ -232,14 +271,19 @@
 
     # TODO : It too slow, need find another way to get all data with less time and cover all format : dwg, rvt, nwd, ifc, ...
     # def get_all_data(self) -> pd.DataFrame:
     #     db_index_ids = [i for i in range(len(self.offsets))]
     #     return self.get_recursive_ids(db_index_ids)
 
     def get_recursive_ids(self, db_ids: List[int]) -> pd.DataFrame:
+        """
+        Get all properties of all objects
+        :param db_ids:  list of database id storage in the manifest file
+        :return:  :class:`pandas.DataFrame` of properties
+        """
         dataframe = pd.DataFrame()
         props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
         if len(db_ids) == 0:
             return dataframe
         for id in db_ids:
             props = self.enumerate_properties(id)
             properties = {}
@@ -261,14 +305,20 @@
             dataframe = pd.concat([dataframe, self.get_recursive_ids(ids)], ignore_index=True)
         if 'dbId' in dataframe.columns:
             dataframe = dataframe[
                 ['dbId'] + [col for col in dataframe.columns if col not in ['dbId']]]
         return dataframe
 
     def get_recursive_ids_by_parameters(self, db_ids: List[int], params: List[str]) -> pd.DataFrame:
+        """
+        Get all properties of all objects by parameters
+        :param db_ids:  list of database id storage in the manifest file
+        :param params:  list of parameters to get
+        :return:  :class:`pandas.DataFrame` of properties
+        """
         dataframe = pd.DataFrame()
         props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
         if len(db_ids) == 0:
             return dataframe
         for id in db_ids:
             props = self.enumerate_properties(id)
             properties = {}
@@ -291,14 +341,18 @@
             ids = self.get_children(id)
             dataframe = pd.concat([dataframe, self.get_recursive_ids_by_parameters(ids, params)], ignore_index=True)
         if 'dbId' in dataframe.columns:
             dataframe = dataframe[['dbId'] + [col for col in dataframe.columns if col not in ['dbId']]]
         return dataframe
 
     def get_all_properties_names(self) -> List[str]:
+        """
+        Get all properties names of all objects
+        :return: :class:`list` of properties names
+        """
         props_names = []
         for i in range(len(self.offsets)):
             av_start = 2 * self.offsets[i]
             av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
             for j in range(av_start, av_end, 2):
                 attr_offset = self.avs[j]
                 attr_obj = self.attrs[attr_offset]
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/Resource.py` & `aps-toolkit-0.6.1/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.6.1/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/Token.py` & `aps-toolkit-0.6.1/src/aps_toolkit/Token.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
 class Token():
-    def __init__(self, access_token, token_type, expires_in, refresh_token=None):
+    def __init__(self, access_token: str, token_type: str, expires_in: int, refresh_token: str = None):
         self.access_token = access_token
         self.token_type = token_type
         self.expires_in = expires_in
         self.refresh_token = refresh_token
 
     def is_expired(self) -> bool:
         return self.expires_in <= 0
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/__init__.py` & `aps-toolkit-0.6.1/src/aps_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/units/DisplayUnits.py` & `aps-toolkit-0.6.1/src/aps_toolkit/units/DisplayUnits.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,16 +25,15 @@
         file_name = "units.json"
         file_path = os.path.join(dir_path, file_name)
         try:
             with open(file_path, "r", encoding="utf-8") as file:
                 self.units = json.load(file)
                 # convert to dict
                 self.units = {unit["TypeId"]: unit["UnitLabel"] for unit in self.units}
-            print("Units loaded")
         except FileNotFoundError:
             print(f"Error: File '{file_path}' not found.")
         except json.JSONDecodeError as e:
             print(f"Error decoding JSON file: {e}")
 
-    def parse_symbol(self, type_id):
+    def parse_symbol(self, type_id: str):
         type_id = type_id.split("-")[0]
         return self.units.get(type_id, "Unknown")
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit/units/units.json` & `aps-toolkit-0.6.1/src/aps_toolkit/units/units.json`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.6.1/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.0/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.6.1/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/context.py` & `aps-toolkit-0.6.1/src/test/context.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_auth.py` & `aps-toolkit-0.6.1/src/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_auth_colab.py` & `aps-toolkit-0.6.1/src/test/test_auth_colab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_bim360.py` & `aps-toolkit-0.6.1/src/test/test_bim360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_bucket.py` & `aps-toolkit-0.6.1/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_db_reader.py` & `aps-toolkit-0.6.1/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_derivative.py` & `aps-toolkit-0.6.1/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_fragment.py` & `aps-toolkit-0.6.1/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_geometries.py` & `aps-toolkit-0.6.1/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_image.py` & `aps-toolkit-0.6.1/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_material.py` & `aps-toolkit-0.6.1/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_mesh.py` & `aps-toolkit-0.6.1/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_prop_reader.py` & `aps-toolkit-0.6.1/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.6.1/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.6.1/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.6.1/src/test/test_prop_reader_revit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.0/src/test/test_svf_reader.py` & `aps-toolkit-0.6.1/src/test/test_svf_reader.py`

 * *Files identical despite different names*


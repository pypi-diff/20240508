# Comparing `tmp/aps-toolkit-0.5.9.tar.gz` & `tmp/aps-toolkit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.5.9.tar", last modified: Wed May  8 06:58:22 2024, max compression
+gzip compressed data, was "aps-toolkit-0.6.0.tar", last modified: Wed May  8 07:39:11 2024, max compression
```

## Comparing `aps-toolkit-0.5.9.tar` & `aps-toolkit-0.6.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.527473 aps-toolkit-0.5.9/
--rw-rw-rw-   0        0        0     1990 2024-05-08 06:58:22.526486 aps-toolkit-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 06:58:22.528472 aps-toolkit-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-05-08 06:57:38.000000 aps-toolkit-0.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.400471 aps-toolkit-0.5.9/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.485473 aps-toolkit-0.5.9/src/aps_toolkit/
--rw-rw-rw-   0        0        0    11183 2024-05-08 03:10:48.000000 aps-toolkit-0.5.9/src/aps_toolkit/Auth.py
--rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.5.9/src/aps_toolkit/AuthGoogleColab.py
--rw-rw-rw-   0        0        0    10333 2024-03-27 07:53:22.000000 aps-toolkit-0.5.9/src/aps_toolkit/BIM360.py
--rw-rw-rw-   0        0        0     9081 2024-04-01 02:00:06.000000 aps-toolkit-0.5.9/src/aps_toolkit/Bucket.py
--rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.5.9/src/aps_toolkit/DbReader.py
--rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.5.9/src/aps_toolkit/Derivative.py
--rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.5.9/src/aps_toolkit/Fragments.py
--rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/InputStream.py
--rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/ManifestItem.py
--rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/MaterialProperties.py
--rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/Materials.py
--rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/PackFileReader.py
--rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/PathInfo.py
--rw-rw-rw-   0        0        0     4586 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderCad.py
--rw-rw-rw-   0        0        0     3592 2024-03-25 01:46:50.000000 aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderNavis.py
--rw-rw-rw-   0        0        0    15835 2024-05-08 06:44:58.000000 aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderRevit.py
--rw-rw-rw-   0        0        0    13956 2024-05-08 06:40:14.000000 aps-toolkit-0.5.9/src/aps_toolkit/PropReader.py
--rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.5.9/src/aps_toolkit/Resource.py
--rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFContent.py
--rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFGeometries.py
--rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFImage.py
--rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFLines.py
--rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFManifestType.py
--rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialGroup.py
--rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMap.py
--rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMapScale.py
--rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterials.py
--rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMesh.py
--rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMetadata.py
--rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFPoints.py
--rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFReader.py
--rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFTransform.py
--rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFUVMap.py
--rw-rw-rw-   0        0        0     1010 2024-04-01 02:00:06.000000 aps-toolkit-0.5.9/src/aps_toolkit/Token.py
--rw-rw-rw-   0        0        0      813 2024-05-08 05:40:51.000000 aps-toolkit-0.5.9/src/aps_toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.490471 aps-toolkit-0.5.9/src/aps_toolkit/units/
--rw-rw-rw-   0        0        0     1511 2024-05-08 06:53:18.000000 aps-toolkit-0.5.9/src/aps_toolkit/units/DisplayUnits.py
--rw-rw-rw-   0        0        0        0 2024-05-08 03:17:26.000000 aps-toolkit-0.5.9/src/aps_toolkit/units/__init__.py
--rw-rw-rw-   0        0        0    36914 2024-05-08 05:15:29.000000 aps-toolkit-0.5.9/src/aps_toolkit/units/units.json
-drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.488470 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1890 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.526486 aps-toolkit-0.5.9/src/test/
--rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.5.9/src/test/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-08 05:42:58.000000 aps-toolkit-0.5.9/src/test/context.py
--rw-rw-rw-   0        0        0     2006 2024-05-06 06:38:44.000000 aps-toolkit-0.5.9/src/test/test_auth.py
--rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.5.9/src/test/test_auth_colab.py
--rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.5.9/src/test/test_bim360.py
--rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.5.9/src/test/test_bucket.py
--rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.5.9/src/test/test_db_reader.py
--rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.5.9/src/test/test_derivative.py
--rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_fragment.py
--rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_geometries.py
--rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_image.py
--rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_material.py
--rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_mesh.py
--rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_metadata.py
--rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.5.9/src/test/test_prop_reader.py
--rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_prop_reader_cad.py
--rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.5.9/src/test/test_prop_reader_navis.py
--rw-rw-rw-   0        0        0     3516 2024-05-08 06:48:33.000000 aps-toolkit-0.5.9/src/test/test_prop_reader_revit.py
--rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_svf_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.408698 aps-toolkit-0.6.0/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 07:39:11.407700 aps-toolkit-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:39:11.408698 aps-toolkit-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2024-05-08 07:38:56.000000 aps-toolkit-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.295759 aps-toolkit-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.373700 aps-toolkit-0.6.0/src/aps_toolkit/
+-rw-rw-rw-   0        0        0    12872 2024-05-08 07:37:37.000000 aps-toolkit-0.6.0/src/aps_toolkit/Auth.py
+-rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.6.0/src/aps_toolkit/AuthGoogleColab.py
+-rw-rw-rw-   0        0        0    10333 2024-03-27 07:53:22.000000 aps-toolkit-0.6.0/src/aps_toolkit/BIM360.py
+-rw-rw-rw-   0        0        0     9081 2024-04-01 02:00:06.000000 aps-toolkit-0.6.0/src/aps_toolkit/Bucket.py
+-rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.6.0/src/aps_toolkit/DbReader.py
+-rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.6.0/src/aps_toolkit/Derivative.py
+-rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.6.0/src/aps_toolkit/Fragments.py
+-rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/InputStream.py
+-rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/ManifestItem.py
+-rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/MaterialProperties.py
+-rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/Materials.py
+-rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/PackFileReader.py
+-rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/PathInfo.py
+-rw-rw-rw-   0        0        0     4586 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderCad.py
+-rw-rw-rw-   0        0        0     3592 2024-03-25 01:46:50.000000 aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderNavis.py
+-rw-rw-rw-   0        0        0    15835 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderRevit.py
+-rw-rw-rw-   0        0        0    13956 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/PropReader.py
+-rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.6.0/src/aps_toolkit/Resource.py
+-rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFContent.py
+-rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFGeometries.py
+-rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFImage.py
+-rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFLines.py
+-rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFManifestType.py
+-rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialGroup.py
+-rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMap.py
+-rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterials.py
+-rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMesh.py
+-rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFMetadata.py
+-rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFPoints.py
+-rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFReader.py
+-rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFTransform.py
+-rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.6.0/src/aps_toolkit/SVFUVMap.py
+-rw-rw-rw-   0        0        0     1010 2024-04-01 02:00:06.000000 aps-toolkit-0.6.0/src/aps_toolkit/Token.py
+-rw-rw-rw-   0        0        0      813 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.378699 aps-toolkit-0.6.0/src/aps_toolkit/units/
+-rw-rw-rw-   0        0        0     1511 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/units/DisplayUnits.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/units/__init__.py
+-rw-rw-rw-   0        0        0    38555 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/aps_toolkit/units/units.json
+drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.376699 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 07:39:10.000000 aps-toolkit-0.6.0/src/aps_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 07:39:11.406698 aps-toolkit-0.6.0/src/test/
+-rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.6.0/src/test/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/test/context.py
+-rw-rw-rw-   0        0        0     2006 2024-05-08 07:26:15.000000 aps-toolkit-0.6.0/src/test/test_auth.py
+-rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.6.0/src/test/test_auth_colab.py
+-rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.6.0/src/test/test_bim360.py
+-rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.6.0/src/test/test_bucket.py
+-rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.6.0/src/test/test_db_reader.py
+-rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.6.0/src/test/test_derivative.py
+-rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_fragment.py
+-rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_geometries.py
+-rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_image.py
+-rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_material.py
+-rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.6.0/src/test/test_mesh.py
+-rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_metadata.py
+-rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.6.0/src/test/test_prop_reader.py
+-rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_prop_reader_cad.py
+-rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.6.0/src/test/test_prop_reader_navis.py
+-rw-rw-rw-   0        0        0     3516 2024-05-08 07:02:44.000000 aps-toolkit-0.6.0/src/test/test_prop_reader_revit.py
+-rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.6.0/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.5.9/PKG-INFO` & `aps-toolkit-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.9
+Version: 0.6.0
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.9/setup.py` & `aps-toolkit-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.5.9",
+    version="0.6.0",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
```

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/Auth.py` & `aps-toolkit-0.6.0/src/aps_toolkit/Auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,14 +41,19 @@
         # Initialize token variables
         self.access_token = None
         self.token_type = None
         self.expires_in = None
         self.refresh_token = None
 
     def auth2leg(self) -> Token:
+        """
+        This method is used to authenticate an application using the 2-legged OAuth flow.
+        https://aps.autodesk.com/en/docs/oauth/v2/tutorials/get-2-legged-token/
+       :return: :class:`Token`: An instance of the Token class containing the access token, token type, and expiration time.
+        """
         Host = "https://developer.api.autodesk.com"
         url = "/authentication/v2/token"
 
         # body
         body = {
             "client_id": self.client_id,
             "client_secret": self.client_secret,
@@ -62,14 +67,21 @@
         self.access_token = content['access_token']
         self.expires_in = content['expires_in']
         self.token_type = content['token_type']
         result = Token(self.access_token, self.token_type, self.expires_in)
         return result
 
     def auth3leg(self, callback_url=None, scopes=None) -> Token:
+        """
+        This method is used to authenticate a user using the 3-legged OAuth flow.
+        https://aps.autodesk.com/en/docs/oauth/v2/tutorials/get-3-legged-token/
+        :param callback_url: This is the URL-encoded callback URL you want the user redirected to after they grant consent. In this example, that URL is http://localhost:8080/oauth/callback/. Replace the value here with the appropriate URL for your web app. Note that it must match the pattern specified for the callback URL in your app’s registration in the APS developer portal.
+        :param scopes: This requests the data:read scope. You can leave this value as it is for the purpose of this example, but in your own app, you should request one or more scopes you actually need. If you need to include multiple scopes, you can include them all as space-delimited items. For example: scope=data:create%20data:read%20data:write includes data:read, data:write, and data:create scopes.
+        :return: :class:`Token`:  An instance of the Token class containing the access token, token type, expiration time, and refresh token (if available).
+        """
         if not scopes:
             scopes = 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'
         if not callback_url:
             # Default callback url
             callback_url = "http://localhost:8080/api/auth/callback"
 
         class CallbackHandler(BaseHTTPRequestHandler):
@@ -119,26 +131,25 @@
         auth_url = f"https://developer.api.autodesk.com/authentication/v2/authorize?response_type=code&client_id={self.client_id}&redirect_uri={callback_url}&scope={scopes}"
         webbrowser.open(auth_url)
         start_callback_server(callback_url)
 
         # Return the token object using the global variables
         return Token(self.access_token, self.token_type, self.expires_in, self.refresh_token)
 
-    def auth3legPkce(self, clientId=None, callback_url=None, scopes=None) -> Token:
+    def auth3legPkce(self, clientId: Optional[str] = None, callback_url: Optional[str] = None,
+                     scopes: Optional[str] = None) -> Token:
+        """
+        This method is used to authenticate a user using the 3-legged OAuth PKCE flow.
+        https://aps.autodesk.com/blog/new-application-types
+        Parameters:
+        :param clientId: The client ID of the application. If not provided, it will use the client ID from the environment variables.
+        :param callback_url: The callback URL where the user will be redirected after authentication. If not provided, it defaults to "http://localhost:8080/api/auth/callback".
+        :param scopes: The scopes for which the application is requesting access. If not provided, it defaults to 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'.
+        :Returns: :class:`Token`: An instance of the Token class containing the access token, token type, expiration time, and refresh token (if available).
         """
-            This method is used to authenticate a user using the 3-legged OAuth PKCE flow.
-            https://aps.autodesk.com/blog/new-application-types
-            Parameters:
-            clientId (str, optional): The client ID of the application. If not provided, it will use the client ID from the environment variables.
-            callback_url (str, optional): The callback URL where the user will be redirected after authentication. If not provided, it defaults to "http://localhost:8080/api/auth/callback".
-            scopes (str, optional): The scopes for which the application is requesting access. If not provided, it defaults to 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'.
-
-            Returns:
-            Token: An instance of the Token class containing the access token, token type, expiration time, and refresh token (if available).
-            """
         if clientId:
             self.client_id = clientId
         if not scopes:
             scopes = 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'
         if not callback_url:
             # Default callback url
             callback_url = "http://localhost:8080/api/auth/callback"
@@ -226,15 +237,20 @@
         self.access_token = content['access_token']
         self.expires_in = content['expires_in']
         self.token_type = content['token_type']
         self.refresh_token = content.get('refresh_token')
         result = Token(self.access_token, self.token_type, self.expires_in, self.refresh_token)
         return result
 
-    def get_user_info(self):
+    def get_user_info(self) -> dict:
+        """
+        This method is used to get user information.
+        https://developer.api.autodesk.com/userprofile/v1/userinfo
+        :return:  A dictionary containing user information.
+        """
         if not self.access_token:
             raise Exception("Access token is required, please authenticate first. Use auth2leg or auth3leg method.")
         url = "https://api.userprofile.autodesk.com/userinfo"
         headers = {
             "Authorization": f"{self.token_type} {self.access_token}"
         }
         response = requests.get(url, headers=headers)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/AuthGoogleColab.py` & `aps-toolkit-0.6.0/src/aps_toolkit/AuthGoogleColab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.6.0/src/aps_toolkit/BIM360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.6.0/src/aps_toolkit/Bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.6.0/src/aps_toolkit/DbReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.6.0/src/aps_toolkit/Derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.6.0/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.6.0/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.6.0/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.6.0/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/Materials.py` & `aps-toolkit-0.6.0/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.6.0/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.6.0/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderCad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.6.0/src/aps_toolkit/ProDbReaderRevit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.6.0/src/aps_toolkit/PropReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/Resource.py` & `aps-toolkit-0.6.0/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.6.0/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/Token.py` & `aps-toolkit-0.6.0/src/aps_toolkit/Token.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/__init__.py` & `aps-toolkit-0.6.0/src/aps_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit/units/DisplayUnits.py` & `aps-toolkit-0.6.0/src/aps_toolkit/units/DisplayUnits.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.6.0/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.9
+Version: 0.6.0
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.9/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.6.0/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/context.py` & `aps-toolkit-0.6.0/src/test/context.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_auth.py` & `aps-toolkit-0.6.0/src/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_auth_colab.py` & `aps-toolkit-0.6.0/src/test/test_auth_colab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_bim360.py` & `aps-toolkit-0.6.0/src/test/test_bim360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_bucket.py` & `aps-toolkit-0.6.0/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_db_reader.py` & `aps-toolkit-0.6.0/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_derivative.py` & `aps-toolkit-0.6.0/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_fragment.py` & `aps-toolkit-0.6.0/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_geometries.py` & `aps-toolkit-0.6.0/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_image.py` & `aps-toolkit-0.6.0/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_material.py` & `aps-toolkit-0.6.0/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_mesh.py` & `aps-toolkit-0.6.0/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_prop_reader.py` & `aps-toolkit-0.6.0/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.6.0/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.6.0/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.6.0/src/test/test_prop_reader_revit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.9/src/test/test_svf_reader.py` & `aps-toolkit-0.6.0/src/test/test_svf_reader.py`

 * *Files identical despite different names*


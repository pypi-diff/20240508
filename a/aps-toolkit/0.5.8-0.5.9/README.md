# Comparing `tmp/aps-toolkit-0.5.8.tar.gz` & `tmp/aps-toolkit-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.5.8.tar", last modified: Mon May  6 10:07:26 2024, max compression
+gzip compressed data, was "aps-toolkit-0.5.9.tar", last modified: Wed May  8 06:58:22 2024, max compression
```

## Comparing `aps-toolkit-0.5.8.tar` & `aps-toolkit-0.5.9.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 10:07:26.714777 aps-toolkit-0.5.8/
--rw-rw-rw-   0        0        0     1990 2024-05-06 10:07:26.713775 aps-toolkit-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-06 10:07:26.714777 aps-toolkit-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      902 2024-05-06 10:07:14.000000 aps-toolkit-0.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:07:26.573825 aps-toolkit-0.5.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 10:07:26.675812 aps-toolkit-0.5.8/src/aps_toolkit/
--rw-rw-rw-   0        0        0    11183 2024-05-06 09:24:37.000000 aps-toolkit-0.5.8/src/aps_toolkit/Auth.py
--rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.5.8/src/aps_toolkit/AuthGoogleColab.py
--rw-rw-rw-   0        0        0    10333 2024-03-27 07:53:22.000000 aps-toolkit-0.5.8/src/aps_toolkit/BIM360.py
--rw-rw-rw-   0        0        0     9081 2024-04-01 02:00:06.000000 aps-toolkit-0.5.8/src/aps_toolkit/Bucket.py
--rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.5.8/src/aps_toolkit/DbReader.py
--rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.5.8/src/aps_toolkit/Derivative.py
--rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.5.8/src/aps_toolkit/Fragments.py
--rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/InputStream.py
--rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/aps_toolkit/ManifestItem.py
--rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/MaterialProperties.py
--rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/Materials.py
--rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/PackFileReader.py
--rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/aps_toolkit/PathInfo.py
--rw-rw-rw-   0        0        0     4586 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/aps_toolkit/ProDbReaderCad.py
--rw-rw-rw-   0        0        0     3592 2024-03-25 01:46:50.000000 aps-toolkit-0.5.8/src/aps_toolkit/ProDbReaderNavis.py
--rw-rw-rw-   0        0        0    13855 2024-03-19 23:58:05.000000 aps-toolkit-0.5.8/src/aps_toolkit/ProDbReaderRevit.py
--rw-rw-rw-   0        0        0    13418 2024-03-27 07:23:53.000000 aps-toolkit-0.5.8/src/aps_toolkit/PropReader.py
--rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.5.8/src/aps_toolkit/Resource.py
--rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFContent.py
--rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFGeometries.py
--rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFImage.py
--rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFLines.py
--rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFManifestType.py
--rw-rw-rw-   0        0        0      910 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterialGroup.py
--rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterialMap.py
--rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterialMapScale.py
--rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterials.py
--rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFMesh.py
--rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFMetadata.py
--rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFPoints.py
--rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFReader.py
--rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFTransform.py
--rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.5.8/src/aps_toolkit/SVFUVMap.py
--rw-rw-rw-   0        0        0     1010 2024-04-01 02:00:06.000000 aps-toolkit-0.5.8/src/aps_toolkit/Token.py
--rw-rw-rw-   0        0        0      767 2024-05-06 09:13:54.000000 aps-toolkit-0.5.8/src/aps_toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:07:26.679778 aps-toolkit-0.5.8/src/aps_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-06 10:07:26.000000 aps-toolkit-0.5.8/src/aps_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1785 2024-05-06 10:07:26.000000 aps-toolkit-0.5.8/src/aps_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 10:07:26.000000 aps-toolkit-0.5.8/src/aps_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 10:07:26.000000 aps-toolkit-0.5.8/src/aps_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-06 10:07:26.000000 aps-toolkit-0.5.8/src/aps_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 10:07:26.712777 aps-toolkit-0.5.8/src/test/
--rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.5.8/src/test/__init__.py
--rw-rw-rw-   0        0        0     1015 2024-05-06 09:14:04.000000 aps-toolkit-0.5.8/src/test/context.py
--rw-rw-rw-   0        0        0     2006 2024-05-06 06:38:44.000000 aps-toolkit-0.5.8/src/test/test_auth.py
--rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.5.8/src/test/test_auth_colab.py
--rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.5.8/src/test/test_bim360.py
--rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.5.8/src/test/test_bucket.py
--rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.5.8/src/test/test_db_reader.py
--rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.5.8/src/test/test_derivative.py
--rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.5.8/src/test/test_fragment.py
--rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.5.8/src/test/test_geometries.py
--rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/test/test_image.py
--rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.5.8/src/test/test_material.py
--rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.5.8/src/test/test_mesh.py
--rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/test/test_metadata.py
--rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.5.8/src/test/test_prop_reader.py
--rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/test/test_prop_reader_cad.py
--rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.5.8/src/test/test_prop_reader_navis.py
--rw-rw-rw-   0        0        0     3472 2024-03-15 07:18:51.000000 aps-toolkit-0.5.8/src/test/test_prop_reader_revit.py
--rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.5.8/src/test/test_svf_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.527473 aps-toolkit-0.5.9/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 06:58:22.526486 aps-toolkit-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:58:22.528472 aps-toolkit-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2024-05-08 06:57:38.000000 aps-toolkit-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.400471 aps-toolkit-0.5.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.485473 aps-toolkit-0.5.9/src/aps_toolkit/
+-rw-rw-rw-   0        0        0    11183 2024-05-08 03:10:48.000000 aps-toolkit-0.5.9/src/aps_toolkit/Auth.py
+-rw-rw-rw-   0        0        0     5608 2024-05-06 10:07:04.000000 aps-toolkit-0.5.9/src/aps_toolkit/AuthGoogleColab.py
+-rw-rw-rw-   0        0        0    10333 2024-03-27 07:53:22.000000 aps-toolkit-0.5.9/src/aps_toolkit/BIM360.py
+-rw-rw-rw-   0        0        0     9081 2024-04-01 02:00:06.000000 aps-toolkit-0.5.9/src/aps_toolkit/Bucket.py
+-rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.5.9/src/aps_toolkit/DbReader.py
+-rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.5.9/src/aps_toolkit/Derivative.py
+-rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.5.9/src/aps_toolkit/Fragments.py
+-rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/InputStream.py
+-rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/ManifestItem.py
+-rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/MaterialProperties.py
+-rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/Materials.py
+-rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/PackFileReader.py
+-rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/PathInfo.py
+-rw-rw-rw-   0        0        0     4586 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderCad.py
+-rw-rw-rw-   0        0        0     3592 2024-03-25 01:46:50.000000 aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderNavis.py
+-rw-rw-rw-   0        0        0    15835 2024-05-08 06:44:58.000000 aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderRevit.py
+-rw-rw-rw-   0        0        0    13956 2024-05-08 06:40:14.000000 aps-toolkit-0.5.9/src/aps_toolkit/PropReader.py
+-rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.5.9/src/aps_toolkit/Resource.py
+-rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFContent.py
+-rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFGeometries.py
+-rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFImage.py
+-rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFLines.py
+-rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFManifestType.py
+-rw-rw-rw-   0        0        0      910 2024-05-08 02:57:09.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialGroup.py
+-rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMap.py
+-rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterials.py
+-rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMesh.py
+-rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFMetadata.py
+-rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFPoints.py
+-rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFReader.py
+-rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFTransform.py
+-rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.5.9/src/aps_toolkit/SVFUVMap.py
+-rw-rw-rw-   0        0        0     1010 2024-04-01 02:00:06.000000 aps-toolkit-0.5.9/src/aps_toolkit/Token.py
+-rw-rw-rw-   0        0        0      813 2024-05-08 05:40:51.000000 aps-toolkit-0.5.9/src/aps_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.490471 aps-toolkit-0.5.9/src/aps_toolkit/units/
+-rw-rw-rw-   0        0        0     1511 2024-05-08 06:53:18.000000 aps-toolkit-0.5.9/src/aps_toolkit/units/DisplayUnits.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 03:17:26.000000 aps-toolkit-0.5.9/src/aps_toolkit/units/__init__.py
+-rw-rw-rw-   0        0        0    36914 2024-05-08 05:15:29.000000 aps-toolkit-0.5.9/src/aps_toolkit/units/units.json
+drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.488470 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 06:58:21.000000 aps-toolkit-0.5.9/src/aps_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 06:58:22.526486 aps-toolkit-0.5.9/src/test/
+-rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.5.9/src/test/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-08 05:42:58.000000 aps-toolkit-0.5.9/src/test/context.py
+-rw-rw-rw-   0        0        0     2006 2024-05-06 06:38:44.000000 aps-toolkit-0.5.9/src/test/test_auth.py
+-rw-rw-rw-   0        0        0     1429 2024-05-06 09:51:01.000000 aps-toolkit-0.5.9/src/test/test_auth_colab.py
+-rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.5.9/src/test/test_bim360.py
+-rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.5.9/src/test/test_bucket.py
+-rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.5.9/src/test/test_db_reader.py
+-rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.5.9/src/test/test_derivative.py
+-rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_fragment.py
+-rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_geometries.py
+-rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_image.py
+-rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_material.py
+-rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.5.9/src/test/test_mesh.py
+-rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_metadata.py
+-rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.5.9/src/test/test_prop_reader.py
+-rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_prop_reader_cad.py
+-rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.5.9/src/test/test_prop_reader_navis.py
+-rw-rw-rw-   0        0        0     3516 2024-05-08 06:48:33.000000 aps-toolkit-0.5.9/src/test/test_prop_reader_revit.py
+-rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.5.9/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.5.8/PKG-INFO` & `aps-toolkit-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.8
+Version: 0.5.9
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.8/setup.py` & `aps-toolkit-0.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.5.8",
+    version="0.5.9",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
@@ -20,9 +20,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9",
-    install_requires=['requests', 'pandas']
+    install_requires=['requests', 'pandas'],
+    include_package_data=True,
+    data_files=[('aps_toolkit/units', ['src/aps_toolkit/units/units.json'])]
 )
```

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/Auth.py` & `aps-toolkit-0.5.9/src/aps_toolkit/Auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/AuthGoogleColab.py` & `aps-toolkit-0.5.9/src/aps_toolkit/AuthGoogleColab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.5.9/src/aps_toolkit/BIM360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.5.9/src/aps_toolkit/Bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.5.9/src/aps_toolkit/DbReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.5.9/src/aps_toolkit/Derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.5.9/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.5.9/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.5.9/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.5.9/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/Materials.py` & `aps-toolkit-0.5.9/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.5.9/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.5.9/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderCad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.5.9/src/aps_toolkit/ProDbReaderRevit.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,179 +98,212 @@
         return json_response["refPointTransformation"]
 
     def get_all_categories(self) -> dict:
         categories = {}
         self._get_recursive_child(categories, 1, "_RC")
         return categories
 
-    def get_all_data(self, is_get_sub_family=False) -> pd.DataFrame:
+    def get_all_data(self, is_get_sub_family=False, display_unit=False) -> pd.DataFrame:
         categories_dict = self.get_all_categories()
         dbids = list(categories_dict.keys())
         dataframe = pd.DataFrame()
         for dbid in dbids:
-            df = self._get_recursive_ids([dbid], is_get_sub_family)
+            df = self._get_recursive_ids([dbid], is_get_sub_family, display_unit)
             dataframe = pd.concat([dataframe, df], ignore_index=True)
         return dataframe
 
     def get_all_families(self) -> dict:
         families = {}
         self._get_recursive_child(families, 1, "_RFN")
         return families
 
     def get_all_families_types(self) -> dict:
         families_types = {}
         self._get_recursive_child(families_types, 1, "_RFT")
         return families_types
 
-    def get_data_by_category(self, category, is_get_sub_family=False) -> pd.DataFrame:
+    def get_data_by_category(self, category, is_get_sub_family=False, display_unit=False) -> pd.DataFrame:
         categories = self.get_all_categories()
         # if category starts with Revit, remove it
         if category.startswith("Revit"):
             category = category[5:].strip()
         category_id = [key for key, value in categories.items() if value == category]
-        dataframe = self._get_recursive_ids(category_id, is_get_sub_family)
+        dataframe = self._get_recursive_ids(category_id, is_get_sub_family, display_unit)
         return dataframe
 
     def get_data_by_categories(self, categories: List[str], is_get_sub_family=False) -> pd.DataFrame:
         dataframe = pd.DataFrame()
         for category in categories:
             dataframe = pd.concat([dataframe, self.get_data_by_category(category, is_get_sub_family)],
                                   ignore_index=True)
         return dataframe
 
     def get_data_by_categories_and_params(self, categories: List[str], params: List[str],
-                                          is_get_sub_family=False) -> pd.DataFrame:
+                                          is_get_sub_family=False, display_unit=False) -> pd.DataFrame:
         dataframe = pd.DataFrame()
         all_categories = self.get_all_categories()
         category_ids = [key for key, value in all_categories.items() if value in categories]
         for category_id in category_ids:
-            dataframe = pd.concat([dataframe, self._get_recursive_ids_prams([category_id], params, is_get_sub_family)],
-                                  ignore_index=True)
+            dataframe = pd.concat(
+                [dataframe, self._get_recursive_ids_prams([category_id], params, is_get_sub_family, display_unit)],
+                ignore_index=True)
         # remove all row have all values is null, ignore dbId and external_id columns
         dataframe = dataframe.dropna(how='all',
                                      subset=[col for col in dataframe.columns if col not in ['dbId', 'external_id']])
         return dataframe
 
-    def get_data_by_family(self, family_name, is_get_sub_family=False) -> pd.DataFrame:
+    def get_data_by_family(self, family_name, is_get_sub_family=False, display_unit=False) -> pd.DataFrame:
         families = self.get_all_families()
         category_id = [key for key, value in families.items() if value == family_name]
-        dataframe = self._get_recursive_ids(category_id, is_get_sub_family)
+        dataframe = self._get_recursive_ids(category_id, is_get_sub_family, display_unit)
         return dataframe
 
-    def get_data_by_family_type(self, family_type, is_get_sub_family=False) -> pd.DataFrame:
+    def get_data_by_family_type(self, family_type, is_get_sub_family=False, display_unit=False) -> pd.DataFrame:
         family_types = self.get_all_families_types()
         type_id = [key for key, value in family_types.items() if value == family_type]
-        dataframe = self._get_recursive_ids(type_id, is_get_sub_family)
+        dataframe = self._get_recursive_ids(type_id, is_get_sub_family, display_unit)
         return dataframe
 
-    def _get_recursive_ids(self, db_ids: List[int], get_sub_family) -> pd.DataFrame:
+    def _get_recursive_ids(self, db_ids: List[int], get_sub_family, display_unit=False) -> pd.DataFrame:
         dataframe = pd.DataFrame()
         props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
         if len(db_ids) == 0:
             return dataframe
         for id in db_ids:
             props = self.enumerate_properties(id)
             flag_sub_families = False
             properties = {}
             # if props contain _RC, _RFN, _RFT, it's not a leaf node, continue to get children
             if len([prop for prop in props if prop.name in ["_RC", "_RFN", "_RFT"]]) > 0:
                 ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
+                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family, display_unit)],
+                                      ignore_index=True)
                 continue
             for prop in props:
                 if prop.category == "__internalref__" and prop.name == "Sub Family":
                     flag_sub_families = True
                 if prop.name not in props_ignore:
                     if prop.name == "name":
                         properties["Name"] = prop.value
                     else:
-                        properties[prop.name] = prop.value
+                        if display_unit:
+                            if prop.data_type_context not in ["", None]:
+                                properties[prop.name] = str(prop.value) + " " + str(
+                                    self.units.parse_symbol(prop.data_type_context))
+                            else:
+                                properties[prop.name] = prop.value
+                        else:
+                            properties[prop.name] = prop.value
             db_id = id
             external_id = self.ids[id]
             properties['dbId'] = db_id
             properties['external_id'] = external_id
             if flag_sub_families and not get_sub_family:
                 ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
+                dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family, display_unit)],
+                                      ignore_index=True)
                 continue
             ins = self.get_instance(id)
             if len(ins) > 0:
                 for instance in ins:
-                    types = self.get_properties(instance)
+                    if display_unit:
+                        types = self.get_all_properties_display_unit(instance)
+                    else:
+                        types = self.get_properties(instance)
                     properties = {**properties, **types}
             singleDF = pd.DataFrame(properties, index=[0])
             dataframe = pd.concat([dataframe, singleDF], ignore_index=True)
             ids = self.get_children(id)
-            dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family)], ignore_index=True)
+            dataframe = pd.concat([dataframe, self._get_recursive_ids(ids, get_sub_family, display_unit)],
+                                  ignore_index=True)
         if 'dbId' in dataframe.columns and 'external_id' in dataframe.columns:
             dataframe = dataframe[
                 ['dbId', 'external_id'] + [col for col in dataframe.columns if col not in ['dbId', 'external_id']]]
         return dataframe
 
-    def _get_recursive_ids_prams(self, childs: List[int], params: List[str], get_sub_family) -> pd.DataFrame:
+    def _get_recursive_ids_prams(self, childs: List[int], params: List[str], get_sub_family,
+                                 display_unit=False) -> pd.DataFrame:
         dataframe = pd.DataFrame()
         props_ignore = ['parent', 'instanceof_objid', 'child', "viewable_in"]
         if len(childs) == 0:
             return dataframe
         for id in childs:
             flag_sub_families = False
             props = self.enumerate_properties(id)
             # if props contain _RC, _RFN, _RFT, it's not a leaf node, continue to get children
             if len([prop for prop in props if prop.name in ["_RC", "_RFN", "_RFT"]]) > 0:
                 ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
-                                      ignore_index=True)
+                dataframe = pd.concat(
+                    [dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family, display_unit)],
+                    ignore_index=True)
                 continue
             properties = {}
             for prop in props:
                 if prop.category == "__internalref__" and prop.name == "Sub Family":
                     flag_sub_families = True
                 if prop.name not in props_ignore:
                     if prop.name == "name":
                         properties["Name"] = prop.value
                     else:
-                        properties[prop.name] = prop.value
+                        if display_unit:
+                            if prop.data_type_context not in ["", None]:
+                                properties[prop.name] = str(prop.value) + " " + str(
+                                    self.units.parse_symbol(prop.data_type_context))
+                            else:
+                                properties[prop.name] = prop.value
+                        else:
+                            properties[prop.name] = prop.value
             db_id = id
             external_id = self.ids[id]
             # filter just get properties name in params list
             properties = {k: v for k, v in properties.items() if k in params}
             properties['dbId'] = db_id
             properties['external_id'] = external_id
             if flag_sub_families and not get_sub_family:
                 ids = self.get_children(id)
-                dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
-                                      ignore_index=True)
+                dataframe = pd.concat(
+                    [dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family, display_unit)],
+                    ignore_index=True)
                 continue
             # get instances
             ins = self.get_instance(id)
             if len(ins) > 0:
                 for instance in ins:
-                    types = self.get_all_properties(instance)
+                    if display_unit:
+                        types = self.get_all_properties_display_unit(instance)
+                    else:
+                        types = self.get_all_properties(instance)
                     types = {k: v for k, v in types.items() if k in params}
+                    # add unit to value
+                    if display_unit:
+                        for key, value in types.items():
+                            if key in params:
+                                if self.units is not None:
+                                    types[key] = str(value) + " " + str(self.units.parse_symbol(key))
                     properties = {**properties, **types}
             single_df = pd.DataFrame(properties, index=[0])
             dataframe = pd.concat([dataframe, single_df], ignore_index=True)
             ids = self.get_children(id)
-            dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family)],
+            dataframe = pd.concat([dataframe, self._get_recursive_ids_prams(ids, params, get_sub_family, display_unit)],
                                   ignore_index=True)
         # set dbid and external_id to first and second column if it exists
         if 'dbId' in dataframe.columns and 'external_id' in dataframe.columns:
             dataframe = dataframe[
                 ['dbId', 'external_id'] + [col for col in dataframe.columns if col not in ['dbId', 'external_id']]]
         return dataframe
 
-    def get_data_by_external_id(self, external_id, is_get_sub_family=False) -> pd.DataFrame:
+    def get_data_by_external_id(self, external_id, is_get_sub_family=False, display_unit=False) -> pd.DataFrame:
         db_id = None
         for idx in range(0, len(self.ids)):
             if self.ids[idx] == external_id:
                 db_id = idx
                 break
         if db_id is None:
             return pd.DataFrame()
-        dataframe = self._get_recursive_ids([db_id], is_get_sub_family)
+        dataframe = self._get_recursive_ids([db_id], is_get_sub_family, display_unit)
         return dataframe
 
     def get_data_by_element_id(self, element_id) -> dict:
         rg = re.compile(r'^__\w+__$')
         properties = {}
         for i in range(0, len(self.ids)):
             props = self.enumerate_properties(i)
```

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.5.9/src/aps_toolkit/PropReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import re
 import codecs
 import requests
 from .Derivative import Derivative
 from .ManifestItem import ManifestItem
 import pandas as pd
 from typing import List
+from .units.DisplayUnits import DisplayUnits
 
 
 class PropReader:
 
     def __init__(self, urn, token, region="US", manifest_item: [ManifestItem] = None):
         # get manifest
         self.host = "https://developer.api.autodesk.com"
@@ -34,14 +35,15 @@
         self.token = token
         self.region = region
         if manifest_item:
             derivative = Derivative(self.urn, self.token, self.region)
             self._read_metadata_item(derivative, manifest_item)
         else:
             self._read_metadata()
+        self.units = DisplayUnits()
 
     def _read_metadata(self):
         derivative = Derivative(self.urn, self.token, self.region)
         manifest_items = derivative.read_svf_manifest_items()
         if len(manifest_items) > 0:
             self._read_metadata_item(derivative, manifest_items[0])
         else:
@@ -126,14 +128,26 @@
 
     def get_all_properties(self, id) -> dict:
         props = {}
         for prop in self.enumerate_properties(id):
             props[prop.name] = prop.value
         return props
 
+    def get_all_properties_display_unit(self, id) -> dict:
+        props = {}
+        for prop in self.enumerate_properties(id):
+            value = prop.value
+            unit_type = prop.data_type_context
+            if unit_type not in ["", None]:
+                unit = self.units.parse_symbol(unit_type)
+                props[prop.name] = f"{value} {unit}"
+            else:
+                props[prop.name] = value
+        return props
+
     def get_property_values_by_names(self, names: List[str]) -> dict:
         result = {}
         for i in range(len(self.offsets)):
             av_start = 2 * self.offsets[i]
             av_end = len(self.avs) if i == len(self.offsets) - 1 else 2 * self.offsets[i + 1]
             for j in range(av_start, av_end, 2):
                 attr_offset = self.avs[j]
```

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/Resource.py` & `aps-toolkit-0.5.9/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.5.9/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/Token.py` & `aps-toolkit-0.5.9/src/aps_toolkit/Token.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit/__init__.py` & `aps-toolkit-0.5.9/src/aps_toolkit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .units.DisplayUnits import DisplayUnits
 from .Auth import Auth
 from .AuthGoogleColab import AuthGoogleColab
 from .BIM360 import BIM360
 from .ProDbReaderRevit import PropDbReaderRevit
 from .ProDbReaderCad import PropDbReaderCad
 from .ProDbReaderNavis import PropDbReaderNavis
 from .PropReader import PropReader
```

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.5.9/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.8
+Version: 0.5.9
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.8/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.5.9/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 src/aps_toolkit/Token.py
 src/aps_toolkit/__init__.py
 src/aps_toolkit.egg-info/PKG-INFO
 src/aps_toolkit.egg-info/SOURCES.txt
 src/aps_toolkit.egg-info/dependency_links.txt
 src/aps_toolkit.egg-info/requires.txt
 src/aps_toolkit.egg-info/top_level.txt
+src/aps_toolkit/units/DisplayUnits.py
+src/aps_toolkit/units/__init__.py
+src/aps_toolkit/units/units.json
 src/test/__init__.py
 src/test/context.py
 src/test/test_auth.py
 src/test/test_auth_colab.py
 src/test/test_bim360.py
 src/test/test_bucket.py
 src/test/test_db_reader.py
```

### Comparing `aps-toolkit-0.5.8/src/test/context.py` & `aps-toolkit-0.5.9/src/test/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 from aps_toolkit import SVFMesh
 from aps_toolkit import Derivative
 from aps_toolkit import SVFReader
 from aps_toolkit import SVFMaterials
 from aps_toolkit import SVFImage
 from aps_toolkit import SVFMetadata
 from aps_toolkit import Bucket
+from aps_toolkit.units import DisplayUnits
 
 APS_CLIENT_ID = os.environ["APS_CLIENT_ID"]
 APS_CLIENT_SECRET = os.environ["APS_CLIENT_SECRET"]
```

### Comparing `aps-toolkit-0.5.8/src/test/test_auth.py` & `aps-toolkit-0.5.9/src/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_auth_colab.py` & `aps-toolkit-0.5.9/src/test/test_auth_colab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_bim360.py` & `aps-toolkit-0.5.9/src/test/test_bim360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_bucket.py` & `aps-toolkit-0.5.9/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_db_reader.py` & `aps-toolkit-0.5.9/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_derivative.py` & `aps-toolkit-0.5.9/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_fragment.py` & `aps-toolkit-0.5.9/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_geometries.py` & `aps-toolkit-0.5.9/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_image.py` & `aps-toolkit-0.5.9/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_material.py` & `aps-toolkit-0.5.9/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_mesh.py` & `aps-toolkit-0.5.9/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_prop_reader.py` & `aps-toolkit-0.5.9/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.5.9/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.5.9/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.8/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.5.9/src/test/test_prop_reader_revit.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,19 @@
         self.assertNotEquals(families, 0)
 
     def test_get_all_families_types(self):
         families_types = self.prop_reader.get_all_families_types()
         self.assertNotEquals(families_types, 0)
 
     def test_get_all_data(self):
-        data = self.prop_reader.get_all_data()
+        data = self.prop_reader.get_all_data(display_unit=True)
         self.assertIsNotNone(data)
 
     def test_get_data_by_category(self):
-        df = self.prop_reader.get_data_by_category("Windows", True)
+        df = self.prop_reader.get_data_by_category("Furniture", True, True)
         # check if dataframe have rows = 1
         df_rows = df.shape[0]
         self.assertNotEquals(df_rows, 0)
 
     def test_get_data_by_categories(self):
         df = self.prop_reader.get_data_by_categories(["Doors", "Windows"])
         self.assertNotEquals(df.empty, True)
@@ -66,15 +66,15 @@
         family_type = "Plastic-Seat"
         df = self.prop_reader.get_data_by_family_type(family_type)
         self.assertNotEquals(df.empty, True)
 
     def test_get_data_by_categories_and_params(self):
         df = self.prop_reader.get_data_by_categories_and_params(["Doors", "Windows"],
                                                                 ["name", "Category", "ElementId", "Width", "Height",
-                                                                 "IfcGUID"], True)
+                                                                 "IfcGUID"], True, display_unit=True)
         self.assertNotEquals(df.empty, True)
 
     def test_get_data_by_external_id(self):
         external_id = "6d22740f-4d3f-4cc6-a442-8c98ddd54f1f-0004923b"
         df = self.prop_reader.get_data_by_external_id(external_id, True)
         self.assertNotEquals(df.empty, True)
```

### Comparing `aps-toolkit-0.5.8/src/test/test_svf_reader.py` & `aps-toolkit-0.5.9/src/test/test_svf_reader.py`

 * *Files identical despite different names*


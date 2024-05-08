# Comparing `tmp/fiqus-2024.4.0.tar.gz` & `tmp/fiqus-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiqus-2024.4.0.tar", last modified: Tue Apr 30 14:32:54 2024, max compression
+gzip compressed data, was "fiqus-2024.5.0.tar", last modified: Wed May  8 15:10:50 2024, max compression
```

## Comparing `fiqus-2024.4.0.tar` & `fiqus-2024.5.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.238603 fiqus-2024.4.0/
--rw-rw-rw-   0        0        0     4607 2024-04-30 14:32:54.237604 fiqus-2024.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1719 2024-04-30 14:27:57.000000 fiqus-2024.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.152605 fiqus-2024.4.0/fiqus/
--rw-rw-rw-   0        0        0    13700 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/MainFiQuS.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.167606 fiqus-2024.4.0/fiqus/data/
--rw-rw-rw-   0        0        0     6396 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     7287 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuSCCT.py
--rw-rw-rw-   0        0        0     2403 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuSMultipole.py
--rw-rw-rw-   0        0        0   109796 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuSPancake3D.py
--rw-rw-rw-   0        0        0     2304 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataMultipole.py
--rw-rw-rw-   0        0        0     9036 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1709 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataWindingsCCT.py
--rw-rw-rw-   0        0        0     7162 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/RegionsModelFiQuS.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.172604 fiqus-2024.4.0/fiqus/geom_generators/
--rw-rw-rw-   0        0        0    49745 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/GeometryCCT.py
--rw-rw-rw-   0        0        0    24171 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/GeometryMultipole.py
--rw-rw-rw-   0        0        0   167791 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/GeometryPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.177604 fiqus-2024.4.0/fiqus/getdp_runners/
--rw-rw-rw-   0        0        0     3012 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpCCT.py
--rw-rw-rw-   0        0        0     4172 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpMultipole.py
--rw-rw-rw-   0        0        0     9744 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.182604 fiqus-2024.4.0/fiqus/mains/
--rw-rw-rw-   0        0        0     4414 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/MainCCT.py
--rw-rw-rw-   0        0        0     5075 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/MainMultipole.py
--rw-rw-rw-   0        0        0    21524 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/MainPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.187604 fiqus-2024.4.0/fiqus/mesh_generators/
--rw-rw-rw-   0        0        0    11338 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/MeshCCT.py
--rw-rw-rw-   0        0        0    14221 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/MeshMultipole.py
--rw-rw-rw-   0        0        0   120547 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/MeshPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.194604 fiqus-2024.4.0/fiqus/parsers/
--rw-rw-rw-   0        0        0      675 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserDAT.py
--rw-rw-rw-   0        0        0     8408 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserGetDPOnSection.py
--rw-rw-rw-   0        0        0     5098 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserGetDPTimeTable.py
--rw-rw-rw-   0        0        0     1912 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserMSH.py
--rw-rw-rw-   0        0        0    10121 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserPOS.py
--rw-rw-rw-   0        0        0     5984 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserRES.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.197607 fiqus-2024.4.0/fiqus/plotters/
--rw-rw-rw-   0        0        0     6333 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/plotters/PlotPythonCCT.py
--rw-rw-rw-   0        0        0      481 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/plotters/PlotPythonMultipole.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.205606 fiqus-2024.4.0/fiqus/post_processors/
--rw-rw-rw-   0        0        0    28443 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/PostProcessCCT.py
--rw-rw-rw-   0        0        0    15649 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/PostProcessMultipole.py
--rw-rw-rw-   0        0        0    13195 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/PostProcessPancake3D.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.208603 fiqus-2024.4.0/fiqus/pre_processors/
--rw-rw-rw-   0        0        0     9217 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pre_processors/PreProcessCCT.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pre_processors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.211604 fiqus-2024.4.0/fiqus/pro_assemblers/
--rw-rw-rw-   0        0        0     2770 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_assemblers/ProAssembler.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_assemblers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.212603 fiqus-2024.4.0/fiqus/pro_material_functions/
--rw-rw-rw-   0        0        0    17835 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_material_functions/ironBHcurves.pro
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.213606 fiqus-2024.4.0/fiqus/pro_templates/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.220603 fiqus-2024.4.0/fiqus/pro_templates/combined/
--rw-rw-rw-   0        0        0    13524 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/CCT_template.pro
--rw-rw-rw-   0        0        0     7956 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/Multipole_template.pro
--rw-rw-rw-   0        0        0   146175 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/Pancake3D_template.pro
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/__init__.py
--rw-rw-rw-   0        0        0     5525 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/materials.pro
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.221603 fiqus-2024.4.0/fiqus/pro_templates/separated/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/separated/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.222603 fiqus-2024.4.0/fiqus/utils/
--rw-rw-rw-   0        0        0    18489 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/utils/Utils.py
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.156604 fiqus-2024.4.0/fiqus.egg-info/
--rw-rw-rw-   0        0        0     4607 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1003 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 14:32:54.239604 fiqus-2024.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1595 2024-04-30 14:32:44.000000 fiqus-2024.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.228606 fiqus-2024.4.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/tests/__init__.py
--rw-rw-rw-   0        0        0    15537 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_FiQuS.py
--rw-rw-rw-   0        0        0     2034 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_geometry_generators.py
--rw-rw-rw-   0        0        0     2112 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_mesh_generators.py
--rw-rw-rw-   0        0        0     4224 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_solvers.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.231604 fiqus-2024.4.0/tests/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/utils/__init__.py
--rw-rw-rw-   0        0        0    24891 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/utils/fiqus_test_classes.py
--rw-rw-rw-   0        0        0     4149 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.900138 fiqus-2024.5.0/
+-rw-rw-rw-   0        0        0     4607 2024-05-08 15:10:50.899148 fiqus-2024.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1719 2024-04-30 14:27:57.000000 fiqus-2024.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.778229 fiqus-2024.5.0/fiqus/
+-rw-rw-rw-   0        0        0    13700 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/MainFiQuS.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.806138 fiqus-2024.5.0/fiqus/data/
+-rw-rw-rw-   0        0        0     6396 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7287 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/DataFiQuSCCT.py
+-rw-rw-rw-   0        0        0     2403 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/DataFiQuSMultipole.py
+-rw-rw-rw-   0        0        0   109796 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/DataFiQuSPancake3D.py
+-rw-rw-rw-   0        0        0     2304 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/DataMultipole.py
+-rw-rw-rw-   0        0        0     9036 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     1709 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/DataWindingsCCT.py
+-rw-rw-rw-   0        0        0     7162 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/RegionsModelFiQuS.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.814139 fiqus-2024.5.0/fiqus/geom_generators/
+-rw-rw-rw-   0        0        0    49745 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/geom_generators/GeometryCCT.py
+-rw-rw-rw-   0        0        0    24171 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/geom_generators/GeometryMultipole.py
+-rw-rw-rw-   0        0        0   167791 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/geom_generators/GeometryPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/geom_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.820138 fiqus-2024.5.0/fiqus/getdp_runners/
+-rw-rw-rw-   0        0        0     3012 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/getdp_runners/RunGetdpCCT.py
+-rw-rw-rw-   0        0        0     4172 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/getdp_runners/RunGetdpMultipole.py
+-rw-rw-rw-   0        0        0     9744 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/getdp_runners/RunGetdpPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/getdp_runners/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.824137 fiqus-2024.5.0/fiqus/mains/
+-rw-rw-rw-   0        0        0     4414 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mains/MainCCT.py
+-rw-rw-rw-   0        0        0     5075 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mains/MainMultipole.py
+-rw-rw-rw-   0        0        0    21524 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mains/MainPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.836140 fiqus-2024.5.0/fiqus/mesh_generators/
+-rw-rw-rw-   0        0        0    11338 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mesh_generators/MeshCCT.py
+-rw-rw-rw-   0        0        0    14221 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mesh_generators/MeshMultipole.py
+-rw-rw-rw-   0        0        0   120547 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mesh_generators/MeshPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/mesh_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.844139 fiqus-2024.5.0/fiqus/parsers/
+-rw-rw-rw-   0        0        0      675 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/parsers/ParserDAT.py
+-rw-rw-rw-   0        0        0     8408 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/parsers/ParserGetDPOnSection.py
+-rw-rw-rw-   0        0        0     5098 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/parsers/ParserGetDPTimeTable.py
+-rw-rw-rw-   0        0        0     1912 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/parsers/ParserMSH.py
+-rw-rw-rw-   0        0        0    10121 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/parsers/ParserPOS.py
+-rw-rw-rw-   0        0        0     5984 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/parsers/ParserRES.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.847139 fiqus-2024.5.0/fiqus/plotters/
+-rw-rw-rw-   0        0        0     6333 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/plotters/PlotPythonCCT.py
+-rw-rw-rw-   0        0        0      481 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/plotters/PlotPythonMultipole.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.851138 fiqus-2024.5.0/fiqus/post_processors/
+-rw-rw-rw-   0        0        0    28443 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/post_processors/PostProcessCCT.py
+-rw-rw-rw-   0        0        0    15649 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/post_processors/PostProcessMultipole.py
+-rw-rw-rw-   0        0        0    13195 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/post_processors/PostProcessPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/post_processors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.854139 fiqus-2024.5.0/fiqus/pre_processors/
+-rw-rw-rw-   0        0        0     9217 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pre_processors/PreProcessCCT.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pre_processors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.856138 fiqus-2024.5.0/fiqus/pro_assemblers/
+-rw-rw-rw-   0        0        0     2770 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_assemblers/ProAssembler.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_assemblers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.857137 fiqus-2024.5.0/fiqus/pro_material_functions/
+-rw-rw-rw-   0        0        0    17835 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_material_functions/ironBHcurves.pro
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.859139 fiqus-2024.5.0/fiqus/pro_templates/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.870137 fiqus-2024.5.0/fiqus/pro_templates/combined/
+-rw-rw-rw-   0        0        0    13524 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_templates/combined/CCT_template.pro
+-rw-rw-rw-   0        0        0     7956 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_templates/combined/Multipole_template.pro
+-rw-rw-rw-   0        0        0   146175 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_templates/combined/Pancake3D_template.pro
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_templates/combined/__init__.py
+-rw-rw-rw-   0        0        0     5525 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_templates/combined/materials.pro
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.871137 fiqus-2024.5.0/fiqus/pro_templates/separated/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/pro_templates/separated/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.873137 fiqus-2024.5.0/fiqus/utils/
+-rw-rw-rw-   0        0        0    18489 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/utils/Utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/fiqus/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.787984 fiqus-2024.5.0/fiqus.egg-info/
+-rw-rw-rw-   0        0        0     4607 2024-05-08 15:10:48.000000 fiqus-2024.5.0/fiqus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2233 2024-05-08 15:10:48.000000 fiqus-2024.5.0/fiqus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:10:48.000000 fiqus-2024.5.0/fiqus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1003 2024-05-08 15:10:48.000000 fiqus-2024.5.0/fiqus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 15:10:48.000000 fiqus-2024.5.0/fiqus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:10:50.901138 fiqus-2024.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1595 2024-05-08 14:19:04.000000 fiqus-2024.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.887140 fiqus-2024.5.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    15537 2024-04-30 14:28:07.000000 fiqus-2024.5.0/tests/test_FiQuS.py
+-rw-rw-rw-   0        0        0     2034 2024-04-30 14:28:07.000000 fiqus-2024.5.0/tests/test_geometry_generators.py
+-rw-rw-rw-   0        0        0     2112 2024-04-30 14:28:07.000000 fiqus-2024.5.0/tests/test_mesh_generators.py
+-rw-rw-rw-   0        0        0     4224 2024-04-30 14:28:07.000000 fiqus-2024.5.0/tests/test_solvers.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:10:50.893139 fiqus-2024.5.0/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:28:07.000000 fiqus-2024.5.0/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0    24891 2024-04-30 14:28:07.000000 fiqus-2024.5.0/tests/utils/fiqus_test_classes.py
+-rw-rw-rw-   0        0        0     4149 2024-04-30 14:28:07.000000 fiqus-2024.5.0/tests/utils/helpers.py
```

### Comparing `fiqus-2024.4.0/PKG-INFO` & `fiqus-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiqus
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Source code for STEAM FiQuS tool
 Home-page: https://gitlab.cern.ch/steam/fiqus
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 Keywords: STEAM,FiQuS,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
```

### Comparing `fiqus-2024.4.0/README.md` & `fiqus-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/MainFiQuS.py` & `fiqus-2024.5.0/fiqus/MainFiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/DataFiQuS.py` & `fiqus-2024.5.0/fiqus/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/DataFiQuSCCT.py` & `fiqus-2024.5.0/fiqus/data/DataFiQuSCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/DataFiQuSMultipole.py` & `fiqus-2024.5.0/fiqus/data/DataFiQuSMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/DataFiQuSPancake3D.py` & `fiqus-2024.5.0/fiqus/data/DataFiQuSPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/DataMultipole.py` & `fiqus-2024.5.0/fiqus/data/DataMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/DataRoxieParser.py` & `fiqus-2024.5.0/fiqus/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/DataWindingsCCT.py` & `fiqus-2024.5.0/fiqus/data/DataWindingsCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/data/RegionsModelFiQuS.py` & `fiqus-2024.5.0/fiqus/data/RegionsModelFiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/geom_generators/GeometryCCT.py` & `fiqus-2024.5.0/fiqus/geom_generators/GeometryCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/geom_generators/GeometryMultipole.py` & `fiqus-2024.5.0/fiqus/geom_generators/GeometryMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/geom_generators/GeometryPancake3D.py` & `fiqus-2024.5.0/fiqus/geom_generators/GeometryPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpCCT.py` & `fiqus-2024.5.0/fiqus/getdp_runners/RunGetdpCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpMultipole.py` & `fiqus-2024.5.0/fiqus/getdp_runners/RunGetdpMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpPancake3D.py` & `fiqus-2024.5.0/fiqus/getdp_runners/RunGetdpPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/mains/MainCCT.py` & `fiqus-2024.5.0/fiqus/mains/MainCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/mains/MainMultipole.py` & `fiqus-2024.5.0/fiqus/mains/MainMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/mains/MainPancake3D.py` & `fiqus-2024.5.0/fiqus/mains/MainPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/mesh_generators/MeshCCT.py` & `fiqus-2024.5.0/fiqus/mesh_generators/MeshCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/mesh_generators/MeshMultipole.py` & `fiqus-2024.5.0/fiqus/mesh_generators/MeshMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/mesh_generators/MeshPancake3D.py` & `fiqus-2024.5.0/fiqus/mesh_generators/MeshPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/parsers/ParserDAT.py` & `fiqus-2024.5.0/fiqus/parsers/ParserDAT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/parsers/ParserGetDPOnSection.py` & `fiqus-2024.5.0/fiqus/parsers/ParserGetDPOnSection.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/parsers/ParserGetDPTimeTable.py` & `fiqus-2024.5.0/fiqus/parsers/ParserGetDPTimeTable.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/parsers/ParserMSH.py` & `fiqus-2024.5.0/fiqus/parsers/ParserMSH.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/parsers/ParserPOS.py` & `fiqus-2024.5.0/fiqus/parsers/ParserPOS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/parsers/ParserRES.py` & `fiqus-2024.5.0/fiqus/parsers/ParserRES.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/plotters/PlotPythonCCT.py` & `fiqus-2024.5.0/fiqus/plotters/PlotPythonCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/post_processors/PostProcessCCT.py` & `fiqus-2024.5.0/fiqus/post_processors/PostProcessCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/post_processors/PostProcessMultipole.py` & `fiqus-2024.5.0/fiqus/post_processors/PostProcessMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/post_processors/PostProcessPancake3D.py` & `fiqus-2024.5.0/fiqus/post_processors/PostProcessPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/pre_processors/PreProcessCCT.py` & `fiqus-2024.5.0/fiqus/pre_processors/PreProcessCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/pro_assemblers/ProAssembler.py` & `fiqus-2024.5.0/fiqus/pro_assemblers/ProAssembler.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/pro_material_functions/ironBHcurves.pro` & `fiqus-2024.5.0/fiqus/pro_material_functions/ironBHcurves.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/pro_templates/combined/CCT_template.pro` & `fiqus-2024.5.0/fiqus/pro_templates/combined/CCT_template.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/pro_templates/combined/Multipole_template.pro` & `fiqus-2024.5.0/fiqus/pro_templates/combined/Multipole_template.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/pro_templates/combined/Pancake3D_template.pro` & `fiqus-2024.5.0/fiqus/pro_templates/combined/Pancake3D_template.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/pro_templates/combined/materials.pro` & `fiqus-2024.5.0/fiqus/pro_templates/combined/materials.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus/utils/Utils.py` & `fiqus-2024.5.0/fiqus/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus.egg-info/PKG-INFO` & `fiqus-2024.5.0/fiqus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiqus
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Source code for STEAM FiQuS tool
 Home-page: https://gitlab.cern.ch/steam/fiqus
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 Keywords: STEAM,FiQuS,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
```

### Comparing `fiqus-2024.4.0/fiqus.egg-info/SOURCES.txt` & `fiqus-2024.5.0/fiqus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/fiqus.egg-info/requires.txt` & `fiqus-2024.5.0/fiqus.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/setup.py` & `fiqus-2024.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "setuptools==65.3.0"
 ]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="fiqus",
-    version="2024.4.0",
+    version="2024.5.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for STEAM FiQuS tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/fiqus",
     keywords=["STEAM", "FiQuS", "CERN"],
```

### Comparing `fiqus-2024.4.0/tests/test_FiQuS.py` & `fiqus-2024.5.0/tests/test_FiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/tests/test_geometry_generators.py` & `fiqus-2024.5.0/tests/test_geometry_generators.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/tests/test_mesh_generators.py` & `fiqus-2024.5.0/tests/test_mesh_generators.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/tests/test_solvers.py` & `fiqus-2024.5.0/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/tests/utils/fiqus_test_classes.py` & `fiqus-2024.5.0/tests/utils/fiqus_test_classes.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.4.0/tests/utils/helpers.py` & `fiqus-2024.5.0/tests/utils/helpers.py`

 * *Files identical despite different names*


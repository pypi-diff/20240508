# Comparing `tmp/mdhelper-0.0.2.tar.gz` & `tmp/mdhelper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdhelper-0.0.2.tar", last modified: Tue Aug  1 03:01:16 2023, max compression
+gzip compressed data, was "mdhelper-1.0.0.tar", last modified: Wed May  8 04:01:43 2024, max compression
```

## Comparing `mdhelper-0.0.2.tar` & `mdhelper-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,72 @@
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.679887 mdhelper-0.0.2/
--rwxrwxrwx   0 bye       (1000) bye       (1000)    35148 2023-07-31 23:42:30.000000 mdhelper-0.0.2/LICENSE
--rwxrwxrwx   0 bye       (1000) bye       (1000)    45730 2023-08-01 03:01:18.677888 mdhelper-0.0.2/PKG-INFO
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4519 2023-08-01 01:10:54.000000 mdhelper-0.0.2/README.md
--rwxrwxrwx   0 bye       (1000) bye       (1000)      889 2023-08-01 00:55:39.000000 mdhelper-0.0.2/pyproject.toml
--rwxrwxrwx   0 bye       (1000) bye       (1000)       38 2023-08-01 03:01:18.679887 mdhelper-0.0.2/setup.cfg
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:17.802352 mdhelper-0.0.2/src/
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:17.879350 mdhelper-0.0.2/src/mdhelper/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      335 2023-08-01 00:06:54.000000 mdhelper-0.0.2/src/mdhelper/__init__.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.064379 mdhelper-0.0.2/src/mdhelper/algorithm/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      297 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    31675 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/correlation.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    22733 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/molecule.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     9398 2023-08-01 00:56:40.000000 mdhelper-0.0.2/src/mdhelper/algorithm/topology.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4078 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/utility.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.191950 mdhelper-0.0.2/src/mdhelper/analysis/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      311 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/analysis/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    12707 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/analysis/base.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    34372 2023-08-01 00:58:08.000000 mdhelper-0.0.2/src/mdhelper/analysis/polymer.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    25470 2023-08-01 01:00:38.000000 mdhelper-0.0.2/src/mdhelper/analysis/profile.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    40452 2023-08-01 01:02:44.000000 mdhelper-0.0.2/src/mdhelper/analysis/structure.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    44274 2023-08-01 01:04:20.000000 mdhelper-0.0.2/src/mdhelper/analysis/transport.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.329887 mdhelper-0.0.2/src/mdhelper/fit/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      442 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     2043 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/distribution.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     5175 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/exponential.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    15872 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/fourier.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    16781 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/gaussian.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    10617 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/polynomial.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     2023 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/power.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.500888 mdhelper-0.0.2/src/mdhelper/openmm/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      339 2023-08-01 00:55:13.000000 mdhelper-0.0.2/src/mdhelper/openmm/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     3125 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/bond.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    12753 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/file.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    32978 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/pair.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     6742 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/reporter.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    27274 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/system.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     8495 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/topology.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     3146 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/unit.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    11770 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/utility.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.558888 mdhelper-0.0.2/src/mdhelper/plot/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      284 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/plot/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4318 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/plot/axis.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     2613 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/plot/rcparam.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)      521 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/utility.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:17.961380 mdhelper-0.0.2/src/mdhelper.egg-info/
--rwxrwxrwx   0 bye       (1000) bye       (1000)    45730 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/PKG-INFO
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1461 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/SOURCES.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)        1 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/dependency_links.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)       48 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/requires.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)        9 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/top_level.txt
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.659886 mdhelper-0.0.2/tests/
--rwxrwxrwx   0 bye       (1000) bye       (1000)    20973 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_correlation.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     6697 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_molecule.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     3583 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_topology.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1394 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_utility.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1676 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_polymer.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1817 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_profile.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4704 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_structure.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     7204 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_transport.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:47.208100 mdhelper-1.0.0/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    35148 2023-08-01 21:14:44.000000 mdhelper-1.0.0/LICENSE
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    44501 2024-05-08 04:01:47.201477 mdhelper-1.0.0/PKG-INFO
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3067 2024-03-21 21:14:52.000000 mdhelper-1.0.0/README.md
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      976 2024-04-19 04:36:40.000000 mdhelper-1.0.0/pyproject.toml
+-rwxrwxrwx   0 bye       (1000) bye       (1000)       38 2024-05-08 04:01:47.209073 mdhelper-1.0.0/setup.cfg
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:45.972852 mdhelper-1.0.0/src/
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:46.047342 mdhelper-1.0.0/src/mdhelper/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      549 2024-03-11 05:05:50.000000 mdhelper-1.0.0/src/mdhelper/__init__.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:46.293076 mdhelper-1.0.0/src/mdhelper/algorithm/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      317 2024-04-28 05:42:29.000000 mdhelper-1.0.0/src/mdhelper/algorithm/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    15417 2024-05-06 02:35:56.000000 mdhelper-1.0.0/src/mdhelper/algorithm/accelerated.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    31169 2024-05-04 23:37:05.000000 mdhelper-1.0.0/src/mdhelper/algorithm/correlation.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    22940 2024-03-11 03:08:47.000000 mdhelper-1.0.0/src/mdhelper/algorithm/molecule.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    20548 2024-03-11 05:18:20.000000 mdhelper-1.0.0/src/mdhelper/algorithm/topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    10406 2024-05-01 07:16:31.000000 mdhelper-1.0.0/src/mdhelper/algorithm/unit.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     5468 2024-05-05 02:15:56.000000 mdhelper-1.0.0/src/mdhelper/algorithm/utility.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:46.471178 mdhelper-1.0.0/src/mdhelper/analysis/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      423 2024-03-09 04:35:59.000000 mdhelper-1.0.0/src/mdhelper/analysis/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    19958 2024-05-08 03:47:26.000000 mdhelper-1.0.0/src/mdhelper/analysis/base.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    18531 2024-03-13 08:33:30.000000 mdhelper-1.0.0/src/mdhelper/analysis/electrostatics.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    43986 2024-03-11 03:56:14.000000 mdhelper-1.0.0/src/mdhelper/analysis/polymer.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    39225 2024-05-08 03:49:36.000000 mdhelper-1.0.0/src/mdhelper/analysis/profile.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    80388 2024-05-08 03:54:19.000000 mdhelper-1.0.0/src/mdhelper/analysis/structure.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     9299 2024-05-01 07:49:47.000000 mdhelper-1.0.0/src/mdhelper/analysis/thermodynamics.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    50033 2024-05-01 07:47:25.000000 mdhelper-1.0.0/src/mdhelper/analysis/transport.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:46.617398 mdhelper-1.0.0/src/mdhelper/fit/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      437 2024-03-11 05:08:08.000000 mdhelper-1.0.0/src/mdhelper/fit/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1992 2024-02-18 06:51:56.000000 mdhelper-1.0.0/src/mdhelper/fit/distribution.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6139 2024-02-18 06:51:53.000000 mdhelper-1.0.0/src/mdhelper/fit/exponential.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    15855 2024-02-18 06:51:50.000000 mdhelper-1.0.0/src/mdhelper/fit/fourier.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    16773 2024-02-18 06:51:47.000000 mdhelper-1.0.0/src/mdhelper/fit/gaussian.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    10566 2024-02-18 06:51:41.000000 mdhelper-1.0.0/src/mdhelper/fit/polynomial.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2012 2024-02-18 06:51:44.000000 mdhelper-1.0.0/src/mdhelper/fit/power.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:46.660398 mdhelper-1.0.0/src/mdhelper/lammps/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      208 2024-03-11 05:07:41.000000 mdhelper-1.0.0/src/mdhelper/lammps/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     7104 2024-03-10 06:35:09.000000 mdhelper-1.0.0/src/mdhelper/lammps/topology.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:46.869906 mdhelper-1.0.0/src/mdhelper/openmm/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      335 2024-02-18 06:52:15.000000 mdhelper-1.0.0/src/mdhelper/openmm/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3580 2024-03-05 21:50:53.000000 mdhelper-1.0.0/src/mdhelper/openmm/bond.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    24156 2024-03-05 21:50:53.000000 mdhelper-1.0.0/src/mdhelper/openmm/file.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    49089 2024-03-05 21:50:53.000000 mdhelper-1.0.0/src/mdhelper/openmm/pair.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6367 2024-02-18 06:52:25.000000 mdhelper-1.0.0/src/mdhelper/openmm/reporter.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    43386 2024-04-30 22:16:15.000000 mdhelper-1.0.0/src/mdhelper/openmm/system.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     8715 2024-02-18 06:52:33.000000 mdhelper-1.0.0/src/mdhelper/openmm/topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3283 2024-03-10 21:54:40.000000 mdhelper-1.0.0/src/mdhelper/openmm/unit.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    11992 2024-03-07 07:49:11.000000 mdhelper-1.0.0/src/mdhelper/openmm/utility.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:46.957419 mdhelper-1.0.0/src/mdhelper/plot/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      281 2024-02-18 06:52:43.000000 mdhelper-1.0.0/src/mdhelper/plot/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4388 2024-02-18 06:52:46.000000 mdhelper-1.0.0/src/mdhelper/plot/axis.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1495 2024-03-21 21:07:18.000000 mdhelper-1.0.0/src/mdhelper/plot/color.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3114 2024-03-11 22:26:09.000000 mdhelper-1.0.0/src/mdhelper/plot/rcparam.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:47.192476 mdhelper-1.0.0/src/mdhelper.egg-info/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    44501 2024-05-08 04:01:45.000000 mdhelper-1.0.0/src/mdhelper.egg-info/PKG-INFO
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1835 2024-05-08 04:01:45.000000 mdhelper-1.0.0/src/mdhelper.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)        1 2024-05-08 04:01:45.000000 mdhelper-1.0.0/src/mdhelper.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)       60 2024-05-08 04:01:45.000000 mdhelper-1.0.0/src/mdhelper.egg-info/requires.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)        9 2024-05-08 04:01:45.000000 mdhelper-1.0.0/src/mdhelper.egg-info/top_level.txt
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-08 04:01:47.170959 mdhelper-1.0.0/tests/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    20854 2024-03-07 07:49:21.000000 mdhelper-1.0.0/tests/test_algorithm_correlation.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6644 2024-03-11 03:09:24.000000 mdhelper-1.0.0/tests/test_algorithm_molecule.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4771 2024-03-10 10:00:40.000000 mdhelper-1.0.0/tests/test_algorithm_topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3001 2024-03-10 21:48:44.000000 mdhelper-1.0.0/tests/test_algorithm_unit.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1530 2024-03-10 21:47:43.000000 mdhelper-1.0.0/tests/test_algorithm_utility.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1157 2024-03-10 10:00:47.000000 mdhelper-1.0.0/tests/test_analysis_electrostatics.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2289 2024-04-19 07:52:59.000000 mdhelper-1.0.0/tests/test_analysis_polymer.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1831 2024-05-08 03:47:35.000000 mdhelper-1.0.0/tests/test_analysis_profile.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    12176 2024-05-08 03:49:31.000000 mdhelper-1.0.0/tests/test_analysis_structure.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     7378 2024-05-05 03:18:17.000000 mdhelper-1.0.0/tests/test_analysis_transport.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     5507 2024-03-10 21:54:54.000000 mdhelper-1.0.0/tests/test_openmm_file_reporter.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3670 2024-03-07 07:50:30.000000 mdhelper-1.0.0/tests/test_openmm_topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1319 2024-02-18 04:17:09.000000 mdhelper-1.0.0/tests/test_openmm_unit.py
```

### Comparing `mdhelper-0.0.2/LICENSE` & `mdhelper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.2/PKG-INFO` & `mdhelper-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mdhelper
-Version: 0.0.2
+Version: 1.0.0
 Summary: A batteries-included toolkit of analysis modules and helper functions 
-Author-email: "Benjamin B. Ye" <bye@caltech.edu>
+Author-email: "Benjamin B. Ye" <bye@caltech.edu>, "Pierre J. Walker" <pjwalker@caltech.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -680,152 +680,91 @@
 Project-URL: Homepage, https://github.com/bbye98/mdhelper
 Project-URL: Bug Tracker, https://github.com/bbye98/mdhelper/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: mdanalysis
+Requires-Dist: netCDF4
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pint
+Requires-Dist: scipy
+Requires-Dist: sympy
+
+<img src="https://raw.githubusercontent.com/bbye98/mdhelper/main/assets/logo.png" align="right" width="256"/>
 
 # MDHelper
 
-MDHelper is a batteries-included toolkit of analysis modules and helper
+[![continuous-integration](https://github.com/bbye98/mdhelper/actions/workflows/ci.yml/badge.svg)](https://github.com/bbye98/mdhelper/actions/workflows/ci.yml)
+
+MDHelper is a toolkit of optimized analysis modules and helper
 functions for molecular dynamics (MD) simulations.
 
 * **Documentation**: https://bbye98.github.io/mdhelper/
+* **Conda**: https://anaconda.org/bbye98/mdhelper
 * **Python Package Index (PyPI)**: https://pypi.org/project/mdhelper/
 
 Note that MDHelper is currently an *experimental* library that has 
 only been tested on Linux and may contain bugs and issues. If you come 
-across one, please 
-[submit a new issue](https://github.com/bbye98/mdhelper/issues/new). If 
-you would like to contribute to MDHelper, please 
-[submit a pull request](https://github.com/bbye98/mdhelper/compare).
+across one or would like to request new features, please 
+[submit a new issue](https://github.com/bbye98/mdhelper/issues/new).
 
 ## Features
 
 * [`algorithm`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/algorithm): 
-Efficient NumPy algorithms for data wrangling and evaluating structural 
-and dynamical properties.
+Efficient NumPy and SciPy algorithms for data wrangling and evaluating 
+structural and dynamical properties.
 * [`analysis`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/analysis): 
 Serial and parallel data analysis tools built on top of the MDAnalysis 
 framework.
 * [`fit`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/fit): 
 Two-dimensional curve fitting models for use with SciPy.
+* [`lammps`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/lammps):
+Helper functions for setting up LAMMPS simulations.
 * [`openmm`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/openmm): 
 Extensions to the high-performance OpenMM toolkit, such as custom 
 bond/pair potentials, support for NetCDF trajectories, and much more.
 * [`plot`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/plot): 
 Settings and additional functionality for Matplotlib figures.
-* [`utility`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/utility): 
-General utility functions.
-
-## Installation and usage
-
-### Prerequisites
-
-If you use pip to manage your Python packages or plan on using OpenMM
-with third-party extensions, such as 
-[`constvplugin`](https://github.com/scychon/openmm_constV) for the
-method of image charges, you must compile and install OpenMM prior to
-installing MDHelper. See the 
-["Compiling OpenMM from Source Code"](http://docs.openmm.org/latest/userguide/library/02_compiling.html) 
-for more section of the OpenMM User Guide for more information. This 
-additional step is necessary since precompiled versions of OpenMM do not
-expose their header files, which are needed to link against custom 
-plugins. Otherwise, the lastest precompiled version of OpenMM on 
-conda-forge will be installed during the installation of MDHelper.
-
-### Virtual environment
-
-It is recommended, but not necessary, that you create a virtual 
-environment to prevent dependency conflicts.
-
-If you are using pip to manage Python packages, use
-
-    virtualenv venv
-    source venv/bin/activate
-
-where `venv` is the name of the new environment.
-
-If you are using Anaconda or Miniconda, use
-
-    conda create --name venv
-    conda activate venv
-
-### Install using pip
-
- 1. Install MDHelper and its dependencies using 
-
-    pip install mdhelper
-
-### Install using Anaconda or Miniconda
-
- 1. Add the conda-forge channel using
-
-        conda config --add channels conda-forge
 
- 2. Install MDHelper and its dependencies using
+## Installation
 
-        conda install mdhelper
+MDHelper requires Python 3.9 or later.
 
-### Build from source
+For the most up-to-date version of MDHelper, clone the repository and install
+the package using pip:
 
- 1. Ensure that the latest version of the Python build frontend, 
-    `build`, is installed:
+    git clone https://github.com/bbye98/mdhelper.git
+    cd mdhelper
+    python -m pip install -e .
 
-        python3 -m pip install --upgrade build
+MDHelper is also available on Conda and PyPI:
 
- 2. Create a local copy of the MDHelper repository on your machine using
+    conda install -c bbye98 mdhelper
+    python -m pip install mdhelper
 
-        git clone https://github.com/bbye98/mdhelper.git
-
- 3. Enter the root directory of MDHelper using
-
-        cd mdhelper
-
- 4. Build the MDHelper wheel using
-
-        python3 -m build
-
-    The Python wheel will be placed in the `dist` directory.
-
- 5. Install MDHelper using
-
-        python3 -m pip install dist/mdhelper-<version>-py3-none-any.whl
-
-    where `<version>` is the version of MDHelper you are installing.
-
-### Portable package
-
- 1. Change to the directory where you want to store a copy of MDHelper using
-
-        cd <directory>
-
-    where `<directory>` is the relative path to the desired directory.
-    
-    If you are already in the correct location, skip this step.
-
- 2. Create a local copy of the MDHelper repository on your machine using
-
-        git clone https://github.com/bbye98/mdhelper.git
-
- 3. Enter the root directory of MDHelper using
-
-        cd mdhelper
-
- 4. Install the dependencies using
+### Prerequisites
 
-        pip install -r requirements.txt
+If you use pip to manage your Python packages, you must compile and 
+install OpenMM prior to installing MDHelper since OpenMM is not 
+available in PyPI. See the 
+["Compiling OpenMM from Source Code"](http://docs.openmm.org/latest/userguide/library/02_compiling.html) 
+section of the OpenMM User Guide for more information.
 
-    or
+If you use Conda, it is recommended that you use the conda-forge 
+channel to install dependencies. To make conda-forge the default 
+channel, use
 
-        conda install --file requirements.txt
+    conda config --add channels conda-forge
 
- 5. Once done, you can use MDHelper by first adding the path to the 
-    `src` directory in your Python scripts:
+### Postrequisites
 
-        import sys
-        sys.path.insert(0, "/path/to/mdhelper/src")
-        import mdhelper
+To use the image of method charges 
+(`mdhelper.openmm.system.add_image_charges()`) in your OpenMM simulations, you must
+compile and install [`constvplugin`](https://github.com/scychon/openmm_constV) or
+[`openmm-ic-plugin`](https://github.com/bbye98/mdhelper/tree/main/lib/openmm-ic-plugin).
```

### Comparing `mdhelper-0.0.2/pyproject.toml` & `mdhelper-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "mdhelper"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
-  { name = "Benjamin B. Ye", email = "bye@caltech.edu" }
+  { name = "Benjamin B. Ye", email = "bye@caltech.edu" },
+  { name = "Pierre J. Walker", email = "pjwalker@caltech.edu" }
 ]
 classifiers = [
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3"
 ]
 dependencies = [
   "matplotlib",
   "mdanalysis",
   "netCDF4",
   "numpy",
+  "pandas",
+  "pint",
   "scipy",
   "sympy"
 ]
 description = """
 A batteries-included toolkit of analysis modules and helper functions 
 for molecular dynamics (MD) simulations.
 """
 license = { file = "LICENSE" }
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.9"
 
 [project.urls]
 "Homepage" = "https://github.com/bbye98/mdhelper"
 "Bug Tracker" = "https://github.com/bbye98/mdhelper/issues"
```

### Comparing `mdhelper-0.0.2/src/mdhelper/algorithm/correlation.py` & `mdhelper-1.0.0/src/mdhelper/algorithm/correlation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 """
 Statistical correlation
 =======================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
-This module contains algorithms for computing the correlation between 
+This module contains algorithms for computing the correlation between
 data with various shapes that evolve over time. This includes real- and
-Fourier-space evaluations of the autocorrelation and cross-correlation 
+Fourier-space evaluations of the autocorrelation and cross-correlation
 functions, and by extension, the mean squared and cross displacements.
 """
 
 import warnings
 
 import numpy as np
 from scipy import fft
 
 def correlation_fft(
-        arr1: np.ndarray, arr2: np.ndarray = None, axis: int = None, *,
-        average: bool = False, double: bool = False, vector: bool = False
-    ) -> np.ndarray:
+        arr1: np.ndarray[float], arr2: np.ndarray[float] = None,
+        axis: int = None, *, average: bool = False, double: bool = False,
+        vector: bool = False) -> np.ndarray[float]:
 
     r"""
     Evaluates the autocorrelation function (ACF) or cross-correlation
-    function (CCF) of a time series using fast Fourier transforms (FFT). 
+    function (CCF) of a time series using fast Fourier transforms (FFT).
 
     The algorithm, better known as the Fast Correlation Algorithm (FCA)
     [1]_ [2]_, is a result of the Wiener–Khinchin theorem and has a time
     complexity of :math:`\mathcal{O}(N\log{N})`. Effectively, the ACF
-    can be computed from the raw data :math:`\mathbf{r}(t)` with two 
+    can be computed from the raw data :math:`\mathbf{r}(t)` with two
     FFTs using
 
     .. math::
 
        \begin{gather*}
          \hat{\mathbf{r}}(\xi)=\mathrm{FFT}(\mathbf{r}(t))\\
          A(\tau)=\mathrm{FFT}^{-1}(\hat{\mathbf{r}}(\xi)\hat{\mathbf{r}}^*(\xi))
        \end{gather*}
 
-    where :math:`\tau` is the time lag and the asterisk (:math:`^*`) 
+    where :math:`\tau` is the time lag and the asterisk (:math:`^*`)
     denotes the complex conjugate.
 
     Similarly, the CCF for species :math:`i` and :math:`j` is evaluated
     using
 
     .. math::
 
        C_{ij}(\tau)=\mathrm{FFT}^{-1}(\mathrm{FFT}(\mathbf{r}_i(t))
        \cdot\mathrm{FFT}(\mathbf{r}_j(t)))
 
     Parameters
     ----------
     arr1 : `numpy.ndarray`
         Time evolution of :math:`N` entities over :math:`N_\mathrm{b}`
-        blocks of :math:`N_t` frames each. 
+        blocks of :math:`N_t` frames each.
 
         .. container::
 
-           **Shape**: 
-           
+           **Shape**:
+
            * Scalar: :math:`(N_t,)`, :math:`(N_t,\,N)`,
              :math:`(N_\mathrm{b},\,N_t)`, or
              :math:`(N_\mathrm{b},\,N_t,\,N)`.
-           * Vector: :math:`(N_t,\,d)`, 
+           * Vector: :math:`(N_t,\,d)`,
              :math:`(N_t,\,N,\,N_\mathrm{d})`,
-             :math:`(N_\mathrm{b},\,N_t,\,N_\mathrm{d})`, or 
-             :math:`(N_\mathrm{b},\,N_t,\,N,\,N_\mathrm{d})`, where 
-             :math:`N_\mathrm{d}` is the number of dimensions each 
+             :math:`(N_\mathrm{b},\,N_t,\,N_\mathrm{d})`, or
+             :math:`(N_\mathrm{b},\,N_t,\,N,\,N_\mathrm{d})`, where
+             :math:`N_\mathrm{d}` is the number of dimensions each
              vector has.
 
     arr2 : `numpy.ndarray`, optional
         Time evolution of another :math:`N` entities. If provided, the
-        CCF for `arr1` and `arr2` is calculated. Otherwise, the ACF for 
+        CCF for `arr1` and `arr2` is calculated. Otherwise, the ACF for
         `arr1` is calculated.
-        
+
         **Shape**: Same as `arr1`.
 
     axis : `int`, optional
         Axis along which to evaluate the ACF/CCF. If `arr1` contains a
         full, unsplit trajectory, the ACF/CCF should be evaluated along
-        the first axis (:code:`axis=0`). If `arr1` contains a 
-        trajectory split into multiple blocks, the ACF/CCF should be 
+        the first axis (:code:`axis=0`). If `arr1` contains a
+        trajectory split into multiple blocks, the ACF/CCF should be
         evaluated along the second axis (:code:`axis=1`). If not
         specified, the axis is determined automatically using the shape
         of `arr1`.
 
     average : `bool`, keyword-only, default: :code:`True`
         Determines whether the ACF/CCF is averaged over all entities if
         the arrays contain information for multiple entities.
 
     double : `bool`, keyword-only, default: :code:`False`
         If :code:`True`, the ACF is doubled or the CCFs for the negative
-        and positive time lags are combined. Useful for evaluating the 
+        and positive time lags are combined. Useful for evaluating the
         mean squared or cross displacement. See
-        :func:`mdhelper.algorithm.correlation.msd_fft` for more 
+        :func:`mdhelper.algorithm.correlation.msd_fft` for more
         information.
 
     vector : `bool`, keyword-only, default: :code:`False`
-        Specifies whether `arr1` and `arr2` contain vectors. If 
+        Specifies whether `arr1` and `arr2` contain vectors. If
         :code:`True`, the ACF/CCF is summed over the last dimension.
 
     Returns
     -------
     corr : `numpy.ndarray`
         Autocorrelation or cross-correlation function.
 
@@ -115,47 +115,45 @@
            * If :code:`vector=True`, the last dimension is removed.
 
            For CCF, the shape is that of `arr1` but with the following
            modifications:
 
            * If :code:`average=True`, the axis containing the :math:`N`
              entities is removed.
-           * If :code:`double=False`, the axis containing the 
+           * If :code:`double=False`, the axis containing the
              :math:`N_t` times now has a length of :math:`2N_t-1` to
              accomodate negative and positive time lags.
            * If :code:`vector=True`, the last dimension is removed.
 
     References
     ----------
-    .. [1] Kneller, G. R.; Keiner, V.; Kneller, M.; Schiller, M. 
-       NMOLDYN: A Program Package for a Neutron Scattering Oriented 
+    .. [1] Kneller, G. R.; Keiner, V.; Kneller, M.; Schiller, M.
+       NMOLDYN: A Program Package for a Neutron Scattering Oriented
        Analysis of Molecular Dynamics Simulations. *Computer Physics
-       Communications* **1995**, *91* (1–3), 191–214. 
+       Communications* **1995**, *91* (1–3), 191–214.
        https://doi.org/10.1016/0010-4655(95)00048-K.
 
     .. [2] Calandrini, V.; Pellegrini, E.; Calligari, P.; Hinsen, K.;
        Kneller, G. R. NMoldyn - Interfacing Spectroscopic Experiments,
        Molecular Dynamics Simulations and Models for Time Correlation
        Functions. *JDN* **2011**, *12*, 201–232.
        https://doi.org/10.1051/sfn/201112010.
     """
 
     # Ensure arrays have valid dimensionality
-    if not isinstance(arr1, np.ndarray):
-        arr1 = np.array(arr1)
+    arr1 = np.asarray(arr1)
     if arr1.size == 0:
         raise ValueError("The arrays must not be empty.")
     ndim = arr1.ndim
     if not 1 <= ndim <= 4:
         emsg = ("The arrays must be one-, two-, three-, or four-"
                 "dimensional.")
         raise ValueError(emsg)
     if arr2 is not None:
-        if not isinstance(arr2, np.ndarray):
-            arr2 = np.array(arr2)
+        arr2 = np.asarray(arr2)
         if arr1.shape != arr2.shape:
             emsg = "The arrays must have the same dimensions."
             raise ValueError(emsg)
 
     # Check or set axis along which to compute the ACF/CCF
     if axis is None:
         if ndim == 4:
@@ -169,156 +167,156 @@
                         "set to the first axis by default.")
                 warnings.warn(wmsg)
     elif axis not in {0, 1}:
         emsg = ("The ACF/CCF can only be evaluated along the first or "
                 "second axis.")
         raise ValueError(emsg)
 
-    # Get number of frames
-    N_t = arr1.shape[axis]
-
     # Calculate the PSD by first zero-padding the arrays for linear
     # convolution, and then invert it to get the ACF/CCF
+    N_t = arr1.shape[axis]
+    all_real = np.isrealobj(arr1) and (arr2 is None or np.isrealobj(arr2))
+    N_fft = 2 * fft.next_fast_len(N_t, real=all_real)
+    if all_real:
+        _fft = fft.rfft
+        _ifft = fft.irfft
+    else:
+        _fft = fft.fft
+        _ifft = fft.ifft
     if arr2 is None:
-        f = fft.rfft(arr1, n=2 * N_t, axis=axis)
-        corr = (double + 1) * fft.irfft(f * f.conjugate(), axis=axis)
-        corr = corr[:, :N_t] if axis else corr[:N_t]
+        f = _fft(arr1, n=N_fft, axis=axis)
+        corr = _ifft(f * f.conj(), axis=axis)
+        corr = (double + 1) * (corr[:, :N_t] if axis else corr[:N_t])
     else:
-        f1 = fft.rfft(arr1, n=2 * N_t, axis=axis)
-        f2 = fft.rfft(arr2, n=2 * N_t, axis=axis)
-        f = f1.conjugate() * f2
+        f1 = _fft(arr1, n=N_fft, axis=axis)
+        f2 = _fft(arr2, n=N_fft, axis=axis)
+        f = f1.conj() * f2
         if double:
-            corr = fft.irfft(f + f1 * f2.conjugate(), axis=axis)
+            corr = _ifft(f + f1 * f2.conj(), axis=axis)
             corr = corr[:, :N_t] if axis else corr[:N_t]
         else:
-            corr = fft.irfft(f, axis=axis)
+            corr = _ifft(f, axis=axis)
 
-    # Determine the axes over which to expand the reversed
-    # time array for correct matrix division
+    # Sum over the last dimension if the arrays contain vectors
     if vector:
-        axes = list(range(ndim - 1))
-        if axis in axes:
-            axes.remove(axis)
-
-        # Sum over the last dimension if the arrays contain vectors
         corr = corr.sum(axis=-1)
-    elif axis:
-        axes = list(range(ndim))
-        if axis in axes:
-            axes.remove(axis)
-    else:
-        axes = list(range(1, ndim))
+
+    # Determine the axes over which to expand the reversed
+    # time array for correct matrix division
+    axes = list(range(ndim - vector))
+    axes.remove(axis)
 
     # Normalize the ACF/CCF
     if axis:
         corr[:, :N_t] /= np.expand_dims(range(N_t, 0, -1), axes)
         if corr.shape[axis] != N_t:
             corr[:, 1 - N_t:] /= np.expand_dims(range(1, N_t), axes)
             corr = np.hstack((corr[:, 1 - N_t:], corr[:, :N_t]))
     else:
         corr[:N_t] /= np.expand_dims(range(N_t, 0, -1), axes)
         if corr.shape[axis] != N_t:
             corr[1 - N_t:] /= np.expand_dims(range(1, N_t), axes)
             corr = np.concatenate((corr[1 - N_t:], corr[:N_t]))
-    
+
     # Average over all entities, if desired
     if average:
-        axis_avg = ndim - 1 - vector
+        axis_avg = ndim - vector - 1
         if axis != axis_avg:
             return corr.mean(axis=axis_avg)
+
     return corr
 
 def correlation_shift(
-        arr1: np.ndarray, arr2: np.ndarray = None, axis: int = None, 
-        vector: bool = False, *, average: bool = False, double: bool = False
-    ) -> np.ndarray:
+        arr1: np.ndarray[float], arr2: np.ndarray[float] = None,
+        axis: int = None, *, average: bool = False, double: bool = False,
+        vector: bool = False) -> np.ndarray[float]:
 
     r"""
     Evaluates the autocorrelation function (ACF) or cross-correlation
     function (CCF) of a time series directly by using sliding windows
     along the time axis.
 
-    For scalars :math:`r` or vectors :math:`\mathbf{r}`, the ACF is 
+    For scalars :math:`r` or vectors :math:`\mathbf{r}`, the ACF is
     defined as
 
     .. math::
 
         A(\tau)=\langle\textbf{r}(t_0+\tau)\cdot\textbf{r}(t_0)\rangle
         =\dfrac{1}{N}\sum_{\alpha=1}^N
         \textbf{r}_\alpha(t_0+\tau)\cdot\textbf{r}_\alpha(t_0)
-        
+
     while the CCF for species :math:`i` and :math:`j` is given by
-    
+
     .. math::
 
         C_{ij}(\tau)=\langle\textbf{r}_i(t_0+\tau)\cdot
         \textbf{r}_j(t_0)\rangle
         =\dfrac{1}{N}\sum_{\alpha=1}^N\textbf{r}_{i,\alpha}(t_0+\tau)\cdot
         \textbf{r}_{j,\alpha}(t_0)
 
-    where :math:`\tau` is the time lag, :math:`t_0` is an arbitrary 
+    where :math:`\tau` is the time lag, :math:`t_0` is an arbitrary
     reference time, and :math:`N` is the number of entities. To reduce
     statistical noise, the ACF/CCF is calculated for and averaged over
-    all possible reference times :math:`t_0`. As such, this algorithm 
+    all possible reference times :math:`t_0`. As such, this algorithm
     has a time complexity of :math:`\mathcal{O}(N^2)`.
 
-    With large data sets, this approach is too slow to be useful. If 
-    your machine supports the fast Fourier transform (FFT), consider 
+    With large data sets, this approach is too slow to be useful. If
+    your machine supports the fast Fourier transform (FFT), consider
     using the much more performant FFT-based algorithm implemented in
     :func:`mdhelper.algorithm.correlation.correlation_fft` instead.
 
     Parameters
     ----------
     arr1 : `numpy.ndarray`
         Time evolution of :math:`N` entities over :math:`N_\mathrm{b}`
-        blocks of :math:`N_t` frames each. 
+        blocks of :math:`N_t` frames each.
 
         .. container::
 
-           **Shape**: 
-           
+           **Shape**:
+
            * Scalar: :math:`(N_t,)`, :math:`(N_t,\,N)`,
              :math:`(N_\mathrm{b},\,N_t)`, or
              :math:`(N_\mathrm{b},\,N_t,\,N)`.
-           * Vector: :math:`(N_t,\,d)`, 
+           * Vector: :math:`(N_t,\,d)`,
              :math:`(N_t,\,N,\,N_\mathrm{d})`,
-             :math:`(N_\mathrm{b},\,N_t,\,N_\mathrm{d})`, or 
-             :math:`(N_\mathrm{b},\,N_t,\,N,\,N_\mathrm{d})`, where 
-             :math:`N_\mathrm{d}` is the number of dimensions each 
+             :math:`(N_\mathrm{b},\,N_t,\,N_\mathrm{d})`, or
+             :math:`(N_\mathrm{b},\,N_t,\,N,\,N_\mathrm{d})`, where
+             :math:`N_\mathrm{d}` is the number of dimensions each
              vector has.
 
     arr2 : `numpy.ndarray`, optional
         Time evolution of another :math:`N` entities. If provided, the
-        CCF for `arr1` and `arr2` is calculated. Otherwise, the ACF for 
+        CCF for `arr1` and `arr2` is calculated. Otherwise, the ACF for
         `arr1` is calculated.
-        
+
         **Shape**: Same as `arr1`.
 
     axis : `int`, optional
         Axis along which to evaluate the ACF/CCF. If `arr1` contains a
         full, unsplit trajectory, the ACF/CCF should be evaluated along
-        the first axis (:code:`axis=0`). If `arr1` contains a 
-        trajectory split into multiple blocks, the ACF/CCF should be 
+        the first axis (:code:`axis=0`). If `arr1` contains a
+        trajectory split into multiple blocks, the ACF/CCF should be
         evaluated along the second axis (:code:`axis=1`). If not
         specified, the axis is determined automatically using the shape
         of `arr1`.
 
     average : `bool`, keyword-only, default: :code:`True`
         Determines whether the ACF/CCF is averaged over all entities if
         the arrays contain information for multiple entities.
 
     double : `bool`, keyword-only, default: :code:`False`
         If :code:`True`, the ACF is doubled or the CCFs for the negative
-        and positive time lags are combined. Useful for evaluating the 
+        and positive time lags are combined. Useful for evaluating the
         mean squared or cross displacement. See
-        :func:`mdhelper.algorithm.correlation.msd_shift` for more 
+        :func:`mdhelper.algorithm.correlation.msd_shift` for more
         information.
 
     vector : `bool`, keyword-only, default: :code:`False`
-        Specifies whether `arr1` and `arr2` contain vectors. If 
+        Specifies whether `arr1` and `arr2` contain vectors. If
         :code:`True`, the ACF/CCF is summed over the last dimension.
 
     Returns
     -------
     corr : `numpy.ndarray`
         Autocorrelation or cross-correlation function.
 
@@ -334,33 +332,31 @@
            * If :code:`vector=True`, the last dimension is removed.
 
            For CCF, the shape is that of `arr1` but with the following
            modifications:
 
            * If :code:`average=True`, the axis containing the :math:`N`
              entities is removed.
-           * If :code:`double=False`, the axis containing the 
+           * If :code:`double=False`, the axis containing the
              :math:`N_t` times now has a length of :math:`2N_t-1` to
              accomodate negative and positive time lags.
            * If :code:`vector=True`, the last dimension is removed.
     """
 
     # Ensure arrays have valid dimensionality
-    if not isinstance(arr1, np.ndarray):
-        arr1 = np.array(arr1)
+    arr1 = np.asarray(arr1)
     if arr1.size == 0:
         raise ValueError("The arrays must not be empty.")
     ndim = arr1.ndim
     if not 1 <= ndim <= 4:
         emsg = ("The arrays must be one-, two-, three-, or four-"
                 "dimensional.")
         raise ValueError(emsg)
     if arr2 is not None:
-        if not isinstance(arr2, np.ndarray):
-            arr2 = np.array(arr2)
+        arr2 = np.asarray(arr2)
         if arr1.shape != arr2.shape:
             emsg = "The arrays must have the same dimensions."
             raise ValueError(emsg)
 
     # Check or set axis along which to compute the ACF/CCF
     if axis is None:
         if ndim == 4:
@@ -374,65 +370,63 @@
                         "set to the first axis by default.")
                 warnings.warn(wmsg)
     elif axis not in {0, 1}:
         emsg = ("The ACF/CCF can only be evaluated along the first or "
                 "second axis.")
         raise ValueError(emsg)
 
-    # Get number of frames
-    N_t = arr1.shape[axis]
-
     # Calculate the ACF/CCF
+    N_t = arr1.shape[axis]
     if arr2 is None:
         if ndim == 1:
             corr = np.fromiter(
-                (np.dot(arr1[i:], arr1[:-i if i else None]) 
+                (np.dot(arr1[i:], arr1[:-i if i else None])
                  for i in range(N_t)),
-                count=N_t, dtype=float
+                dtype=float, count=N_t,
             )
         elif axis:
             axes = f"bt...{'d' * vector}"
             corr = np.stack(
-                [np.einsum(f"{axes},{axes}->b...", 
-                           arr1[:, i:], arr1[:, :-i if i else None]) 
+                [np.einsum(f"{axes},{axes}->b...",
+                           arr1[:, i:], arr1[:, :-i if i else None])
                  for i in range(N_t)],
                 axis=1
             )
         else:
             axes = f"t...{'d' * vector}"
             corr = np.stack(
-                [np.einsum(f"{axes},{axes}->...", 
-                           arr1[i:], arr1[:-i if i else None]) 
+                [np.einsum(f"{axes},{axes}->...",
+                           arr1[i:], arr1[:-i if i else None])
                  for i in range(N_t)]
             )
     else:
         start = np.r_[np.zeros(N_t - 1, dtype=int), 0:N_t]
         stop = np.r_[1:N_t + 1, N_t * np.ones(N_t - 1, dtype=int)]
         if ndim == 1:
             corr = np.fromiter(
-                (np.dot(arr1[i:j], arr2[k:l]) 
-                 for i, j, k, l in zip(start[::-1], stop[::-1], start, stop)),
-                count=2 * N_t - 1, dtype=float
+                (np.dot(arr1[i:j], arr2[k:m])
+                 for i, j, k, m in zip(start[::-1], stop[::-1], start, stop)),
+                dtype=float, count=2 * N_t - 1
             )
         elif axis:
             axes = f"bt...{'d' * vector}"
             corr = np.stack(
-                [np.einsum(f"{axes},{axes}->b...", arr1[:, i:j], arr2[:, k:l])
-                 for i, j, k, l in zip(start[::-1], stop[::-1], start, stop)], 
+                [np.einsum(f"{axes},{axes}->b...", arr1[:, i:j], arr2[:, k:m])
+                 for i, j, k, m in zip(start[::-1], stop[::-1], start, stop)],
                 axis=1
             )
         else:
             axes = f"t...{'d' * vector}"
             corr = np.stack(
-                [np.einsum(f"{axes},{axes}->...", arr1[i:j], arr2[k:l]) 
-                 for i, j, k, l in zip(start[::-1], stop[::-1], start, stop)]
+                [np.einsum(f"{axes},{axes}->...", arr1[i:j], arr2[k:m])
+                 for i, j, k, m in zip(start[::-1], stop[::-1], start, stop)]
             )
 
-    # Doubles the ACF or overlaps the CCF for negative and positive 
-    # lags, if desired
+    # Double the ACF or overlap the CCF for negative and positive lags,
+    # if desired
     if double:
         if arr2 is None:
             corr *= 2
         elif axis:
             corr = corr[:, N_t - 1:] + corr[:, N_t - 1::-1]
         else:
             corr = corr[N_t - 1:] + corr[N_t - 1::-1]
@@ -457,26 +451,27 @@
             corr[:N_t - 1] /= np.expand_dims(range(1, N_t), axes)
 
     # Average over all entities, if desired
     if average:
         axis_avg = ndim - 1 - vector
         if axis != axis_avg:
             return corr.mean(axis=axis_avg)
+
     return corr
 
 def msd_fft(
-        pos1: np.ndarray, pos2: np.ndarray = None, axis: int = None, *,
-        average: bool = True) -> np.ndarray:
+        pos1: np.ndarray[float], pos2: np.ndarray[float] = None,
+        axis: int = None, *, average: bool = True) -> np.ndarray[float]:
 
     r"""
-    Calculates the mean squared displacement (MSD) or the analogous 
+    Evaluates the mean squared displacement (MSD) or the analogous
     cross displacement (CD) using fast Fourier transforms (FFT).
-    
+
     The algorithm [1]_ [2]_ is
-    
+
     .. math::
 
         \mathrm{MSD}_m&=\frac{1}{N_t-m}\sum_{k=0}^{N_t-m-1}
         \left[\textbf{r}_{k+m}-\textbf{r}_k\right]^2\\
         &=\frac{1}{N_t-m}\sum_{k=0}^{N_t-m-1}
         \left[\textbf{r}_{k+m}^2+\textbf{r}_k^2\right]
         -\frac{2}{N_t-m}\sum_{k=0}^{N_t-m-1}
@@ -494,91 +489,91 @@
         \begin{gather*}
           D_k=\textbf{r}_k^2\\
           Q_{-1}=2\sum_{k=0}^{N_t-1}D_k\\
           Q_m=Q_{m-1}-D_{m-1}-D_{N_t-m}\\
           S_m=\dfrac{Q_m}{N_t-m}
         \end{gather*}
 
-    Similarly, when two distinct sets of positions are provided, the CD 
+    Similarly, when two distinct sets of positions are provided, the CD
     is computed using
 
     .. math::
 
        \mathrm{CD}_{ij,m}=S_m-2C_{ij,m}
 
-    where :math:`C_{ij,m}` is the cross-correlation of the two sets of 
+    where :math:`C_{ij,m}` is the cross-correlation of the two sets of
     positions and :math:`D_k` in :math:`S_m` is replaced with the
     analogous :math:`D_{ij,k} = \textbf{r}_{i,k}\cdot\textbf{r}_{j,k}`.
 
     .. note::
-    
-       To evaluate the sum in the expression used to calculate the 
+
+       To evaluate the sum in the expression used to calculate the
        Onsager transport coefficients [3]_
 
        .. math::
-            
+
           L_{ij}=\frac{1}{6k_\mathrm{B}T}\lim_{t\rightarrow\infty}
           \frac{d}{dt}\left\langle\sum_{\alpha=1}^{N_i}
-          [\mathrm{r}_\alpha(t)-\mathrm{r}_\alpha(0)]\cdot
-          \sum_{\beta=1}^{N_j}[\mathrm{r}_\beta(t)-\mathrm{r}_\beta(0)]
-          \right\rangle
+          [\mathrm{r}_\alpha(t_0+t)-\mathrm{r}_\alpha(t_0)]\cdot
+          \sum_{\beta=1}^{N_j}[\mathrm{r}_\beta(t_0+t)
+          -\mathrm{r}_\beta(t_0)]\right\rangle
 
        `pos1` and `pos2` should be summed over all atoms before being
        passed to this function.
 
     Parameters
     ----------
     pos1 : `numpy.ndarray`
         Individual or averaged position(s) of the :math:`N` particles
         in the first particle group over :math:`N_\mathrm{b}`
-        blocks of :math:`N_t` frames each. 
-        
+        blocks of :math:`N_t` frames each.
+
         **Shape**: :math:`(N_t,\,3)`, :math:`(N_t,\,N,\,3)`, or
         :math:`(N_\mathrm{b},\,N_t,\,N,\,3)`.
-        
+
         **Reference unit**: :math:`\mathrm{Å}`.
 
     pos2 : `numpy.ndarray`, optional
         Individual or averaged position(s) of the :math:`N` particles
-        in the second particle group over :math:`N_t` frames. 
-        
+        in the second particle group over :math:`N_t` frames.
+
         **Shape**: Same as `pos1`.
 
         **Reference unit**: :math:`\mathrm{Å}`.
 
     axis : `int`, optional
         Axis along which to evaluate the MSD/CD. If `pos1` and/or `pos2`
         contain a full, unsplit trajectory, the MSD/CD should be
         evaluated along the first axis (:code:`axis=0`). If `pos1`
         and/or `pos2` contain a trajectory split into multiple blocks,
-        the MSD should be evaluated along the second axis 
-        (:code:`axis=1`). If not provided, the axis is selected 
+        the MSD should be evaluated along the second axis
+        (:code:`axis=1`). If not provided, the axis is selected
         automatically using the shape of `pos1`.
 
     average : `bool`, keyword-only, default: :code:`True`
         Determines whether the MSD is averaged over all particles if the
         position arrays contain information for multiple particles.
 
     Returns
     -------
     disp : `numpy.ndarray`
         Mean-squared or cross displacement.
-        
-        **Shape**: The shape of `pos`, except with the last dimension 
-        removed. If :code:`average=True`, the axis containing the 
+
+        **Shape**: The shape of `pos`, except with the last dimension
+        removed. If :code:`average=True`, the axis containing the
         :math:`N` entities is also removed.
-        
+
         **Reference unit**: :math:`\text{Å}^2`.
 
     References
     ----------
-    .. [1] Kneller, G. R.; Keiner, V.; Kneller, M.; Schiller, M. 
-       NMOLDYN: A Program Package for a Neutron Scattering Oriented 
+    .. [1] Kneller, G. R.; Keiner, V.; Kneller, M.; Schiller, M.
+       NMOLDYN: A Program Package for a Neutron Scattering Oriented
        Analysis of Molecular Dynamics Simulations. *Computer Physics
-       Communications* **1995**, *91* (1–3), 191–214. 
+       Communications* **1995**, *91* (1–3), 191–214.
        https://doi.org/10.1016/0010-4655(95)00048-K.
 
     .. [2] Calandrini, V.; Pellegrini, E.; Calligari, P.; Hinsen, K.;
        Kneller, G. R. NMoldyn - Interfacing Spectroscopic Experiments,
        Molecular Dynamics Simulations and Models for Time Correlation
        Functions. *JDN* **2011**, *12*, 201–232.
        https://doi.org/10.1051/sfn/201112010.
@@ -587,26 +582,24 @@
        Onsager Transport Coefficients and Transference Numbers in
        Polyelectrolyte Solutions and Polymerized Ionic Liquids.
        *Macromolecules* **2020**, *53* (21), 9503–9512.
        https://doi.org/10.1021/acs.macromol.0c02001.
     """
 
     # Ensure arrays have valid dimensionality
-    if not isinstance(pos1, np.ndarray):
-        pos1 = np.array(pos1)
+    pos1 = np.asarray(pos1)
     if pos1.size == 0:
         raise ValueError("The position arrays must not be empty.")
     ndim = pos1.ndim
     if not 2 <= ndim <= 4:
         emsg = ("The position arrays must be two-, three-, or four-"
                 "dimensional.")
         raise ValueError(emsg)
     if pos2 is not None:
-        if not isinstance(pos2, np.ndarray):
-            pos2 = np.array(pos2)
+        pos2 = np.asarray(pos2)
         if pos1.shape != pos2.shape:
             emsg = "The position arrays must have the same dimensions."
             raise ValueError(emsg)
 
     # Check or set axis along which to compute the MSD/CD
     if axis is None:
         if ndim == 4:
@@ -620,63 +613,70 @@
                         "set to the first axis by default.")
                 warnings.warn(emsg)
     elif axis not in {0, 1}:
         emsg = ("The MSD/CD can only be evaluated along the first or "
                 "second axis.")
         raise ValueError(emsg)
 
-    # Get number of frames
-    N_t = pos1.shape[axis]
-
     # Get intermediate quantities required for the MSD/CD calculation
-    s2 = correlation_fft(pos1, pos2, axis, average=False, double=True, 
+    s2 = correlation_fft(pos1, pos2, axis, average=False, double=True,
                          vector=True)
     r1r2 = (pos1 * (pos1 if pos2 is None else pos2)).sum(axis=-1)
 
+    N_t = pos1.shape[axis]
     if ndim - axis == 3:
 
         # Calculate the MSD/CD for each particle
         if not average:
             stack = np.vstack if ndim == 3 else np.hstack
             shape = np.array(pos1.shape[:-1])
             mask = np.ones(len(shape), dtype=bool)
             mask[axis] = False
             zeros = np.expand_dims(np.zeros(shape[mask]), (axis,))
             D = stack((r1r2, zeros))
             if axis:
-                ssum = 2 * D.sum(axis=axis)[:, None] * np.ones((1, N_t, 1)) \
-                       - np.cumsum(D[:, range(-1, N_t - 1)] + D[:, N_t:0:-1],
-                                   axis=axis)
+                ssum = (
+                    2 * D.sum(axis=axis)[:, None] * np.ones((1, N_t, 1))
+                    - np.cumsum(D[:, range(-1, N_t - 1)] + D[:, N_t:0:-1],
+                                axis=axis)
+                )
             else:
-                ssum = 2 * D.sum(axis=axis) * np.ones((N_t, 1)) \
-                       - np.cumsum(D[range(-1, N_t - 1)] + D[N_t:0:-1],
-                                   axis=axis)
+                ssum = (
+                    2 * D.sum(axis=axis) * np.ones((N_t, 1))
+                    - np.cumsum(D[range(-1, N_t - 1)] + D[N_t:0:-1],
+                                axis=axis)
+                )
             return ssum / np.arange(N_t, 0, -1)[:, None] - s2
 
         # Average the intermediate quantities over all particles
         s2 = s2.mean(axis=ndim - 2)
         r1r2 = r1r2.mean(axis=ndim - 2)
 
     # Calculate the averaged MSD/CD
     if axis:
-        ssum = 2 * r1r2.sum(axis=axis)[:, None] * np.ones((1, N_t)) \
-               - np.insert(np.cumsum(r1r2[:, :N_t - 1] + r1r2[:, N_t - 1:0:-1],
-                                     axis=axis),
-                           0, 0, axis=axis)
+        ssum = (
+            2 * r1r2.sum(axis=axis)[:, None] * np.ones((1, N_t))
+            - np.insert(
+                np.cumsum(r1r2[:, :N_t - 1] + r1r2[:, N_t - 1:0:-1], axis=axis),
+                0, 0, axis=axis
+            )
+        )
     else:
-        ssum = 2 * r1r2.sum() * np.ones(N_t) \
-               - np.insert(np.cumsum(r1r2[:N_t - 1] + r1r2[N_t - 1:0:-1]), 0, 0)
+        ssum = (
+            2 * r1r2.sum() * np.ones(N_t)
+            - np.insert(np.cumsum(r1r2[:N_t - 1] + r1r2[N_t - 1:0:-1]), 0, 0)
+        )
     return ssum / np.arange(N_t, 0, -1) - s2
 
 def msd_shift(
-        pos1: np.ndarray, pos2: np.ndarray = None, axis: int = None, *,
-        average: bool = True) -> np.ndarray:
+        pos1: np.ndarray[float], pos2: np.ndarray[float] = None,
+        axis: int = None, *, average: bool = True) -> np.ndarray[float]:
 
     r"""
-    Calculates the mean squared displacement (MSD) or the analogous 
+    Evaluates the mean squared displacement (MSD) or the analogous
     cross displacement (CD) using the Einstein relation.
 
     The MSD is defined as
 
     .. math::
 
         \mathrm{MSD}(\tau)=\langle\left[
@@ -691,100 +691,98 @@
         \mathrm{CD}_{ij}(\tau)&=\langle
         (\textbf{r}_i(t_0+\tau)-\textbf{r}_i(t_0))\cdot
         (\textbf{r}_j(t_0+\tau)-\textbf{r}_j(t_0))\rangle\\
         &=\dfrac{1}{N}\sum_{\alpha=1}^N
         (\textbf{r}_{i,\alpha}(t_0+\tau)-\textbf{r}_{i,\alpha}(t_0))\cdot
         (\textbf{r}_{j,\alpha}(t_0+\tau)-\textbf{r}_{j,\alpha}(t_0))
 
-    where :math:`\tau` is the time lag, :math:`t_0` is an arbitrary 
+    where :math:`\tau` is the time lag, :math:`t_0` is an arbitrary
     reference time, and :math:`N` is the number of entities. To reduce
     statistical noise, the MSD/CD is calculated for and averaged over
     all possible reference times :math:`t_0`.
 
     .. note::
-    
-       To evaluate the sum in the expression used to calculate the 
+
+       To evaluate the sum in the expression used to calculate the
        Onsager transport coefficients [1]_,
 
        .. math::
-        
+
           L_{ij}=\frac{1}{6k_\mathrm{B}T}\lim_{t\rightarrow\infty}
           \frac{d}{dt}\left\langle\sum_{\alpha=1}^{N_i}
-          [\mathrm{r}_\alpha(t)-\mathrm{r}_\alpha(0)]\cdot
-          \sum_{\beta=1}^{N_j}[\mathrm{r}_\beta(t)-\mathrm{r}_\beta(0)]
-          \right\rangle
+          [\mathrm{r}_\alpha(t_0+t)-\mathrm{r}_\alpha(t_0)]\cdot
+          \sum_{\beta=1}^{N_j}[\mathrm{r}_\beta(t_0+t)
+          -\mathrm{r}_\beta(t_0)]\right\rangle
 
        `pos1` and `pos2` should be summed over all atoms before being
        passed to this function.
 
     Parameters
     ----------
     pos1 : `numpy.ndarray`
         Individual or averaged position(s) of the :math:`N` particles
-        in the first particle group over :math:`N_t` frames. 
-        
+        in the first particle group over :math:`N_t` frames.
+
         **Shape**: :math:`(N_t,\,3)`, :math:`(N_t,\,N,\,3)`, or
         :math:`(N_\mathrm{b},\,N_t,\,N,\,3)`.
-        
+
         **Reference unit**: :math:`\mathrm{Å}`.
 
     pos2 : `numpy.ndarray`, optional
         Individual or averaged position(s) of the :math:`N` particles
-        in the second particle group over :math:`N_t` frames. 
-        
+        in the second particle group over :math:`N_t` frames.
+
         **Shape**: Same as `pos1`.
 
         **Reference unit**: :math:`\mathrm{Å}`.
 
     axis : `int`, optional
         Axis along which to evaluate the MSD/CD. If `pos1` and/or `pos2`
         contain a full, unsplit trajectory, the MSD/CD should be
         evaluated along the first axis (:code:`axis=0`). If `pos1`
         and/or `pos2` contain a trajectory split into multiple blocks,
-        the MSD should be evaluated along the second axis 
-        (:code:`axis=1`). If not provided, the axis is selected 
+        the MSD should be evaluated along the second axis
+        (:code:`axis=1`). If not provided, the axis is selected
         automatically using the shape of `pos1`.
 
     average : `bool`, keyword-only, default: :code:`True`
         Determines whether the MSD is averaged over all particles if the
         position arrays contain information for multiple particles.
 
     Returns
     -------
     disp : `numpy.ndarray`
         Mean-squared or cross displacement.
-        
-        **Shape**: The shape of `pos`, except with the last dimension 
-        removed. If :code:`average=True`, the axis containing the 
+
+        **Shape**: The shape of `pos`, except with the last dimension
+        removed. If :code:`average=True`, the axis containing the
         :math:`N` entities is also removed.
-        
+
         **Reference unit**: :math:`\text{Å}^2`.
 
     References
     ----------
     .. [1] Fong, K. D.; Self, J.; McCloskey, B. D.; Persson, K. A.
        Onsager Transport Coefficients and Transference Numbers in
        Polyelectrolyte Solutions and Polymerized Ionic Liquids.
        *Macromolecules* **2020**, *53* (21), 9503–9512.
        https://doi.org/10.1021/acs.macromol.0c02001.
     """
 
     # Ensure arrays have valid dimensionality
-    if not isinstance(pos1, np.ndarray):
-        pos1 = np.array(pos1)
+    pos1 = np.asarray(pos1)
     if pos1.size == 0:
         raise ValueError("The position arrays must not be empty.")
     ndim = pos1.ndim
     if not 2 <= ndim <= 4:
         emsg = ("The position arrays must be two-, three-, or four-"
                 "dimensional.")
         raise ValueError(emsg)
     if pos2 is not None:
-        if not isinstance(pos2, np.ndarray):
-            pos2 = np.array(pos2)
+        pos2 = np.asarray(pos2)
         if pos1.shape != pos2.shape:
             emsg = "The position arrays must have the same dimensions."
             raise ValueError(emsg)
 
     # Check or set axis along which to compute the MSD/CD
     if axis is None:
         if ndim == 4:
@@ -798,18 +796,16 @@
                         "set to the first axis by default.")
                 warnings.warn(emsg)
     elif axis not in {0, 1}:
         emsg = ("The MSD/CD can only be evaluated along the first or "
                 "second axis.")
         raise ValueError(emsg)
 
-    # Get number of frames
-    N_t = pos1.shape[axis]
-    
     # Calculate the MSD/CD for each atom
+    N_t = pos1.shape[axis]
     if pos2 is None:
         if axis:
             disp = np.stack(
                 [
                     (
                         (pos1[:, :-i if i else None] - pos1[:, i:]) ** 2
                     ).sum(axis=-1).mean(axis=axis) for i in range(N_t)
@@ -825,30 +821,30 @@
                 ]
             )
     else:
         if axis:
             disp = np.stack(
                 [
                     np.einsum(
-                        "bt...d,bt...d->bt...", 
-                        pos1[:, :-i if i else None] - pos1[:, i:], 
+                        "bt...d,bt...d->bt...",
+                        pos1[:, :-i if i else None] - pos1[:, i:],
                         pos2[:, :-i if i else None] - pos2[:, i:]
                     ).mean(axis=axis) for i in range(N_t)
                 ],
                 axis=1
             )
         else:
             disp = np.stack(
                 [
                     np.einsum(
-                        "t...d,t...d->t...", 
-                        pos1[:-i if i else None] - pos1[i:], 
+                        "t...d,t...d->t...",
+                        pos1[:-i if i else None] - pos1[i:],
                         pos2[:-i if i else None] - pos2[i:]
                     ).mean(axis=axis) for i in range(N_t)
                 ]
             )
-    
+
     # Average over all particles, if desired
     if ndim - axis == 3 and average:
         disp = disp.mean(axis=ndim - 2)
 
     return disp
```

### Comparing `mdhelper-0.0.2/src/mdhelper/algorithm/molecule.py` & `mdhelper-1.0.0/src/mdhelper/algorithm/molecule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 """
 Molecular structure
 ===================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 This module contains algorithms for computing structural information
 for a collection of particles.
 """
 
 from typing import Union
 
 import MDAnalysis as mda
 import numpy as np
 
-from .. import ArrayLike
-
 def center_of_mass(
         group: mda.AtomGroup = None, grouping: str = None, *,
-        masses: ArrayLike = None, positions: ArrayLike = None,
-        images: np.ndarray = None, dims: np.ndarray = None,
+        masses: Union[list[float], np.ndarray[float]] = None,
+        positions: Union[list[float], np.ndarray[float]] = None,
+        images: np.ndarray[int] = None, dimensions: np.ndarray[float] = None,
         n_groups: int = None, raw: bool = False
-    ) -> np.ndarray:
-    
+    ) -> Union[np.ndarray[float],
+               tuple[np.ndarray[float], np.ndarray[float], np.ndarray[float]]]:
+
     r"""
     Computes the center(s) of mass for a collection of particles.
 
     For a group with :math:`N` particles with masses :math:`m_i` and
     positions :math:`\mathbf{r}_i`, the center of mass is defined as
 
     .. math::
 
        \mathbf{R}_\mathrm{com}=\dfrac{\sum_{i=1}^N m_i
        \mathbf{r}_i}{\sum_{i=1}^N m_i}
 
     .. note::
 
-       This function supports a wide variety of inputs, depending on 
-       how the particle information is provided and what should be 
+       This function supports a wide variety of inputs, depending on
+       how the particle information is provided and what should be
        calculated.
 
-       When an :class:`MDAnalysis.core.groups.AtomGroup` object is 
-       provided, the particle masses and positions are extracted from 
-       it. If the :code:`AtomGroup` abides by the standard topological 
-       heirarchy, you can specify the desired grouping and the 
+       When an :class:`MDAnalysis.core.groups.AtomGroup` object is
+       provided, the particle masses and positions are extracted from
+       it. If the :code:`AtomGroup` abides by the standard topological
+       heirarchy, you can specify the desired grouping and the
        appropriate center(s) of mass will be calculated. Otherwise, if
        and only if the :code:`AtomGroup` contains equisized or identical
-       groups corresponding to the desired grouping, you can provide the 
+       groups corresponding to the desired grouping (i.e., the
+       :code:`AtomGroup` has particles that are or can be treated as
+       nonbonded entities or topological groups with the same number of
+       but not necessarily identical constituents), you can provide the
        total number of groups and the particle masses and positions will
-       be distributed accordingly. If the :code:`AtomGroup` does not 
-       have the correct structural information and the residues or 
-       segments do not contain the same number of atoms, see the final
-       paragraph.
+       be distributed accordingly. If the :code:`AtomGroup` does not
+       have the correct structural information and the residues or
+       segments do not contain the same number of atoms, see the
+       second-to-last paragraph.
 
-       If the trajectory is not unwrapped, the number of periodic 
+       If the trajectory is not unwrapped, the number of periodic
        boundary crossings (and optionally, the system dimensions if they
        are not embedded in the :code:`AtomGroup`) can be provided.
 
-       Alternatively, the *unwrapped* particle masses and positions can 
+       Alternatively, the *unwrapped* particle masses and positions can
        be provided directly as a :class:`numpy.ndarray`, list, or tuple.
        To calculate the overall center of mass, the array-like object
-       holding the masses should be one-dimensional, while that 
+       holding the masses should be one-dimensional, while that
        containing the positions should be two-dimensional. To calculate
        center(s) of mass for group(s), the array-like object holding the
-       masses should be two-dimensional (indexing: group, particle 
-       mass), while that containing the positions should be 
-       three-dimensional (indexing: group, particle position, 
-       dimension). When a list or tuple is used, the inner arrays do not
-       have to be homogeneously shaped, thus allowing you to calculate 
-       the centers of mass for different residues or segments.
+       masses should be two-dimensional (order: group, particle mass),
+       while that containing the positions should be three-dimensional
+       (order: group, particle position, axis). When a list or tuple is
+       used, the inner arrays do not have to be homogeneously shaped,
+       thus allowing you to calculate the centers of mass for residues
+       or segments with different numbers of atoms.
 
-       You may also provide only one of the particle masses or 
+       You may also provide only one of the particle masses or
        positions, in which case the missing information will be
        retrieved from the :code:`AtomGroup`. This is generally not
        recommended since the shapes of the provided and retrieved
        arrays may be incompatible.
 
     Parameters
     ----------
     group : `MDAnalysis.AtomGroup`, optional
         Collection of atoms to compute the center(s) of mass for. If not
         provided, the particle masses and posititions must be provided
         directly in `masses` and `positions`.
 
     grouping : `str`, optional
-        Determines which center of mass is calculated if particle 
+        Determines which center of mass is calculated if particle
         massses and positions are retrieved from `group`.
 
         .. container::
 
            **Valid values**:
 
            * :code:`None`: Center of mass of all particles in `group`.
            * :code:`"residues"`: Centers of mass for each residue in
              `group`.
-           * :code:`"segments"`: Centers of mass for each chain in 
+           * :code:`"segments"`: Centers of mass for each chain in
              `group`.
 
     masses : array-like, keyword-only, optional
         Particle masses.
 
         .. container::
 
@@ -112,15 +115,15 @@
              the number of residues, or
            * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg}` for the segment
              center(s) of mass, where :math:`N_\mathrm{seg}` is
              the number of segments.
 
            For groups with different numbers of atoms, the array-like
            object should contain inner lists or tuples holding the
-           masses of the particles in each group. 
+           masses of the particles in each group.
 
         **Reference unit**: :math:`\mathrm{g/mol}`.
 
     positions : array-like, keyword-only, optional
         Unwrapped particle positions.
 
         .. container::
@@ -128,303 +131,288 @@
            **Shape**:
 
            The general shape is :math:`(N,\,3)`.
 
            For equisized or identical groups,
 
            * :math:`(N,\,3)` for the overall center of mass,
-           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res},\,3)` for the 
+           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res},\,3)` for the
              residue center(s) of mass, or
-           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg},\,3)` for the 
+           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg},\,3)` for the
              segment center(s) of mass.
 
            For groups with different numbers of atoms, the array-like
            object should contain inner lists or tuples holding the
-           coordinates of the particles in each group. 
+           coordinates of the particles in each group.
 
         **Reference unit**: :math:`\mathrm{Å}`.
 
     images : `numpy.ndarray`, keyword-only, optional
-        Image flags for the particles in `group`. Must be provided for 
+        Image flags for the particles in `group`. Must be provided for
         correct results if particle positions are wrapped.
 
         **Shape**: :math:`(N,\,3)`.
 
-    dims : `numpy.ndarray`, keyword-only, optional
+    dimensions : `numpy.ndarray`, keyword-only, optional
         System dimensions. Must be provided if `images` is provided and
         `group` does not contain the system dimensions.
 
         **Shape**: :math:`(3,)`.
-        
+
         **Reference unit**: :math:`\mathrm{Å}`.
 
     n_groups : `int`, keyword-only, optional
         Number of residues or segments. Must be provided if `group` has
-        an irregular topological heirarchy or the `masses` and 
+        an irregular topological heirarchy or the `masses` and
         `positions` arrays have the generic shapes.
-    
+
     raw : `bool`, keyword-only, default: :code:`False`
         Determines whether particle masses and positions are returned if
         they were retrieved from `group`.
 
     Returns
     -------
     com : `numpy.ndarray`
         Center(s) of mass.
 
         .. container::
 
            **Shape**:
 
            * :math:`(3,)` for :code:`grouping=None`.
-           * :math:`(N_\mathrm{res},\,3)` for 
+           * :math:`(N_\mathrm{res},\,3)` for
              :code:`grouping="residues"`.
-           * :math:`(N_\mathrm{seg},\,3)` for 
+           * :math:`(N_\mathrm{seg},\,3)` for
              :code:`grouping="segments"`.
 
     masses : `numpy.ndarray`
         Particle masses. Only returned if `group` was provided
-        and contains equisized or identical groups, and 
+        and contains equisized or identical groups, and
         :code:`raw=True`.
 
         .. container::
 
            **Shape**:
 
            * :math:`(N,)` for :code:`grouping=None`.
-           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res})` for 
+           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res})` for
              :code:`grouping="residues"`.
-           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg})` for 
+           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg})` for
              :code:`grouping="segments"`.
 
         **Reference unit**: :math:`\mathrm{g/mol}`.
 
     positions : `numpy.ndarray`
-        Unwrapped particle positions. Only returned if `group` was 
-        provided and contains equisized or identical groups, and 
+        Unwrapped particle positions. Only returned if `group` was
+        provided and contains equisized or identical groups, and
         :code:`raw=True`.
 
         .. container::
 
            **Shape**:
 
            * :math:`(N,\,3)` for :code:`grouping=None`.
-           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res},\,3)` for 
+           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res},\,3)` for
              :code:`grouping="residues"`.
-           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg},\,3)` for 
+           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg},\,3)` for
              :code:`grouping="segments"`.
 
         **Reference unit**: :math:`\mathrm{Å}`.
     """
-    
+
     # Check whether grouping is valid
     if grouping not in {None, "residues", "segments"}:
         emsg = (f"Invalid grouping: '{grouping}'. Valid options are "
                 "None, 'residues', and 'segments'.")
         raise ValueError(emsg)
-    
+
     # Get particle masses and positions from the trajectory, if necessary
     missing = (masses is None, positions is None)
     if any(missing):
-
-        # Ensure a trajectory is available
         if group is None:
             emsg = ("Either a group of atoms or atom positions and "
                     "masses must be provided.")
             raise ValueError(emsg)
 
         # Check whether the groups are identical
         if grouping:
             groups = getattr(group, grouping)
-            same = all(r.atoms.n_atoms == groups[0].atoms.n_atoms 
-                        for r in groups)
+            same = all(g.atoms.n_atoms == groups[0].atoms.n_atoms
+                       for g in groups)
         else:
             same = True
 
         # Calculate and return the centers of mass for different groups
-        # here if unwrapping and the mass and position arrays are not 
+        # here if unwrapping and the mass and position arrays are not
         # needed
         if not same and images is None and not raw:
             return np.array([g.atoms.center_of_mass() for g in groups])
 
-        # Get particle positions, if necessary
+        # Get and unwrap particle positions, if necessary
         if missing[1]:
             positions = group.positions
-
-            # Unwrap particle positions, if necessary
             if images is not None:
-                if dims is None:
+                if dimensions is None:
                     try:
-                        dims = group.dimensions[:3]
-                    except:
+                        dimensions = group.dimensions[:3]
+                    except TypeError:
                         emsg = ("The number of periodic boundary "
                                 "crossings was provided, but no "
                                 "system dimensions were provided or "
                                 "found in the trajectory.")
                         raise ValueError(emsg)
-                positions += images * dims[:3]
+                positions += images * dimensions[:3]
 
+        # Get particle masses and ensure correct dimensionality, if
+        # necessary
         if same:
-
-            # Get particle masses, if necessary
             if missing[0]:
                 masses = group.masses
-
-            # Reshape the mass and position arrays, if necessary
             if grouping or n_groups:
-                shape = (n_groups, -1, 3) if n_groups \
-                        else (getattr(group, f"n_{grouping}"), -1, 3)
+                shape = ((n_groups, -1, 3) if n_groups
+                         else (getattr(group, f"n_{grouping}"), -1, 3))
                 masses = masses.reshape(shape[:-1])
                 positions = positions.reshape(shape)
         else:
-
-            # Get particle masses, if necessary
             if missing[0]:
                 masses = [g.atoms.masses for g in groups]
-
-            # Reshape the position array, if necessary
             if missing[1]:
                 positions = [positions[g.atoms.ix] for g in groups]
-
     else:
 
         # Try to convert arrays to NumPy arrays if they are not already
         # to take advantage of vectorized operations later
-        if not isinstance(positions, np.ndarray):
-            try:
-                positions = np.array(positions)
-            except:
-                pass
-        if not isinstance(masses, np.ndarray):
-            try:
-                masses = np.array(masses)
-            except:
-                pass
+        try:
+            positions = np.asarray(positions)
+            masses = np.asarray(masses)
+        except ValueError:
+            pass
         if type(masses) != type(positions):
             emsg = ("The shapes of the arrays containing the particle "
                     "masses and positions are incompatible.")
             raise ValueError(emsg)
 
         # Reshape the mass and position arrays based on the specified
         # number of groups
         if n_groups and isinstance(positions, np.ndarray):
             masses = masses.reshape((n_groups, -1))
             positions = positions.reshape((n_groups, -1, 3))
 
     # Calculate the center(s) of mass for the specified grouping
     if isinstance(positions, np.ndarray):
-        com = np.einsum("...a,...ad->...d", masses, positions) \
-                  / masses.sum(axis=-1, keepdims=True)
+        com = (np.einsum("...a,...ad->...d", masses, positions)
+               / masses.sum(axis=-1, keepdims=True))
     else:
-        com = np.array([np.dot(m, p) / m.sum() 
-                       for m, p in zip(masses, positions)], dtype=float)
-    
-    # Return the center(s) of mass
-    if raw and any(missing):
+        com = np.array([np.dot(m, p) / m.sum()
+                        for m, p in zip(masses, positions)])
 
-        # Also return the particle masses and positions, if desired
+    if raw and any(missing):
         return com, masses, positions
     return com
 
 def radius_of_gyration(
         group: mda.AtomGroup = None, grouping: str = None, *,
-        positions: ArrayLike = None, masses: ArrayLike = None,
-        com: ArrayLike = None, images: np.ndarray = None, 
-        dims: np.ndarray = None, n_groups: int = None, components: bool = False
-    ) -> Union[float, np.ndarray]:
-    
+        positions: Union[list[tuple[tuple[float]]], np.ndarray[float]] = None,
+        masses: Union[list[tuple[float]], np.ndarray[float]] = None,
+        com: np.ndarray[float] = None, images: np.ndarray[int] = None,
+        dimensions: np.ndarray[float] = None, n_groups: int = None,
+        components: bool = False) -> Union[float, np.ndarray[float]]:
+
     r"""
     Computes the radii of gyration for a collection of particles.
 
     For a group with :math:`N` particles with masses :math:`m_i` and
     positions :math:`\mathbf{r}_i`, the radius of gyration is defined as
 
     .. math::
 
         R_\mathrm{g}=\sqrt{
         \frac{\sum_i^N m_i\|\mathbf{r}_i-\mathbf{R}_\mathrm{com}\|^2}
         {\sum_i^N m_i}}
 
     where :math:`\mathbf{R}_\mathrm{com}` is the center of mass.
 
-    Alternatively, the radii of gyration around the coordinate axes can 
+    Alternatively, the radii of gyration around the coordinate axes can
     be calculated by only summing the radii components orthogonal to
-    each axis. For example, the radius of gyration around the 
+    each axis. For example, the radius of gyration around the
     :math:`x`-axis is
 
     .. math::
-     
+
        R_{\mathrm{g},x}=\sqrt{
        \frac{\sum_i^N m_i[(\mathbf{r}_{i,y}-\mathbf{R}_{\mathrm{com},y})^2
        +(\mathbf{r}_{i,z}-\mathbf{R}_{\mathrm{com},z})^2]}{\sum_i^N m_i}}
 
     .. note::
 
-       This function supports a wide variety of inputs, depending on 
-       how the particle information is provided and what should be 
+       This function supports a wide variety of inputs, depending on
+       how the particle information is provided and what should be
        calculated.
 
-       When an :class:`MDAnalysis.core.groups.AtomGroup` object is 
-       provided, the particle masses and positions are extracted from 
-       it. If the :code:`AtomGroup` abides by the standard topological 
-       heirarchy, you can specify the desired grouping and the 
+       When an :class:`MDAnalysis.core.groups.AtomGroup` object is
+       provided, the particle masses and positions are extracted from
+       it. If the :code:`AtomGroup` abides by the standard topological
+       heirarchy, you can specify the desired grouping and the
        appropriate radii of gyration will be calculated. Otherwise, if
        and only if the :code:`AtomGroup` contains equisized or identical
-       groups corresponding to the desired grouping, you can provide the 
+       groups corresponding to the desired grouping (i.e., the
+       :code:`AtomGroup` has particles that are or can be treated as
+       nonbonded entities or topological groups with the same number of
+       but not necessarily identical constituents), you can provide the
        total number of groups and the particle masses and positions will
-       be distributed accordingly. If the :code:`AtomGroup` does not 
-       have the correct structural information and the residues or 
-       segments do not contain the same number of atoms, see the final
-       paragraph.
+       be distributed accordingly. If the :code:`AtomGroup` does not
+       have the correct structural information and the residues or
+       segments do not contain the same number of atoms, see the
+       second-to-last paragraph.
 
-       If the trajectory is not unwrapped, the number of periodic 
+       If the trajectory is not unwrapped, the number of periodic
        boundary crossings (and optionally, the system dimensions if they
        are not embedded in the :code:`AtomGroup`) can be provided.
 
-       Alternatively, the *unwrapped* particle masses and positions can 
+       Alternatively, the *unwrapped* particle masses and positions can
        be provided directly as a :class:`numpy.ndarray`, list, or tuple.
-       To calculate the overall radius of gyration, the array-like object
-       holding the masses should be one-dimensional, while that 
+       To calculate the overall radius of gyration, the array-like
+       object holding the masses should be one-dimensional, while that
        containing the positions should be two-dimensional. To calculate
        radii of gyration for group(s), the array-like object holding the
-       masses should be two-dimensional (indexing: group, particle 
-       mass), while that containing the positions should be 
-       three-dimensional (indexing: group, particle position, 
-       dimension). When a list or tuple is used, the inner arrays do not
-       have to be homogeneously shaped, thus allowing you to calculate 
-       the radii of gyration for different residues or segments.
+       masses should be two-dimensional (order: group, particle mass),
+       while that containing the positions should be three-dimensional
+       (order: group, particle position, axis). When a list or tuple is
+       used, the inner arrays do not have to be homogeneously shaped,
+       thus allowing you to calculate the radii of gyration for residues
+       or segments with different numbers of atoms.
 
-       You may also provide only one of the particle masses or 
+       You may also provide only one of the particle masses or
        positions, in which case the missing information will be
        retrieved from the :code:`AtomGroup`. This is generally not
        recommended since the shapes of the provided and retrieved
        arrays may be incompatible.
 
     Parameters
     ----------
     group : `MDAnalysis.AtomGroup`, optional
         Collection of atoms to compute the radii of gyration for. If not
         provided, the particle masses and posititions must be provided
         directly in `masses` and `positions`.
 
     grouping : `str`, optional
-        Determines which radius of gyration is calculated if particle 
+        Determines which radius of gyration is calculated if particle
         massses and positions are retrieved from `group`.
 
         .. container::
 
            **Valid values**:
 
-           * :code:`None`: Radius of gyration of all particles in 
+           * :code:`None`: Radius of gyration of all particles in
              `group`.
            * :code:`"residues"`: Radius of gyration for each residue in
              `group`.
-           * :code:`"segments"`: Radius of gyration for each chain in 
+           * :code:`"segments"`: Radius of gyration for each chain in
              `group`.
-    
+
     masses : array-like, keyword-only, optional
         Particle masses.
 
         .. container::
 
            **Shape**:
 
@@ -438,15 +426,15 @@
              the number of residues, or
            * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg}` for the segment
              radii of gyration, where :math:`N_\mathrm{seg}` is
              the number of segments.
 
            For groups with different numbers of atoms, the array-like
            object should contain inner lists or tuples holding the
-           masses of the particles in each group. 
+           masses of the particles in each group.
 
         **Reference unit**: :math:`\mathrm{g/mol}`.
 
     positions : array-like, keyword-only, optional
         Unwrapped particle positions.
 
         .. container::
@@ -454,55 +442,55 @@
            **Shape**:
 
            The general shape is :math:`(N,\,3)`.
 
            For equisized or identical groups,
 
            * :math:`(N,\,3)` for the overall radius of gyration,
-           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res},\,3)` for the 
+           * :math:`(N_\mathrm{res},\,N/N_\mathrm{res},\,3)` for the
              residue radii of gyration, or
-           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg},\,3)` for the 
+           * :math:`(N_\mathrm{seg},\,N/N_\mathrm{seg},\,3)` for the
              segment radii of gyration.
 
            For groups with different numbers of atoms, the array-like
            object should contain inner lists or tuples holding the
-           coordinates of the particles in each group. 
+           coordinates of the particles in each group.
 
         **Reference unit**: :math:`\mathrm{Å}`.
 
     com : `numpy.ndarray`, keyword-only, optional
         Center(s) of mass.
 
         .. container::
 
            **Shape**:
 
            * :math:`(3,)` for the overall radius of gyration.
-           * :math:`(N_\mathrm{res},\,3)` for the residue radii of 
+           * :math:`(N_\mathrm{res},\,3)` for the residue radii of
              gyration.
            * :math:`(N_\mathrm{seg},\,3)` for the segment radii of
              gyration.
 
     images : `numpy.ndarray`, keyword-only, optional
-        Image flags for the particles in `group`. Must be provided for 
+        Image flags for the particles in `group`. Must be provided for
         correct results if particle positions are wrapped.
 
         **Shape**: :math:`(N,\,3)`.
 
-    dims : `numpy.ndarray`, keyword-only, optional
+    dimensions : `numpy.ndarray`, keyword-only, optional
         System dimensions. Must be provided if `images` is provided and
         `group` does not contain the system dimensions.
 
         **Shape**: :math:`(3,)`.
-        
+
         **Reference unit**: :math:`\mathrm{Å}`.
 
     n_groups : `int`, keyword-only, optional
         Number of residues or segments. Must be provided if `group` has
-        an irregular topological heirarchy or the `masses` and 
+        an irregular topological heirarchy or the `masses` and
         `positions` arrays have the generic shapes.
 
     components : `bool`, keyword-only, default: :code:`False`
         Specifies whether the components of the radii of gyration are
         calculated and returned instead.
 
     Returns
@@ -527,68 +515,73 @@
                 "None, 'residues', and 'segments'.")
         raise ValueError(emsg)
 
     # Get particle masses and positions from the trajectory and the
     # center(s) of mass, if necessary
     missing = (masses is None, positions is None, com is None)
     if any(missing[:2]):
-        com, masses, positions = center_of_mass(group, grouping, masses=masses, 
+        com, masses, positions = center_of_mass(group, grouping, masses=masses,
                                                 positions=positions, raw=True,
-                                                images=images, dims=dims)
+                                                images=images, dimensions=dimensions)
     elif missing[2]:
-        com = center_of_mass(masses=masses, positions=positions, n_groups=n_groups)
+        com = center_of_mass(masses=masses, positions=positions,
+                             n_groups=n_groups)
 
     if isinstance(positions, np.ndarray):
         if components:
-            cpos = (positions - np.expand_dims(com, axis=positions.ndim - 2)) ** 2
-            if grouping or n_groups:
+            cpos = (positions
+                    - np.expand_dims(com, axis=positions.ndim - 2)) ** 2
 
-                # Compute the radii of gyration in each direction for 
-                # equisized or identical group(s)
+            # Compute the radii of gyration in each direction for
+            # equisized or identical group(s)
+            if grouping or n_groups:
                 return np.sqrt(
-                    np.einsum("ga,gad->gd", masses, 
-                              np.stack((cpos[:, :, (1, 2)].sum(axis=2), 
-                                        cpos[:, :, (0, 2)].sum(axis=2), 
-                                        cpos[:, :, (0, 1)].sum(axis=2)), axis=2))
+                    np.einsum("ga,gad->gd", masses,
+                              np.stack((cpos[:, :, (1, 2)].sum(axis=2),
+                                        cpos[:, :, (0, 2)].sum(axis=2),
+                                        cpos[:, :, (0, 1)].sum(axis=2)),
+                                       axis=2))
                     / masses.sum(axis=1, keepdims=True)
                 )
-            
+
             # Compute the radius of gyration in each direction for all
             # atoms
             return np.sqrt(
-                np.dot(masses, np.hstack(
-                    (cpos[:, (1, 2)].sum(axis=1, keepdims=True), 
-                     cpos[:, (0, 2)].sum(axis=1, keepdims=True), 
-                     cpos[:, (0, 1)].sum(axis=1, keepdims=True))
-                )) / masses.sum()
+                np.dot(
+                    masses,
+                    np.hstack((cpos[:, (1, 2)].sum(axis=1, keepdims=True),
+                               cpos[:, (0, 2)].sum(axis=1, keepdims=True),
+                               cpos[:, (0, 1)].sum(axis=1, keepdims=True)))
+                ) / masses.sum()
             )
+
+        # Compute the overall radii of gyration for equisized or
+        # identical group(s)
         elif grouping or n_groups:
+            return np.sqrt(
+                np.einsum("ga,gad->gd", masses,
+                          (positions - com[:, None]) ** 2).sum(axis=1)
+                / masses.sum(axis=1)
+            )
 
-            # Compute the overall radii of gyration for equisized or 
-            # identical group(s)
-            return np.sqrt(np.einsum("ga,gad->gd", masses,
-                                     (positions - com[:, None]) ** 2).sum(axis=1) \
-                   / masses.sum(axis=1))
-        
         # Compute the overall radius of gyration for all atoms
-        return np.sqrt(np.dot(masses, (positions - com) ** 2).sum() \
-               / masses.sum())
-    if components:
+        return np.sqrt(np.dot(masses, (positions - com) ** 2).sum()
+                       / masses.sum())
 
-        # Compute the radii of gyration in each direction for asymmetric
-        # groups
-        gyradii = np.empty(com.shape, dtype=float)
+    # Compute the radii of gyration in each direction for asymmetric
+    # groups
+    if components:
+        gyradii = np.empty(com.shape)
         for i, (m, p, c) in enumerate(zip(masses, positions, com)):
             cpos = (p - c) ** 2
             gyradii[i] = np.array(
                 (np.dot(m, cpos[:, (1, 2)].sum(axis=1)),
                  np.dot(m, cpos[:, (0, 2)].sum(axis=1)),
                  np.dot(m, cpos[:, (0, 1)].sum(axis=1)))
             ) / m.sum()
         return np.sqrt(gyradii)
-    
+
     # Compute the overall radii of gyration for asymmetric groups
     return np.sqrt(
-        [np.einsum("a,ad->d", m, (p - c) ** 2).sum() / m.sum() 
-            for m, p, c in zip(masses, positions, com)]
-    )
-                
+        [np.einsum("a,ad->d", m, (p - c) ** 2).sum() / m.sum()
+         for m, p, c in zip(masses, positions, com)]
+    )
```

### Comparing `mdhelper-0.0.2/src/mdhelper/analysis/polymer.py` & `mdhelper-1.0.0/src/mdhelper/analysis/polymer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 """
 Polymeric analysis
 ==================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 This module contains classes to determine the structural
 and dynamical properties of polymeric systems.
 """
 
 from typing import Union
 import warnings
 
 import MDAnalysis as mda
 from MDAnalysis.lib.log import ProgressBar
+from MDAnalysis.lib.mdamath import make_whole
 import numpy as np
-from openmm import unit
-from scipy import optimize
+from scipy import optimize, special
 
-from .base import SerialAnalysisBase, ParallelAnalysisBase
-from .. import ArrayLike
-from ..algorithm import correlation, molecule
+from .base import DynamicAnalysisBase
+from .. import FOUND_OPENMM, Q_, ureg
+from ..algorithm import correlation
+from ..algorithm.molecule import center_of_mass, radius_of_gyration
+from ..algorithm.topology import unwrap, unwrap_edge
+from ..algorithm.unit import strip_unit
 from ..fit.exponential import stretched_exp
 
+if FOUND_OPENMM:
+    from openmm import unit
+
 def correlation_fft(*args, **kwargs):
 
     """
     Evaluates the autocorrelation function (ACF) or cross-correlation
-    function (CCF) of a time series using fast Fourier transforms (FFT). 
+    function (CCF) of a time series using fast Fourier transforms (FFT).
 
     .. note::
 
        This is an alias function. For more information, see
        :func:`mdhelper.algorithm.correlation.correlation_fft`.
     """
 
@@ -43,65 +49,69 @@
     along the time axis.
 
     .. note::
 
        This is an alias function. For more information, see
        :func:`mdhelper.algorithm.correlation.correlation_shift`.
     """
-    
+
     return correlation.correlation_shift(*args, **kwargs)
 
-def relaxation_time(time: np.ndarray, acf: np.ndarray) -> float:
+def calculate_relaxation_time(
+        time: np.ndarray[float], acf: np.ndarray[float]) -> float:
 
     r"""
-    Estimates the orientational relaxation time using an ACF.
-    
-    A stretched exponential function
+    Calculates the orientational relaxation time :math:`\tau_\mathrm{r}`
+    of a polymer using the end-to-end vector autocorrelation function
+    (ACF) time series :math:`C_\mathrm{ee}`.
+
+    A stretched exponential function with :math:`\tau` and :math:`\beta`
+    as coefficients,
 
     .. math::
 
-       C_\mathrm{ee}=\exp{\left[-(t/\tau_\mathrm{r})^\beta\right]}
-    
-    is fitted to the end-to-end vector autocorrelation function (ACF) vs.
-    time relationship and evaluating
+       C_\mathrm{ee}=\exp{\left[-(t/\tau)^\beta\right]}
+
+    is fitted to the ACF time series, and the relaxation time is estimated
+    using
 
     .. math::
 
-       \tau=\int_0^\infty C_\mathrm{ee}\,dt=\tau_\mathrm{r}
+       \tau_\mathrm{r}=\int_0^\infty C_\mathrm{ee}\,dt=\tau\Gamma(1/\beta)
 
     Parameters
     ----------
     time : `numpy.ndarray`
         Changes in time :math:`t-t_0`.
 
         **Shape**: :math:`(N_t,)`.
 
         **Reference unit**: :math:`\textrm{ps}`.
 
     acf : `numpy.ndarray`
         End-to-end vector ACFs for the :math:`N_\textrm{g}` groups over
-        :math:`N_\textrm{b}` blocks of :math:`N_t` trajectory frames 
+        :math:`N_\textrm{b}` blocks of :math:`N_t` trajectory frames
         each.
 
-        **Shape**: 
+        **Shape**:
         :math:`(N_\textrm{g},\,N_\textrm{b},\,N_t)`.
 
     Returns
     -------
     relaxation_time : `float`
         Average orientational relaxation time.
 
         **Reference unit**: :math:`\textrm{ps}`.
     """
 
     tau_r, beta = optimize.curve_fit(stretched_exp, time / time[1], acf,
                                      bounds=(0, np.inf))[0]
-    return tau_r * time[1] * np.math.gamma(1 + beta ** -1)
+    return tau_r * time[1] * special.gamma(1 + beta ** -1)
 
-class _PolymerAnalysisBase(SerialAnalysisBase):
+class _PolymerAnalysisBase(DynamicAnalysisBase):
 
     r"""
     An analysis base object for polymer systems.
 
     Parameters
     ----------
     groups : `MDAnalysis.AtomGroup` or array-like
@@ -109,21 +119,31 @@
         must have the same chain length.
 
     groupings : `str` or array-like, default: :code:`"atoms"`
         Determines whether the centers of mass are used in lieu of
         individual atom positions. If `groupings` is a `str`, the same
         value is used for all `groups`.
 
+        .. note::
+
+           In a standard trajectory file, segments (or chains) contain
+           residues (or molecules), and residues contain atoms. This
+           heirarchy must be adhered to for this analysis module to
+           function correctly. If your trajectory file does not contain
+           the correct segment or residue information, provide the
+           number of chains and chain lengths in `n_chains` and
+           `n_monomers`, respectively.
+
         .. container::
 
            **Valid values**:
 
            * :code:`"atoms"`: Atom positions (for coarse-grained polymer
              simulations).
-           * :code:`"residues"`: Residues' centers of mass (for 
+           * :code:`"residues"`: Residues' centers of mass (for
              atomistic polymer simulations).
 
     n_chains : `int` or array-like, optional
         Number of chains in each polymer group. Must be provided if the
         trajectory does not adhere to the standard container heirarchy
         (see Notes).
 
@@ -131,143 +151,142 @@
         Number of monomers in each chain in each polymer group. Must be
         provided if the trajectory does not adhere to the standard
         container heirarchy (see Notes).
 
     unwrap : `bool`, keyword-only, default: :code:`False`
         Determines whether atom positions are unwrapped.
 
+    parallel : `bool`, keyword-only, default: :code:`False`
+        Determines whether the analysis is performed in parallel.
+
     verbose : `bool`, keyword-only, default: :code:`True`
         Determines whether detailed progress is shown.
 
     **kwargs
         Additional keyword arguments to pass to
         :class:`MDAnalysis.analysis.base.AnalysisBase`.
-    
+
     Attributes
     ----------
     universe : `MDAnalysis.Universe`
         :class:`MDAnalysis.core.universe.Universe` object containing all
         information describing the system.
-
-    results.units : `dict`
-        Reference units for the results. For example, to get the 
-        reference units for :code:`results.time`, call 
-        :code:`results.units["results.time"]`. Only available if OpenMM
-        is installed.
-
-    Notes
-    -----
-    In a standard trajectory file, segments (or chains) contain
-    residues, and residues contain atoms. This heirarchy must be adhered
-    to for this analysis module to function correctly. If your
-    trajectory file does not contain the correct segment or residue
-    information, provide the number of chains and chain lengths in
-    `n_chains` and `n_monomers`, respectively.
     """
 
     def __init__(
-            self, groups: Union[mda.AtomGroup, ArrayLike],
-            groupings: Union[str, ArrayLike] = "atoms", 
-            n_chains: Union[int, ArrayLike] = None, 
-            n_monomers: Union[int, ArrayLike] = None, *, unwrap: bool = False,
-            verbose: bool = True, **kwargs):
-        
+            self, groups: Union[mda.AtomGroup, tuple[mda.AtomGroup]],
+            groupings: Union[str, tuple[str]] = "atoms",
+            n_chains: Union[int, tuple[int]] = None,
+            n_monomers: Union[int, tuple[int]] = None, *, unwrap: bool = False,
+            parallel: bool = False, verbose: bool = True, **kwargs) -> None:
+
         self._groups = [groups] if isinstance(groups, mda.AtomGroup) else groups
         self.universe = self._groups[0].universe
-        super().__init__(self.universe.trajectory, verbose=verbose, **kwargs)
-        if self.universe.dimensions is None:
-            self._dims = None
-        else:
-            self._dims = self.universe.dimensions[:3].copy()
+
+        super().__init__(self.universe.trajectory, parallel, verbose, **kwargs)
+
+        self._dimensions = self.universe.dimensions
+        if self._dimensions is not None:
+            self._dimensions = self._dimensions[:3].copy()
 
         self._n_groups = len(self._groups)
         if isinstance(groupings, str):
-            if groupings not in {"atoms", "residues"}:
-                emsg = (f"Invalid grouping '{groupings}'. The options are "
-                        "'atoms' and 'residues'.")
+            if groupings not in (GROUPINGS := {"atoms", "residues"}):
+                emsg = (f"Invalid grouping '{groupings}'. Valid values: "
+                        f"{', '.join(GROUPINGS)}.")
                 raise ValueError(emsg)
             self._groupings = self._n_groups * [groupings]
         else:
             if self._n_groups != len(groupings):
-                emsg = ("The number of grouping values is not equal to the "
-                        "number of groups.")
+                emsg = ("The number of grouping values is not equal to "
+                        "the number of groups.")
                 raise ValueError(emsg)
             for g in groupings:
-                if g not in {"atoms", "residues"}:
-                    emsg = (f"Invalid grouping '{g}'. The options are "
-                            "'atoms' and 'residues'.")
+                if g not in (GROUPINGS := {"atoms", "residues"}):
+                    emsg = (f"Invalid grouping '{g}'. Valid values: "
+                            f"{', '.join(GROUPINGS)}.")
                     raise ValueError(emsg)
             self._groupings = groupings
-        
-        if hasattr(self.universe, "segments"):
-            self._n_chains = np.zeros(self._n_groups, dtype=int)
-            self._n_monomers = np.zeros(self._n_groups, dtype=int)
+
+        if n_chains is None or n_monomers is None:
+            self._internal = True
+            self._n_chains = np.empty(self._n_groups, dtype=int)
+            self._n_monomers = np.empty_like(self._n_chains)
             for i, g in enumerate(self._groups):
                 self._n_chains[i] = g.segments.n_segments
                 self._n_monomers[i] = g.n_atoms // self._n_chains[i]
         else:
-            if isinstance(n_chains, int):
+            self._internal = False
+            if isinstance(n_chains, (int, np.integer)):
                 self._n_chains = n_chains * np.ones(self._n_groups, dtype=int)
             elif self._n_groups == len(n_chains):
                 self._n_chains = n_chains
             else:
                 emsg = ("The number of polymer counts is not equal to the "
                         "number of groups.")
                 raise ValueError(emsg)
-            if isinstance(n_monomers, int):
+            if isinstance(n_monomers, (int, np.integer)):
                 self._n_monomers = n_monomers * np.ones(n_monomers, dtype=int)
             elif self._n_groups == len(n_monomers):
                 self._n_monomers = n_monomers
             else:
                 emsg = ("The number of chain lengths is not equal to the "
                         "number of groups.")
                 raise ValueError(emsg)
 
         self._unwrap = unwrap
         self._verbose = verbose
 
-        self.results.units = {"_dims": unit.angstrom}
-
 class Gyradius(_PolymerAnalysisBase):
 
     r"""
-    A serial implementation to calculate the radius of gyration 
-    :math:`R_\mathrm{g}` of a polymer.
+    Serial and parallel implementations to calculate the radius of
+    gyration :math:`R_\mathrm{g}` of a polymer.
 
-    The radius of gyration is used to describe the dimensions of a 
+    The radius of gyration is used to describe the dimensions of a
     polymer chain, and is defined as
 
     .. math::
 
         R_\mathrm{g}=\sqrt{
         \frac{\sum_i^N m_i\|\mathbf{r}_i-\mathbf{R}_\mathrm{com}\|^2}
         {\sum_i^N m_i}}
 
-    where :math:`m_i` and :math:`\mathbf{r}_i` are the mass and 
-    position, respectively, of particle :math:`i`, and 
+    where :math:`m_i` and :math:`\mathbf{r}_i` are the mass and
+    position, respectively, of particle :math:`i`, and
     :math:`\mathbf{R}_\mathrm{com}` is the center of mass.
 
     Parameters
     ----------
     groups : `MDAnalysis.AtomGroup` or `array_like`
         Group(s) of polymers to be analyzed. All polymers in each group
         must have the same chain length.
 
     groupings : `str` or array-like, default: :code:`"atoms"`
         Determines whether the centers of mass are used in lieu of
         individual atom positions. If `groupings` is a `str`, the same
         value is used for all `groups`.
 
+        .. note::
+
+           In a standard trajectory file, segments (or chains) contain
+           residues (or molecules), and residues contain atoms. This
+           heirarchy must be adhered to for this analysis module to
+           function correctly. If your trajectory file does not contain
+           the correct segment or residue information, provide the
+           number of chains and chain lengths in `n_chains` and
+           `n_monomers`, respectively.
+
         .. container::
 
            **Valid values**:
 
            * :code:`"atoms"`: Atom positions (for coarse-grained polymer
              simulations).
-           * :code:`"residues"`: Residues' centers of mass (for 
+           * :code:`"residues"`: Residues' centers of mass (for
              atomistic polymer simulations).
 
     n_chains : `int` or array-like, optional
         Number of chains in each polymer group. Must be provided if the
         trajectory does not adhere to the standard container heirarchy
         (see Notes).
 
@@ -279,120 +298,220 @@
     components : `bool`, keyword-only, default: :code:`False`
         Specifies whether the components of the radii of gyration are
         calculated and returned instead.
 
     unwrap : `bool`, keyword-only, default: :code:`False`
         Determines whether atom positions are unwrapped.
 
+    parallel : `bool`, keyword-only, default: :code:`False`
+        Determines whether the analysis is performed in parallel.
+
     verbose : `bool`, keyword-only, default: :code:`True`
         Determines whether detailed progress is shown.
 
     **kwargs
         Additional keyword arguments to pass to
         :class:`MDAnalysis.analysis.base.AnalysisBase`.
-    
+
     Attributes
     ----------
     universe : `MDAnalysis.Universe`
         :class:`MDAnalysis.core.universe.Universe` object containing all
         information describing the system.
 
     results.units : `dict`
-        Reference units for the results. For example, to get the 
-        reference units for :code:`results.time`, call 
-        :code:`results.units["results.time"]`. Only available if OpenMM
-        is installed.
-
-    results.gyradius : `numpy.ndarray`
-        Radii of gyration for the :math:`N_\textrm{g}` groups over 
-        :math:`N_t` trajectory frames. 
-        
-        **Shape**: :math:`(N_\textrm{g},\,N_t)` 
-        (:code:`components=False`) or :math:`(N_\textrm{g},\,N_t,\,3)` 
+        Reference units for the results. For example, to get the
+        reference units for :code:`results.gyradii`, call
+        :code:`results.units["results.gyradii"]`.
+
+    results.gyradii : `numpy.ndarray`
+        Radii of gyration for the :math:`N_\textrm{g}` groups over
+        :math:`N_t` trajectory frames.
+
+        **Shape**: :math:`(N_\textrm{g},\,N_t)`
+        (:code:`components=False`) or :math:`(N_\textrm{g},\,N_t,\,3)`
         (:code:`components=True`).
 
         **Reference unit**: :math:`\textrm{Å}`.
-
-    Notes
-    -----
-    In a standard trajectory file, segments (or chains) contain
-    residues, and residues contain atoms. This heirarchy must be adhered
-    to for this analysis module to function correctly. If your
-    trajectory file does not contain the correct segment or residue
-    information, provide the number of chains and chain lengths in
-    `n_chains` and `n_monomers`, respectively.
     """
 
     def __init__(
-            self, groups: Union[mda.AtomGroup, ArrayLike],
-            groupings: Union[str, ArrayLike] = "atoms", 
-            n_chains: Union[int, ArrayLike] = None, 
-            n_monomers: Union[int, ArrayLike] = None, *, 
-            components: bool = False, unwrap: bool = False, 
-            verbose: bool = True, **kwargs):
-        
+            self, groups: Union[mda.AtomGroup, tuple[mda.AtomGroup]],
+            groupings: Union[str, tuple[str]] = "atoms",
+            n_chains: Union[int, tuple[int]] = None,
+            n_monomers: Union[int, tuple[int]] = None, *,
+            components: bool = False, unwrap: bool = False,
+            parallel: bool = False, verbose: bool = True, **kwargs):
+
         super().__init__(groups, groupings, n_chains, n_monomers,
-                         unwrap=unwrap, verbose=verbose, **kwargs)
+                         unwrap=unwrap, parallel=parallel, verbose=verbose,
+                         **kwargs)
+
+        # Determine the number of particles in each group and their
+        # corresponding indices
+        self._Ns = np.fromiter(
+            (M * N_p for M, N_p in zip(self._n_chains, self._n_monomers)),
+            dtype=int,
+            count=self._n_groups
+        )
+        self._N = self._Ns.sum()
+        self._slices = []
+        index = 0
+        for N in self._Ns:
+            self._slices.append(slice(index, index + N))
+            index += N
+
         self._components = components
-    
+
     def _prepare(self) -> None:
 
-        # Unwrap particle positions if necessary
         if self._unwrap:
             self.universe.trajectory[
-                self._sliced_trajectory.frames[0] 
-                if hasattr(self._sliced_trajectory, "frames") 
+                self._sliced_trajectory.frames[0]
+                if hasattr(self._sliced_trajectory, "frames")
                 else (self.start or 0)
             ]
-            self._positions_old = [np.empty((M * N_p, 3), dtype=float) 
-                                   for M, N_p in zip(self._n_chains, 
-                                                     self._n_monomers)]
-            for i, (g, gr) in enumerate(zip(self._groups, self._groupings)):
-                self._positions_old[i] = g.positions if gr == "atoms" \
-                                         else molecule.center_of_mass(g, gr)
-            self._images = [np.zeros(p.shape, dtype=int) 
-                            for p in self._positions_old]
-            self._threshold = self._dims / 2
 
-        # Preallocate arrays to store results
-        shape = (self._n_groups, self.n_frames, 3) if self._components \
-                else (self._n_groups, self.n_frames)
-        self.results.gyradius = np.empty(shape, dtype=float)
-        
-        # Store reference units
-        self.results.units = {"results.gyradius": unit.angstrom}
+            # Preallocate arrays to store number of boundary crossings for
+            # each particle
+            self._positions_old = np.empty((self._N, 3))
+            for g, gr, s, M, N_p in zip(self._groups, self._groupings,
+                                        self._slices, self._n_chains,
+                                        self._n_monomers):
+                if self._internal and gr == "residues":
+                    for f in g.fragments:
+                        make_whole(f)
+                    self._positions_old[s] = center_of_mass(g, gr)
+                else:
+                    positions = unwrap_edge(
+                        positions=g.positions, 
+                        bonds=np.array([(i * N_p + j, i * N_p + j + 1) 
+                                        for i in range(M) for j in range(N_p - 1)]), 
+                        dimensions=self._dimensions, 
+                        masses=g.masses
+                    )
+                    self._positions_old[s] = (
+                        positions if gr == "atoms"
+                        else center_of_mass(
+                            positions=positions.reshape(M, N_p, -1, 3),
+                            masses=g.masses.reshape(M, N_p, -1)
+                        )
+                    )
+            self._images = np.zeros((self._N, 3), dtype=int)
+            self._thresholds = self._dimensions / 2
+
+            # Store unwrapped particle positions in a shared memory array
+            # for parallel analysis
+            if self._parallel:
+                self._positions = np.empty((self.n_frames, self._N, 3))
+                for i, _ in enumerate(self.universe.trajectory[
+                        list(self._sliced_trajectory.frames)
+                        if hasattr(self._sliced_trajectory, "frames")
+                        else slice(self.start, self.stop, self.step)
+                    ]):
+                    for g, gr, s in zip(self._groups, self._groupings, self._slices):
+                        if self._internal and gr == "residues":
+                            self._positions[i, s] = center_of_mass(g, gr)
+                        else:
+                            self._positions[i, s] = (
+                                g.positions if gr == "atoms"
+                                else center_of_mass(
+                                    positions=g.positions.reshape(M, N_p, -1, 3),
+                                    masses=g.masses.reshape(M, N_p, -1)
+                                )
+                            )
+
+                    unwrap(self._positions[i], self._positions_old,
+                           self._dimensions, thresholds=self._thresholds,
+                           images=self._images)
+
+                # Clean up memory
+                del self._positions_old
+                del self._images
+                del self._thresholds
+
+        if not self._parallel:
+            shape = [self._n_groups, self.n_frames]
+            if self._components:
+                shape.append(3)
+            self.results.gyradii = np.empty(shape)
+        self.results.units = {"results.gyradii": ureg.angstrom}
 
     def _single_frame(self) -> None:
 
-        for i, (g, gr, M, N_p) in enumerate(
-                zip(self._groups, self._groupings, self._n_chains, 
-                    self._n_monomers)):
-
-            # Store atom or center-of-mass positions in the current frame
-            positions = g.positions if gr == "atoms" \
-                        else molecule.center_of_mass(g, gr)
-
-            # Unwrap particle positions if necessary
+        for i, (g, gr, M, N_p, s) in enumerate(
+                zip(self._groups, self._groupings, self._n_chains,
+                    self._n_monomers, self._slices)
+            ):
+            if self._internal and gr == "residues":
+                positions = center_of_mass(g, gr)
+            else:
+                positions = (
+                    g.positions if gr == "atoms"
+                    else center_of_mass(
+                        positions=g.positions.reshape(M, N_p, -1, 3),
+                        masses=g.masses.reshape(M, N_p, -1)
+                    )
+                )
             if self._unwrap:
-                dpos = positions - self._positions_old[i]
-                mask = np.abs(dpos) >= self._threshold
-                self._images[i][mask] -= np.sign(dpos[mask]).astype(int)
-                self._positions_old[i] = positions.copy()
-                positions += self._images[i] * self._dims
-
-            # Calculate radius of gyration
-            self.results.gyradius[i, self._frame_index] = \
-                molecule.radius_of_gyration(
+                unwrap(positions, self._positions_old[s], self._dimensions,
+                       thresholds=self._thresholds, images=self._images[s])
+
+            self.results.gyradii[i, self._frame_index] \
+                = radius_of_gyration(
                     grouping="segments",
                     positions=positions.reshape((M, N_p, 3)),
                     masses=g.masses.reshape((M, N_p)),
                     components=self._components
+                ).mean(axis=0)
+
+    def _single_frame_parallel(
+            self, frame: int, index: int) -> tuple[int, np.ndarray[float]]:
+
+        self._trajectory[frame]
+        shape = [self._n_groups]
+        if self._components:
+            shape.append(3)
+        results = np.empty(shape)
+
+        for i, (g, gr, M, N_p, s) in enumerate(
+                zip(self._groups, self._groupings, self._n_chains,
+                    self._n_monomers, self._slices)
+            ):
+            if self._unwrap:
+                positions = self._positions[index, s]
+            elif self._internal and gr == "residues":
+                positions = center_of_mass(g, gr)
+            else:
+                positions = (
+                    g.positions if gr == "atoms"
+                    else center_of_mass(
+                        positions=g.positions.reshape(M, N_p, -1, 3),
+                        masses=g.masses.reshape(M, N_p, -1)
+                    )
                 )
 
-class Relaxation(_PolymerAnalysisBase):
+            results[i] = radius_of_gyration(
+                grouping="segments",
+                positions=positions.reshape((M, N_p, 3)),
+                masses=g.masses.reshape((M, N_p)),
+                components=self._components
+            ).mean(axis=0)
+
+        return index, results
+
+    def _conclude(self) -> None:
+
+        # Consolidate parallel results
+        if self._parallel:
+            self.results.gyradii = np.stack(
+                [r[1] for r in sorted(self._results)], axis=1
+            )
+
+class EndToEndVector(_PolymerAnalysisBase):
 
     r"""
     A serial implementation to calculate the end-to-end vector
     autocorrelation function (ACF) :math:`C_\mathrm{ee}(t)` and
     estimate the orientational relaxation time :math:`\tau_\mathrm{r}`
     of a polymer.
 
@@ -409,15 +528,15 @@
 
     The orientational relaxation time can then be estimated by fitting
     a stretched exponential function
 
     .. math::
 
        C_\mathrm{ee}=\exp{\left[-(t/\tau)^\beta\right]}
-    
+
     to the end-to-end vector ACF and evaluating
 
     .. math::
 
        \tau_\mathrm{r}=\int_0^\infty C_\mathrm{ee}\,dt
        =\tau\Gamma(\frac{1}{\beta}+1)
 
@@ -428,21 +547,31 @@
         must have the same chain length.
 
     groupings : `str` or array-like, default: :code:`"atoms"`
         Determines whether the centers of mass are used in lieu of
         individual atom positions. If `groupings` is a `str`, the same
         value is used for all `groups`.
 
+        .. note::
+
+           In a standard trajectory file, segments (or chains) contain
+           residues (or molecules), and residues contain atoms. This
+           heirarchy must be adhered to for this analysis module to
+           function correctly. If your trajectory file does not contain
+           the correct segment or residue information, provide the
+           number of chains and chain lengths in `n_chains` and
+           `n_monomers`, respectively.
+
         .. container::
 
            **Valid values**:
 
            * :code:`"atoms"`: Atom positions (for coarse-grained polymer
              simulations).
-           * :code:`"residues"`: Residues' centers of mass (for 
+           * :code:`"residues"`: Residues' centers of mass (for
              atomistic polymer simulations).
 
     n_chains : `int` or array-like, optional
         Number of chains in each polymer group. Must be provided if the
         trajectory does not adhere to the standard container heirarchy
         (see Notes).
 
@@ -450,99 +579,104 @@
         Number of monomers in each chain in each polymer group. Must be
         provided if the trajectory does not adhere to the standard
         container heirarchy (see Notes).
 
     n_blocks : `int`, keyword-only, default: :code:`1`
         Number of blocks to split the trajectory into.
 
-    fft : `bool`, keyword-only, default: :code:`True`
-        Determines whether fast Fourier transforms (FFT) are used to
-        evaluate the ACFs.
-
     dt : `float` or `openmm.unit.Quantity`, keyword-only, optional
         Time between frames :math:`\Delta t`. While this is normally
         determined from the trajectory, the trajectory may not have the
         correct information if the data is in reduced units. For
         example, if your reduced timestep is :math:`0.01` and you output
-        trajectory data every :math:`10000` timesteps, then
-        :math:`\Delta t=100`. 
-        
+        trajectory data every :math:`10,000` timesteps, then
+        :math:`\Delta t=100`.
+
         **Reference unit**: :math:`\mathrm{ps}`.
 
+    fft : `bool`, keyword-only, default: :code:`True`
+        Determines whether fast Fourier transforms (FFT) are used to
+        evaluate the ACFs.
+
     unwrap : `bool`, keyword-only, default: :code:`False`
         Determines whether atom positions are unwrapped.
 
     verbose : `bool`, keyword-only, default: :code:`True`
         Determines whether detailed progress is shown.
 
     **kwargs
         Additional keyword arguments to pass to
         :class:`MDAnalysis.analysis.base.AnalysisBase`.
-    
+
     Attributes
     ----------
     universe : `MDAnalysis.Universe`
         :class:`MDAnalysis.core.universe.Universe` object containing all
         information describing the system.
 
     results.units : `dict`
-        Reference units for the results. For example, to get the 
-        reference units for :code:`results.time`, call 
-        :code:`results.units["results.time"]`. Only available if OpenMM
-        is installed.
+        Reference units for the results. For example, to get the
+        reference units for :code:`results.times`, call
+        :code:`results.units["results.times"]`.
 
-    results.time : `numpy.ndarray`
+    results.times : `numpy.ndarray`
         Changes in time :math:`t-t_0`.
 
         **Shape**: :math:`(N_t,)`.
 
         **Reference unit**: :math:`\textrm{ps}`.
 
     results.acf : `numpy.ndarray`
         End-to-end vector ACFs for the :math:`N_\textrm{g}` groups over
-        :math:`N_\textrm{b}` blocks with :math:`N_t` trajectory frames 
+        :math:`N_\textrm{b}` blocks with :math:`N_t` trajectory frames
         each.
 
-        **Shape**: 
+        **Shape**:
         :math:`(N_\textrm{g},\,N_\textrm{b},\,N_t)`.
-    
-    results.relaxation_time : `numpy.ndarray`
-        Average orientational relaxation times for the 
+
+    results.relaxation_times : `numpy.ndarray`
+        Average orientational relaxation times for the
         :math:`N_\textrm{g}` groups over :math:`N_t` trajectory frames
         split into :math:`N_\textrm{b}` blocks.
 
     Notes
     -----
     In a standard trajectory file, segments (or chains) contain
     residues, and residues contain atoms. This heirarchy must be adhered
     to for this analysis module to function correctly. If your
     trajectory file does not contain the correct segment or residue
     information, provide the number of chains and chain lengths in
     `n_chains` and `n_monomers`, respectively.
     """
 
     def __init__(
-            self, groups: Union[mda.AtomGroup, ArrayLike],
-            groupings: Union[str, ArrayLike] = "atoms", 
-            n_chains: Union[int, ArrayLike] = None, 
-            n_monomers: Union[int, ArrayLike] = None, *, n_blocks: int = 1,
-            fft: bool = True, dt: Union[float, unit.Quantity] = None, 
+            self, groups: Union[mda.AtomGroup, tuple[mda.AtomGroup]],
+            groupings: Union[str, tuple[str]] = "atoms",
+            n_chains: Union[int, tuple[int]] = None,
+            n_monomers: Union[int, tuple[int]] = None, *, n_blocks: int = 1,
+            dt: Union[float, "unit.Quantity", Q_] = None, fft: bool = True,
             unwrap: bool = False, verbose: bool = True, **kwargs) -> None:
 
-        super().__init__(groups, groupings, n_chains, n_monomers, 
+        # Disable parallel support for this analysis class
+        if "parallel" in kwargs:
+            del kwargs["parallel"]
+
+        super().__init__(groups, groupings, n_chains, n_monomers,
                          unwrap=unwrap, verbose=verbose, **kwargs)
-                        
+
+        self._N_chains = self._n_chains.sum()
+        self._slices = []
+        index = 0
+        for N in self._n_chains:
+            self._slices.append(slice(index, index + N))
+            index += N
+
         self._n_blocks = n_blocks
+        self._dt = strip_unit(dt or self._trajectory.dt, "picosecond")[0]
         self._fft = fft
-        if dt:
-            self._dt = dt
-            if type(dt).__name__ == "Quantity":
-                self._dt /= unit.picosecond
-        else:
-            self._dt = self._trajectory.dt
 
     def _prepare(self) -> None:
 
         # Determine number of frames used when the trajectory is split
         # into blocks
         self._n_frames_block = self.n_frames // self._n_blocks
         self._n_frames = self._n_blocks * self._n_frames_block
@@ -552,106 +686,131 @@
                     f"blocks, so the last {extra_frames:,} frame(s) will be "
                     "discarded. To maximize performance, set appropriate "
                     "starting and ending frames in run() so that the number "
                     "of frames to be analyzed is divisible by the number of "
                     "blocks.")
             warnings.warn(wmsg)
 
-        # Preallocate array(s) to store positions of first and last
-        # monomers of each polymer chain (and number of boundary
-        # crossings)
-        self._positions_end = [np.empty((self.n_frames, M, 2, 3), dtype=float)
-                               for M in self._n_chains]
-        
-        # Unwrap particle positions if necessary
+        self._e2e = np.empty((self.n_frames, self._N_chains, 3))
         if self._unwrap:
             self.universe.trajectory[
-                self._sliced_trajectory.frames[0] 
-                if hasattr(self._sliced_trajectory, "frames") 
+                self._sliced_trajectory.frames[0]
+                if hasattr(self._sliced_trajectory, "frames")
                 else (self.start or 0)
             ]
-            self._positions_end_prev = [np.empty((M, 2, 3), dtype=float) 
-                                       for M in self._n_chains]
-            for i, (g, gr, N_p) in enumerate(zip(self._groups, self._groupings,
-                                                 self._n_monomers)):
-                self._positions_end_prev[i] = (
-                    g.positions if gr == "atoms"
-                    else molecule.center_of_mass(g, gr)
-                ).reshape(-1, N_p, 3)[:, (0, -1)]
-            self._images = [np.zeros(p.shape, dtype=int) 
-                            for p in self._positions_end_prev]
-            self._threshold = self._dims / 2
-        
-        # Preallocate arrays to store results
-        self.results.time = self.step * self._dt * np.arange(self._n_frames //
-                                                             self._n_blocks)
-        self.results.acf = np.empty((self._n_groups, self._n_blocks, self._n_frames_block),
-                                    dtype=float)
-        
-    def _single_frame(self) -> None:
 
-        for i, (g, gr, N_p) in enumerate(zip(self._groups, self._groupings,
-                                             self._n_monomers)):
-            
-            # Store atom or center-of-mass positions in the current frame
-            self._positions_end[i][self._frame_index] = (
-                g.positions if gr == "atoms" 
-                else molecule.center_of_mass(g, gr)
-            ).reshape(-1, N_p, 3)[:, (0, -1)]
+            # Preallocate arrays to store number of boundary crossings for
+            # the first and last monomer in each chain
+            self._positions_end_old = np.empty((self._N_chains, 2, 3))
+            for g, gr, s, M, N_p in zip(self._groups, self._groupings,
+                                        self._slices, self._n_chains,
+                                        self._n_monomers):
+                if self._internal and gr == "residues":
+                    for f in g.fragments:
+                        make_whole(f)
+                    self._positions_end_old[s] = np.stack(
+                        [center_of_mass(s.residues[[0, -1]].atoms, "residues")
+                         for s in g.segments]
+                    )
+                else:
+                    positions = unwrap_edge(
+                        positions=g.positions, 
+                        bonds=np.array([(i * N_p + j, i * N_p + j + 1) 
+                                        for i in range(M) for j in range(N_p - 1)]), 
+                        dimensions=self._dimensions, 
+                        masses=g.masses
+                    ).reshape(M, N_p, -1, 3)[:, (0, -1)]
+                    self._positions_end_old[s] = (
+                        positions[:, :, 0] if gr == "atoms"
+                        else center_of_mass(
+                            positions=positions,
+                            masses=g.masses.reshape(M, N_p, -1)[:, (0, -1)]
+                        )
+                    )
+            self._images = np.zeros((self._N_chains, 2, 3), dtype=int)
+            self._thresholds = self._dimensions / 2
+
+        self.results.times = self.step * self._dt * np.arange(self._n_frames //
+                                                              self._n_blocks)
+        self.results.acf = np.empty(
+            (self._n_groups, self._n_blocks, self._n_frames_block)
+        )
+        self.results.units = {"results.times": ureg.picosecond}
+
+    def _single_frame(self) -> None:
 
-            # Unwrap particle positions if necessary
+        for g, gr, s, M, N_p in zip(self._groups, self._groupings,
+                                    self._slices, self._n_chains,
+                                    self._n_monomers):
+            if self._internal and gr == "residues":
+                positions_end = np.stack(
+                    center_of_mass(s.residues[[0, -1]].atoms, "residues")
+                    for s in g.segments
+                )
+            else:
+                positions_end = g.positions.reshape(M, N_p, -1, 3)[:, (0, -1)]
+                positions_end = (
+                    positions_end[:, :, 0] if gr == "atoms"
+                    else center_of_mass(
+                        positions=positions_end,
+                        masses=g.masses.reshape(M, N_p, -1)[:, (0, -1)]
+                    )
+                )
             if self._unwrap:
-                dpos = self._positions_end[i][self._frame_index] \
-                       - self._positions_end_prev[i]
-                mask = np.abs(dpos) >= self._threshold
-                self._images[i][mask] -= np.sign(dpos[mask]).astype(int)
-                self._positions_end_prev[i] = \
-                    self._positions_end[i][self._frame_index].copy()
-                self._positions_end[i][self._frame_index] += \
-                    self._images[i] * self._dims
+                unwrap(positions_end, self._positions_end_old[s],
+                       self._dimensions, thresholds=self._thresholds,
+                       images=self._images[s])
+            self._e2e[self._frame_index, s] \
+                = np.diff(positions_end, axis=1)[:, 0]
 
     def _conclude(self) -> None:
 
-        # Compute the end-to-end vector autocorrelation function
+        # Clean up memory
+        if self._unwrap:
+            del self._positions_end_old
+            del self._images
+            del self._thresholds
+
         _acf = correlation_fft if self._fft else correlation_shift
-        for i, M in ProgressBar(enumerate(self._n_chains)):
-            e2e = np.diff(self._positions_end[i], axis=2)[:, :, 0]
+        for i, (s, M) in ProgressBar(enumerate(zip(self._slices, 
+                                                   self._n_chains))):
             self.results.acf[i] = _acf(
-                (e2e / np.linalg.norm(e2e, axis=2, keepdims=True)).reshape(
-                    self._n_blocks, -1, M, 3
-                )
+                (self._e2e[:, s] 
+                 / np.linalg.norm(self._e2e[:, s], axis=-1, keepdims=True))
+                .reshape(self._n_blocks, -1, M, 3),
+                average=True, vector=True
             )
 
     def calculate_relaxation_time(self) -> None:
-        
+
         """
         Calculates the orientational relaxation time.
         """
 
         if not hasattr(self.results, "acf"):
-            emsg = ("Call Relaxation.run() before "
-                    "Relaxation.calculate_relaxation_time().")
+            emsg = ("Call EndToEndVector.run() before "
+                    "EndToEndVector.calculate_relaxation_time().")
             raise RuntimeError(emsg)
-        
-        self.results.relaxation_time = np.empty(
-            (self._n_groups, self._n_blocks), dtype=float
-        )
+
+        self.results.relaxation_times = np.empty((self._n_groups,
+                                                  self._n_blocks))
+        self.results.units["results.relaxation_times"] = ureg.picosecond
 
         for i, g in enumerate(self.results.acf):
             for j, acf in enumerate(g):
                 valid = np.where(acf >= 0)[0]
-                self.results.relaxation_time[i, j] = relaxation_time(
-                    self.results.time[valid], acf[valid]
+                self.results.relaxation_times[i, j] = calculate_relaxation_time(
+                    self.results.times[valid], acf[valid]
                 )
 
-class SingleChainStructureFactor(SerialAnalysisBase):
+class SingleChainStructureFactor(DynamicAnalysisBase):
 
     r"""
-    A serial implementation to calculate the single-chain structure
-    factor :math:`S_\mathrm{sc}(q)` of a homopolymer.
+    Serial and parallel implementations to calculate the single-chain
+    structure factor :math:`S_\mathrm{sc}(q)` of a homopolymer.
 
     It is defined as
 
     .. math::
 
        S_{\mathrm{sc}}(\mathbf{q})=\frac{1}{MN_\mathrm{p}}
        \sum_{m=1}^M\sum_{i,j=1}^{N_\mathrm{p}}\left\langle
@@ -661,221 +820,311 @@
     chain length, :math:`\mathbf{q}` is the scattering wavevector, and
     :math:`\mathbf{r}_i` is the position of the :math:`i`-th monomer.
 
     .. container::
 
        The single-chain structure factor reveals information about the
        characteristic length scales of the polymer:
-       
-       * In the Guinier regime (:math:`qR_g\ll1`), 
+
+       * In the Guinier regime (:math:`qR_g\ll1`),
          :math:`S_{\mathrm{sc}}(q)^{-1}\approx N_\mathrm{p}(1-(qR_g)^2/3)`
          can be used to determine the radius of gyration :math:`R_g`.
-       * In the Porod regime (:math:`qR_g\gg1`), 
+       * In the Porod regime (:math:`qR_g\gg1`),
          :math:`S_{\mathrm{sc}}(q)=1` since the only contribution is the
-         self-scattering of the monomers. 
+         self-scattering of the monomers.
        * In the intermediate regime, the slope :math:`s` of the log-log
-         plot of :math:`S_{\mathrm{sc}}(q)` is related to the scaling 
+         plot of :math:`S_{\mathrm{sc}}(q)` is related to the scaling
          exponent :math:`\nu` via :math:`\nu=-1/s`.
+
+    Parameters
+    ----------
+    group : `MDAnalysis.AtomGroup`
+        Group of polymers to be analyzed. All polymers in the group
+        must have the same chain length.
+
+    grouping : `str`, default: :code:`"atoms"`
+        Determines whether the centers of mass are used in lieu of
+        individual atom positions.
+
+        .. note::
+
+           In a standard trajectory file, segments (or chains) contain
+           residues (or molecules), and residues contain atoms. This
+           heirarchy must be adhered to for this analysis module to
+           function correctly. If your trajectory file does not contain
+           the correct segment or residue information, provide the
+           number of chains and chain lengths in `n_chains` and
+           `n_monomers`, respectively.
+
+        .. container::
+
+           **Valid values**:
+
+           * :code:`"atoms"`: Atom positions (for coarse-grained polymer
+             simulations).
+           * :code:`"residues"`: Residues' centers of mass (for
+             atomistic polymer simulations).
+
+    n_points : `int`, default: :code:`32`
+        Number of points to sample the wavevector space.
+
+    n_chains : `int`, optional
+        Number of chains in `group`. Must be provided if the topology
+        does not contain segment information.
+
+    n_monomers : `int`, optional
+        Number of monomers per chain. Must be provided if the topology
+        does not contain segment information.
+
+    dimensions : `numpy.ndarray` or `openmm.unit.Quantity`, optional
+        System dimensions. If the
+        :class:`MDAnalysis.core.universe.Universe` object that `group`
+        belongs to does not contain dimensionality information, provide
+        it here.
+
+        **Shape**: :math:`(3,)`.
+
+        **Reference unit**: :math:`\textrm{Å}`.
+
+    unwrap : `bool`, keyword-only, default: :code:`False`
+        Determines whether atom positions are unwrapped.
+
+    parallel : `bool`, keyword-only, default: :code:`False`
+        Determines whether the analysis is performed in parallel.
+
+    verbose : `bool`, keyword-only, default: :code:`True`
+        Determines whether detailed progress is shown.
+
+    **kwargs
+        Additional keyword arguments to pass to
+        :class:`MDAnalysis.analysis.base.AnalysisBase`.
+
+    Attributes
+    ----------
+    universe : `MDAnalysis.Universe`
+        :class:`MDAnalysis.core.universe.Universe` object containing all
+        information describing the system.
+
+    results.units : `dict`
+        Reference units for the results. For example, to get the
+        reference units for :code:`results.wavenumbers`, call
+        :code:`results.units["results.wavenumbers"]`.
+
+    results.wavenumbers : `numpy.ndarray`
+        Unique wavenumbers.
+
+        **Shape**: :math:`(N_q,)`.
+
+        **Reference unit**: :math:`\textrm{Å}^{-1}`.
+
+    results.scsf : `numpy.ndarray`
+        Single-chain structure factors for the unique wavenumbers.
+
+        **Shape**: :math:`(N_q,)`.
+
+    Notes
+    -----
+    In a standard trajectory file, segments (or chains) contain
+    residues, and residues contain atoms. This heirarchy must be adhered
+    to for this analysis module to function correctly. If your
+    trajectory file does not contain the correct segment or residue
+    information, provide the number of chains and chain lengths in
+    `n_chains` and `n_monomers`, respectively.
     """
 
     def __init__(
-            self, group: mda.AtomGroup, grouping: str = "atoms", 
-            n_chains: int = None, n_monomers: int = None,
-            n_points: int = 32, *, unwrap: bool = False, 
-            verbose: bool = True, **kwargs):
-        
+            self, group: mda.AtomGroup, grouping: str = "atoms",
+            n_points: int = 32, *, n_chains: int = None, n_monomers: int = None,
+            dimensions: Union[np.ndarray[float], "unit.Quantity", Q_] = None,
+            unwrap: bool = False, parallel: bool = False, verbose: bool = True,
+            **kwargs) -> None:
+
         self._group = group
         self.universe = group.universe
-        super().__init__(self.universe.trajectory, verbose=verbose, **kwargs)
-        self._dims = self.universe.dimensions[:3].copy()
 
+        super().__init__(self.universe.trajectory, parallel, verbose, **kwargs)
+
+        if dimensions is not None:
+            if len(dimensions) != 3:
+                raise ValueError("'dimensions' must have length 3.")
+            self._dimensions = np.asarray(strip_unit(dimensions, "angstrom")[0])
+        elif self.universe.dimensions is not None:
+            self._dimensions = self.universe.dimensions[:3].copy()
+        else:
+            raise ValueError("No system dimensions found or provided.")
+
+        if grouping not in (groupings := {"atoms", "residues"}):
+            emsg = (f"Invalid grouping '{grouping}'. Valid values: "
+                    f"{', '.join(groupings)}.")
+            raise ValueError(emsg)
         self._grouping = grouping
-        if hasattr(self.universe, "segments"):
+
+        if n_chains is None or n_monomers is None:
+            self._internal = True
             self._n_chains = self._group.segments.n_segments
             self._n_monomers = self._group.n_atoms // self._n_chains
         else:
-            if isinstance(n_chains, int):
+            self._internal = False
+            if isinstance(n_chains, (int, np.integer)):
                 self._n_chains = n_chains
             else:
                 emsg = ("The number of chains must be specified when "
                         "the universe does not contain segment "
                         "information.")
                 raise ValueError(emsg)
-            if isinstance(n_monomers, int):
+            if isinstance(n_monomers, (int, np.integer)):
                 self._n_monomers = n_monomers
             else:
                 emsg = ("The number of monomers per chain must be "
                         "specified when the universe does not contain "
                         "segment information.")
                 raise ValueError(emsg)
 
         self._n_points = n_points
         self._wavevectors = np.stack(
             np.meshgrid(
                 *[2 * np.pi * np.arange(self._n_points) / L
-                 for L in self._dims]
+                 for L in self._dimensions]
             ), -1
         ).reshape(-1, 3)
         self._wavenumbers = np.linalg.norm(self._wavevectors, axis=1)
 
         self._unwrap = unwrap
         self._verbose = verbose
 
-        self.results.units = {"_dims": unit.angstrom}
-
     def _prepare(self) -> None:
 
-        # Unwrap particle positions if necessary
+        # Unwrap particle positions, if necessary
         if self._unwrap:
             self.universe.trajectory[
-                self._sliced_trajectory.frames[0] 
-                if hasattr(self._sliced_trajectory, "frames") 
+                self._sliced_trajectory.frames[0]
+                if hasattr(self._sliced_trajectory, "frames")
                 else (self.start or 0)
             ]
-            self._positions_old = self._group.positions \
-                                  if self._grouping == "atoms" \
-                                  else molecule.center_of_mass(self._group, 
-                                                               self._grouping)
+
+            if self._internal and self._grouping == "residues":
+                self._positions_old = center_of_mass(self._group,
+                                                     self._grouping)
+            else:
+                self._positions_old = (
+                    self._group.positions if self._grouping == "atoms"
+                    else center_of_mass(
+                        positions=self._group.positions.reshape(
+                            self._n_chains, self._n_monomers, -1, 3
+                        ),
+                        masses=self._group.masses.reshape(
+                            self._n_chains, self._n_monomers, -1
+                        )
+                    )
+                )
             self._images = np.zeros(self._positions_old.shape, dtype=int)
-            self._threshold = self._dims / 2
+            self._thresholds = self._dimensions / 2
 
         # Determine the unique wavenumbers
         self.results.wavenumbers = np.unique(self._wavenumbers.round(11))
-        self.results.units["results.wavenumbers"] = unit.angstrom ** -1
+        self.results.units = {"results.wavenumbers": ureg.angstrom ** -1}
+
+        # Store unwrapped atom positions in a shared memory array for
+        # parallel analysis
+        if self._parallel:
+            self._positions = np.empty(
+                (self.n_frames, self._n_chains * self._n_monomers, 3)
+            )
+
+            # Store particle positions in a shared memory array
+            for i, _ in enumerate(self.universe.trajectory[
+                    list(self._sliced_trajectory.frames)
+                    if hasattr(self._sliced_trajectory, "frames")
+                    else slice(self.start, self.stop, self.step)
+                ]):
+
+                # Store atom or center-of-mass positions in the current frame
+                if self._internal and self._grouping == "residues":
+                    self._positions[i] = center_of_mass(self._group,
+                                                        self._grouping)
+                else:
+                    self._positions[i] = (
+                        self._group.positions if self._grouping == "atoms"
+                        else center_of_mass(
+                            positions=self._group.positions.reshape(
+                                self._n_chains, self._n_monomers, -1, 3
+                            ),
+                            masses=self._group.masses.reshape(
+                                self._n_chains, self._n_monomers, -1
+                            )
+                        )
+                    )
+
+                # Unwrap particle positions if necessary
+                if self._unwrap:
+                    unwrap(self._positions[i], self._positions_old,
+                           self._dimensions, thresholds=self._thresholds,
+                           images=self._images)
+
+            # Clean up memory
+            del self._positions_old
+            del self._thresholds
+            del self._images
 
         # Preallocate arrays to store results
-        self.results.scsf = np.zeros(len(self._wavevectors), dtype=float)
+        else:
+            self.results.scsf = np.zeros(len(self._wavevectors))
 
     def _single_frame(self) -> None:
 
         # Get atom or center-of-mass positions in the current frame
-        positions = self._group.positions if self._grouping == "atoms" \
-                    else molecule.center_of_mass(self._group, 
-                                                 self._grouping)
+        if self._internal and self._grouping == "residues":
+            positions = center_of_mass(self._group, self._grouping)
+        else:
+            positions = (
+                self._group.positions if self._grouping == "atoms"
+                else center_of_mass(
+                    positions=self._group.positions.reshape(
+                        self._n_chains, self._n_monomers, -1, 3
+                    ),
+                    masses=self._group.masses.reshape(
+                        self._n_chains, self._n_monomers, -1
+                    )
+                )
+            )
 
         # Unwrap particle positions if necessary
         if self._unwrap:
-            dpos = positions - self._positions_old
-            mask = np.abs(dpos) >= self._threshold
-            self._images[mask] -= np.sign(dpos[mask]).astype(int)
-            self._positions_old = positions.copy()
-            positions += self._images * self._dims
+            unwrap(positions, self._positions_old, self._dimensions,
+                   thresholds=self._thresholds, images=self._images)
 
         # Calculate single-chain structure factor contributions
         for chain in positions.reshape((self._n_chains, self._n_monomers, 3)):
             arg = np.einsum("ij,kj->ki", self._wavevectors, chain)
-            self.results.scsf += np.sin(arg).sum(axis=0) ** 2 \
-                                 + np.cos(arg).sum(axis=0) ** 2
-
-    def _conclude(self) -> None:
-
-        # Normalize the single-chain structure factor by
-        # dividing by the total number of monomers and timesteps
-        self.results.scsf /= self._n_chains * self._n_monomers \
-                             * self.n_frames
-
-        # Flatten the array for each combination by combining 
-        # values sharing the same wavevector magnitude
-        self.results.scsf = np.fromiter(
-            (self.results.scsf[np.isclose(q, self._wavenumbers)].mean() 
-             for q in self.results.wavenumbers),
-            dtype=float, 
-            count=len(self.results.wavenumbers)
-        )
-
-class ParallelSingleChainStructureFactor(
-        SingleChainStructureFactor, ParallelAnalysisBase):
-
-    r"""
-    A multithreaded implementation to calculate the single-chain 
-    structure factor :math:`S_\mathrm{sc}(q)` of a homopolymer.
-    
-    .. note::
-       For a theoretical background and a complete list of parameters,
-       attributes, and available methods, see 
-       :class:`SingleChainStructureFactor`.
-    """
-
-    def __init__(
-            self, group: mda.AtomGroup, grouping: str = "atoms", 
-            n_chains: int = None, n_monomers: int = None,
-            n_points: int = 32, *, unwrap: bool = False, 
-            verbose: bool = True, **kwargs):
-        
-        SingleChainStructureFactor.__init__(
-            self, group, grouping, n_chains, n_monomers, n_points, 
-            unwrap=unwrap, verbose=verbose, **kwargs
-        )
-        ParallelAnalysisBase.__init__(self, self.universe.trajectory, 
-                                      verbose=verbose, **kwargs)
-        
-    def _prepare(self) -> None:
+            self.results.scsf += (np.sin(arg).sum(axis=0) ** 2
+                                  + np.cos(arg).sum(axis=0) ** 2)
 
-        # Unwrap particle positions if necessary
-        self._positions = np.empty(
-            (self.n_frames, self._n_chains * self._n_monomers, 3),
-            dtype=float
-        )
-        if self._unwrap:
-            self.universe.trajectory[
-                self._sliced_trajectory.frames[0] 
-                if hasattr(self._sliced_trajectory, "frames") 
-                else (self.start or 0)
-            ]
-            positions_old = self._group.positions \
-                            if self._grouping == "atoms" \
-                            else molecule.center_of_mass(self._group, 
-                                                         self._grouping)
-            images = np.zeros(positions_old.shape, dtype=int)
-            threshold = self._dims / 2
-
-        # Store particle positions in a shared memory array
-        for i, _ in enumerate(self.universe.trajectory[
-                list(self._sliced_trajectory.frames) 
-                if hasattr(self._sliced_trajectory, "frames")
-                else slice(self.start, self.stop, self.step)
-            ]):
-
-            # Store atom or center-of-mass positions in the current frame
-            self._positions[i] = self._group.positions \
-                                 if self._grouping == "atoms" \
-                                 else molecule.center_of_mass(self._group, 
-                                                              self._grouping)
-
-            # Unwrap particle positions if necessary
-            if self._unwrap:
-                dpos = self._positions[i] - positions_old
-                mask = np.abs(dpos) >= threshold
-                images[mask] -= np.sign(dpos[mask]).astype(int)
-                positions_old = self._positions[i].copy()
-                self._positions[i] += images * self._dims
-
-        # Determine the unique wavenumbers
-        self.results.wavenumbers = np.unique(self._wavenumbers.round(11))
-
-    def _single_frame(self, frame: int, timestep: int) -> np.ndarray:
+    def _single_frame_parallel(
+            self, frame: int, index: int) -> np.ndarray[float]:
 
         # Compute the single-chain structure factor by squaring the
         # cosine and sine terms and adding them together
         scsf = np.zeros(len(self._wavevectors), dtype=float)
-        for chain in self._positions[timestep].reshape((self._n_chains, -1, 3)):
+        for chain in self._positions[index].reshape((self._n_chains, -1, 3)):
             arg = np.einsum("ij,kj->ki", self._wavevectors, chain)
             scsf += np.sin(arg).sum(axis=0) ** 2 + np.cos(arg).sum(axis=0) ** 2
-        
         return scsf
 
-    def _conclude(self):
+    def _conclude(self) -> None:
 
         # Tally single-chain structure factor for each wavevector over
         # all frames and normalize by the number of particles and timesteps
-        self.results.scsf = np.vstack(self._results).sum(axis=0) \
-                            / (self._n_chains * self._n_monomers 
-                               * self.n_frames)
-        
-        # Flatten the array by combining values sharing the same
-        # wavevector magnitude
+        if self._parallel:
+            self.results.scsf = np.vstack(self._results).sum(axis=0)
+
+        # Normalize the single-chain structure factor by
+        # dividing by the total number of monomers and timesteps
+        self.results.scsf /= self._n_chains * self._n_monomers * self.n_frames
+
+        # Flatten the array for each combination by combining
+        # values sharing the same wavevector magnitude
         self.results.scsf = np.fromiter(
-            (self.results.scsf[np.isclose(q, self._wavenumbers)].mean() 
+            (self.results.scsf[np.isclose(q, self._wavenumbers)].mean()
              for q in self.results.wavenumbers),
-            dtype=float, 
+            dtype=float,
             count=len(self.results.wavenumbers)
         )
```

### Comparing `mdhelper-0.0.2/src/mdhelper/analysis/structure.py` & `mdhelper-1.0.0/src/mdhelper/analysis/profile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1142 +1,996 @@
 """
-Bulk structural analysis
-========================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+Linear profiles
+===============
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
-This module contains classes to analyze the structure of bulk fluid and
-electrolyte systems.
+This module contains classes to quantify properties along axes, such as
+density profiles.
 """
 
+import logging
+from numbers import Real
 from typing import Union
 import warnings
 
 import MDAnalysis as mda
-from MDAnalysis.lib import distances
 import numpy as np
-from openmm import unit
-from scipy.integrate import simpson
-from scipy.signal import argrelextrema
-
-from .base import SerialAnalysisBase, ParallelAnalysisBase
-from .. import ArrayLike
-from ..algorithm import molecule
-
-def radial_histogram(
-        pos1: np.ndarray, pos2: np.ndarray, n_bins: int, range: ArrayLike,
-        dims: ArrayLike, *, exclusion: ArrayLike = None) -> np.ndarray:
-    
-    r"""
-    Calculates the radial histogram of distances between particles of
-    the same type or two different types.
-
-    Parameters
-    ----------
-    pos1 : `numpy.ndarray`
-        :math:`N_1` positions or center of masses of particles in the
-        first group.
-        
-        **Shape**: :math:`(N_1,\,3)`.
-
-    pos2 : `numpy.ndarray`
-        :math:`N_2` positions or center of masses of particles in the
-        second group.
+from scipy import integrate, sparse
 
-        **Shape**: :math:`(N_2,\,3)`.
+from .base import DynamicAnalysisBase
+from .. import FOUND_OPENMM, Q_, ureg
+from ..algorithm.molecule import center_of_mass
+from ..algorithm.topology import unwrap, wrap
+from ..algorithm.unit import strip_unit
+
+if FOUND_OPENMM:
+    from openmm import unit
+
+def calculate_potential_profile(
+        bins: np.ndarray[float], charge_density: np.ndarray[float],
+        L: float, dielectric: float = 1, *, sigma_q: float = None,
+        dV: float = None, threshold: float = 1e-5, V0: float = 0,
+        method: str = "integral", pbc: bool = False, reduced: bool = False
+    ) -> np.ndarray[float]:
 
-    n_bins : `int`
-        Number of histogram bins :math:`N_\mathrm{bins}`.
-
-    range : array-like
-        Range of radii values.
-
-        **Shape**: :math:`(2,)`.
-
-        **Reference unit**: :math:`\mathrm{Å}`.
+    r"""
+    Calculates the potential profile :math:`\Psi(z)` using the charge
+    density profile by numerically solving Poisson's equation for
+    electrostatics.
 
-    dims : array-like
-        System dimensions and orthogonality.
+    Poisson's equation is given by
 
-        **Shape**: :math:`(6,)`.
-        
-        **Reference unit**: :math:`\mathrm{Å}` (dimensions), 
-        :math:`^\circ` (orthogonality).
+    .. math::
 
-    exclusion : array-like, keyword-only, optional
-        Tiles to exclude from the interparticle distances.
+       \varepsilon_0\varepsilon_\mathrm{r}\nabla^2\Psi(z)=-\rho_q(z)
 
-        **Shape**: :math:`(2,)`.
+    where :math:`\varepsilon_0` is the vacuum permittivity,
+    :math:`\varepsilon_\mathrm{r}` is the relative permittivity,
+    :math:`\rho_q` is the charge density, and :math:`\Psi` is the
+    potential.
 
-        **Example**: :code:`(1, 1)` to exclude self-interactions.
+    The boundary conditions (BCs) are
 
-    Returns
-    -------
-    histogram : `numpy.ndarray`
-        Radial histogram.
+    .. math::
 
-        **Shape**: :math:`(N_\mathrm{bins},)`.
-    """
+       \left.\frac{\partial\Psi}{\partial z}\right\rvert_{z=0}&
+       =-\frac{\sigma_q}{\varepsilon_0\varepsilon_\mathrm{r}}\\
+       \left.\Psi\right\rvert_{z=0}&=\Psi_0
+
+    The first BC is used to ensure that the electric field in the bulk
+    of the solution is zero, while the second BC is used to set the
+    potential on the left electrode.
+
+    Poisson's equation can be evaluated by using the trapezoidal rule
+    to numerically integrate the charge density profile twice:
+
+    1. Integrate the charge density profile.
+    2. Apply the first BC by adding :math:`\sigma_q` to all points.
+    3. Integrate the profile from Step 2.
+    4. Divide by :math:`-\varepsilon_0\varepsilon_\mathrm{r}`.
+    5. Apply the second BC by adding :math:`\Psi_0` to all points.
 
-    # Get pair separation distances of atom pairs within range
-    pairs, dist = distances.capped_distance(pos1, pos2, range[1], 
-                                            box=dims)
-    
-    # TODO: MAKE MEMORY SAFE
-    
-    # Exclude atom pairs with the same atoms or atoms from the
-    # same residue
-    if exclusion is not None:
-        dist = dist[np.where(pairs[:, 0] // exclusion[0] 
-                             != pairs[:, 1] // exclusion[1])[0]]
-    
-    return np.histogram(dist, bins=n_bins, range=range)[0]
-
-def coordination_number(
-        bins: np.ndarray, rdf: np.ndarray, rho: float, *, 
-        n: int = 2, threshold: float = 0.1) -> np.ndarray:
+    This method is fast but requires many histogram bins to accurately
+    resolve the potential profile.
 
-    r"""
-    Calculates coordination numbers :math:`n_k` from a radial 
-    distribution function :math:`g_{ij}(r)`.
-
-    The definition is
+    Alternatively, Poisson's equation can be written as a system of
+    linear equations
 
     .. math::
-       
-       n_k=4\pi\rho_j\int_{r_{k-1}}^{r_k}r^2g_{ij}(r)\,dr
-
-    where :math:`k` is the index, :math:`\rho_j` is the bulk number 
-    density of species :math:`j` and :math:`r_k` is the 
-    :math:`(k + 1)`-th local minimum of :math:`g_{ij}(r)`.
-
-    If the radial distribution function :math:`g_{ij}(r)` does not 
-    contain as many local minima as `n`, this method will return 
-    `numpy.nan` for the coordination numbers that could not be 
-    calculated.
-
-    Parameters
-    ----------
-    bins : `numpy.ndarray`
-        Centers of the histogram bins.
 
-        **Shape**: :math:`(N_\mathrm{bins},)`.
-        
-        **Reference unit**: :math:`\mathrm{Å}`.
+       A\mathbf{\Psi}=\mathbf{b}
 
-    rdf : `numpy.ndarray`
-        Radial distribution function :math:`g_{ij}(r)`.
+    using second-order finite differences. :math:`A` is a tridiagonal
+    matrix and :math:`b` is a vector containing the charge density
+    profile, with boundary conditions applied in the first and last
+    rows.
 
-        **Shape**: :math:`(N_\mathrm{bins},)`.
+    The inner equations are given by
 
-    rho : `float`
-        Number density :math:`\rho_j` of species :math:`j`.
-        
-        **Reference unit**: :math:`\mathrm{Å}^{-3}`.
-
-    n : `int`, keyword-only, default: :code:`2`
-        Number of coordination numbers to calculate.
-
-    threshold : `float`, keyword-only, default: :code:`0.1`
-        Minimum :math:`g_{ij}(r)` value that must be reached before 
-        local minima are found.
+    .. math::
 
-    Returns
-    -------
-    coord_nums : `numpy.ndarray`
-        Coordination numbers :math:`n_k`.
-    """
+       \Psi_i^{''}=\frac{\Psi_{i-1}-2\Psi_i+\Psi_{i+1}}{h^2}
+       =-\frac{1}{\varepsilon_0\varepsilon_\mathrm{r}}\rho_{q,\,i}
 
-    coord_nums = np.empty(n, dtype=float)
-    coord_nums[:] = np.nan
+    where :math:`i` is the bin index and :math:`h` is the bin width.
 
-    # Find indices of minima in the radial distribution function
-    i_min, = argrelextrema(rdf, np.less)
-    i_min = i_min[rdf[i_min] >= threshold]
-    n_min = len(i_min)
-
-    # Integrate the radial distribution function to get the coordination
-    # number(s)
-    if n_min:
-        r = bins[:i_min[0] + 1]
-        coord_nums[0] = 4 * np.pi * rho \
-                        * simpson(r ** 2 * rdf[:i_min[0] + 1], r)
-        for i in range(min(n, n_min) - 1):
-            r = bins[i_min[i]:i_min[i + 1] + 1]
-            coord_nums[i + 1] = \
-                4 * np.pi * rho \
-                * simpson(r ** 2 * rdf[i_min[i]:i_min[i + 1] + 1], r)
-    else:
-        warnings.warn("No local minima found.")
+    In the case of periodic boundary conditions, the first and last
+    equations are given by
 
-    return coord_nums
+    .. math::
 
-def radial_fourier_transform(
-        r: np.ndarray, f: np.ndarray, q: np.ndarray) -> np.ndarray:
+       \Psi_0^{''}&=\frac{\Psi_{N-1}-2\Psi_0+\Psi_1}{h^2}
+       =-\frac{1}{\varepsilon_0\varepsilon_\mathrm{r}}\rho_{q,\,0}\\
+       \Psi_{N-1}^{''}&=\frac{\Psi_{N-2}-2\Psi_{N-1}+\Psi_0}{h^2}
+       =-\frac{1}{\varepsilon_0\varepsilon_\mathrm{r}}\rho_{q,\,N-1}
 
-    r"""
-    Computes the radial Fourier transform :math:`\hat{f}(q)` of
-    discrete data :math:`f(r)`.
+    When the system has slab geometry, the boundary conditions are
+    implemented via
 
     .. math::
 
-       \hat{f}(q)=\frac{4\pi}{q}\int_0^\infty f(r)r\sin(qr)\,dr
+       \Psi_0&=\Psi_0\\
+       \Psi_0^\prime&=\frac{-3\Psi_0+4\Psi_1-\Psi_2}{2h}
+       =-\frac{\sigma_q}{\varepsilon_0\varepsilon_\mathrm{r}}
+
+    This method is slower but can be more accurate even with fewer
+    histogram bins for bulk systems with periodic boundary conditions.
 
     Parameters
     ----------
-    r : `numpy.ndarray`
-        Radii :math:`r`.
+    bins : array-like
+        Histogram bin centers corresponding to the charge density
+        profile in `charge_density`.
 
-        **Reference unit**: :math:`\mathrm{Å}`.
-
-    f : `numpy.ndarray`
-        Discrete data :math:`f(r)` to Fourier transform. 
-        
-        **Shape**: Same as `r`.
-        
-    q : `numpy.ndarray`
-        Wavenumbers :math:`q` to evaluate the Fourier transforms at.
+        **Shape**: :math:`(N_\mathrm{bins},)`.
 
-        **Reference unit**: :math:`\mathrm{Å}^{-1}`.
+        **Reference unit**: :math:`\mathrm{Å}`.
 
-    Returns
-    -------
-    rft : `numpy.ndarray`
-        Radial Fourier transform of the discrete data.
+    charge_density : array-like
+        Array containing the charge density profile.
 
-        **Shape**: Same as `q`.
-    """
+        **Shape**: :math:`(N_\mathrm{bins},)`.
 
-    rft = 4 * np.pi * np.divide(simpson(f * r * np.sin(np.outer(q, r)), r), q)
-    if 0 in q:
-        rft[q == 0] = 4 * np.pi * simpson(f * r ** 2, r)
-    return rft
-
-def structure_factor(
-        r: np.ndarray, g: np.ndarray, equal: bool, rho: float,
-        x_i: float = 1, x_j: float = None, q: np.ndarray = None, *, 
-        q_lower: float = None, q_upper: float = None, n_q: int = 1000,
-        formalism: str = "FZ") -> tuple[np.ndarray, np.ndarray]:
-    
-    r"""
-    Computes the (partial) static structure factor :math:`S_{ij}(q)` 
-    using the radial histogram bins :math:`r` and the radial 
-    distribution function :math:`g_{ij}(r)` for an isotropic fluid.
+        **Reference unit**: :math:`\mathrm{e/Å}^{-3}`.
 
-    Parameters
-    ----------
-    r : `numpy.ndarray`
-        Radii :math:`r`.
+    L : `float`
+        System size in the dimension that `bins` and `charge_density`
+        were calculated in.
 
         **Reference unit**: :math:`\mathrm{Å}`.
-    
-    g : `numpy.ndarray`
-        Radial distribution function :math:`g_{ij}(r)`.
-
-        **Shape**: Same as `r`.
-
-    equal : `bool`
-        Specifies whether `g` is between the same species, or 
-        :math:`i = j`. If :code:`False`, the number concentrations of
-        species :math:`i` and :math:`j` must be specified in `x_i` and
-        `x_j`.
-    
-    rho : `float`
-        Bulk number density :math:`\rho`.
-
-        **Reference unit**: :math:`\mathrm{Å}^{-3}`.
-
-    x_i : `float`, default: :code:`1`
-        Number concentration of species :math:`i`. Required if
-        :code:`equal=False`.
-
-    x_j : `float`, optional
-        Number concentration of species :math:`j`. Required if
-        :code:`equal=False`.
-
-    q : `numpy.ndarray`, optional
-        Wavenumbers :math:`q`.
-
-        **Reference unit**: :math:`\mathrm{Å}^{-1}`.
-
-    q_lower : `float`, keyword-only, optional
-        Lower bound for the wavenumbers :math:`q`. Has no effect if `q`
-        is specified.
-
-        **Reference unit**: :math:`\mathrm{Å}^{-1}`.
-    
-    q_upper : `float`, keyword-only, optional
-        Upper bound for the wavenumbers :math:`q`. Has no effect if `q`
-        is specified.
-
-        **Reference unit**: :math:`\mathrm{Å}^{-1}`.
-    
-    n_q : `int`, keyword-only, default: :code:`1000`
-        Number of wavenumbers :math:`q` to generate. Has no effect if `q`
-        is specified.
-
-    formalism : `str`, keyword-only, default: :code:`"FZ"`
-        Formalism to use for the partial structure factor. Has no effect
-        if :code:`equal=True`.
 
-        .. container::
-        
-           **Valid values**: 
-           
-           * :code:`"general"`: A general formalism given by
+    dielectric : `float`, default: :code:`1`
+        Relative permittivity or static dielectric constant
+        :math:`\varepsilon_\mathrm{r}`.
 
-             .. math::
+    sigma_q : `float`, keyword-only, optional
+        Total surface charge density :math:`\sigma_q`. Used to
+        ensure that the electric field in the bulk of the solution
+        is zero. If not provided, it is determined using `dV` and
+        the charge density profile, or the average value in the
+        center of the integrated charge density profile if
+        :code:`method="integral"`.
 
-                S_{ij}(q)=1+x_ix_j\frac{4\pi\rho}{q}\int_0^\infty 
-                (g_{ij}(r)-1)r\sin{(qr)}\,dr
-           
-           * :code:`"FZ"`: Faber–Ziman formalism [1]_
+        .. note::
 
-             .. math::
+           This value should be negative if the potential difference
+           is positive and vice versa.
 
-                S_{ij}(q)=1+\frac{4\pi\rho}{q}\int_0^\infty
-                (g_{ij}(r)-1)r\sin{(qr)}\,dr
-             
-           * :code:`"AL"`: Ashcroft–Langreth formalism [2]_
+        **Reference unit**: :math:`\mathrm{e/Å^2}`.
 
-             .. math::
+    dV : `float`, keyword-only, optional
+        Potential difference :math:`\Delta\Psi` across the system
+        dimension specified in `axis`. Has no effect if `sigma_q` is
+        provided since this value is used solely to calculate
+        `sigma_q`.
 
-                S_{ij}(q)=\delta_{ij}+(x_ix_j)^{1/2}\frac{4\pi\rho}{q}
-                \int_0^\infty (g_{ij}(r)-1)r\sin{(qr)}\,dr
+        **Reference unit**: :math:`\mathrm{V}`.
 
-    Returns
-    -------
-    q : `numpy.ndarray`
-        Wavenumbers :math:`q`.
+    threshold : `float`, keyword-only, default: :code:`1e-5`
+        Threshold for determining the plateau region of the first
+        integral of the charge density profile to calculate
+        `sigma_q`. Has no effect if `sigma_q` is provided or if
+        `sigma_q` can be calculated using `dV` and `dielectric`.
 
-        **Shape**: :math:`(N_q,)`.
-    
-    S : `numpy.ndarray`
-        (Partial) static structure factor :math:`S(q)`. 
+    V0 : `float`, keyword-only, default: :code:`0`
+        Potential :math:`\Psi_0` at the left boundary.
 
-        **Shape**: :math:`(N_q,)`.
+        **Reference unit**: :math:`\mathrm{V}`.
 
-    References
-    ----------
-    .. [1] T. E. Faber and J. M. Ziman, A Theory of the Electrical 
-       Properties of Liquid Metals: III. the Resistivity of Binary 
-       Alloys, *Philosophical Magazine* **11**, **153** (1965).
-       https://doi.org/10.1080/14786436508211931
-
-    .. [2] N. W. Ashcroft and D. C. Langreth, Structure of Binary Liquid
-       Mixtures. I, *Phys. Rev.* **156**, **685** (1967).
-       https://doi.org/10.1103/PhysRev.156.685
-    """
+    method : `str`, keyword-only, default: :code:`"integral"`
+        Method to use to calculate the potential profile.
 
-    if q is None:
-        if q_lower is None:
-            q_lower = 2 * np.pi / r[-1]
-        if q_upper is None:
-            q_upper = 2 * np.pi / r[0]
-        q = np.linspace(q_lower, q_upper, 
-                        int((q_upper - q_lower) / q_lower) 
-                        if n_q is None else n_q)
-    
-    rho_sft = rho * radial_fourier_transform(r, g - 1, q)
-    if equal or formalism == "FZ":
-        return q, 1 + rho_sft
-    elif not equal:
-        if formalism == "AL":
-            return q, (x_i == x_j) + np.sqrt(x_i * x_j) * rho_sft
-        elif formalism == "general":
-            return q, 1 + x_i * x_j * rho_sft
-    raise ValueError("Invalid formalism.")
+        **Valid values**: :code:`"integral"`, :code:`"matrix"`.
 
-class RDF(SerialAnalysisBase):
+    pbc : `bool`, keyword-only, default: :code:`False`
+        Specifies whether the axis has periodic boundary conditions.
+        Only used when :code:`method="matrix"`.
 
-    r"""
-    A serial implementation to calculate the radial distribution 
-    function (RDF) :math:`g_{ij}(r)` between types :math:`i` and 
-    :math:`j`.
+    reduced : `bool`, keyword-only, default: :code:`False`
+        Specifies whether the data is in reduced units.
 
-    It is given by
+    Returns
+    -------
+    potential : `numpy.ndarray`
+        Potential profile :math:`\Psi(z)`.
 
-    .. math::
+        **Shape**: :math:`(N_\mathrm{bins},)`.
 
-       g_{ij}(r)=\frac{1}{N_iN_j}\sum_\alpha\sum_\beta \left\langle
-       \delta\left(|\pmb{r}_\alpha-\pmb{r}_\beta|-r\right)\right\rangle
+        **Reference unit**: :math:`\mathrm{V}`.
+    """
 
-    where :math:`N_i` and :math:`N_j` are the number of particles, and
-    :math:`\pmb{r}_\alpha` and :math:`\pmb{r}_\beta` are the positions 
-    of particles :math:`\alpha` and :math:`\beta` belonging to 
-    species :math:`i` and :math:`j`, respectively. The RDF is normalized
-    such that :math:`\lim_{r\rightarrow\infty}g_{ij}(r)=1` in a 
-    homogeneous system.
-
-    (A closely related quantity is the single particle density 
-    :math:`n_{ij}(r)=\rho_jg_{ij}(r)`, where :math:`\rho_j` is the
-    number density of species :math:`j`.)
+    if len(bins) != len(charge_density):
+        emsg = ("'bins' and 'charge_density' arrays must have the same "
+                "length.")
+        raise ValueError(emsg)
+
+    CONVERSION_FACTOR = 4 * np.pi if reduced else (
+        1 * ureg.elementary_charge / (ureg.vacuum_permittivity * ureg.angstrom)
+    ).m_as(ureg.volt)
+
+    # Calculate surface charge density for system with perfectly
+    # conducting boundaries
+    if sigma_q is None and dV is not None:
+        sigma_q = (integrate.trapezoid(bins * charge_density, bins)
+                   - dielectric * dV / CONVERSION_FACTOR) / L
+
+    if method == "integral":
+        potential = integrate.cumulative_trapezoid(charge_density, bins,
+                                                   initial=0)
+
+        if sigma_q is None:
+            wmsg = ("No surface charge density information. The value "
+                    "will be extracted from the integrated charge "
+                    "density profile, which may be inaccurate due to "
+                    "numerical errors.")
+            warnings.warn(wmsg)
+
+            # Get surface charge density from the integrated charge
+            # density profile
+            cut_indices = np.where(
+                np.diff(np.abs(np.gradient(potential)) < threshold)
+            )[0] + 1
+            if len(cut_indices) == 0:
+                logging.warning(
+                    "No bulk plateau region found in the charge "
+                    "density profile. The average value over the "
+                    "entire profile will be used."
+                )
+                sigma_q = potential.mean()
+            else:
+                target_index = len(potential) // 2
+                sigma_q = potential[
+                    cut_indices[cut_indices <= target_index][-1]:
+                    cut_indices[cut_indices >= target_index][0]
+                ].mean()
+
+        return (
+            -CONVERSION_FACTOR
+            * integrate.cumulative_trapezoid(potential + sigma_q, bins,
+                                             initial=V0) / dielectric
+        )
 
-    The cumulative RDF is
+    elif method == "matrix":
+        if sigma_q is None:
+            emsg = ("No surface charge density information. Either "
+                    "'sigma_q' or 'dV' must be provided when "
+                    "method='matrix'.")
+            raise ValueError(emsg)
 
-    .. math::
+        h = bins[1] - bins[0]
+        if not np.allclose(np.diff(bins), h):
+            raise ValueError("'bins' must be uniformly spaced.")
+
+        # Set up matrix and load vector for second-order finite
+        # difference method
+        N = len(bins)
+        A = sparse.diags((1, -2, 1), (-1, 0, 1), shape=(N, N), format="csc")
+        b = charge_density.copy()
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore",
+                                  category=sparse.SparseEfficiencyWarning)
+            if pbc:
+                A[0, -1] = A[-1, 0] = 1
+                b *= -CONVERSION_FACTOR * h ** 2 / dielectric
+                psi = np.empty_like(b)
+                psi[1:] = sparse.linalg.spsolve(A[1:, 1:], b[1:])
+                psi[0] = psi[-1]
+                return psi
+            else:
+                A[0, :3] = -1.5, 2, -0.5
+                A[-1, 0] = 1
+                A[-1, -2:] = 0
+                b[0] = -CONVERSION_FACTOR * h * sigma_q / dielectric
+                b[1:-1] *= -CONVERSION_FACTOR * h ** 2 / dielectric
+                b[-1] = 0
+                return sparse.linalg.spsolve(A, b)
 
-       G_{ij}(r)=\int_0^r4\pi Rg_{ij}(R)\,dR
+class DensityProfile(DynamicAnalysisBase):
 
-    and the average number of :math:`j` particles found within radius
-    :math:`r` is
+    """
+    Serial and parallel implementations to calculate the number and
+    charge density profiles :math:`\\rho_i(z)` and :math:`\\rho_q(z)` of
+    a system along the specified axes.
+
+    The microscopic number density profile of species :math:`i` in a
+    constant-volume system is calculated by binning particle positions
+    along an axis :math:`z` using
 
     .. math::
 
-       N_{ij}(r)=\rho_jG_{ij}(r)
+       \\rho_i(z)=\\frac{V}{N_\\mathrm{bin}}\\left\\langle
+       \\sum_\\alpha\\delta(z-z_\\alpha)\\right\\rangle
 
-    The expression above can be used to compute the coordination numbers
-    (number of neighbors in each solvation shell) by setting :math:`r`
-    to the :math:`r`-values where :math:`g_{ij}(r)` is locally 
-    maximized, which signify the solvation shell boundaries.
+    where :math:`V` is the system volume and :math:`N_\\mathrm{bins}` is
+    the number of bins. The angular brackets denote an ensemble average.
 
-    .. container::
+    If the species carry charges, the charge density profile can be
+    obtained using
 
-       The RDF can also be used to obtain other relevant structural 
-       properties, such as
+    .. math::
 
-       * the potential of mean force
+       \\rho_q(z)=\\sum_i z_ie\\rho_i(z)
 
-         .. math::
+    where :math:`z_i` is the charge number of species :math:`i` and
+    :math:`e` is the elementary charge.
 
-            w_{ij}(r)=-k_\mathrm{B}T\ln{g_{ij}(r)}
+    With the charge density profile, the potential profile can be
+    computed by numerically solving Poisson's equation for
+    electrostatics:
 
-         where :math:`k_\mathrm{B}` is the Boltzmann constant and 
-         :math:`T` is the system temperature, and
+    .. math::
 
-       * the (partial) static structure factor (see 
-         :func:`structure_factor` for the possible definitions).
+       \\varepsilon_0\\varepsilon_\\mathrm{r}\\nabla^2\\Psi(z)=-\\rho_q(z)
 
     Parameters
     ----------
-    ag1 : `MDAnalysis.AtomGroup`
-        First atom group :math:`i`.
+    groups : `MDAnalysis.AtomGroup` or array-like
+        Groups of atoms for which density profiles are calculated.
 
-    ag2 : `MDAnalysis.AtomGroup`
-        Second atom group :math:`j`.
-    
-    n_bins : `int`, default: :code:`201`
-        Number of histogram bins :math:`N_\mathrm{bins}`.
+    groupings : `str` or array-like, default: :code:`"atoms"`
+        Determines whether the centers of mass are used in lieu of
+        individual atom positions. If `groupings` is a `str`, the same
+        value is used for all `groups`.
 
-    range : array-like, default: :code:`(0.0, 15.0)`
-        Range of radii values.
+        .. note::
 
-        **Shape**: :math:`(2,)`.
+           If the desired grouping is not :code:`"atoms"`,
 
-        **Reference unit**: :math:`\mathrm{Å}`.
+           * the trajectory file should have segments (or chains)
+             containing residues (or molecules) and residues containing
+             atoms, and
+
+           * residues and segments should be locally unwrapped at the
+             simulation box edges, if not already, using
+             :class:`MDAnalysis.transformations.wrap.unwrap`,
+             :meth:`MDAnalysis.core.groups.AtomGroup.unwrap`, or
+             :func:`MDAnalysis.lib.mdamath.make_whole`.
 
-    norm : `str`, keyword-only, default: :code:`"rdf"`
-        Determines how the radial histograms are normalized.
-        
         .. container::
 
-           **Valid values**: 
-        
-           * :code:`norm="rdf"`: The radial distribution function
-             :math:`g_{ij}(r)` is computed.
-           * :code:`norm="density"`: The single particle density 
-             :math:`n_{ij}(r)` is computed.
-           * :code:`norm=None`: The raw particle pair count in the 
-             radial histogram bins is returned.
-
-    exclusion : array-like, keyword-only, optional
-        Tiles to exclude from the interparticle distances. The 
-        `groupings` parameter dictates what a tile represents.
-
-        **Shape**: :math:`(2,)`.
+           **Valid values**:
 
-        **Example**: :code:`(1, 1)` to exclude self-interactions.
+           * :code:`"atoms"`: Atom positions (generally or for
+             coarse-grained simulations).
+           * :code:`"residues"`: Residues' centers of mass (for
+             atomistic simulations).
+           * :code:`"segments"`: Segments' centers of mass (for
+             atomistic polymer simulations).
 
-    groupings : `str` or array-like, keyword-only, default: :code:`"atoms"`
-        Determines whether the centers of mass are used in lieu of
-        individual atom positions. If `groupings` is a `str`, the same
-        value is used for all `groups`.
+    axes : `int`, `str`, or array-like, default: :code:`"xyz"`
+        Axes along which to compute the density profiles.
 
         .. container::
 
-           **Valid values**: 
+           **Examples**:
 
-           * :code:`"atoms"`: Atom positions (generally for 
-             coarse-grained simulations).
-           * :code:`"residues"`: Residues' centers of mass (for 
-             atomistic simulations).
-           * :code:`"segments"`: Segments' centers of mass (for 
-             atomistic polymer simulations).
+           * :code:`2` for the :math:`z`-direction.
+           * :code:`"xy"` for the :math:`x`- and :math:`y`-directions.
+           * :code:`(0, 1)` for the :math:`x`- and :math:`y`-directions.
+
+    n_bins : `int` or array-like
+        Number of bins for each axis. If an `int` is provided, the same
+        value is used for all axes. If :code:`parallel=True`, the number
+        of bins in all axes must be the same.
+
+    charges : array-like, keyword-only, optional
+        Charge numbers :math:`z_i` for the specified `groupings` in the
+        :math:`N_\\mathrm{g}` `groups`. If not provided, it will be
+        retrieved from the main
+        :class:`MDAnalysis.core.universe.Universe` object if available.
+
+        .. note::
+
+           Depending on the grouping for a specific group, all atoms,
+           residues, or segments should have the same charge since the
+           charge density profile for the group would not make sense
+           otherwise. If this condition does not hold, change how the
+           particles are grouped in `grouping` such that all entities
+           share the same charge.
+
+        **Shape**: :math:`(N_\\mathrm{g})`.
+
+        **Reference unit**: :math:`\\mathrm{e}`.
+
+    dimensions : array-like, keyword-only, optional
+        System dimensions. If the
+        :class:`MDAnalysis.core.universe.Universe` object that the
+        groups in `groups` belong to does not contain dimensionality
+        information, provide it here. Affected by `scales`.
+
+        **Shape**: :math:`(3,)`.
+
+        **Reference unit**: :math:`\\mathrm{Å}`.
+
+    dt : `float`, `openmm.unit.Quantity`, or `pint.Quantity`, \
+    keyword-only, optional
+        Time between frames :math:`\\Delta t`. While this is normally
+        determined from the trajectory, the trajectory may not have the
+        correct information if the data is in reduced units. For
+        example, if your reduced timestep is :math:`0.01` and you output
+        trajectory data every :math:`10,000` timesteps, then
+        :math:`\\Delta t = 100`.
+
+        **Reference unit**: :math:`\\mathrm{ps}`.
+
+    scales : array-like, keyword-only, optional
+        Scaling factors for each system dimension. If an `int` is
+        provided, the same value is used for all axes.
+
+        **Shape**: :math:`(3,)`.
+
+    average : `bool`, keyword-only, default: :code:`True`
+        Determines whether the density profiles are averaged over the
+        specified frames.
+
+    recenter : `int`, `list`, `MDAnalysis.AtomGroup`, or `tuple`, \
+    keyword-only, optional
+        Constrains the center of mass of an atom group by adjusting the
+        particle coordinates every analysis frame. Either specify an
+        :class:`MDAnalysis.core.groups.AtomGroup`, its index within
+        `groups`, or a tuple containing the aforementioned information
+        and the fixed center of mass coordinates, in that order. To
+        avoid recentering in a specific dimension, set the coordinate to
+        :code:`numpy.nan`. If the center of mass is not specified, the
+        center of the simulation box is used.
+
+        **Shape**: :math:`(3,)` for the fixed center of mass.
 
     reduced : `bool`, keyword-only, default: :code:`False`
-        Specifies whether the data is in reduced units.
+        Specifies whether the data is in reduced units. Affects
+        `results.number_densities`, `results.charge_densities`, etc.
+
+    parallel : `bool`, keyword-only, default: :code:`False`
+        Determines whether the analysis is performed in parallel.
 
     verbose : `bool`, keyword-only, default: :code:`True`
         Determines whether detailed progress is shown.
 
     **kwargs
         Additional keyword arguments to pass to
         :class:`MDAnalysis.analysis.base.AnalysisBase`.
-    
+
     Attributes
     ----------
     universe : `MDAnalysis.Universe`
         :class:`MDAnalysis.core.universe.Universe` object containing all
-        information describing the system.
+        information describing the simulation system.
 
     results.units : `dict`
-        Reference units for the results. For example, to get the 
-        reference units for :code:`results.bins`, call 
-        :code:`results.units["results.bins"]`. Only available if OpenMM
-        is installed.
+        Reference units for the results. For example, to get the
+        reference units for :code:`results.bins`, call
+        :code:`results.units["results.bins"]`.
 
-    results.edges : `numpy.ndarray`
-        Edges of the histogram bins.
+    results.times : `numpy.ndarray`
+        Times at which the density profiles are calculated.
 
-        **Shape**: :math:`(N_\mathrm{bins}+1,)`.
-
-        **Reference unit**: :math:`\textrm{Å}`.
-
-    results.bins : `numpy.ndarray`
-        Centers of the histogram bins.
-
-        **Shape**: :math:`(N_\mathrm{bins},)`.
+        **Shape**: :math:`(N_\\mathrm{frames},)`.
 
-        **Reference unit**: :math:`\textrm{Å}`.
+        **Reference unit**: :math:`\\mathrm{ps}`.
 
-    results.counts : `numpy.ndarray`
-        Raw particle pair counts in the radial histogram bins.
+    results.bins : `list`
+        Bin centers corresponding to the density profiles in each
+        dimension.
 
-        **Shape**: :math:`(N_\mathrm{bins},)`.
+        **Shape**: :math:`(N_\\mathrm{axes},)` list of
+        :math:`(N_\\mathrm{bins},)` arrays.
 
-    results.rdf : `numpy.ndarray`
-        .. container::
+        **Reference unit**: :math:`\\mathrm{Å}`.
 
-           One of
-        
-           * :code:`norm="rdf"`: the radial distribution function
-             :math:`g_{ij}(r)`,
-           * :code:`norm="density"`: the single particle density
-             :math:`n_{ij}(r)`, or
-           * :code:`norm=None`: the raw particle pair count in the
-             radial histogram bins.
+    results.number_densities : `list`
+        Number density profiles.
 
-        **Shape**: :math:`(N_\mathrm{bins},)`.
+        **Shape**: :math:`(N_\\mathrm{axes},)` list of
+        :math:`(N_\\mathrm{bins},)` arrays.
 
-    results.coordination_numbers : `numpy.ndarray`
-        Coordination numbers :math:`n_k`. Only available after running 
-        :meth:`calculate_coordination_number`.
-
-    results.pmf : `numpy.ndarray`
-        Potential of mean force :math:`w(r)`. Only available after
-        running :meth:`calculate_pmf`.
+        **Reference unit**: :math:`\\mathrm{Å}^{-3}`.
 
-        **Shape**: :math:`(N_\mathrm{bins},)`.
+    results.charge_densities : `list`
+        Charge density profiles, if charge information is available.
 
-        **Reference unit**: :math:`\mathrm{kJ/mol}`.
+        **Shape**: :math:`(N_\\mathrm{axes},)` list of
+        :math:`(N_\\mathrm{bins},)` arrays.
 
-    results.wavenumbers : `numpy.ndarray`
-        Wavenumbers :math:`q`. Only available after running
-        :meth:`calculate_structure_factor`.
+        **Reference unit**: :math:`\\mathrm{e/Å}^{-3}`.
 
-        **Reference unit**: :math:`\textrm{Å}^{-1}`.
+    results.potentials : `dict`
+        Potential profiles, if charge information is available, with
+        the key being the axis index (e.g., :code:`1` for the :math:`z`-
+        direction if :code:`axes="yz"`). Only available after running
+        :meth:`calculate_potential_profile`.
 
-    results.ssf : `numpy.ndarray`
-        (Partial) static structure factor. Only available after running
-        :meth:`calculate_structure_factor`.
+        **Shape**: :math:`(N_\\mathrm{bins},)` for the potential
+        profiles.
 
-        **Shape**: Same as `results.wavenumbers`.
+        **Reference unit**: :math:`\\mathrm{V}`.
     """
 
-    _GROUPINGS = {"atoms", "residues", "segments"}
-
     def __init__(
-            self, ag1: mda.AtomGroup, ag2: mda.AtomGroup = None,
-            n_bins: int = 201, range: ArrayLike = (0.0, 15.0), *,
-            norm: str = "rdf", exclusion: ArrayLike = None,
-            groupings: Union[str, ArrayLike] = "atoms",
-            reduced: bool = False, verbose: bool = False, **kwargs) -> None:
-
-        self.ag1 = ag1
-        self.ag2 = ag1 if ag2 is None else ag2
-        self.universe = self.ag1.universe
-        if self.universe.dimensions is None and self._ts.dimensions is None:
-            raise ValueError("Trajectory does not contain system "
-                             "dimension information.")
-        super().__init__(self.universe.trajectory, verbose=verbose, **kwargs)
+            self, groups: Union[mda.AtomGroup, tuple[mda.AtomGroup]],
+            groupings: Union[str, tuple[str]] = "atoms",
+            axes: Union[int, str, tuple[Union[int, str]]] = "xyz",
+            n_bins: Union[int, tuple[int]] = 201, *,
+            charges: Union[np.ndarray[float], "unit.Quantity", Q_] = None,
+            dimensions: Union[np.ndarray[float], "unit.Quantity", Q_] = None,
+            dt: Union[float, "unit.Quantity", Q_] = None,
+            scales: Union[float, tuple[float]] = 1, average: bool = True,
+            recenter: Union[mda.AtomGroup, int,
+                            tuple[Union[mda.AtomGroup, int],
+                                  np.ndarray[float]]] = None,
+            reduced: bool = False, parallel: bool = False,
+            verbose: bool = True, **kwargs) -> None:
+
+        self._groups = [groups] if isinstance(groups, mda.AtomGroup) else groups
+        self.universe = self._groups[0].universe
 
+        super().__init__(self.universe.trajectory, parallel, verbose, **kwargs)
+
+        self._n_groups = len(self._groups)
         if isinstance(groupings, str):
-            if groupings not in self._GROUPINGS:
-                emsg = (f"Invalid grouping '{groupings}'. The options are "
-                        "'atoms', 'residues', and 'segments'.")
+            if groupings not in (GROUPINGS := {"atoms", "residues",
+                                               "segments"}):
+                emsg = (f"Invalid grouping '{groupings}'. Valid values: "
+                        f"{', '.join(GROUPINGS)}.")
                 raise ValueError(emsg)
-            self._groupings = 2 * [groupings]
+            self._groupings = self._n_groups * [groupings]
         else:
+            if self._n_groups != len(groupings):
+                emsg = ("The number of grouping values is not equal to "
+                        "the number of groups.")
+                raise ValueError(emsg)
             for g in groupings:
-                if g not in self._GROUPINGS:
-                    emsg = (f"Invalid grouping '{g}'. The options are "
-                            "'atoms', 'residues', and 'segments'.")
+                if g not in (GROUPINGS := {"atoms", "residues", "segments"}):
+                    emsg = (f"Invalid grouping '{g}'. Valid values: "
+                            f"{', '.join(GROUPINGS)}.")
                     raise ValueError(emsg)
-            self._groupings = 2 * groupings if len(groupings) == 1 else groupings
-
-        self._n_bins = n_bins
-        self._range = range
-        self._norm = norm
-        self._exclusion = exclusion
-        self._reduced = reduced
-        self._verbose = verbose
-
-    def _prepare(self) -> None:
-
-        # Preallocate arrays to store neighbor counts
-        self.results.edges = np.linspace(*self._range, self._n_bins + 1)
-        self.results.bins = (self.results.edges[:-1] 
-                             + self.results.edges[1:]) / 2
-        self.results.counts = np.zeros(self._n_bins, dtype=int)
-        if not self._reduced:
-            self.results.units = {"results.bins": unit.angstrom,
-                                  "results.edges": unit.angstrom}
-
-        # Preallocate floating-point number for total volume analyzed
-        # (for when system dimensions can change, such as during NpT
-        # equilibration)
-        if self._norm == "rdf":
-            self._volume = 0.0
-
-    def _single_frame(self) -> None:
-
-        # Tally counts in each pair separation distance bin
-        self.results.counts += radial_histogram(
-            pos1=self.ag1.positions 
-                 if self._groupings[0] == "atoms"
-                 else molecule.center_of_mass(self.ag1, self._groupings[0]),
-            pos2=self.ag2.positions 
-                 if self._groupings[1] == "atoms"
-                 else molecule.center_of_mass(self.ag2, self._groupings[1]),
-            n_bins=self._n_bins,
-            range=self._range,
-            dims=self._ts.dimensions,
-            exclusion=self._exclusion
-        )
-        
-        # Add volume analyzed
-        if self._norm == "rdf":
-            self._volume += self._ts.volume
-            
-    def _conclude(self):
-
-        # Compute the normalization factor
-        norm = self.n_frames
-        if self._norm is not None:
-            norm *= 4 * np.pi * np.diff(self.results.edges ** 3) / 3
-            if self._norm == "rdf":
-                _N2 = getattr(self.ag2, f"n_{self._groupings[1]}")
-                if self._exclusion:
-                    _N2 -= self._exclusion[1]
-                norm *= (getattr(self.ag1, f"n_{self._groupings[0]}") * _N2
-                         * self.n_frames / self._volume)
-        
-        # Compute and store the radial distribution function, the single
-        # particle density, or the raw radial pair counts
-        self.results.rdf = self.results.counts / norm
-
-    def _get_rdf(self) -> np.ndarray:
-
-        """
-        Returns the existing radial distribution function (RDF) if 
-        :code:`norm="rdf"` was passed to the :class:`RDF` constructor. 
-        Otherwise, the RDF is calculated and returned.
-
-        Returns
-        -------
-        rdf : `numpy.ndarray`
-            Radial distribution function :math:`g_{ij}(r)`.
-        """
+            self._groupings = groupings
 
-        if self._norm == "rdf":
-            return self.results.rdf
+        if isinstance(axes, int):
+            self._axes = np.array((axes,), dtype=int)
         else:
-            _N2 = getattr(self.ag2, f"n_{self._groupings[1]}")
-            if self._exclusion:
-                _N2 -= self._exclusion[1]
-            return 3 * self._volume * self.results.counts / (
-                4 * np.pi * self.n_frames ** 2 * _N2 
-                * getattr(self.ag1, f"n_{self._groupings[0]}") 
-                * np.diff(self.results.edges ** 3)
+            self._axes = np.fromiter(
+                (ord(a.lower()) - 120 if isinstance(a, str) else a
+                 for a in axes),
+                count=len(axes),
+                dtype=int
             )
 
-    def calculate_coordination_number(
-            self, rho: float, *, n: int = 2, threshold: float = 0.1) -> None:
-
-        r"""
-        Calculates the coordination numbers :math:`n_k`.
-
-        If the radial distribution function :math:`g_{ij}(r)` does not 
-        contain :math:`k` local minima, this method will return 
-        `numpy.nan` for the coordination numbers that could not be 
-        calculated.
-
-        Parameters
-        ----------
-        rho : `float`
-            Number density :math:`\rho_j` of species :math:`j`.
-            
-            **Reference unit**: :math:`\mathrm{nm}^{-3}`.
-
-        n : `int`, keyword-only, default: :code:`2`
-            Number of coordination numbers to calculate.
-
-        threshold : `float`, keyword-only, default: :code:`0.1`
-            Minimum :math:`g_{ij}(r)` value for a local minimum to be
-            considered the boundary of a radial shell.
-        """
-
-        self.results.coordination_numbers = coordination_number(
-            self.results.bins, self._get_rdf(), rho, n=n, threshold=threshold
-        )
-
-    def calculate_pmf(self, temp: Union[float, unit.Quantity]) -> None:
-
-        r"""
-        Calculates the potential of mean force :math:`w_{ij}(r)`.
+        if isinstance(n_bins, int):
+            self._n_bins = n_bins * np.ones(self._axes.shape, dtype=int)
+        elif not isinstance(n_bins, str):
+            if len(n_bins) == len(self._axes):
+                if parallel and np.any(n_bins != n_bins[0]):
+                    emsg = ("All axes must use the same number of bins "
+                            "when parallel=True.")
+                    raise ValueError(emsg)
+                self._n_bins = n_bins
+            else:
+                emsg = ("The dimension of the array of bin counts is "
+                        "incompatible with the number of axes to "
+                        "calculate density profiles along.")
+                raise ValueError(emsg)
+        else:
+            emsg = ("The specified bin counts must be an integer or an "
+                    "iterable object.")
+            raise ValueError(emsg)
 
-        Parameters
-        ----------
-        temp : `float` or `openmm.unit.Quantity`
-            System temperature :math:`T`.
+        if charges is not None:
+            if len(charges) != self._n_groups:
+                emsg = ("The number of group charges is not equal to "
+                        "the number of groups.")
+                raise ValueError(emsg)
+            charges, unit_ = strip_unit(charges, "elementary_charge")
+            if reduced and not isinstance(unit_, str):
+                emsg = "'charges' cannot have units when reduced=True."
+                raise TypeError(emsg)
+            self._charges = np.asarray(charges)
+        elif hasattr(self.universe.atoms, "charges"):
+            self._charges = np.empty(self._n_groups)
+            for i, (g, gr) in enumerate(zip(self._groups, self._groupings)):
+                qs = getattr(g, gr).charges
+                if not np.allclose((q := qs[0]), qs):
+                    self._charges = None
+                    wmsg = (f"Not all {gr} in group {i} share the same "
+                            "charge. The charge density profile will "
+                            "be calculated.")
+                    warnings.warn(wmsg)
+                    break
+                self._charges[i] = q
+        else:
+            self._charges = None
 
-            .. note::
+        if dimensions is not None:
+            if len(dimensions) != 3:
+                raise ValueError("'dimensions' must have length 3.")
+            self._dimensions = np.asarray(
+                strip_unit(dimensions, "angstrom")[0]
+            )
+        elif self.universe.dimensions is not None:
+            self._dimensions = self.universe.dimensions[:3].copy()
+        else:
+            raise ValueError("No system dimensions found or provided.")
 
-               If :code:`reduced=True` was set in the :class:`RDF` 
-               constructor, `temp` should be equal to the energy scale.
-               When the Lennard-Jones potential is used, it generally
-               means that :math:`T^*=1`, or `temp=1`.
+        if isinstance(scales, Real) or (len(scales) == 3
+                                        and isinstance(scales[0], Real)):
+            self._dimensions *= scales
+        else:
+            emsg = ("The scaling factor(s) must be provided as a "
+                    "floating-point number or in an array with shape "
+                    "(3,).")
+            raise ValueError(emsg)
 
-            **Reference unit**: :math:`\mathrm{K}`.
-        """
+        self._dt, unit_ = strip_unit(dt or self._trajectory.dt, "picosecond")
+        if reduced and not isinstance(unit_,  str):
+            raise TypeError("'dt' cannot have units when reduced=True.")
 
-        if self._reduced:
-            kBT = temp
+        if recenter is None:
+            self._recenter = recenter
         else:
-            if isinstance(temp, (int, float)):
-                kBT = (unit.AVOGADRO_CONSTANT_NA 
-                       * unit.BOLTZMANN_CONSTANT_kB * temp * unit.kelvin
-                       / unit.kilojoule_per_mole)
+            if isinstance(recenter, (int, mda.AtomGroup)):
+                recenter_group = recenter
+                recenter_position = self._dimensions / 2
+            elif isinstance(recenter, tuple) and len(recenter) == 2:
+                recenter_group, recenter_position = recenter
+                recenter_position = np.asarray(recenter_position)
             else:
-                kBT = (unit.AVOGADRO_CONSTANT_NA * unit.BOLTZMANN_CONSTANT_kB
-                       * temp / unit.kilojoule_per_mole)
-            self.results.units = {"results.pmf": unit.kilojoule_per_mole}
-
-        self.results.pmf = -kBT * np.log(self._get_rdf())
-
-    def calculate_structure_factor(
-            self, rho: float, x_i: float = None, x_j: float = None, 
-            q: np.ndarray = None, *, q_lower: float = None, 
-            q_upper: float = None, n_q: int = 1000, formalism: str = "FZ"
-        ) -> None:
-    
-        r"""
-        Computes the (partial) static structure factor :math:`S_{ij}(q)`
-        using the radial histogram bins :math:`r` and the radial 
-        distribution function :math:`g_{ij}(r)` for an isotropic fluid.
-
-        Parameters
-        ----------
-        rho : `float`
-            Bulk number density :math:`rho`.
-
-            **Reference unit**: :math:`\mathrm{Å}^{-3}`.
-
-        x_i : `float`, default: :code:`1`
-            Number concentration of species :math:`i`. Required if
-            the two atom groups are not identical.
-
-        x_j : `float`, optional
-            Number concentration of species :math:`j`. Required if
-            the two atom groups are not identical.
-            
-        q : `numpy.ndarray`, optional
-            Wavenumbers :math:`q`.
-
-            **Reference unit**: :math:`\mathrm{Å}^{-1}`.
-
-        q_lower : `float`, keyword-only, optional
-            Lower bound for the wavenumbers :math:`q`. Has no effect if `q`
-            is specified.
-
-            **Reference unit**: :math:`\mathrm{Å}^{-1}`.
-        
-        q_upper : `float`, keyword-only, optional
-            Upper bound for the wavenumbers :math:`q`. Has no effect if `q`
-            is specified.
-
-            **Reference unit**: :math:`\mathrm{Å}^{-1}`.
-        
-        n_q : `int`, keyword-only, default: :code:`1000`
-            Number of wavenumbers :math:`q` to generate. Has no effect if `q`
-            is specified.
-
-        formalism :`str`, keyword-only, default: :code:`"FZ"`
-            Formalism to use for the partial structure factor. Has no effect
-            if the two atom groups are the same.
-
-            .. container::
-            
-               **Valid values**: 
-            
-               * :code:`"general"`: A general formalism similar to that
-                 of the static structure factor, except the second term
-                 is multiplied by :math:`x_ix_j`.
-               * :code:`"FZ"`: Faber–Ziman formalism.
-               * :code:`"AL"`: Ashcroft–Langreth formalism.
-        """
-
-        self.results.wavenumbers, self.results.ssf = structure_factor(
-            self.results.bins, self._get_rdf(), self.ag1 == self.ag2, 
-            rho, x_i, x_j, q=q, q_lower=q_lower, q_upper=q_upper, 
-            n_q=n_q, formalism=formalism
-        )
-
-class ParallelRDF(RDF, ParallelAnalysisBase):
-
-    """
-    A multithreaded implementation to calculate the radial distribution
-    function :math:`g_{ij}(r)` and its related properties.
-    
-    .. note::
-       For a theoretical background and a complete list of
-       parameters, attributes, and available methods, see :class:`RDF`.
-    """
+                emsg = ("Invalid value passed to 'recenter'. The argument "
+                        "must either be a MDAnalysis.AtomGroup, its index "
+                        "in 'groups', multiple groups/indices, or a tuple "
+                        "containing the aforementioned information and a "
+                        "specified center of mass, in that order.")
+                raise ValueError(emsg)
+            if isinstance(recenter_group, int) \
+                    and not 0 <= recenter_group < self._n_groups:
+                raise ValueError("Invalid group index passed to 'recenter'.")
+            elif isinstance(recenter_group, mda.AtomGroup):
+                try:
+                    recenter_group = self._groups.index(recenter_group)
+                except ValueError:
+                    emsg = ("The specified AtomGroup in 'recenter' is not "
+                            "in 'groups'.")
+                    raise ValueError(emsg)
+            self._recenter = (recenter_group, recenter_position)
 
-    def __init__(
-            self, ag1: mda.AtomGroup, ag2: mda.AtomGroup = None,
-            n_bins: int = 201, range: ArrayLike = (0.0, 15.0), *,
-            norm: str = "rdf", exclusion: ArrayLike = None, 
-            groupings: Union[str, ArrayLike] = "atoms",
-            reduced: bool = False, verbose: bool = True, **kwargs) -> None:
-
-        RDF.__init__(self, ag1, ag2, n_bins, range, norm=norm,
-                     exclusion=exclusion, groupings=groupings, 
-                     reduced=reduced, verbose=verbose, **kwargs)
-        ParallelAnalysisBase.__init__(self, ag1.universe.trajectory,
-                                      verbose=verbose, **kwargs)
-
-    def _single_frame(self, frame: int, timestep: int) -> np.ndarray:
-
-        _ts = self._trajectory[frame]
-        result = np.empty(1 + self._n_bins, dtype=float)
-
-        # Compute radial histogram for a single frame
-        result[:self._n_bins] = radial_histogram(
-            pos1=self.ag1.positions 
-                 if self._groupings[0] == "atoms"
-                 else molecule.center_of_mass(self.ag1, self._groupings[0]),
-            pos2=self.ag2.positions 
-                 if self._groupings[1] == "atoms"
-                 else molecule.center_of_mass(self.ag2, self._groupings[1]),
-            n_bins=self._n_bins,
-            range=self._range,
-            dims=_ts.dimensions,
-            exclusion=self._exclusion
+        # Determine the number of particles in each group and their
+        # corresponding indices
+        self._Ns = np.fromiter(
+            (getattr(a, f"n_{g}")
+             for (a, g) in zip(self._groups, self._groupings)),
+            dtype=int,
+            count=self._n_groups
         )
+        self._N = self._Ns.sum()
+        self._slices = []
+        index = 0
+        for N in self._Ns:
+            self._slices.append(slice(index, index + N))
+            index += N
 
-        # Store system volume of current frame in the last slot of the
-        # results array
-        result[self._n_bins] = _ts.volume
-
-        return result
-
-    def _conclude(self):
-
-        # Tally counts in each pair separation distance bin over all
-        # frames
-        self._results = np.vstack(self._results).sum(axis=0)
-        self.results.counts[:] = self._results[:self._n_bins]
-        self._volume = self._results[self._n_bins]
-
-        # Compute the normalization factor
-        norm = self.n_frames
-        if self._norm is not None:
-            norm *= 4 * np.pi * np.diff(self.results.edges ** 3) / 3
-            if self._norm == "rdf":
-                _N2 = getattr(self.ag2, f"n_{self._groupings[1]}")
-                if self._exclusion:
-                    _N2 -= self._exclusion[1]
-                norm *= (getattr(self.ag1, f"n_{self._groupings[0]}") * _N2
-                         * self.n_frames / self._volume)
-        
-        # Compute and store the radial distribution function, the single
-        # particle density, or the raw radial pair counts
-        self.results.rdf = self.results.counts / norm
-        
-class StructureFactor(SerialAnalysisBase):
-
-    r"""
-    The static structure factor :math:`S(q)` is a measure of how a
-    material scatters incident radiation. It is defined as
-
-    .. math::
-
-        S(\mathbf{q})&=\frac{1}{N}\left\langle\sum_{j=1}^N\sum_{k=1}^N
-        \exp{[-i\mathbf{q}\cdot(\mathbf{r}_j-\mathbf{r}_k)]}\right\rangle\\
-        &=\frac{1}{N}\left\langle\left[
-        \sum_{j=1}^N\sin{(\mathbf{q}\cdot\mathbf{r}_j)}\right]^2+\left[
-        \sum_{j=1}^N\cos{(\mathbf{q}\cdot\mathbf{r}_j)}\right]^2\right\rangle
-
-    where :math:`N` is the number of particles, :math:`\mathbf{q}` is
-    the scattering wavevector, and :math:`\mathbf{r}_i` is the position 
-    of the :math:`i`-th monomer.
+        self._average = average
+        self._reduced = reduced
+        self._verbose = verbose
 
-    Parameters
-    ----------
-    groups : `MDAnalysis.AtomGroup` or array-like
-        Group(s) of atoms that share the same grouping type. All atoms
-        in the universe must be assigned to a group.
+    def _prepare(self) -> None:
 
-    groupings : `str` or array-like, default: :code:`"atoms"`
-        Determines whether the centers of mass are used in lieu of
-        individual atom positions. If `groupings` is a `str`, the same
-        value is used for all `groups`.
+        self.results.bins = [
+            np.linspace(
+                self._dimensions[a] / (2 * self._n_bins[i]),
+                self._dimensions[a]
+                - self._dimensions[a] / (2 * self._n_bins[i]),
+                self._n_bins[i]
+            ) for i, a in enumerate(self._axes)
+        ]
 
-        .. container::
+        if self._recenter is not None:
 
-           **Valid values**:
+            # Navigate to first frame in analysis
+            self.universe.trajectory[
+                self._sliced_trajectory.frames[0]
+                if hasattr(self._sliced_trajectory, "frames")
+                else (self.start or 0)
+            ]
 
-           * :code:`"atoms"`: Atom positions (generally for 
-             coarse-grained simulations).
-           * :code:`"residues"`: Residues' centers of mass (for 
-             atomistic simulations).
-           * :code:`"segments"`: Segments' centers of mass (for 
-             atomistic polymer simulations).
+            # Preallocate arrays to store number of boundary crossings
+            # for each particle
+            self._positions_old = np.empty((self._N, 3))
+            for g, gr, s in zip(self._groups, self._groupings, self._slices):
+                self._positions_old[s] = (g.positions if gr == "atoms"
+                                          else center_of_mass(g, gr))
+            self._images = np.zeros((self._N, 3), dtype=int)
+            self._thresholds = self._dimensions / 2
+
+            # [Parallel] Store unwrapped particle positions in a shared
+            # memory array for parallel analysis
+            if self._parallel:
+                self._positions = np.empty((self.n_frames, self._N, 3))
+
+                # Store atom or center-of-mass positions in the current
+                # frame
+                for i, _ in enumerate(self._sliced_trajectory):
+                    for g, gr, s in zip(self._groups, self._groupings,
+                                        self._slices):
+                        self._positions[i, s] = (g.positions if gr == "atoms"
+                                                 else center_of_mass(g, gr))
+
+                    # Globally unwrap positions for correct center of
+                    # mass calculation
+                    unwrap(self._positions[i], self._positions_old,
+                           self._dimensions, thresholds=self._thresholds,
+                           images=self._images)
+
+                    # Calculate difference in center of mass and
+                    # shift particle positions by the difference
+                    scom = center_of_mass(
+                        positions=self._positions
+                                  [i, self._slices[self._recenter[0]]],
+                        masses=getattr(
+                            self._groups[self._recenter[0]],
+                            self._groupings[self._recenter[0]]
+                        ).masses
+                    )
+                    self._positions[i] -= np.fromiter(
+                        (0 if np.isnan(cx) else sx - cx
+                         for sx, cx in zip(scom, self._recenter[1])),
+                        dtype=float,
+                        count=3
+                    )
+
+                # Wrap positions back into the simulation box so that they
+                # belong to a histogram bin
+                wrap(self._positions, self._dimensions)
+
+        # [Serial] Preallocate arrays to hold atom positions for a
+        # given frame so that it doesn't have to be recreated each
+        # frame, and number density profiles
+        if not self._parallel:
+            self._positions = np.empty((self._N, 3))
+            shape = [self._n_groups]
+            if not self._average:
+                shape.append(self.n_frames)
+            self.results.number_densities = [np.zeros((*shape, n))
+                                             for n in self._n_bins]
+
+        # Store time information
+        if not self._average:
+            if hasattr(self._sliced_trajectory, "frames"):
+                self.results.times \
+                    = np.asarray(self._sliced_trajectory.frames) * self._dt
+            else:
+                self.results.times = self._dt * np.arange(
+                    self._sliced_trajectory.start,
+                    self._sliced_trajectory.stop,
+                    self._sliced_trajectory.step
+                )
+
+        # Store reference units
+        self.results.units = {
+            "results.bins": ureg.angstrom,
+            "results.number_densities": ureg.angstrom ** -3
+        }
+        if self._charges is not None:
+            self.results.charge_densities = [None for _ in self._axes]
+            self.results.units["results.charge_densities"] = (
+                ureg.elementary_charge / ureg.angstrom ** 3
+            )
 
-    n_points : `int`, default: :code:`32`
-        Number of points in the scattering wavevector grid.
+    def _single_frame(self):
 
-    unwrap : `bool`, keyword-only, default: :code:`False`
-        Determines whether atom positions are unwrapped.
+        # Store atom or center-of-mass positions in the current frame
+        for g, gr, s in zip(self._groups, self._groupings, self._slices):
+            self._positions[s] = (g.positions if gr == "atoms"
+                                  else center_of_mass(g, gr))
 
-    verbose : `bool`, keyword-only, default: :code:`True`
-        Determines whether detailed progress is shown.
+        if self._recenter is not None:
 
-    **kwargs
-        Additional keyword arguments to pass to
-        :class:`MDAnalysis.analysis.base.AnalysisBase`.
+            # Globally unwrap positions for correct center of mass
+            # calculation
+            unwrap(self._positions, self._positions_old, self._dimensions,
+                   thresholds=self._thresholds, images=self._images)
+
+            # Calculate difference in centers of mass and shift particle
+            # positions by the difference
+            scom = center_of_mass(
+                positions=self._positions[self._slices[self._recenter[0]]],
+                masses=getattr(self._groups[self._recenter[0]],
+                               self._groupings[self._recenter[0]]).masses
+            )
+            self._positions -= np.fromiter(
+                (0 if np.isnan(cx) else sx - cx
+                 for sx, cx in zip(scom, self._recenter[1])),
+                dtype=float,
+                count=3
+            )
 
-    Attributes
-    ----------
-    universe : `MDAnalysis.Universe`
-        :class:`MDAnalysis.core.universe.Universe` object containing all
-        information describing the system.
+        # Wrap positions back into the simulation box so that they
+        # belong to a histogram bin
+        wrap(self._positions, self._dimensions)
+
+        # Compute and tally the bin counts for the current positions
+        for i, (gr, s) in enumerate(zip(self._groupings, self._slices)):
+            for a, (axis, n_bins) in enumerate(zip(self._axes, self._n_bins)):
+                if self._average:
+                    self.results.number_densities[a][i] += np.histogram(
+                        self._positions[s, axis], n_bins,
+                        (0, self._dimensions[axis])
+                    )[0]
+                else:
+                    self.results.number_densities[a][i, self._frame_index] \
+                        = np.histogram(self._positions[s, axis], n_bins,
+                                       (0, self._dimensions[axis]))[0]
+
+    def _single_frame_parallel(
+            self, frame: int, index: int) -> tuple[int, np.ndarray[float]]:
 
-    results.units : `dict`
-        Reference units for the results. For example, to get the 
-        reference units for :code:`results.wavenumbers`, call 
-        :code:`results.units["results.wavenumbers"]`. Only available if
-        OpenMM is installed.
+        # Set current trajectory frame
+        self._trajectory[frame]
 
-    results.wavenumbers : `numpy.ndarray`
-        Scattering wavenumbers :math:`q`.
+        # Preallocate array to hold bin counts for the current frame
+        results = np.empty((len(self._axes), self._n_groups, self._n_bins[0]))
 
-    results.ssf : `numpy.ndarray`
-        Static structure factor :math:`S(q)`.
+        if self._recenter is None:
+            positions = np.empty((self._N, 3))
+            for g, gr, s in zip(self._groups, self._groupings, self._slices):
+                positions[s] = (g.positions if gr == "atoms"
+                                else center_of_mass(g, gr))
+            wrap(positions, self._dimensions)
+        else:
+            positions = self._positions[index]
 
-        **Shape**: Same as `results.wavenumbers`.
-    """
+        # Compute and tally the bin counts for the current positions
+        for i, (gr, s) in enumerate(zip(self._groupings, self._slices)):
+            for a, axis in enumerate(self._axes):
+                results[a, i] = np.histogram(
+                    positions[s, axis], self._n_bins[0], (0, self._dimensions[axis])
+                )[0]
 
-    def __init__(
-            self, groups: Union[mda.AtomGroup, ArrayLike],
-            groupings: Union[str, ArrayLike] = "atoms", n_points: int = 32,
-            *, unwrap: bool = False, verbose: bool = True, **kwargs):
+        return index, results
 
-        self._groups = [groups] if isinstance(groups, mda.AtomGroup) else groups
-        self.universe = self._groups[0].universe
-        if sum(g.n_atoms for g in self._groups) != self.universe.atoms.n_atoms:
-            emsg = ("The provided atom groups do not contain all atoms "
-                    "in the universe.")
-            raise ValueError(emsg)
-        
-        super().__init__(self.universe.trajectory, verbose=verbose, **kwargs)
-        self._dims = self.universe.dimensions[:3].copy()
+    def _conclude(self):
 
-        self._n_groups = len(self._groups)
-        if isinstance(groupings, str):
-            if groupings not in {"atoms", "residues"}:
-                emsg = (f"Invalid grouping '{groupings}'. The options are "
-                        "'atoms' and 'residues'.")
-                raise ValueError(emsg)
-            self._groupings = self._n_groups * [groupings]
+        # Consolidate parallel results and clean up memory by deleting
+        # arrays that will not be reused
+        if self._parallel:
+            if self._recenter is not None:
+                del self._positions
+            self.results.number_densities = np.stack(
+                [r[1] for r in sorted(self._results)], axis=1
+            )
+            if self._average:
+                self.results.number_densities \
+                    = self.results.number_densities.sum(axis=1)
         else:
-            if self._n_groups != len(groupings):
-                emsg = ("The number of grouping values is not equal to the "
-                        "number of groups.")
-                raise ValueError(emsg)
-            for g in groupings:
-                if g not in {"atoms", "residues"}:
-                    emsg = (f"Invalid grouping '{g}'. The options are "
-                            "'atoms' and 'residues'.")
-                    raise ValueError(emsg)
-            self._groupings = groupings
-
-        self._Ns = tuple(getattr(a, f"n_{g}")
-                         for (a, g) in zip(self._groups, self._groupings))
-        self._N = sum(self._Ns)
-        self._slices = []
-        index = 0
-        for N in self._Ns:
-            self._slices.append(slice(index, index + N))
-            index += N
-
-        self._n_points = n_points
-        self._wavevectors = np.stack(
-            np.meshgrid(
-                *[2 * np.pi * np.arange(self._n_points) / L
-                 for L in self._dims]
-            ), -1
-        ).reshape(-1, 3)
-        self._wavenumbers = np.linalg.norm(self._wavevectors, axis=1)
+            del self._positions
+        if self._recenter is not None:
+            del self._positions_old, self._images, self._thresholds
+
+        V = np.prod(self._dimensions)
+        for a in range(len(self._axes)):
+            denom = self._n_bins[a] / V
+            if self._average:
+                denom /= self.n_frames
+            self.results.number_densities[a] *= denom
+
+            if self._charges is not None:
+                self.results.charge_densities[a] = np.einsum(
+                    "g,...gb->...b",
+                    self._charges,
+                    self.results.number_densities[a]
+                )
+
+    def calculate_potential_profile(
+            self, dielectric: float, axis: Union[int, str], *,
+            sigma_q: Union[float, "unit.Quantity", Q_] = None,
+            dV: Union[float, "unit.Quantity", Q_] = None,
+            threshold: float = 1e-5, V0: Union[float, "unit.Quantity", Q_] = 0,
+            method: str = "integral", pbc: bool = False) -> None:
 
-        self._unwrap = unwrap
-        self._verbose = verbose
+        """
+        Calculates the average potential profile in the given dimension
+        using the charge density profile by numerically solving Poisson's
+        equation for electrostatics.
 
-        self.results.units = {"_dims": unit.angstrom}
+        Parameters
+        ----------
+        dielectric : `float`
+            Relative permittivity or dielectric constant
+            :math:`\\varepsilon_\\mathrm{r}`.
 
-    def _prepare(self) -> None:
+        axis : `int` or `str`
+            Axis along which to compute the potential profiles.
 
-        # Unwrap particle positions if necessary
-        self._positions = np.empty((self._N, 3), dtype=float)
-        if self._unwrap:
-            self.universe.trajectory[
-                self._sliced_trajectory.frames[0] 
-                if hasattr(self._sliced_trajectory, "frames") 
-                else (self.start or 0)
-            ]
-            self._positions_old = np.empty(self._positions.shape, dtype=float)
-            for g, gr, s in zip(self._groups, self._groupings, self._slices):
-                self._positions_old[s] = \
-                    g.positions if gr == "atoms" \
-                    else molecule.center_of_mass(g, gr)
-            self._images = np.zeros(self._positions_old.shape, dtype=int)
-            self._threshold = self._dims / 2
-
-        # Determine the unique wavenumbers
-        self.results.wavenumbers = np.unique(self._wavenumbers.round(11))
-        self.results.units["results.wavenumbers"] = unit.angstrom ** -1
-
-        # Preallocate arrays to store results
-        self.results.ssf = np.zeros(len(self._wavenumbers), dtype=float)
-        
-    def _single_frame(self) -> None:
+            .. container::
 
-        for g, gr, s in zip(self._groups, self._groupings, self._slices):
-            
-            # Store atom or center-of-mass positions in the current frame
-            self._positions[s] = g.positions if gr == "atoms" \
-                                 else molecule.center_of_mass(g, gr)
-
-            # Unwrap particle positions if necessary
-            if self._unwrap:
-                dpos = self._positions[s] - self._positions_old[s]
-                mask = np.abs(dpos) >= self._threshold
-                self._images[s][mask] -= np.sign(dpos[mask]).astype(int)
-                self._positions_old[s] = self._positions[s].copy()
-                self._positions[s] += self._images[s] * self._dims
-
-        # Compute the static structure factor by squaring the
-        # cosine and sine terms and adding them together
-        arg = np.einsum("ij,kj->ki", self._wavevectors, self._positions)
-        self.results.ssf += np.sin(arg).sum(axis=0) ** 2 \
-                            + np.cos(arg).sum(axis=0) ** 2
-
-    def _conclude(self) -> None:
-
-        # Normalize the static structure factor by the number of 
-        # particles and timesteps
-        self.results.ssf /= self._N * self.n_frames
-        
-        # Flatten the array by combining values sharing the same
-        # wavevector magnitude
-        self.results.ssf = np.fromiter(
-            (self.results.ssf[np.isclose(q, self._wavenumbers)].mean() 
-             for q in self.results.wavenumbers),
-            dtype=float, 
-            count=len(self.results.wavenumbers)
-        )
+               **Examples**:
 
-class ParallelStructureFactor(StructureFactor, ParallelAnalysisBase):
+               * :code:`2` for the :math:`z`-direction.
+               * :code:`"x"` for the :math:`x`-direction.
 
-    """
-    A multithreaded implementation to calculate the static structure 
-    factor :math:`S(q)`.
-    
-    .. note::
-       For a theoretical background and a complete list of parameters,
-       attributes, and available methods, see :class:`StructureFactor`.
-    """
+        sigma_q : `float`, `openmm.unit.Quantity`, or `pint.Quantity`, \
+        keyword-only, optional
+            Total surface charge density :math:`\\sigma_q`. Used to
+            ensure that the electric field in the bulk of the solution
+            is zero. If not provided, it is determined using `dV` and
+            the charge density profile, or the average value in the
+            center of the integrated charge density profile.
+
+            **Reference unit**: :math:`\\mathrm{e/Å^2}`.
+
+        dV : `float`, `openmm.unit.Quantity`, or `pint.Quantity`, \
+        keyword-only, optional
+            Potential difference :math:`\\Delta\\Psi` across the system
+            dimension specified in `axis`. Has no effect if `sigma_q` is
+            provided since this value is used solely to calculate
+            `sigma_q`.
+
+            **Reference unit**: :math:`\\mathrm{V}`.
+
+        threshold : `float`, keyword-only, default: :code:`1e-5`
+            Threshold for determining the plateau region of the first
+            integral of the charge density profile to calculate
+            `sigma_q`. Has no effect if `sigma_q` is provided, or if
+            `sigma_q` can be calculated using `dV` and `dielectric`.
+
+        V0 : `float`, `openmm.unit.Quantity`, or `pint.Quantity`, \
+        keyword-only, default: :code:`0`
+            Potential :math:`\\Psi_0` at the left boundary.
+
+            **Reference unit**: :math:`\\mathrm{V}`.
+
+        method : `str`, keyword-only, default: :code:`"integral"`
+            Method to use to calculate the potential profile.
+
+            **Valid values**: :code:`"integral"`, :code:`"matrix"`.
+
+        pbc : `bool`, keyword-only, default: :code:`False`
+            Specifies whether the system has periodic boundary conditions.
+            Only used when :code:`method="matrix"`.
+        """
 
-    def __init__(
-            self, groups: Union[mda.AtomGroup, ArrayLike],
-            groupings: Union[str, ArrayLike] = "atoms", n_points: int = 32,
-            *, unwrap: bool = False, verbose: bool = True, **kwargs):
-        
-        StructureFactor.__init__(self, groups, groupings, n_points, 
-                                 unwrap=unwrap, verbose=verbose, **kwargs)
-        ParallelAnalysisBase.__init__(self, self.universe.trajectory, 
-                                      verbose=verbose, **kwargs)
-        
-    def _prepare(self) -> None:
+        if not hasattr(self.results, "charge_densities"):
+            emsg = ("Either call run() before calculate_potential_profile() "
+                    "or provide charge information when initializing "
+                    "the DensityProfile object.")
+            raise RuntimeError(emsg)
+
+        if not hasattr(self.results, "potentials"):
+            self.results.potentials = {}
+            self.results.units["results.potentials"] = ureg.volt
+
+        if isinstance(axis, str):
+            axis = ord(axis.lower()) - 120
+        index = np.where(self._axes == axis)[0][0]
+
+        if sigma_q is not None:
+            sigma_q, unit_ = strip_unit(sigma_q,
+                                        "elementary_charge/angstrom**2")
+            if self._reduced and not isinstance(unit_, str):
+                emsg = "'sigma_q' cannot have units when reduced=True."
+                raise ValueError(emsg)
 
-        # Unwrap particle positions if necessary
-        self._positions = np.empty((self.n_frames, self._N, 3), dtype=float)
-        if self._unwrap:
-            self.universe.trajectory[
-                self._sliced_trajectory.frames[0] 
-                if hasattr(self._sliced_trajectory, "frames") 
-                else (self.start or 0)
-            ]
-            positions_old = np.empty((self._N, 3), dtype=float)
-            for g, gr, s in zip(self._groups, self._groupings, self._slices):
-                positions_old[s] = g.positions if gr == "atoms" \
-                                   else molecule.center_of_mass(g, gr)
-            images = np.zeros(positions_old.shape, dtype=int)
-            threshold = self._dims / 2
-
-        # Store particle positions in a shared memory array
-        for i, _ in enumerate(self.universe.trajectory[
-                list(self._sliced_trajectory.frames) 
-                if hasattr(self._sliced_trajectory, "frames")
-                else slice(self.start, self.stop, self.step)
-            ]):
+        if dV is not None:
+            dV, unit_ = strip_unit(dV, "volt")
+            if self._reduced and not isinstance(unit_, str):
+                emsg = "'dV' cannot have units when reduced=True."
+                raise ValueError(emsg)
 
-            for g, gr, s in zip(self._groups, self._groupings, self._slices):
+        if V0 is not None:
+            V0, unit_ = strip_unit(V0, "volt")
+            if self._reduced and not isinstance(unit_, str):
+                emsg = "'V0' cannot have units when reduced=True."
+                raise ValueError(emsg)
 
-                # Store atom or center-of-mass positions in the current frame
-                self._positions[i, s] = g.positions if gr == "atoms" \
-                                        else molecule.center_of_mass(g, gr)
-                
-                # Unwrap particle positions if necessary
-                if self._unwrap:
-                    dpos = self._positions[i, s] - positions_old[s]
-                    mask = np.abs(dpos) >= threshold
-                    images[s][mask] -= np.sign(dpos[mask]).astype(int)
-                    positions_old[s] = self._positions[i, s].copy()
-                    self._positions[i, s] += images[s] * self._dims
-
-        # Determine the unique wavenumbers
-        self.results.wavenumbers = np.unique(self._wavenumbers.round(11))
-
-    def _single_frame(self, frame: int, timestep: int) -> np.ndarray:
-
-        # Compute the static structure factor by squaring the
-        # cosine and sine terms and adding them together
-        arg = np.einsum("ij,kj->ki", self._wavevectors, 
-                        self._positions[timestep])
-        return np.sin(arg).sum(axis=0) ** 2 + np.cos(arg).sum(axis=0) ** 2
-    
-    def _conclude(self) -> None:
-
-        # Tally static structure factor for each wavevector over all
-        # frames and normalize by the number of particles and timesteps
-        self.results.ssf = np.vstack(self._results).sum(axis=0) \
-                           / (self._N * self.n_frames)
-        
-        # Flatten the array by combining values sharing the same
-        # wavevector magnitude
-        self.results.ssf = np.fromiter(
-            (self.results.ssf[np.isclose(q, self._wavenumbers)].mean() 
-             for q in self.results.wavenumbers),
-            dtype=float, 
-            count=len(self.results.wavenumbers)
+        charge_density = self.results.charge_densities[index]
+        if charge_density.ndim == 3:
+            charge_density = charge_density.mean(axis=1)
+        self.results.potentials[index] = calculate_potential_profile(
+            self.results.bins[index],
+            charge_density,
+            self._dimensions[axis],
+            dielectric,
+            sigma_q=sigma_q,
+            dV=dV,
+            threshold=threshold,
+            V0=V0,
+            method=method,
+            pbc=pbc,
+            reduced=self._reduced
         )
```

### Comparing `mdhelper-0.0.2/src/mdhelper/analysis/transport.py` & `mdhelper-1.0.0/src/mdhelper/analysis/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,116 +1,123 @@
 """
 Transport properties
 ====================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 This module contains classes to evaluate the transport properties of
 fluid systems.
 """
 
 import itertools
 from typing import Union
 import warnings
 
 import MDAnalysis as mda
 from MDAnalysis.lib.log import ProgressBar
+from MDAnalysis.lib.mdamath import make_whole
 import numpy as np
-from openmm import unit
 from scipy import optimize
 
 from .base import SerialAnalysisBase
-from .. import ArrayLike
-from ..algorithm import correlation, molecule
+from .. import FOUND_OPENMM, Q_, ureg
+from ..algorithm import correlation
+from ..algorithm.molecule import center_of_mass
+from ..algorithm.topology import unwrap, wrap
+from ..algorithm.unit import strip_unit
 from ..fit.polynomial import poly1
 
-def msd_fft(*args, **kwargs) -> np.ndarray:
+if FOUND_OPENMM:
+    from openmm import unit
+
+def msd_fft(*args, **kwargs) -> np.ndarray[float]:
 
     """
-    Calculates the mean squared displacement (MSD) or the analogous 
+    Calculates the mean squared displacement (MSD) or the analogous
     cross displacement (CD) using fast Fourier transforms (FFT).
 
     .. note::
 
        This is an alias function. For more information, see
        :func:`mdhelper.algorithm.correlation.msd_fft`.
     """
 
     return correlation.msd_fft(*args, **kwargs)
 
 def msd_shift(*args, **kwargs) -> np.ndarray:
 
     """
-    Calculates the mean squared displacement (MSD) or the analogous 
+    Calculates the mean squared displacement (MSD) or the analogous
     cross displacement (CD) using the Einstein relation.
 
     .. note::
 
        This is an alias function. For more information, see
        :func:`mdhelper.algorithm.correlation.msd_shift`.
     """
-    
+
     return correlation.msd_shift(*args, **kwargs)
 
-def coefficients(
-        time: np.ndarray, msd_cross: np.ndarray, msd_self: np.ndarray, 
-        Ns: np.ndarray, dims: np.ndarray, kBT: float, start: int = 1, 
-        stop: int = None, scale: str = "log", *, start_self: int = None, 
-        stop_self: int = None, scale_self: str = None, 
+def calculate_transport_coefficients(
+        time: np.ndarray[float], msd_cross: np.ndarray[float],
+        msd_self: np.ndarray[float], Ns: np.ndarray[int],
+        dimensions: np.ndarray[float], kBT: float, start: int = 1,
+        stop: int = None, scale: str = "log", *, start_self: int = None,
+        stop_self: int = None, scale_self: str = None,
         enforce_linear: bool = True, verbose: bool = False
-    ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+    ) -> tuple[np.ndarray[float], np.ndarray[float], np.ndarray[float]]:
 
     r"""
     Fits the mean squared displacements (MSDs) or the analogous cross
-    displacements (CDs) to evaluate the self-diffusion coefficients 
-    :math:`D_i` and the Onsager transport coefficients :math:`L_{ij}` 
+    displacements (CDs) to evaluate the self-diffusion coefficients
+    :math:`D_i` and the Onsager transport coefficients :math:`L_{ij}`
     and :math:`L_{ii}^\mathrm{self}`.
 
     Parameters
     ----------
     time : `numpy.ndarray`
         Changes in time :math:`t-t_0`.
-        
+
         **Shape**: :math:`(N_t,)`.
 
         **Reference unit**: :math:`\mathrm{ps}`.
 
     msd_cross : `numpy.ndarray`
-        MSDs/CDs for the :math:`N_\mathrm{g}` groups over 
-        :math:`N_\mathrm{b}` blocks of :math:`N_t` trajectory frames 
-        each. Includes the dimensionality scaling factor. 
-        
-        **Shape**: :math:`(_{N_\mathrm{g}+1}\mathrm{C}_{2},\,N_t)` or
-        :math:`(_{N_\mathrm{g}+1}\mathrm{C}_{2},\,N_\mathrm{b},\,N_t)`.
+        MSDs/CDs for the :math:`N_\mathrm{g}` groups over
+        :math:`N_\mathrm{b}` blocks of :math:`N_t` trajectory frames
+        each. Includes the dimensionality scaling factor.
+
+        **Shape**: :math:`(C(N_\mathrm{g}+1,\,2),\,N_t)` or
+        :math:`(C(N_\mathrm{g}+1,\,2),\,N_\mathrm{b},\,N_t)`.
 
         **Reference unit**: :math:`\mathrm{Å}^2`.
 
     msd_self : `numpy.ndarray`
-        Self MSDs for the :math:`N_\mathrm{g}` groups over 
-        :math:`N_\mathrm{b}` blocks of :math:`N_t` trajectory frames 
-        each. Includes the dimensionality scaling factor. 
+        Self MSDs for the :math:`N_\mathrm{g}` groups over
+        :math:`N_\mathrm{b}` blocks of :math:`N_t` trajectory frames
+        each. Includes the dimensionality scaling factor.
 
         **Shape**: :math:`(N_\mathrm{g},\,N_t)` or
         :math:`(N_\mathrm{g},\,N_\mathrm{b},\,N_t)`.
 
         **Reference unit**: :math:`\mathrm{Å}^2`.
 
     Ns : `numpy.ndarray`
-        Number of particles or centers of masses :math:`N` in each 
+        Number of particles or centers of masses :math:`N` in each
         group.
 
-    dims : `numpy.ndarray`
-        System dimensions. 
+    dimensions : `numpy.ndarray`
+        System dimensions.
 
         **Shape**: :math:`(3,)`.
-        
+
         **Reference unit**: :math:`\mathrm{Å}`.
 
     kBT : `float`
-        Thermal energy scale. 
-        
+        Thermal energy scale.
+
         **Reference unit**: :math:`\mathrm{kJ/mol}`.
 
     start : `int`, default: :code:`1`
         Starting frame with respect to the interval used in
         :meth:`Onsager.run` for fitting the MSDs (or their analogs).
 
     stop : `int`, optional
@@ -125,19 +132,19 @@
 
            **Valid values**:
 
            * :code:`"linear"`: Linear :math:`x`- and :math:`y`-axes.
            * :code:`"log"`: Logarithmic :math:`x`- and :math:`y`-axes.
 
     start_self : `int`, keyword-only, optional
-        Starting frame for fitting the self MSDs. If not provided, 
+        Starting frame for fitting the self MSDs. If not provided,
         `start_self` shares a value with `start`.
 
     stop_self : `int`, keyword-only, optional
-        Ending frame for fitting the self MSDs. If not provided, 
+        Ending frame for fitting the self MSDs. If not provided,
         `stop_self` shares a value with `stop`.
 
     scale_self : `str`, keyword-only, optional
         Data scaling for fitting the self MSDs against time. If not
         provided, `scale_self` shares a value with `scale`.
 
         .. container::
@@ -146,46 +153,46 @@
 
            * :code:`"linear"`: Linear :math:`x`- and :math:`y`-axes.
            * :code:`"log"`: Logarithmic :math:`x`- and :math:`y`-axes.
 
     enforce_linear : `bool`, keyword-only, default: :code:`True`
         Enforce linear fits for data on a logarithmic scale by
         setting the slope to :math:`1`, or
-        
-        .. math:: 
-        
+
+        .. math::
+
            \log(\mathrm{MSD})=\log(t)+b
 
     verbose : `bool`, keyword-only, default: :code:`False`
         Determines if detailed progress is shown.
 
     Returns
     -------
     L_ij : `numpy.ndarray`
         Onsager transport coefficients :math:`L_{ij}`.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g},\,N_\mathrm{g})`.
-        
+
         **Reference unit**:
-        :math:`\mathrm{mol/(kJ}\cdot\mathrm{Å}\cdot\mathrm{ps)}`.
+        :math:`\mathrm{mol/(kJ\cdotÅ\cdot\mathrm ps)}`.
 
     L_ii_self : `numpy.ndarray`
-        Self Onsager transport coefficient terms 
+        Self Onsager transport coefficient terms
         :math:`L_{ii}^\mathrm{self}`.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
 
         **Reference unit**:
-        :math:`\mathrm{mol/(kJ}\cdot\mathrm{Å}\cdot\mathrm{ps)}`.
+        :math:`\mathrm{mol/(kJ\cdotÅ\cdot\mathrm ps)}`.
 
     D_i : `numpy.ndarray`
         Self-diffusion coefficients :math:`D_i`.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
-        
+
         **Reference unit**: :math:`\mathrm{Å}/\mathrm{ps)}`.
     """
 
     # Set default settings for fitting self MSDs
     if start_self is None:
         start_self = start
     if stop_self is None:
@@ -193,34 +200,34 @@
     if scale_self is None:
         scale_self = scale
 
     # Preallocate arrays to hold Onsager transport coefficients and
     # self-diffusion coefficients
     ndim = msd_self.ndim
     if ndim not in (2, 3):
-        raise ValueError("The arrays containing the cross- and self-MSDs have "
-                         "invalid shapes.")
+        emsg = ("The arrays containing the cross- and self-MSDs have "
+                "invalid shapes.")
+        raise ValueError(emsg)
     elif ndim == 2:
         n_groups = msd_self.shape[0]
         n_blocks = 1
     elif ndim == 3:
         n_groups, n_blocks = msd_self.shape[:2]
-    L_ij = np.zeros((n_blocks, n_groups, n_groups), dtype=float)
-    D_i = np.zeros((n_blocks, n_groups), dtype=float)
+    L_ij = np.zeros((n_blocks, n_groups, n_groups))
+    D_i = np.zeros((n_blocks, n_groups))
 
     # Get indices of upper-triangular entries in L_ij and D_i
     # arrays
     r_ud, c_ud = np.triu_indices(n_groups)
 
     # Calculate MSD "normalization" factor (kBT * V)
-    denom = kBT * dims.prod()
+    denom = kBT * dimensions[~np.isclose(dimensions, 0)].prod()
 
     # Iterate through all blocks
     for b in ProgressBar(range(n_blocks), verbose=verbose):
-
         # Iterate through all unique group pairings
         for i, msd in enumerate(msd_cross[:, b] / denom):
             y = msd[start:stop]
             valid = np.isfinite(y) & (y > 0)
             y = y[valid]
             x = time[start:stop][valid]
 
@@ -240,21 +247,21 @@
                         if abs(1 - fit[0]) >= 0.01:
                             wmsg = ("The slope for log(MSDc) vs. log(t) fit "
                                     f"is {fit[0]:.6f}.")
                             warnings.warn(wmsg)
                         L_ij[b, r_ud[i], c_ud[i]] = np.exp(fit[1])
             else:
                 L_ij[b, r_ud[i], c_ud[i]] = np.nan
-        
+
         # Mirror the L_ij matrix over the diagonal
         L_ij[b] = L_ij[b] + L_ij[b].T - np.diag(np.diag(L_ij[b]))
 
         # Iterate through all self groups
-        for i, msd_self in enumerate(msd_self[:, b]):
-            y = msd_self[start_self:stop_self]
+        for i, msd in enumerate(msd_self[:, b]):
+            y = msd[start_self:stop_self]
             valid = np.isfinite(y) & (y > 0)
             y = y[valid]
             x = time[start_self:stop_self][valid]
 
             if len(x) > 1:
 
                 # Calculate D_i
@@ -272,577 +279,672 @@
                             wmsg = ("The slope for log(MSD) vs. log(t) fit is "
                                     f"{fit[0]:.6f}!")
                             warnings.warn(wmsg)
                         D_i[b, i] = np.exp(fit[1])
             else:
                 D_i[b, i] = np.nan
 
-        return L_ij, Ns * D_i / denom, D_i
+    return L_ij, Ns * D_i / denom, D_i
 
-def conductivity(
-        L_ij: np.ndarray[float], z: ArrayLike, *, reduced: bool = False
+def calculate_conductivity(
+        L_ij: np.ndarray[float], z: np.ndarray[float], *, reduced: bool = False
     ) -> np.ndarray[float]:
 
     r"""
     Calculates the ionic conductivity :math:`\kappa` using the
     Onsager transport coefficients :math:`L_{ij}`.
 
     Parameters
     ----------
     L_ij : `numpy.ndarray`
         Onsager transport coefficients :math:`L_{ij}` for the atoms or
-        residues in the :math:`N_\mathrm{g}` groups and 
+        residues in the :math:`N_\mathrm{g}` groups and
         :math:`N_\mathrm{b}` trajectory blocks.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g},\,N_\mathrm{g})`.
-        
+
         **Reference unit**:
         :math:`\mathrm{mol/(kJ}\cdot\mathrm{Å}\cdot\mathrm{ps)}`.
-    
+
     z : array-like
         Charge numbers :math:`z_i` of the atoms or residues in the
         :math:`N_\mathrm{g}` groups.
 
         **Shape**: :math:`(N_\mathrm{g},)`.
 
     reduced : `bool`, keyword-only, default: :code:`False`
         Specifies whether the data is in reduced units.
 
     Returns
     -------
-    conductivity : `numpy.ndarray`
-        Conductivities :math:`\kappa` for the atoms or residues in the
-        :math:`N_\mathrm{g}` groups and :math:`N_\mathrm{b}` trajectory
-        blocks.
+    kappas : `numpy.ndarray`
+        Conductivities :math:`\kappa` for the :math:`N_\mathrm{b}`
+        trajectory blocks.
 
-        **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
-        
-        **Reference unit**: :math:`\mathrm{C}^2/(\mathrm{kJ}\cdot 
+        **Shape**: :math:`(N_\mathrm{b},\,)`.
+
+        **Reference unit**: :math:`\mathrm{C}^2/(\mathrm{kJ}\cdot
         \mathrm{Å}\cdot\mathrm{ps})`.
-        
+
         **To SI unit**: :math:`1\times10^{19}\,\mathrm{S}/\mathrm{m}`.
     """
 
-    conductivity = np.einsum("ij, ij", L_ij, z * z[:, None])
+    kappas = np.einsum("bij,ij->b", L_ij, z * z[:, None])
     if not reduced:
-        conductivity *= (unit.AVOGADRO_CONSTANT_NA
-                         * unit.elementary_charge ** 2 * unit.mole
-                         / unit.coulomb ** 2)
-    return conductivity
-
-def electrophoretic_mobility(
-        L_ij: np.ndarray[float], z: ArrayLike, rho: ArrayLike, *,
-        reduced: bool = False) -> np.ndarray[float]:
+        kappas = (kappas * ureg.avogadro_constant
+                  * ureg.elementary_charge ** 2 * ureg.mole
+                  / ureg.coulomb ** 2).to_reduced_units().magnitude
+    return kappas
+
+def calculate_electrophoretic_mobility(
+        L_ij: np.ndarray[float], z: np.ndarray[float], rho: np.ndarray[float],
+        *, reduced: bool = False) -> np.ndarray[float]:
 
     r"""
     Calculates the electrophoretic mobility :math:`\mu_i` of each
     species using the Onsager transport coefficients :math:`L_{ij}`.
 
     Parameters
     ----------
     L_ij : `numpy.ndarray`
         Onsager transport coefficients :math:`L_{ij}` for the atoms or
-        residues in the :math:`N_\mathrm{g}` groups and 
+        residues in the :math:`N_\mathrm{g}` groups and
         :math:`N_\mathrm{b}` trajectory blocks.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g},\,N_\mathrm{g})`.
-        
+
         **Reference unit**:
         :math:`\mathrm{mol/(kJ}\cdot\mathrm{Å}\cdot\mathrm{ps)}`.
 
     z : array-like
         Charge numbers :math:`z_i` of the atoms or residues in the
         :math:`N_\mathrm{g}` groups.
 
         **Shape**: :math:`(N_\mathrm{g},)`.
-    
+
     rho : array-like
         Number densities :math:`n_i` of the atoms or residues in the
         :math:`N_\mathrm{g}` groups.
 
         **Shape**: :math:`(N_\mathrm{g},)`.
-        
+
         **Reference unit**: :math:`\mathrm{Å}^{-3}`.
 
     reduced : `bool`, keyword-only, default: :code:`False`
         Specifies whether the data is in reduced units.
 
     Returns
     -------
-    electrophoretic_mobility : `numpy.ndarray`
-        Electrophoretic mobilities :math:`\mu_i` for the atoms or 
-        residues in the :math:`N_\mathrm{g}` groups and 
+    mus : `numpy.ndarray`
+        Electrophoretic mobilities :math:`\mu_i` for the atoms or
+        residues in the :math:`N_\mathrm{g}` groups and
         :math:`N_\mathrm{b}` trajectory blocks.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
-        
+
         **Reference unit**:
         :math:`\mathrm{Å}^2\cdot\mathrm{C/(kJ}\cdot\mathrm{ps)}`.
-        
+
         **To SI unit**: :math:`1\times 10^{-11}\,\mathrm{m}^2 /
         (\mathrm{V}\cdot\mathrm{s})`.
     """
 
-    mobility = (L_ij * z / rho[:, None]).sum(axis=1)
+    mus = (L_ij * z / rho[:, None]).sum(axis=-1)
     if not reduced:
-        mobility *= (unit.AVOGADRO_CONSTANT_NA * unit.elementary_charge
-                     * unit.mole / unit.coulomb)
-    return mobility
+        mus = (mus * ureg.avogadro_constant * ureg.elementary_charge
+               * ureg.mole / ureg.coulomb).to_reduced_units().magnitude
+    return mus
 
-def transference_number(
-        L_ij: np.ndarray[float], z: ArrayLike) -> np.ndarray[float]:
+def calculate_transference_number(
+        L_ij: np.ndarray[float], z: np.ndarray[float]) -> np.ndarray[float]:
 
     r"""
     Calculates the transference number :math:`t_i` of each species using
     the Onsager transport coefficients :math:`L_{ij}`.
 
     Parameters
     ----------
     L_ij : `numpy.ndarray`
         Onsager transport coefficients :math:`L_{ij}` for the atoms or
-        residues in the :math:`N_\mathrm{g}` groups and 
+        residues in the :math:`N_\mathrm{g}` groups and
         :math:`N_\mathrm{b}` trajectory blocks.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g},\,N_\mathrm{g})`.
-        
+
         **Reference unit**:
         :math:`\mathrm{mol/(kJ}\cdot\mathrm{Å}\cdot\mathrm{ps)}`.
 
     z : array-like
         Charge numbers :math:`z_i` of the atoms or residues in the
         :math:`N_\mathrm{g}` groups.
 
         **Shape**: :math:`(N_\mathrm{g},)`.
 
     Returns
     -------
-    transference_number : `numpy.ndarray`
+    ts : `numpy.ndarray`
         Transference numbers :math:`t_i` for the atoms or residues in
-        the :math:`N_\mathrm{g}` groups and :math:`N_\mathrm{b}` 
+        the :math:`N_\mathrm{g}` groups and :math:`N_\mathrm{b}`
         trajectory blocks.
 
         **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
     """
 
-    return (z * (L_ij * z).sum(axis=1) /
-            np.einsum("ij, ij", L_ij, z * z[:, None]))
+    s = z * (L_ij * z).sum(axis=-1)
+    return s / s.sum(axis=-1)
 
 class Onsager(SerialAnalysisBase):
 
-    r"""
-    A serial implementation to calculate the Onsager transport 
+    """
+    A serial implementation to calculate the Onsager transport
     coefficients and its related properties.
 
-    The Onsager transport framework [1]_ can be used to analyze 
-    transport properties in bulk constant-volume fluids and 
-    electrolytic systems, such as those in the canonical 
+    .. note::
+
+       The simulation must have been run with a constant timestep
+       :math:`\\Delta t` and the frames to be analyzed must be evenly
+       spaced and proceed forward in time for this analysis module to
+       function correctly.
+
+    The Onsager transport framework [1]_ can be used to analyze
+    transport properties in bulk constant-volume fluids and
+    electrolytic systems, such as those in the canonical
     (:math:`NVT`), microcanonical (:math:`NVE`), and grand
-    canonical (:math:`\mu VT`) ensembles.
-    
+    canonical (:math:`\\mu VT`) ensembles.
+
     The Onsager transport equation
 
     .. math::
 
-       \pmb{J}_i=-\sum_j L_{ij}\nabla\bar{\mu}_j
+       \\pmb{J}_i=-\\sum_j L_{ij}\\nabla\\bar{\\mu}_j
 
-    relates the flux :math:`\pmb{J}_i` of species :math:`i` to the
+    relates the flux :math:`\\pmb{J}_i` of species :math:`i` to the
     Onsager transport coefficients :math:`L_{ij}` and the
-    electrochemical potential :math:`\bar{\mu}_j` of species :math:`j`.
-    There is an Onsager transport coefficient for each pair of species
-    that, unlike the Nernst–Einstein equation, captures the strong 
-    cross-correlations in electrolytes.
+    electrochemical potential :math:`\\bar{\\mu}_j` of species
+    :math:`j`. There is an Onsager transport coefficient for each pair
+    of species that, unlike the Nernst–Einstein equation, captures the
+    strong cross-correlations in electrolytes.
 
     The Onsager transport coefficients can be calculated from the
     particle positions over time using the Einstein relation
 
     .. math::
 
-       L_{ij}=\frac{1}{6k_\mathrm{B}TV}
-       \lim_{t\rightarrow\infty}\frac{d}{dt}\left\langle\sum_\alpha
-       \left[\pmb{r}_{i,\alpha}(t)-\pmb{r}_{i,\alpha}(0)\right]\cdot
-       \sum_\beta\left[\pmb{r}_{j,\beta}(t)-\pmb{r}_{j,\beta}(0)\right]
-       \right\rangle
+       L_{ij}=\\frac{1}{6k_\\mathrm{B}TV}
+       \\lim_{t\\rightarrow\\infty}\\frac{d}{dt}\\left\\langle\\sum_\\alpha
+       \\left[\\pmb{r}_{i,\\alpha}(t)-\\pmb{r}_{i,\\alpha}(0)\\right]
+       \\cdot\\sum_\\beta\\left[\\pmb{r}_{j,\\beta}(t)
+       -\\pmb{r}_{j,\\beta}(0)\\right]\\right\\rangle
 
-    where :math:`k_\mathrm{B}` is the Boltzmann constant, :math:`T` is
+    where :math:`k_\\mathrm{B}` is the Boltzmann constant, :math:`T` is
     the system temperature, :math:`V` is the system volume, :math:`t` is
-    time, and :math:`\pmb{r}_\alpha` and :math:`\pmb{r}_\beta` are the 
-    positions of particles :math:`\alpha` and :math:`\beta` belonging to
-    species :math:`i` and :math:`j`, respectively. The angular brackets
-    denote the ensemble average. It is evident that 
+    time, and :math:`\\pmb{r}_\\alpha` and :math:`\\pmb{r}_\\beta` are
+    the positions of particles :math:`\\alpha` and :math:`\\beta`
+    belonging to species :math:`i` and :math:`j`, respectively. The
+    angular brackets denote the ensemble average. It is evident that
     :math:`L_{ij}=L_{ji}`; hence, the equation above is an Onsager
     reciprocal relation.
 
     The diagonal terms :math:`L_{ii}` in the matrix of Onsager transport
     coefficients captures the self-diffusion and self-correlations for
     a single species :math:`i` and has two contributions:
 
     .. math::
 
-       L_{ii}=L_{ii}^\mathrm{self}+L_{ii}^\mathrm{distinct}
+       L_{ii}=L_{ii}^\\mathrm{self}+L_{ii}^\\mathrm{distinct}
 
     The self term
 
     .. math::
 
-       L_{ii}^\mathrm{self}=\frac{1}{6k_\mathrm{B}TV} 
-       \lim_{t\rightarrow\infty}\frac{d}{dt} 
-       \sum_\alpha\left\langle\left[ 
-       \pmb{r}_{i,\alpha}(t)-\pmb{r}_{i,\alpha}(0) 
-       \right]^2\right\rangle
+       L_{ii}^\\mathrm{self}=\\frac{1}{6k_\\mathrm{B}TV}
+       \\lim_{t\\rightarrow\\infty}\\frac{d}{dt}
+       \\sum_\\alpha\\left\\langle\\left[
+       \\pmb{r}_{i,\\alpha}(t)-\\pmb{r}_{i,\\alpha}(0)
+       \\right]^2\\right\\rangle
 
     is given by the autocorrelation function of the flux of a single
-    particle :math:`\alpha` when :math:`\alpha=\beta`, while the 
+    particle :math:`\\alpha` when :math:`\\alpha=\\beta`, while the
     distinct term
-    
+
     .. math::
 
-       L_{ii}^\mathrm{self}=\frac{1}{6k_\mathrm{B}TV} 
-       \lim_{t\rightarrow\infty}\frac{d}{dt} 
-       \sum_\alpha\sum_{\beta\neq\alpha}\left\langle\left[ 
-       \pmb{r}_{i,\alpha}(t)-\pmb{r}_{i,\alpha}(0)\right]\cdot 
-       \left[\pmb{r}_{i,\beta}(t)-\pmb{r}_{i,\beta}(0)\right] 
-       \right\rangle
-    
+       L_{ii}^\\mathrm{self}=\\frac{1}{6k_\\mathrm{B}TV}
+       \\lim_{t\\rightarrow\\infty}\\frac{d}{dt}
+       \\sum_\\alpha\\sum_{\\beta\\neq\\alpha}\\left\\langle\\left[
+       \\pmb{r}_{i,\\alpha}(t)-\\pmb{r}_{i,\\alpha}(0)\\right]\\cdot
+       \\left[\\pmb{r}_{i,\\beta}(t)-\\pmb{r}_{i,\\beta}(0)\\right]
+       \\right\\rangle
+
     is given by the cross-correlation between two distinct particles
-    when :math:`\alpha\neq\beta`. Naturally, the self term is
+    when :math:`\\alpha\\neq\\beta`. Naturally, the self term is
     related to the self-diffusion coefficient :math:`D_i` via
 
     .. math::
 
-       L_{ii}^\mathrm{self}=\frac{D_i\rho_i}{k_\mathrm{B}T}
+       L_{ii}^\\mathrm{self}=\\frac{D_i\\rho_i}{k_\\mathrm{B}T}
 
-    where :math:`\rho_i` is the number density of species :math:`i`.
+    where :math:`\\rho_i` is the number density of species :math:`i`.
 
-    Finally, the Onsager transport coefficients can be used to 
+    Finally, the Onsager transport coefficients can be used to
     obtain experimentally relevant transport properties:
 
     * Ionic conductivity:
 
       .. math::
 
-         \kappa=F^2\sum_i\sum_j z_iz_jL_{ij}
-        
+         \\kappa=F^2\\sum_i\\sum_j z_iz_jL_{ij}
+
       :math:`F` is the Faraday constant.
 
     * Electrophoretic mobility:
 
       .. math::
 
-         \mu_i=\frac{F}{\rho_i}\sum_j z_jL_{ij}
-      
+         \\mu_i=\\frac{F}{\\rho_i}\\sum_j z_jL_{ij}
+
     * Transference number:
 
       .. math::
 
-         t_i=\frac{\sum_j z_iz_jL_{ij}}{\sum_k\sum_l z_kz_lL_{kl}}
+         t_i=\\frac{\\sum_j z_iz_jL_{ij}}{\\sum_k\\sum_l z_kz_lL_{kl}}
 
     Parameters
     ----------
     groups : `MDAnalysis.AtomGroup` or array-like
         Group(s) of atoms for which the mean squared displacements (or
         analogs) are calculated.
 
     groupings : `str` or array-like, default: :code:`"atoms"`
         Determines whether the centers of mass are used in lieu of
         individual atom positions. If `groupings` is a `str`, the same
         value is used for all `groups`.
 
+        .. note::
+
+           In a standard trajectory file, segments (or chains) contain
+           residues (or molecules), and residues contain atoms. This
+           heirarchy must be adhered to for this analysis module to
+           function correctly, unless your selected grouping is always
+           :code:`"atoms"`.
+
         .. container::
 
            **Valid values**:
 
-           * :code:`"atoms"`: Atom positions (generally for 
+           * :code:`"atoms"`: Atom positions (generally for
              coarse-grained simulations).
-           * :code:`"residues"`: Residues' centers of mass (for 
+           * :code:`"residues"`: Residues' centers of mass (for
              atomistic simulations).
-           * :code:`"segments"`: Segments' centers of mass (for 
+           * :code:`"segments"`: Segments' centers of mass (for
              atomistic polymer simulations).
 
-    temp : `float` or `openmm.unit.Quantity`, default: :code:`300`
+    temperature : `float`, `openmm.unit.Quantity`, or `pint.Quantity`, \
+    default: :code:`300`
         System temperature :math:`T`.
 
         .. note::
 
-           If :code:`reduced=True`, `temp` should be equal to the energy
-           scale. When the Lennard-Jones potential is used, it generally
-           means that :math:`T^* = 1`, or `temp=1`.
+           If :code:`reduced=True`, `temperature` should be equal to the
+           energy scale. When the Lennard-Jones potential is used, it
+           generally means that :math:`T^* = 1`, or `temperature=1`.
+
+        **Reference unit**: :math:`\\mathrm{K}`.
+
+    charges : array-like, `openmm.unit.Quantity`, or `pint.Quantity`, \
+    keyword-only, optional
+        Charge numbers :math:`z_i` for the specified `groupings` in the
+        :math:`N_\\mathrm{g}` `groups`. If not provided, it will be
+        retrieved from the topology or trajectory.
+
+        **Shape**: :math:`(N_\\mathrm{g},)`.
+
+        **Reference unit**: :math:`\\mathrm{e}`.
+
+    dimensions : array-like, `openmm.unit.Quantity`, or \
+    `pint.Quantity`, keyword-only, optional
+        System dimensions. If not provided, they are retrieved from the
+        topology or trajectory.
+
+        .. tip::
+
+           You can zero out dimensions by setting them to :code:`0` if
+           your simulation is pseudo-1D or pseudo-2D. For example, if
+           you have a one-layer thick slab in the :math:`xy`-plane, you
+           can set :code:`dimensions=np.array((L_x, L_y, 0))` to
+           evaluate the transport properties in 2D. Note that this
+           affects the reference units of the Onsager transport
+           coefficients and its related properties, but not the
+           self-diffusivity.
+
+        **Shape**: :math:`(3,)`.
+
+        **Reference unit**: :math:`\\mathrm{Å}`.
+
+    dt : `float`, `openmm.unit.Quantity`, or `pint.Quantity`, \
+    keyword-only, optional
+        Time between frames :math:`\\Delta t`. While this is normally
+        determined from the trajectory, the trajectory may not have the
+        correct information if the data is in reduced units. For
+        example, if your reduced timestep is :math:`0.01` and you output
+        trajectory data every :math:`10,000` timesteps, then
+        :math:`\\Delta t=100`.
+
+        **Reference unit**: :math:`\\mathrm{ps}`.
 
-        **Reference unit**: :math:`\mathrm{K}`.
- 
     n_blocks : `int`, keyword-only, default: :code:`1`
-        Number of blocks :math:`N_\mathrm{b}` to split the trajectory 
+        Number of blocks :math:`N_\\mathrm{b}` to split the trajectory
         into.
 
     center : `bool`, keyword-only, default: :code:`False`
-        Determines whether the system center of mass is subtracted from 
+        Determines whether the system center of mass is subtracted from
         the positions used to compute the transport properties.
 
-    com_wrap : `bool`, keyword-only, default: :code:`False`
-        Determines whether the system center of mass is computed using 
+    center_atom : `bool`, keyword-only, default: :code:`False`
+        Determines whether the system center of mass is computed using
+        the atom positions, regardless of `groupings`. Has no effect if
+        :code:`center=False`.
+
+    center_wrap : `bool`, keyword-only, default: :code:`False`
+        Determines whether the system center of mass is computed using
         the wrapped particle positions. Has no effect if
         :code:`center=False`.
 
     fft : `bool`, keyword-only, default: :code:`True`
-        Determines whether fast Fourier transforms (FFT) are used to 
+        Determines whether fast Fourier transforms (FFT) are used to
         evaluate the mean squared displacements (or analogs).
 
+    reduced : `bool`, keyword-only, default: :code:`False`
+        Specifies whether the data is in reduced units. Affects
+        `temperature`, `results.times`, etc.
+
     unwrap : `bool`, keyword-only, default: :code:`False`
-        Determines if atom positions are unwrapped. Ensure that 
+        Determines if atom positions are unwrapped. Ensure that
         :code:`unwrap=False` when the trajectory already contains
         unwrapped particle positions, as this parameter is used in
-        conjunction with `com_wrap` to determine the appropriate
+        conjunction with `center_wrap` to determine the appropriate
         system center of mass.
 
-    reduced : `bool`, keyword-only, default: :code:`False`
-        Specifies whether the data is in reduced units. Affects `temp`,
-        `results.time`, etc.
-    
-    dt : `float` or `openmm.unit.Quantity`, keyword-only, optional
-        Time between frames :math:`\Delta t`. While this is normally
-        determined from the trajectory, the trajectory may not have the
-        correct information if the data is in reduced units. For
-        example, if your reduced timestep is :math:`0.01` and you output
-        trajectory data every :math:`10000` timesteps, then
-        :math:`\Delta t = 100`. 
-        
-        **Reference unit**: :math:`\mathrm{ps}`.
-
     verbose : `bool`, keyword-only, default: :code:`True`
         Determines whether detailed progress is shown.
 
     **kwargs
         Additional keyword arguments to pass to
         :class:`MDAnalysis.analysis.base.AnalysisBase`.
-    
+
     Attributes
     ----------
     universe : `MDAnalysis.Universe`
         :class:`MDAnalysis.core.universe.Universe` object containing all
         information describing the system.
-    
+
+    results.units : `dict`
+        Reference units for the results. For example, to get the
+        reference units for :code:`results.times`, call
+        :code:`results.units["results.times"]`.
+
     results.pairs : `tuple`
         All unique pairs of indices of the groups of atoms in `groups`.
         The ordering coincides with the column indices in
         `results.msd`.
 
-    results.units : `dict`
-        Reference units for the results. For example, to get the 
-        reference units for :code:`results.time`, call 
-        :code:`results.units["results.time"]`. Only available if OpenMM
-        is installed.
-
-    results.time : `numpy.ndarray`
+    results.times : `numpy.ndarray`
         Changes in time :math:`t-t_0`.
 
         **Shape**: :math:`(N_t,)`.
 
-        **Reference unit**: :math:`\mathrm{ps}`.
+        **Reference unit**: :math:`\\mathrm{ps}`.
 
     results.msd_cross : `numpy.ndarray`
-        MSDs (or analogs) for the :math:`N_\mathrm{g}` groups over 
-        :math:`N_\mathrm{b}` blocks of :math:`N_t` trajectory frames 
-        each. Includes the dimensionality scaling factor. See Notes 
+        MSDs (or analogs) for the :math:`N_\\mathrm{g}` groups over
+        :math:`N_\\mathrm{b}` blocks of :math:`N_t` trajectory frames
+        each. Includes the dimensionality scaling factor. See Notes
         about what this value actually means.
 
-        **Shape**: 
-        :math:`(_{N_\mathrm{g}+1}\mathrm{C}_{2},\,N_\mathrm{b},\,N_t)`.
+        **Shape**:
+        :math:`(_{N_\\mathrm{g}+1}\\mathrm{C}_{2},\\,N_\\mathrm{b},\\,
+        N_t)`.
 
-        **Reference unit**: :math:`\mathrm{Å}^2`.
+        **Reference unit**: :math:`\\mathrm{Å}^2`.
 
     results.msd_self : `numpy.ndarray`
-        Self MSDs (or analogs) for the :math:`N_\mathrm{g}` groups over
-        :math:`N_\mathrm{b}` blocks of :math:`N_t` trajectory frames 
+        Self MSDs (or analogs) for the :math:`N_\\mathrm{g}` groups over
+        :math:`N_\\mathrm{b}` blocks of :math:`N_t` trajectory frames
         each. Includes the dimensionality scaling factor. See Notes
         about what this value actually means.
 
-        **Shape**: :math:`(N_\mathrm{g},\,N_\mathrm{b},\,N_t)`.
+        **Shape**: :math:`(N_\\mathrm{g},\\,N_\\mathrm{b},\\,N_t)`.
 
-        **Reference unit**: :math:`\mathrm{Å}^2`.
+        **Reference unit**: :math:`\\mathrm{Å}^2`.
 
     results.L_ij : `numpy.ndarray`
         Onsager transport coefficients :math:`L_{ij}`. Only available
-        after running :meth:`calculate_coefficients`.
+        after running :meth:`calculate_transport_coefficients`.
+
+        **Shape**:
+        :math:`(N_\\mathrm{b},\\,N_\\mathrm{g},\\,N_\\mathrm{g})`.
 
-        **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g},\,N_\mathrm{g})`.
-        
         **Reference unit**:
-        :math:`\mathrm{mol/(kJ}\cdot\mathrm{Å}\cdot\mathrm{ps)}`.
+        :math:`\\mathrm{mol/(kJ}\\cdot\\mathrm{Å}\\cdot\\mathrm{ps)}`.
 
     results.L_ii_self : `numpy.ndarray`
-        Self Onsager transport coefficient terms 
-        :math:`L_{ii}^\mathrm{self}`. Note that
-        :math:`L_{ii}^\mathrm{self}` is related to :math:`D_i` via
+        Self Onsager transport coefficient terms
+        :math:`L_{ii}^\\mathrm{self}`. Note that
+        :math:`L_{ii}^\\mathrm{self}` is related to :math:`D_i` via
 
         .. math::
 
-            L_{ii}^\mathrm{self}=\dfrac{N}{k_\mathrm{B}TV}D_i
+            L_{ii}^\\mathrm{self}=\\dfrac{N}{k_\\mathrm{B}TV}D_i
 
-        Only available after running :meth:`calculate_coefficients`.
+        Only available after running
+        :meth:`calculate_transport_coefficients`.
 
-        **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
+        **Shape**: :math:`(N_\\mathrm{b},\\,N_\\mathrm{g})`.
 
         **Reference unit**:
-        :math:`\mathrm{mol/(kJ}\cdot\mathrm{Å}\cdot\mathrm{ps)}`.
+        :math:`\\mathrm{mol/(kJ}\\cdot\\mathrm{Å}\\cdot\\mathrm{ps)}`.
 
     results.D_i : `numpy.ndarray`
         Self-diffusion coefficients :math:`D_i`. Only available after
-        running :meth:`calculate_coefficients`.
+        running :meth:`calculate_transport_coefficients`.
 
-        **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
-        
-        **Reference unit**: :math:`\mathrm{Å}^2/\mathrm{ps)}`.
+        **Shape**: :math:`(N_\\mathrm{b},\\,N_\\mathrm{g})`.
 
-    results.conductivity : `numpy.ndarray`
-        Conductivities :math:`\kappa`. Only available after running
-        :meth:`calculate_conductivity`. 
-        
-        **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
-        
-        **Reference unit**: :math:`\mathrm{C}^2/(\mathrm{kJ}\cdot 
-        \mathrm{Å}\cdot\mathrm{ps})`.
-        
-        **To SI unit**: :math:`1\times10^{19}\,\mathrm{S}/\mathrm{m}`.
-    
-    results.electrophoretic_mobility : `numpy.ndarray`
-        Electrophoretic mobilities :math:`\mu_i`. Only available after 
+        **Reference unit**: :math:`\\mathrm{Å}^2/\\mathrm{ps)}`.
+
+    results.conductivities : `numpy.ndarray`
+        Conductivities :math:`\\kappa`. Only available after running
+        :meth:`calculate_conductivity`.
+
+        **Shape**: :math:`(N_\\mathrm{b},\\,N_\\mathrm{g})`.
+
+        **Reference unit**: :math:`\\mathrm{C}^2/(\\mathrm{kJ}\\cdot
+        \\mathrm{Å}\\cdot\\mathrm{ps})`.
+
+        **To SI unit**: :math:`1\times10^{19}\\,\\mathrm{S}/\\mathrm{m}`.
+
+    results.electrophoretic_mobilities : `numpy.ndarray`
+        Electrophoretic mobilities :math:`\\mu_i`. Only available after
         running :meth:`calculate_electrophoretic_mobility`.
 
-        **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
-        
+        **Shape**: :math:`(N_\\mathrm{b},\\,N_\\mathrm{g})`.
+
         **Reference unit**:
-        :math:`\mathrm{Å}^2\cdot\mathrm{C/(kJ}\cdot\mathrm{ps)}`.
-        
-        **To SI unit**: :math:`1\times10^{-11}\,\mathrm{m}^2/
-        (\mathrm{V}\cdot\mathrm{s})`.
+        :math:`\\mathrm{Å}^2\\cdot\\mathrm{C/(kJ}\\cdot\\mathrm{ps)}`.
 
-    results.transference_number : `numpy.ndarray`
+        **To SI unit**: :math:`1\times10^{-11}\\,\\mathrm{m}^2/
+        (\\mathrm{V}\\cdot\\mathrm{s})`.
+
+    results.transference_numbers : `numpy.ndarray`
         Transference numbers :math:`t_i`. Only available after running
         :meth:`calculate_transference_number`.
 
-        **Shape**: :math:`(N_\mathrm{b},\,N_\mathrm{g})`.
+        **Shape**: :math:`(N_\\mathrm{b},\\,N_\\mathrm{g})`.
 
     Notes
     -----
-    * In a standard trajectory file, segments (or chains) contain
-      residues, and residues contain atoms. This heirarchy must be
-      adhered to for this analysis module to function correctly.
-
     * The values in `results.msd_cross` are actually "summed squared
       displacements"—that is, `results.msd_cross` contains the sum of
-      all particles' squared displacements instead of their average. 
+      all particles' squared displacements instead of their average.
       However, it is extremely unlikely the raw values in
       `results.msd_cross` will be used other than to calculate the
       Onsager transport coefficients. On the other hand,
       `results.msd_self` is averaged over all particles. Therefore, it
-      can be plotted against `results.time` to get the self-diffusion
+      can be plotted against `results.times` to get the self-diffusion
       coefficients.
 
     References
     ----------
     .. [1] Fong, K. D.; Self, J.; McCloskey, B. D.; Persson, K. A.
        Onsager Transport Coefficients and Transference Numbers in
        Polyelectrolyte Solutions and Polymerized Ionic Liquids.
        *Macromolecules* **2020**, **53** (21), 9503–9512.
        https://doi.org/10.1021/acs.macromol.0c02001.
     """
 
-    _GROUPINGS = {"atoms", "residues", "segments"}
-
     def __init__(
-            self, groups: Union[mda.AtomGroup, ArrayLike],
-            groupings: Union[str, ArrayLike] = "atoms",
-            temp: Union[float, unit.Quantity] = 300, *, n_blocks: int = 1,
-            center: bool = False, com_wrap: bool = False, 
-            dt: Union[float, unit.Quantity] = None, fft: bool = True, 
-            reduced: bool = False, unwrap: bool = False, verbose: bool = True,
-            **kwargs) -> None:
-        
+            self, groups: Union[mda.AtomGroup, tuple[mda.AtomGroup]],
+            groupings: Union[str, tuple[str]] = "atoms",
+            temperature: Union[float, "unit.Quantity", Q_] = 300, *,
+            charges: Union[np.ndarray[float], "unit.Quantity", Q_] = None,
+            dimensions: Union[np.ndarray[float], "unit.Quantity", Q_] = None,
+            dt: Union[float, "unit.Quantity", Q_] = None,
+            n_blocks: int = 1, center: bool = False, center_atom: bool = False,
+            center_wrap: bool = False, fft: bool = True, reduced: bool = False,
+            unwrap: bool = False, verbose: bool = True, **kwargs) -> None:
+
         self._groups = [groups] if isinstance(groups, mda.AtomGroup) else groups
         self.universe = self._groups[0].universe
         super().__init__(self.universe.trajectory, verbose=verbose, **kwargs)
-        if self.universe.dimensions is None:
-            self._dims = None
-        else:
-            self._dims = self.universe.dimensions[:3].copy()
 
         self._n_groups = len(self._groups)
         if isinstance(groupings, str):
-            if groupings not in self._GROUPINGS:
-                emsg = (f"Invalid grouping '{groupings}'. The options are "
-                        "'atoms', 'residues', and 'segments'.")
+            if groupings not in (GROUPINGS := {"atoms", "residues",
+                                               "segments"}):
+                emsg = (f"Invalid grouping '{groupings}'. Valid values: "
+                        f"{', '.join(GROUPINGS)}.")
                 raise ValueError(emsg)
             self._groupings = self._n_groups * [groupings]
         else:
             if self._n_groups != len(groupings):
                 emsg = ("The number of grouping values is not equal to the "
                         "number of groups.")
                 raise ValueError(emsg)
             for g in groupings:
-                if g not in self._GROUPINGS:
-                    emsg = (f"Invalid grouping '{g}'. The options are "
-                            "'atoms', 'residues', and 'segments'.")
+                if g not in GROUPINGS:
+                    emsg = (f"Invalid grouping '{g}'. Valid values: "
+                            f"{', '.join(GROUPINGS)}.")
                     raise ValueError(emsg)
             self._groupings = groupings
 
-        self._reduced = reduced
-        if self._reduced:
-            self._kBT = temp
+        temperature, unit_ = strip_unit(temperature, "temperature")
+        if reduced:
+            if not isinstance(unit_, str):
+                emsg = "'temperature' cannot have units when reduced=True."
+                raise TypeError(emsg)
+            self._kBT = temperature
         else:
-            if isinstance(temp, (int, float)):
-                self._kBT = (unit.AVOGADRO_CONSTANT_NA 
-                             * unit.BOLTZMANN_CONSTANT_kB
-                             * temp * unit.kelvin 
-                             / unit.kilojoule_per_mole)
-            else:
-                self._kBT = (unit.AVOGADRO_CONSTANT_NA * unit.BOLTZMANN_CONSTANT_kB
-                             * temp / unit.kilojoule_per_mole)
-            self.results.units = {"_dims": unit.angstrom,
-                                  "_kBT": unit.kilojoule_per_mole}
-        
-        self._n_blocks = n_blocks
-        self._center = center
-        self._com_wrap = com_wrap
-        if dt:
-            self._dt = dt
-            if isinstance(dt, unit.Quantity):
-                self._dt /= unit.picosecond
+            self._kBT = (
+                ureg.avogadro_constant * ureg.boltzmann_constant
+                * temperature * ureg.kelvin
+            ).m_as(self.results.units["_kBT"])
+
+        if dimensions is not None:
+            if len(dimensions) != 3:
+                raise ValueError("'dimensions' must have length 3.")
+            self._dimensions = np.asarray(strip_unit(dimensions, "angstrom")[0])
+        elif self.universe.dimensions is not None:
+            self._dimensions = self.universe.dimensions[:3].copy()
         else:
-            self._dt = self._trajectory.dt
-        self._fft = fft
-        self._unwrap = unwrap
-        self._verbose = verbose
+            raise ValueError("No system dimensions found or provided.")
+
+        self._dt, unit_ = strip_unit(dt or self._trajectory.dt, "picosecond")
+        if reduced and not isinstance(unit_,  str):
+            raise TypeError("'dt' cannot have units when reduced=True.")
 
-        if hasattr(self.universe.atoms, "charges"):
+        if charges is not None:
+            if len(charges) != self._n_groups:
+                emsg = ("The number of group charges is not equal to "
+                        "the number of groups.")
+                raise ValueError(emsg)
+            charges, unit_ = strip_unit(charges, "elementary_charge")
+            if reduced and not isinstance(unit_, str):
+                emsg = "'charges' cannot have units when reduced=True."
+                raise TypeError(emsg)
+            self._charges = np.asarray(charges)
+        elif hasattr(self.universe.atoms, "charges"):
             self._charges = np.fromiter(
-                (getattr(g, gr).charges[0] 
-                 for g, gr in zip(self._groups, self._groupings)), 
+                (getattr(g, gr).charges[0]
+                 for g, gr in zip(self._groups, self._groupings)),
+                count=self._n_groups,
                 dtype=int
             )
         else:
             self._charges = None
-        self._rhos = None
-    
+
+        # Determine the number of particles in each group and their
+        # corresponding indices
+        self._Ns = tuple(getattr(a, f"n_{g}")
+                         for (a, g) in zip(self._groups, self._groupings))
+        self._N = sum(self._Ns)
+        self._slices = []
+        index = 0
+        for N in self._Ns:
+            self._slices.append(slice(index, index + N))
+            index += N
+
+        if np.all(~np.isclose(self._dimensions, 0)):
+            self._rhos = np.fromiter(
+                (getattr(g, f"n_{gr}")
+                for g, gr in zip(self._groups, self._groupings)),
+                count=self._n_groups,
+                dtype=float
+            ) / self._dimensions.prod()
+
+        self._n_blocks = n_blocks
+        self._center = center
+        self._center_atom = center_atom
+        self._center_wrap = center_wrap
+        self._fft = fft
+        self._reduced = reduced
+        self._unwrap = unwrap
+        self._verbose = verbose
+
     def _prepare(self) -> None:
 
+        # Ensure frames are evenly spaced and proceed forward in time
+        if hasattr(self._sliced_trajectory, "frames"):
+            df = np.diff(self._sliced_trajectory.frames)
+            if df[0] <= 0 or not np.allclose(df, df[0]):
+                emsg = ("The selected frames must be evenly spaced and "
+                        "proceed forward in time.")
+                raise ValueError(emsg)
+        elif hasattr(self._sliced_trajectory, "step") \
+                and self._sliced_trajectory.step <= 0:
+            raise ValueError("The analysis must proceed forward in time.")
+
         # Find all unique AtomGroup combinations
         self.results.pairs = tuple(
             itertools.combinations_with_replacement(range(self._n_groups), 2)
         )
 
-        # Preallocate array(s) to store positions (and number of
-        # boundary crossings) for each AtomGroup
-        self._Ns = tuple(getattr(a, f"n_{g}")
-                         for (a, g) in zip(self._groups, self._groupings))
-        self._positions = [np.empty((self.n_frames, N, 3), dtype=float)
-                           for N in self._Ns]
+        # Preallocate arrays to store positions and number of boundary
+        # crossings
+        self._positions = np.empty((self.n_frames, self._N, 3))
         if self._unwrap:
-            self._trajectory[self.start]
+            self.universe.trajectory[
+                self._sliced_trajectory.frames[0]
+                if hasattr(self._sliced_trajectory, "frames")
+                else (self.start or 0)
+            ]
+            for f in self.universe.atoms.fragments:
+                make_whole(f)
             self._positions_old = self.universe.atoms.positions
             self._images = np.zeros((self.universe.atoms.n_atoms, 3), dtype=int)
-            self._threshold = self._dims / 2
+            self._thresholds = self._dimensions / 2
 
         # Determine number of frames used when the trajectory is split
         # into blocks
         self._n_frames_block = self.n_frames // self._n_blocks
         self._n_frames = self._n_blocks * self._n_frames_block
         extra_frames = self.n_frames - self._n_frames
         if extra_frames > 0:
@@ -851,127 +953,120 @@
                     "discarded. To maximize performance, set appropriate "
                     "starting and ending frames in run() so that the number "
                     "of frames to be analyzed is divisible by the number of "
                     "blocks.")
             warnings.warn(wmsg)
 
         # Preallocate arrays to store results
-        self.results.time = self.step * self._dt * np.arange(self._n_frames //
-                                                             self._n_blocks)
+        self.results.times = self.step * self._dt * np.arange(self._n_frames //
+                                                              self._n_blocks)
         self.results.msd_cross = np.empty(
-            (len(self.results.pairs), self._n_blocks, self._n_frames_block), 
+            (len(self.results.pairs), self._n_blocks, self._n_frames_block),
             dtype=float
         )
         self.results.msd_self = np.empty(
-            (self._n_groups, self._n_blocks, self._n_frames_block), 
+            (self._n_groups, self._n_blocks, self._n_frames_block),
             dtype=float
         )
 
         # Store reference units
-        if not self._reduced:
-            self.results.units["results.time"] = unit.picosecond
-            self.results.units["results.msd_cross"] = unit.angstrom ** 2
-            self.results.units["results.msd_self"] = unit.angstrom ** 2
-    
+        self.results.units = {"results.times": ureg.picosecond}
+        self.results.units["results.msd_cross"] = \
+            self.results.units["results.msd_self"] = ureg.angstrom ** 2
+
     def _single_frame(self) -> None:
 
-        # Unwrap all particle positions, if necessary
         positions = self.universe.atoms.positions.copy()
         if self._unwrap:
-            dpos = positions - self._positions_old
-            mask = np.abs(dpos) >= self._threshold
-            self._images[mask] -= np.sign(dpos[mask]).astype(int)
-            self._positions_old = self.universe.atoms.positions.copy()
-            positions += self._images * self._dims
-
-        for i, (a, g) in enumerate(zip(self._groups, self._groupings)):
-
-            # Store particle or center-of-mass positions
-            self._positions[i][self._frame_index] = (
-                positions[a.indices] if g == "atoms" 
-                else molecule.center_of_mass(
-                    a, grouping=g,
-                    images=self._images[a.indices] if hasattr(self, "_images")
+            unwrap(positions, self._positions_old, self._dimensions,
+                   thresholds=self._thresholds, images=self._images)
+
+        for g, gr, s in zip(self._groups, self._groupings, self._slices):
+            self._positions[self._frame_index, s] = (
+                positions[g.indices] if gr == "atoms"
+                else center_of_mass(
+                    g, gr,
+                    images=self._images[g.indices] if hasattr(self, "_images")
                            else None
                 )
             )
 
+        # Subtract system center-of-mass from particle or molecule
+        # center-of-mass positions
         if self._center:
-
-            # Compute the system center-of-mass using the unwrapped or
-            # wrapped particle positions
-            if self._com_wrap:
-                if self._unwrap:
-                    positions = self.universe.atoms.positions.copy()
+            if self._center_atom:
+                if self._center_wrap:
+                    wrap(positions, self._dimensions)
+                scom = center_of_mass(positions=positions,
+                                      masses=self.universe.atoms.masses)
+            else:
+                if self._center_wrap:
+                    positions = wrap(self._positions[self._frame_index],
+                                     self._dimensions, in_place=False)
                 else:
-                    indices = (positions < 0) | (positions > self._dims)
-                    positions[indices] -= (np.floor(positions / self._dims) 
-                                           * self._dims)[indices]
-            com = molecule.center_of_mass(positions=positions,
-                                          masses=self.universe.atoms.masses)
-            
-            # Subtract system center-of-mass from particle or
-            # center-of-mass positions
-            for i in range(self._n_groups):
-                self._positions[i][self._frame_index] -= com
-            
+                    positions = self._positions[self._frame_index]
+                scom = center_of_mass(
+                    positions=positions,
+                    masses=np.concatenate(
+                        [getattr(g, gr).masses
+                         for g, gr in zip(self._groups, self._groupings)]
+                    )
+                )
+            self._positions[self._frame_index] -= scom
+
     def _conclude(self) -> None:
 
         # Truncate the positions array if there are extra frames
         if self.n_frames != self._n_frames:
-            for i, pos in enumerate(self._positions):
-                self._positions[i] = pos[:self._n_frames]
+            self._positions = self._positions[:self._n_frames]
 
         # Compute the MSDs (or their analogs) for each unique AtomGroup
         # pair
         msd = msd_fft if self._fft else msd_shift
-        for i, (a1, a2) in enumerate(ProgressBar(self.results.pairs,
+        delete_dimensions = np.isclose(self._dimensions, 0)
+        for i, (i1, i2) in enumerate(ProgressBar(self.results.pairs,
                                                  verbose=self._verbose)):
-            if a1 == a2:
-                if self._Ns[a1] and self._Ns[a2]:
-                    pos = self._positions[a1].reshape(
-                        (self._n_blocks, -1, self._Ns[a1], 3)
+            if i1 == i2:
+                if self._Ns[i1]:
+                    positions = self._positions[:, self._slices[i1]].reshape(
+                        (self._n_blocks, -1, self._Ns[i1], 3)
                     )
-                    self.results.msd_cross[i] = msd(pos.sum(axis=2), axis=1)
-                    self.results.msd_self[a1] = (
-                        msd(pos, axis=1, average=False).sum(axis=-1) / 
-                        self._Ns[a1]
+                    positions[:, :, :, delete_dimensions] = 0
+                    self.results.msd_cross[i] = msd(positions.sum(axis=2),
+                                                    axis=1)
+                    self.results.msd_self[i1] = (
+                        msd(positions, axis=1, average=False).sum(axis=-1) /
+                        self._Ns[i1]
                     )
                 else:
-                    self.results.msd_cross[i] = self.results.msd_self[a1] = np.nan
-            elif self._Ns[a1] and self._Ns[a2]:
-                self.results.msd_cross[i] = msd(
-                    self._positions[a1].reshape(
-                        (self._n_blocks, -1, self._Ns[a1], 3)
-                    ).sum(axis=2),
-                    self._positions[a2].reshape(
-                        (self._n_blocks, -1, self._Ns[a2], 3)
-                    ).sum(axis=2),
-                    axis=1
-                )
+                    self.results.msd_cross[i] \
+                        = self.results.msd_self[i1] = np.nan
+            elif self._Ns[i1] and self._Ns[i2]:
+                positions1 = self._positions[:, self._slices[i1]].reshape(
+                    (self._n_blocks, -1, self._Ns[i1], 3)
+                ).sum(axis=2)
+                positions2 = self._positions[:, self._slices[i2]].reshape(
+                    (self._n_blocks, -1, self._Ns[i2], 3)
+                ).sum(axis=2)
+                positions1[:, :, delete_dimensions] \
+                    = positions2[:, :, delete_dimensions] = 0
+                self.results.msd_cross[i] = msd(positions1, positions2, axis=1)
             else:
                 self.results.msd_cross[i] = np.nan
-        
-        # Account for dimensionality by dividing by 2 * n
-        if self._dims is None:
-            d = 6
-            wmsg = ("No system size information found in the "
-                    "trajectory. The simulation box is assumed to be "
-                    "three-dimensional.")
-            warnings.warn(wmsg)
-        else:
-            d = 2 * (~np.isclose(self._dims, 0)).sum()
-        self.results.msd_cross /= d
-        self.results.msd_self /= d
 
-    def calculate_coefficients(
+        # Account for dimensionality by dividing by 2 * D
+        D = 2 * (~delete_dimensions).sum()
+        self.results.msd_cross /= D
+        self.results.msd_self /= D
+
+    def calculate_transport_coefficients(
             self, start: int = 1, stop: int = None, scale: str = "log", *,
             start_self: int = None, stop_self: int = None,
             scale_self: str = None, enforce_linear: bool = True) -> None:
-        
+
         r"""
         Fits the mean squared displacements (MSDs) (or analogs) to
         evaluate the Onsager transport coefficients :math:`L_{ij}` and
         :math:`L_{ii}^\mathrm{self}`.
 
         Parameters
         ----------
@@ -992,20 +1087,20 @@
                **Valid values**:
 
                * :code:`"linear"`: Linear :math:`x`- and :math:`y`-axes.
                * :code:`"log"`: Logarithmic :math:`x`- and :math:`y`-axes.
 
         start_self : `int`, keyword-only, optional
             Starting frame with respect to the interval used in
-            :meth:`Onsager.run` for fitting the self MSDs. If not 
+            :meth:`Onsager.run` for fitting the self MSDs. If not
             provided, `start_self` shares a value with `start`.
 
         stop_self : `int`, keyword-only, optional
             Ending frame with respect to the interval used in
-            :meth:`Onsager.run` for fitting the self MSDs. If not 
+            :meth:`Onsager.run` for fitting the self MSDs. If not
             provided, `stop_self` shares a value with `stop`.
 
         scale_self : `str`, keyword-only, optional
             Data scaling for fitting the self MSDs against time. If not
             provided, `scale_self` shares a value with `scale`.
 
             .. container::
@@ -1014,178 +1109,214 @@
 
                * :code:`"linear"`: Linear :math:`x`- and :math:`y`-axes.
                * :code:`"log"`: Logarithmic :math:`x`- and :math:`y`-axes.
 
         enforce_linear : `bool`, keyword-only, default: :code:`True`
             Enforce linear fits for data on a logarithmic scale by
             setting the slope to :math:`1`, or
-            
+
             .. math::
 
                 \log(\mathrm{MSD})=\log(t)+b
         """
 
-        if self._dims is None:
-            emsg = "No system size information found in the trajectory."
-            raise ValueError(emsg)
-
         if not hasattr(self.results, "msd_cross"):
             emsg = ("Call Onsager.run() before "
-                    "Onsager.calculate_coefficients().")
+                    "Onsager.calculate_transport_coefficients().")
             raise RuntimeError(emsg)
-        
-        self.results.L_ij, self.results.L_ii_self, self.results.D_i = \
-            coefficients(
-                self.results.time, 
-                self.results.msd_cross, self.results.msd_self, 
-                self._Ns, self._dims, self._kBT, 
-                start, stop, scale, 
-                start_self=start_self, 
-                stop_self=stop_self, 
+
+        self.results.L_ij, self.results.L_ii_self, self.results.D_i \
+            = calculate_transport_coefficients(
+                self.results.times,
+                self.results.msd_cross,
+                self.results.msd_self,
+                self._Ns,
+                self._dimensions,
+                self._kBT,
+                start,
+                stop,
+                scale,
+                start_self=start_self,
+                stop_self=stop_self,
                 scale_self=scale_self,
-                enforce_linear=enforce_linear, 
+                enforce_linear=enforce_linear,
                 verbose=self._verbose
             )
 
         # Store reference units
         if not self._reduced:
-            self.results.units["results.D_i"] = (unit.angstrom ** 2 
-                                                 / unit.picosecond)
-            self.results.units["results.L_ii_self"] = \
-            self.results.units["results.L_ij"] = \
-                1 / (unit.kilojoule_per_mole * unit.angstrom * unit.picosecond)
-
-    def calculate_conductivity(self, *, charges: ArrayLike = None) -> None:
+            self.results.units["results.D_i"] = (ureg.angstrom ** 2
+                                                 / ureg.picosecond)
+            self.results.units["results.L_ii_self"] \
+                = self.results.units["results.L_ij"] \
+                = 1 / (ureg.kilojoule * ureg.angstrom * ureg.picosecond
+                       / ureg.mole)
+
+    def calculate_conductivity(
+            self, *,
+            charges: Union[np.ndarray[float], "unit.Quantity", Q_] = None
+        ) -> None:
 
-        r"""
-        Calculates the ionic conductivity :math:`\kappa` using the
+        """
+        Calculates the ionic conductivity :math:`\\kappa` using the
         Onsager transport coefficients :math:`L_{ij}`.
 
         Parameters
         ----------
-        charges : array-like
-            Charge numbers :math:`z_i` of the atoms or residues in the
-            :math:`N_\mathrm{g}` groups. This argument is optional only
+        charges : array-like, `openmm.unit.Quantity`, or \
+        `pint.Quantity`, keyword-only, optional
+            Charge numbers :math:`z_i` of the groupings in the
+            :math:`N_\\mathrm{g}` groups. This argument is optional only
             if `charges` has previously been passed to a calculation
             method belonging to this class.
 
-            **Shape**: :math:`(N_\mathrm{g},)`.
+            **Shape**: :math:`(N_\\mathrm{g},)`.
 
-            **Reference unit**: :math:`\mathrm{e}`.
+            **Reference unit**: :math:`\\mathrm{e}`.
         """
 
         if not hasattr(self.results, "L_ij"):
-            emsg = ("Call Onsager.calculate_coefficients() before "
+            emsg = ("Call Onsager.calculate_transport_coefficients() before "
                     "Onsager.calculate_conductivity().")
             raise RuntimeError(emsg)
 
         if charges is not None:
-            self._charges = charges if isinstance(charges, np.ndarray) \
-                            else np.array(charges)
+            if len(charges) != self._n_groups:
+                emsg = ("The number of group charges is not equal to "
+                        "the number of groups.")
+                raise ValueError(emsg)
+            charges, unit_ = strip_unit(charges, "elementary_charge")
+            if self._reduced and not isinstance(unit_, str):
+                emsg = "'charges' cannot have units when reduced=True."
+                raise TypeError(emsg)
+            self._charges = np.asarray(charges)
         if self._charges is None:
             raise ValueError("No charge number information available.")
-        
-        self.results.conductivity = conductivity(
-            self.results.L_ij.mean(axis=0), self._charges, 
+
+        self.results.conductivities = calculate_conductivity(
+            self.results.L_ij, self._charges,
             reduced=self._reduced
         )
 
-        if not self._reduced:
-            self.results.units["results.conductivity"] = \
-                unit.coulomb ** 2 / (unit.kilojoule * unit.angstrom
-                                     * unit.picosecond)
+        self.results.units["results.conductivities"] = \
+            ureg.coulomb ** 2 / (ureg.kilojoule * ureg.angstrom
+                                 * ureg.picosecond)
 
     def calculate_electrophoretic_mobility(
-            self, *, charges: ArrayLike = None, rhos: ArrayLike = None
+            self, *,
+            charges: Union[np.ndarray[float], "unit.Quantity", Q_] = None,
+            rhos: Union[np.ndarray[float], "unit.Quantity", Q_] = None
         ) -> None:
 
-        r"""
-        Calculates the electrophoretic mobility :math:`\mu_i` of each
+        """
+        Calculates the electrophoretic mobility :math:`\\mu_i` of each
         species using the Onsager transport coefficients :math:`L_{ij}`.
 
         Parameters
         ----------
-        charges : array-like
-            Charge numbers :math:`z_i` of the atoms or residues in the
-            :math:`N_\mathrm{g}` groups. This argument is optional only 
-            if `charges` has previously been passed to a calculation 
+        charges : array-like, `openmm.unit.Quantity`, or \
+        `pint.Quantity`, keyword-only, optional
+            Charge numbers :math:`z_i` of the groupings in the
+            :math:`N_\\mathrm{g}` groups. This argument is optional only
+            if charge information is present in the topology or
+            `charges` has previously been passed to a calculation
             method belonging to this class.
 
-            **Shape**: :math:`(N_\mathrm{g},)`.
+            **Shape**: :math:`(N_\\mathrm{g},)`.
+
+            **Reference unit**: :math:`\\mathrm{e}`.
+
+        rhos : array-like, `openmm.unit.Quantity`, or \
+        `pint.Quantity`, keyword-only, optional
+            Number densities :math:`n_i` of the groupings in the
+            :math:`N_\\mathrm{g}` groups.
+
+            **Shape**: :math:`(N_\\mathrm{g},)`.
 
-            **Reference unit**: :math:`\mathrm{e}`.
-        
-        rhos : array_like, keyword-only, optional
-            Number densities :math:`n_i` of the atoms or residues in the
-            :math:`N_\mathrm{g}` groups. This argument is optional only 
-            if `rhos` has previously been passed to a calculation method
-            belonging to this class. 
-
-            **Shape**: :math:`(N_\mathrm{g},)`.
-            
-            **Reference unit**: :math:`\mathrm{Å}^{-3}`.
+            **Reference unit**: :math:`\\mathrm{Å}^{-3}`.
         """
 
         if not hasattr(self.results, "L_ij"):
-            emsg = ("Call Onsager.calculate_coefficients() before "
+            emsg = ("Call Onsager.calculate_transport_coefficients() before "
                     "Onsager.calculate_electrophoretic_mobility().")
             raise RuntimeError(emsg)
 
         if charges is not None:
-            self._charges = charges if isinstance(charges, np.ndarray) \
-                            else np.array(charges)
+            if len(charges) != self._n_groups:
+                emsg = ("The number of group charges is not equal to "
+                        "the number of groups.")
+                raise ValueError(emsg)
+            charges, unit_ = strip_unit(charges, "elementary_charge")
+            if self._reduced and not isinstance(unit_, str):
+                emsg = "'charges' cannot have units when reduced=True."
+                raise TypeError(emsg)
+            self._charges = np.asarray(charges)
         if self._charges is None:
             raise ValueError("No charge number information available.")
 
         if rhos is not None:
-            if isinstance(rhos, unit.Quantity):
-                self.results.units["_rho"] = rhos.units
-                rhos = rhos.value_in_unit(self.results.units)
-            self._rhos = rhos if isinstance(rhos, np.ndarray) \
-                         else np.array(rhos)
+            if len(rhos) != self._n_groups:
+                emsg = ("The number of group number densities is not "
+                        "equal to the number of groups.")
+                raise ValueError(emsg)
+            rhos, unit_ = strip_unit(rhos, "angstrom**-3")
+            if self._reduced and not isinstance(unit_, str):
+                emsg = "'rhos' cannot have units when reduced=True."
+                raise TypeError(emsg)
+            self._rhos = np.asarray(rhos)
         if self._rhos is None:
             raise ValueError("No number density information available.")
 
-        self.results.mobility = electrophoretic_mobility(
-            self.results.L_ij.mean(axis=0), charges, rhos,
+        self.results.electrophoretic_mobilities = calculate_electrophoretic_mobility(
+            self.results.L_ij, self._charges, self._rhos,
             reduced=self._reduced
         )
-        
-        if not self._reduced:
-            self.results.units["results.mobility"] = \
-                unit.angstrom ** 2 * unit.coulomb / (unit.kilojoule
-                                                     * unit.picosecond)
+
+        self.results.units["results.electrophoretic_mobilities"] = \
+            ureg.angstrom ** 2 * ureg.coulomb / (ureg.kilojoule
+                                                 * ureg.picosecond)
 
     def calculate_transference_number(
-            self, *, charges: ArrayLike = None) -> None:
+            self, *,
+            charges: Union[np.ndarray[float], "unit.Quantity", Q_] = None
+        ) -> None:
 
-        r"""
+        """
         Calculates the transference number of each species using the
         Onsager transport coefficients :math:`L_{ij}`.
 
         Parameters
         ----------
-        charges : array-like
-            Charge numbers :math:`z_i` of the atoms or residues in the
-            :math:`N_\mathrm{g}` groups. This argument is optional only 
-            if `charges` has previously been passed to a calculation 
+        charges : array-like, `openmm.unit.Quantity`, or \
+        `pint.Quantity`, keyword-only, optional
+            Charge numbers :math:`z_i` of the groupings in the
+            :math:`N_\\mathrm{g}` groups. This argument is optional only
+            if charge information is present in the topology or
+            `charges` has previously been passed to a calculation
             method belonging to this class.
 
-            **Shape**: :math:`(N_\mathrm{g},)`.
+            **Shape**: :math:`(N_\\mathrm{g},)`.
 
-            **Reference unit**: :math:`\mathrm{e}`.
+            **Reference unit**: :math:`\\mathrm{e}`.
         """
 
         if not hasattr(self.results, "L_ij"):
-            emsg = ("Call Onsager.calculate_coefficients() before "
+            emsg = ("Call Onsager.calculate_transport_coefficients() before "
                     "Onsager.calculate_transference_number().")
             raise RuntimeError(emsg)
 
         if charges is not None:
-            self._charges = charges if isinstance(charges, np.ndarray) \
-                            else np.array(charges)
+            if len(charges) != self._n_groups:
+                emsg = ("The number of group charges is not equal to "
+                        "the number of groups.")
+                raise ValueError(emsg)
+            charges, unit_ = strip_unit(charges, "elementary_charge")
+            if self._reduced and not isinstance(unit_, str):
+                emsg = "'charges' cannot have units when reduced=True."
+                raise TypeError(emsg)
+            self._charges = np.asarray(charges)
         if self._charges is None:
             raise ValueError("No charge number information available.")
-        
-        self.results.transference_number = transference_number(
-            self.results.L_ij.mean(axis=0), self._charges
+
+        self.results.transference_numbers = calculate_transference_number(
+            self.results.L_ij, self._charges
         )
```

### Comparing `mdhelper-0.0.2/src/mdhelper/fit/distribution.py` & `mdhelper-1.0.0/src/mdhelper/fit/distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 r"""
 Weibull distribution models
 ===========================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 The Weibull distribution is widely used in reliability and life (failure
 rate) data analysis. This module provides the one-, two-, and
 three-parameter Weibull distributions.
 
 The three-parameter Weibull distribution is
 
@@ -42,40 +42,38 @@
     Parameters
     ----------
     x : `numpy.ndarray`
         One-dimensional array containing :math:`x`-values.
 
     a : `float`
         Scale parameter :math:`a`.
-    
+
     b : `float`
         Shape parameter :math:`b`. If specified to be a constant, the
         one-parameter Weibull distribution is used.
-    
-    Other parameters
-    ----------------
-    c : `float`, default: :code:`0`
+
+    c : `float`, keyword-only, default: :code:`0`
         Location parameter :math:`c`. If not specified as a parameter,
         the two-parameter Weibull distribution is used.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
 
     Examples
     --------
     Create a three-parameter Weibull distribution model for fitting.
 
     >>> model = lambda x, a, b, c: weibull(x, a, b, c)
 
     Create a two-parameter Weibull distribution model for fitting.
-    
+
     >>> model = lambda x, a, b: weibull(x, a, b)
 
     Create a one-parameter Weibull distribution model for fitting, with
     :math:`b = 1`.
-    
+
     >>> model = lambda x, a: weibull(x, a, 1)
     """
 
     return a * b * (x - c) ** (b - 1) * np.exp(-a * (x - c) ** b)
```

### Comparing `mdhelper-0.0.2/src/mdhelper/fit/exponential.py` & `mdhelper-1.0.0/src/mdhelper/fit/exponential.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 r"""
 Exponential models
 ==================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 Exponentials are often used when the rate of change of a quantity is
 proportional to the initial amount of the quantity. The general
 exponential model is given by
 
 .. math::
 
@@ -30,39 +30,39 @@
 where :math:`\beta` is the stretching exponent. This expression is
 obtained by inserting a fractional power law into the exponential
 function.
 
 This model is generally meaningful only for :math:`x>0`. The graph of
 :math:`\log{(y)}` vs. :math:`x` is characteristically stretched when
 :math:`0\leq\beta\leq 1` and compressed when :math:`\beta>1` (the latter
-case has less practical importance). When :math:`\beta=1`, the one-term 
-exponential model is recovered. When :math:`\beta=2`, the probability 
+case has less practical importance). When :math:`\beta=1`, the one-term
+exponential model is recovered. When :math:`\beta=2`, the probability
 density function for the normal distribution is obtained.
 """
 
 import numpy as np
 
 def exp(x: np.ndarray, *args: float) -> np.ndarray:
 
     r"""
     General exponential model.
 
     .. math::
 
        y=\sum_{k=1}^na_k\exp{(b_kx)}
-    
+
     Parameters
     ----------
     x : `numpy.ndarray`
         One-dimensional array containing :math:`x`-values.
 
     *args : `float`
         Fitting parameters for the exponential term(s), ordered as
-        :math:`a_1,\,b_1,\,a_2,\,b_2,\ldots,\,a_n,\,b_n`, where 
-        :math:`n` is the number of terms in the model. As such, the 
+        :math:`a_1,\,b_1,\,a_2,\,b_2,\ldots,\,a_n,\,b_n`, where
+        :math:`n` is the number of terms in the model. As such, the
         number of variable positional arguments must be even.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
 
@@ -73,39 +73,42 @@
     exponential model.
 
     >>> from scipy import optimize
     >>> rng = np.random.default_rng()
     >>> x = np.linspace(-0.1, 0.1, 10)
     >>> err = (2 * rng.random(x.shape) - 1) / 10
     >>> y = np.exp(-8 * x) + np.exp(12 * x) + err
-    >>> pk, _ = optimize.curve_fit(lambda x, a1, b1, a2, b2: exp(x, a1, b1, a2, b2), x, y)
+    >>> pk, _ = optimize.curve_fit(
+            lambda x, a1, b1, a2, b2: exp(x, a1, b1, a2, b2), x, y
+        )
     >>> pk
     array([ 1.13072662, -6.90042351,  0.88706719, 12.87854508])
 
     Evaluate the fitted :math:`y`-values using the coefficients.
 
     >>> exp(x, *pk)
     array([2.49915084, 2.25973234, 2.09274413, 2.00061073, 1.98962716,
            2.07080543, 2.26106343, 2.58486089, 3.07642312, 3.78274065])
     """
 
     n = len(args)
-    assert n >= 2 and n % 2 == 0, \
-        "Number of fitting parameters must be greater than 2 and even."
+    if n < 2 or n % 2 != 0:
+        emsg = "Number of fitting parameters must be greater than 2 and even."
+        raise ValueError(emsg)
     return np.exp(args[1::2] * x[:, None]) @ args[::2]
 
 def exp1(x: np.ndarray, a: float, b: float) -> np.ndarray:
 
     r"""
     Convenience function for the :code:`exp1` model from MATLAB.
 
     .. math::
 
        y=a\exp{(bx)}
-    
+
     Parameters
     ----------
     x : `numpy.ndarray`
         One-dimensional array containing :math:`x`-values.
 
     a : `float`
         Coefficient :math:`a` for the :math:`\exp` term.
@@ -126,15 +129,15 @@
 
     r"""
     Convenience function for the :code:`exp2` model from MATLAB.
 
     .. math::
 
        y=a\exp{(bx)}+c\exp{(dx)}
-    
+
     Parameters
     ----------
     x : `numpy.ndarray`
         One-dimensional array containing :math:`x`-values.
 
     a : `float`
         Coefficient :math:`a` for the first :math:`\exp` term.
@@ -154,14 +157,55 @@
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return exp(x, a, b, c, d)
 
+def biexp(
+        x: np.ndarray, y0: float, a: float, b: float, c: float, d: float
+    ) -> np.ndarray:
+
+    r"""
+    Bi-exponential function.
+
+    .. math::
+
+       y=y_0+a\exp{\left(-\frac{x}{b}\right)}+c\exp{\left(-\frac{x}{d}\right)}
+
+    Parameters
+    ----------
+    x : `numpy.ndarray`
+        One-dimensional array containing :math:`x`-values.
+
+    y0 : `float`
+        Offset :math:`y_0`.
+
+    a : `float`
+        Coefficient :math:`a` for the first :math:`\exp` term.
+
+    b : `float`
+        Coefficient :math:`b` for the :math:`x` term in the first
+        :math:`\exp` term.
+
+    c : `float`
+        Coefficient :math:`a` for the second :math:`\exp` term.
+
+    d : `float`
+        Coefficient :math:`b` for the :math:`x` term in the second
+        :math:`\exp` term.
+
+    Returns
+    -------
+    fit : `numpy.ndarray`
+        Fitted :math:`y`-values.
+    """
+
+    return y0 + a * np.exp(-x / b) + c * np.exp(-x / d)
+
 def stretched_exp(x: np.ndarray, alpha: float, beta: float) -> np.ndarray:
 
     r"""
     Stretched exponential function.
 
     .. math::
```

### Comparing `mdhelper-0.0.2/src/mdhelper/fit/fourier.py` & `mdhelper-1.0.0/src/mdhelper/fit/fourier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 r"""
 Fourier series models
 =====================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 The Fourier series is a sum of sine and cosine functions that describes
 a periodic signal, and can be represented in trigonometric form as
 
 .. math::
 
    y=a_0+\sum_{k=1}^na_k\cos{(k\omega x)}+b_k\sin{(k\omega x)}
@@ -28,15 +28,15 @@
 
     r"""
     General Fourier series model.
 
     .. math::
 
        y=a_0+\sum_{k=1}^na_i\cos{(k\omega x)}+b_i\sin{(k\omega x)}
-    
+
     Parameters
     ----------
     x : `numpy.ndarray`
         :math:`x`-values.
 
     omega : `float`
         Fundamental frequency :math:`\omega` of the signal.
@@ -63,15 +63,17 @@
     Fourier series model.
 
     >>> from scipy import optimize
     >>> rng = np.random.default_rng()
     >>> x = np.linspace(0, 5, 20)
     >>> err = (2 * rng.random(x.shape) - 1) / 10
     >>> y = 1 + 2 * np.cos(x / 2) + 3 * np.sin(x / 2) + err
-    >>> pk, _ = optimize.curve_fit(lambda x, omega, a0, a1, b1: fourier(x, omega, a0, a1, b1), x, y)
+    >>> pk, _ = optimize.curve_fit(
+            lambda x, omega, a0, a1, b1: fourier(x, omega, a0, a1, b1), x, y
+        )
     >>> pk
     array([0.51185734, 1.15090712, 1.87471839, 2.87117784])
 
     Evaluate the fitted :math:`y`-values using the coefficients.
 
     >>> fourier(x, *pk)
     array([3.0256255 , 3.39422104, 3.72217562, 4.00354785, 4.23324026,
@@ -116,15 +118,15 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1)
 
 def fourier2(
         x: np.ndarray, a0: float, a1: float, b1: float, a2: float,
         b2: float, omega: float) -> np.ndarray:
 
     r"""
@@ -160,15 +162,15 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1, a2, b2)
 
 def fourier3(
         x: np.ndarray, a0: float, a1: float, b1: float, a2: float,
         b2: float, a3: float, b3: float, omega: float) -> np.ndarray:
 
     r"""
@@ -211,15 +213,15 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1, a2, b2, a3, b3)
 
 def fourier4(
         x: np.ndarray, a0: float, a1: float, b1: float, a2: float,
         b2: float, a3: float, b3: float, a4: float, b4: float, omega: float
     ) -> np.ndarray:
 
@@ -270,15 +272,15 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1, a2, b2, a3, b3, a4, b4)
 
 def fourier5(
         x: np.ndarray, a0: float, a1: float, b1: float, a2: float,
         b2: float, a3: float, b3: float, a4: float, b4: float,
         a5: float, b5: float, omega: float) -> np.ndarray:
 
@@ -334,15 +336,15 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1, a2, b2, a3, b3, a4, b4, a5, b5)
 
 def fourier6(
         x: np.ndarray, a0: float, a1: float, b1: float, a2: float,
         b2: float, a3: float, b3: float, a4: float, b4: float,
         a5: float, b5: float, a6: float, b6: float, omega: float
     ) -> np.ndarray:
@@ -405,15 +407,15 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1, a2, b2, a3, b3, a4, b4, a5, b5,
                    a6, b6)
 
 def fourier7(
         x: np.ndarray, a0: float, a1: float, b1: float, a2: float,
         b2: float, a3: float, b3: float, a4: float, b4: float,
         a5: float, b5: float, a6: float, b6: float, a7: float,
@@ -483,15 +485,15 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1, a2, b2, a3, b3, a4, b4, a5, b5,
                    a6, b6, a7, b7)
 
 def fourier8(
         x: np.ndarray, a0: float, a1: float, b1: float, a2: float,
         b2: float, a3: float, b3: float, a4: float, b4: float,
         a5: float, b5: float, a6: float, b6: float, a7: float,
@@ -567,10 +569,10 @@
         Fundamental frequency :math:`\omega` of the signal.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return fourier(x, omega, a0, a1, b1, a2, b2, a3, b3, a4, b4, a5, b5,
                    a6, b6, a7, b7, a8, b8)
```

### Comparing `mdhelper-0.0.2/src/mdhelper/fit/gaussian.py` & `mdhelper-1.0.0/src/mdhelper/fit/gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 r"""
 Gaussian models
 ===============
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 The Gaussian model fits peaks, and is given by
 
 .. math::
 
    y=\sum_{k=1}^na_k\exp{\left[-\left(\frac{x-b_k}{c_k}\right)^2\right]}
 
 where :math:`a` is the amplitude, :math:`b` is the centroid (location),
 :math:`c` is related to the peak width, and :math:`n` is the number of
 peaks to fit.
 
-This module provides the general Gaussian model above for any number of 
+This module provides the general Gaussian model above for any number of
 terms :math:`k`, as well as convenience functions for Gaussian models
 with :math:`1\leq n\leq8` analogous to MATLAB's :code:`gauss1`,
 :code:`gauss2`, etc.
 """
 
 import numpy as np
 
@@ -65,15 +65,15 @@
 
     Evaluate the fitted :math:`y`-values using the coefficients.
 
     >>> gauss(x, *pk)
     array([0.06157175, 0.19415629, 0.45650326, 0.80031095, 1.04615509,
            1.01966105, 0.74103382, 0.40155281, 0.16224441, 0.04887866])
     """
-    
+
     n = len(args)
     assert n >= 3 and n % 3 == 0, \
         "Number of fitting parameters must be greater than and divisible by 3."
     return np.exp(-((x[:, None] - args[1::3]) / args[2::3]) ** 2) @ args[::3]
 
 def gauss1(x: np.ndarray, a1: float, b1: float, c1: float) -> np.ndarray:
```

### Comparing `mdhelper-0.0.2/src/mdhelper/fit/polynomial.py` & `mdhelper-1.0.0/src/mdhelper/fit/polynomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 r"""
 Polynomial models
 =================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 Polynomial models for curves are given by
 
 .. math::
 
    y=\sum_{k=0}^np_kx^k
 
@@ -30,15 +30,15 @@
 """
 
 import numpy as np
 
 def poly(x: np.ndarray, *args: float) -> np.ndarray:
 
     r"""
-    The general polynomial model is
+    General polynomial model.
 
     .. math::
 
        y=\sum_{k=0}^np_kx^k
 
     Parameters
     ----------
@@ -46,15 +46,15 @@
         One-dimensional array containing :math:`x`-values.
 
     *args : `float`
         Fitting parameters for each :math:`x^k` term, starting with the
         :math:`x^0` term. The number of positional arguments,
         :math:`n+1`, determines the order :math:`n` of the polynomial
         model.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
 
     Examples
     --------
@@ -73,15 +73,15 @@
 
     Evaluate the fitted :math:`y`-values using the coefficients.
 
     >>> poly(x, *pk)
     array([ 0.9883393 , -0.02840946,  0.98225396,  4.02032955,  9.08581731])
     """
 
-    return args @ x ** np.arange(len(args))[:, None]
+    return args @ (x ** np.arange(len(args))[:, None])
 
 def poly1(x: np.ndarray, p1: float, p2: float) -> np.ndarray:
 
     r"""
     Convenience function for the :code:`poly1` model from MATLAB:
 
     .. math::
@@ -94,21 +94,21 @@
         One-dimensional array containing :math:`x`-values.
 
     p1 : `float`
         Coefficient :math:`p_1` for the :math:`x` term.
 
     p2 : `float`
         Constant term :math:`p_2`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
-    
+
     return poly(x, p2, p1)
 
 def poly2(x: np.ndarray, p1: float, p2: float, p3: float) -> np.ndarray:
 
     r"""
     Convenience function for the :code:`poly2` model from MATLAB:
 
@@ -125,15 +125,15 @@
         Coefficient :math:`p_1` for the :math:`x^2` term.
 
     p2 : `float`
         Coefficient :math:`p_2` for the :math:`x` term.
 
     p3 : `float`
         Constant term :math:`p_3`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p3, p2, p1)
@@ -161,15 +161,15 @@
         Coefficient :math:`p_2` for the :math:`x^2` term.
 
     p3 : `float`
         Coefficient :math:`p_3` for the :math:`x` term.
 
     p4 : `float`
         Constant term :math:`p_4`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p4, p3, p2, p1)
@@ -200,15 +200,15 @@
         Coefficient :math:`p_3` for the :math:`x^2` term.
 
     p4 : `float`
         Coefficient :math:`p_4` for the :math:`x` term.
 
     p5 : `float`
         Constant term :math:`p_5`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p5, p4, p3, p2, p1)
@@ -242,15 +242,15 @@
         Coefficient :math:`p_4` for the :math:`x^2` term.
 
     p5 : `float`
         Coefficient :math:`p_5` for the :math:`x` term.
 
     p6 : `float`
         Constant term :math:`p_6`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p6, p5, p4, p3, p2, p1)
@@ -287,15 +287,15 @@
         Coefficient :math:`p_5` for the :math:`x^2` term.
 
     p6 : `float`
         Coefficient :math:`p_6` for the :math:`x` term.
 
     p7 : `float`
         Constant term :math:`p_7`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p7, p6, p5, p4, p3, p2, p1)
@@ -335,15 +335,15 @@
         Coefficient :math:`p_6` for the :math:`x^2` term.
 
     p7 : `float`
         Coefficient :math:`p_7` for the :math:`x` term.
 
     p8 : `float`
         Constant term :math:`p_8`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p8, p7, p6, p5, p4, p3, p2, p1)
@@ -386,15 +386,15 @@
         Coefficient :math:`p_7` for the :math:`x^2` term.
 
     p8 : `float`
         Coefficient :math:`p_8` for the :math:`x` term.
 
     p9 : `float`
         Constant term :math:`p_9`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p9, p8, p7, p6, p5, p4, p3, p2, p1)
@@ -440,15 +440,15 @@
         Coefficient :math:`p_9` for the :math:`x^2` term.
 
     p9 : `float`
         Coefficient :math:`p_9` for the :math:`x` term.
 
     p10 : `float`
         Constant term :math:`p_{10}`.
-    
+
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
 
     return poly(x, p10, p9, p8, p7, p6, p5, p4, p3, p2, p1)
```

### Comparing `mdhelper-0.0.2/src/mdhelper/fit/power.py` & `mdhelper-1.0.0/src/mdhelper/fit/power.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 r"""
 Power models
 ============
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 The power model is given by
 
 .. math::
 
    y=ax^b+c
 
@@ -32,17 +32,15 @@
 
     a : `float`
         Coefficient for the :math:`x^b` term.
 
     b : `float`
         Power constant :math:`b` for the :math:`x^b` term.
 
-    Other parameters
-    ----------------
-    c : `float`
+    c : `float`, keyword-only, default: :code:`0`
         Constant for the :math:`y`-intercept.
 
     Returns
     -------
     fit : `numpy.ndarray`
         Fitted :math:`y`-values.
     """
```

### Comparing `mdhelper-0.0.2/src/mdhelper/openmm/bond.py` & `mdhelper-1.0.0/src/mdhelper/openmm/bond.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,111 @@
 """
 Custom OpenMM bond potentials
 =============================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 This module contains implementations of commonly used bond potentials
 that are not available in OpenMM, such as the finite extension nonlinear
 elastic (FENE) potential. Generally, the bond potentials are named after
 their LAMMPS :code:`bond_style` counterparts, if available.
 """
 
-from typing import Any, Iterable, Union
+from typing import Union
 
 import openmm
 from openmm import unit
 
-from .pair import ljts
+from .pair import wca as pwca
 
 def _setup_bond(
         cbforce: openmm.CustomBondForce,
         global_params: dict[str, Union[float, unit.Quantity]],
-        per_params: Iterable[Any]) -> None:
+        per_params: list[str]) -> None:
+
+    """
+    Sets up a :class:`openmm.CustomBondForce` object.
+
+    Parameters
+    ----------
+    cbforce : `openmm.CustomBondForce`
+        Custom bond force object.
+
+    global_params : `dict`
+        Global parameters.
+
+    per_params : `list`
+        Per-particle parameters.
+    """
 
     for param in global_params.items():
         cbforce.addGlobalParameter(*param)
     for param in per_params:
         cbforce.addPerBondParameter(param)
 
 def fene(
-        globals: dict[str, Union[float, unit.Quantity]] = {},
-        pers: Iterable[str] = ["k", "r0"], wca: bool = True, **kwargs
+        global_args: dict[str, Union[float, unit.Quantity]] = None,
+        wca: bool = True, **kwargs
     ) -> tuple[openmm.CustomBondForce, openmm.CustomNonbondedForce]:
 
     r"""
     Implements the finite extensible nonlinear elastic (FENE) potential
-    used for bead-spring polymer models:
+    used for bead-spring polymer models.
+
+    The potential energy between two bonded particles is given by
 
     .. math::
 
        u_\textrm{FENE}=-\frac{1}{2}k_{12}r_{0,12}^2
        \ln{\left[1-\left(\frac{r_{12}}{r_{0,12}}\right)^2\right]}
        +4\epsilon_{12}\left[\left(\frac{\sigma_{12}}{r_{12}}\right)^{12}
        -\left(\frac{\sigma_{12}}{r_{12}}\right)^6\right]+\epsilon_{12}
 
     where :math:`k_{12}` is the bond coefficient in
     :math:`\textrm{kJ}/(\textrm{nm}^2\cdot\textrm{mol})`,
     :math:`r_{0,12}` is the equilibrium bond length in
-    :math:`\textrm{nm}`, :math:`\sigma_{12}` is the size of the particle
-    in :math:`\textrm{nm}`, and :math:`\epsilon_{12}` is the dispersion
-    energy in :math:`\textrm{kJ/mol}`. :math:`k_{12}`, :math:`r_{0,12}`,
-    :math:`\sigma_{12}` and :math:`\epsilon_{12}` are  determined from 
-    per-particle parameters `k`, `r0`, `sigma` and `epsilon`, 
-    respectively, which are set in the main script using
+    :math:`\textrm{nm}`, :math:`\sigma_{12}` is the average particle
+    size in :math:`\textrm{nm}`, and :math:`\epsilon_{12}` is the
+    dispersion energy in :math:`\textrm{kJ/mol}`. :math:`k_{12}`,
+    :math:`r_{0,12}`, :math:`\sigma_{12}` and :math:`\epsilon_{12}` are
+    determined from per-bond and per-particle parameters `k`, `r0`,
+    `sigma` and `epsilon`, respectively, which are set using
     :meth:`openmm.openmm.CustomBondForce.addBond` and
     :meth:`openmm.openmm.NonbondedForce.addParticle`.
 
     Parameters
     ----------
-    globals : `dict`, optional
-        Additional global parameters for use in the definition of
-        :math:`k_{12}` and :math:`r_{0,12}`.
-
-    pers : `array_like`, optional
-        Additional per-particle parameters for use in the definition of
-        :math:`k_{12}` and :math:`r_{0,12}`.
-
-    wca : `bool`, default: `True`
-        Determines whether the Weeks–Chander–Andersen (WCA) potential is
-        included.
+    global_args : `dict`, optional
+        Constant values :math:`k_{12}` and :math:`r_{0,12}` to use
+        instead of per-bond parameters. The corresponding per-bond
+        parameters will not be registered, but the remaining
+        per-bond parameters will still have to be provided in their
+        default order.
+
+    wca : `bool`, default: :code:`True`
+        Determines whether the Weeks–Chandler–Andersen (WCA) potential
+        is included.
 
     **kwargs
-        Keyword arguments to be passed to 
-        :meth:`mdhelper.openmm.pair.ljts` if :code:`wca=True`.
-    
+        Keyword arguments to be passed to
+        :meth:`mdhelper.openmm.pair.wca` if :code:`wca=True`.
+
     Returns
     -------
     bond_fene : `openmm.CustomBondForce`
         FENE bond potential.
-    
+
     pair_wca : `openmm.CustomNonbondedForce`
         WCA pair potential, if :code:`wca=True`.
     """
 
     bond_fene = openmm.CustomBondForce("-0.5*k*r0^2*log(1-(r/r0)^2)")
-    _setup_bond(bond_fene, globals, pers)
+    per_args = ["k", "r0"]
+    for param in global_args.keys():
+        if param in per_args:
+            per_args.remove(param)
+    _setup_bond(bond_fene, global_args, per_args)
 
     if wca:
-        pair_wca = ljts(wca=wca, **kwargs)
+        pair_wca = pwca(**kwargs)
         return bond_fene, pair_wca
 
     return bond_fene
```

### Comparing `mdhelper-0.0.2/src/mdhelper/openmm/reporter.py` & `mdhelper-1.0.0/src/mdhelper/openmm/reporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Custom OpenMM reporters
 =======================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 This module provides custom optimized OpenMM reporters.
 """
 
 from typing import Union
-import warnings
 
 import numpy as np
 import openmm
 from openmm import app, unit
 
-from .file import FOUND_NETCDF, NetCDFFile
+from .file import NetCDFFile
 
 class NetCDFReporter():
 
     """
     A NetCDF trajectory reporter for OpenMM that can report velocities
     and forces in addition to time and coordinates for all particles in
     the simulation or just a subset.
@@ -27,15 +26,15 @@
     file : `str`
         Filename of NetCDF file to which the data is saved. If `file`
         does not have the :code:`.nc` extension, it will automatically
         be appended.
 
     interval : `int`
         Interval (in timesteps) at which to write frames.
-    
+
     append : `bool`, keyword-only, default: :code:`False`
         If :code:`True`, the existing NetCDF file is opened for data to
         be appended to. If :code:`False`, a new NetCDF file is opened
         (and will clobber an existing file with the same name).
 
     periodic : `bool`, keyword-only, optional
         Specifies whether particle positions should be translated so the
@@ -58,27 +57,17 @@
         are determined from the atoms found in the topology.
     """
 
     def __init__(
             self, file: str, interval: int, append: bool = False,
             periodic: bool = None, *, velocities: bool = False,
             forces: bool = False,
-            subset: Union[slice, np.ndarray, app.Topology] = None) -> None:
+            subset: Union[slice, np.ndarray[int], app.Topology] = None) -> None:
 
-        if not ".nc".endswith(".nc"):
-            file += ".nc"
         self._out = NetCDFFile(file, "a" if append else "w")
-        if not FOUND_NETCDF:
-            wmsg = ("The netCDF4 package was not found, so the NetCDF "
-                    "reporter is falling back on scipy.io.netcdf_file. "
-                    "netCDF4 writes NetCDF files significantly faster than "
-                    "scipy.io.netcdf_file and can make a huge difference when "
-                    "used as an OpenMM trajectory reporter. Consider "
-                    "installing netCDF4 via pip or Conda if possible.")
-            warnings.warn(wmsg)
         self._interval = interval
         self._periodic = periodic
         self._subset = np.fromiter((a.index for a in subset.atoms()), dtype=int) \
                        if isinstance(subset, app.Topology) else subset
         self._velocities = velocities
         self._forces = forces
 
@@ -105,15 +94,15 @@
                A six-element tuple containing
 
                1. the number of steps until the next report,
                2. whether the report will require coordinates,
                3. whether the report will require velocities,
                4. whether the report will require forces,
                5. whether the report will require energies, and
-               6. whether coordinates should be wrapped to lie in a 
+               6. whether coordinates should be wrapped to lie in a
                   single periodic box.
         """
 
         return (self._interval - simulation.currentStep % self._interval,
                 True, self._velocities, self._forces, False, self._periodic)
 
     def report(self, simulation: app.Simulation, state: openmm.State) -> None:
@@ -123,50 +112,61 @@
 
         Parameters
         ----------
         simulation : `openmm.app.Simulation`
             OpenMM simulation to generate a report for.
 
         state : `openmm.State`
-            Current state of the simulation.
+            Current OpenMM simulation state.
         """
 
         # Get all requested state data from OpenMM State
         data = {}
         if self._subset is None:
-            data["coordinates"] = state.getPositions(asNumpy=True) \
-                                  / unit.angstrom
+            data["coordinates"] \
+                = state.getPositions(asNumpy=True).value_in_unit(unit.angstrom)
             if self._velocities:
-                data["velocities"] = state.getVelocities(asNumpy=True) \
-                                     / (unit.angstrom / unit.picosecond)
+                data["velocities"] \
+                    = state.getVelocities(asNumpy=True).value_in_unit(
+                        unit.angstrom / unit.picosecond
+                    )
             if self._forces:
-                data["forces"] = state.getForces(asNumpy=True) \
-                                 / (unit.kilocalorie_per_mole / unit.angstrom)
+                data["forces"] = state.getForces(asNumpy=True).value_in_unit(
+                    unit.kilocalorie_per_mole / unit.angstrom
+                )
         else:
-            data["coordinates"] = state.getPositions(asNumpy=True)[self._subset] \
-                                  / unit.angstrom
+            data["coordinates"] \
+                = state.getPositions(asNumpy=True)[self._subset].value_in_unit(
+                    unit.angstrom
+                )
             if self._velocities:
-                data["velocities"] = state.getVelocities(asNumpy=True)[self._subset] \
-                                     / (unit.angstrom / unit.picosecond)
+                data["velocities"] \
+                    = state.getVelocities(asNumpy=True)[self._subset].value_in_unit(
+                        unit.angstrom / unit.picosecond
+                    )
             if self._forces:
-                data["forces"] = state.getForces(asNumpy=True)[self._subset] \
-                                 / (unit.kilocalorie_per_mole / unit.angstrom)
+                data["forces"] \
+                    = state.getForces(asNumpy=True)[self._subset].value_in_unit(
+                        unit.kilocalorie_per_mole / unit.angstrom
+                    )
 
         # Initialize NetCDF file headers, if not done already
         if not hasattr(self._out._nc, "Conventions"):
-            self._out._initialize(
+            self._out.write_header(
                 simulation.topology.getNumAtoms() if self._subset is None \
                     else len(self._subset),
                 simulation.topology.getPeriodicBoxVectors() is not None,
                 self._velocities, self._forces
             )
 
         # Get the lengths and angles that define the size and shape of the
         # simulation box
         pbv = state.getPeriodicBoxVectors()
         if pbv is not None:
-            (a, b, c, alpha, beta, gamma) = app.internal.unitcell.computeLengthsAndAngles(pbv)
+            (a, b, c, alpha, beta, gamma) = \
+                app.internal.unitcell.computeLengthsAndAngles(pbv)
             data["cell_lengths"] = 10 * np.array((a, b, c))
             data["cell_angles"] = 180 * np.array((alpha, beta, gamma)) / np.pi
 
         # Write current frame
-        self._out.write_model(state.getTime() / unit.picosecond, **data)
+        self._out.write_model(state.getTime().value_in_unit(unit.picosecond),
+                              **data)
```

### Comparing `mdhelper-0.0.2/src/mdhelper/openmm/system.py` & `mdhelper-1.0.0/src/mdhelper/openmm/system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,142 @@
 """
-OpenMM system transformations
-=============================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
-
-This module contains implementations of common OpenMM topology 
-transformations, like the Yeh–Berkowitz slab correction, the method of
-image charges, and adding an external electric field.
+OpenMM system extensions and tools
+==================================
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
+
+This module contains implementations of common OpenMM system
+transformations, like the slab correction method for pseudo-2D slab
+systems, the method of image charges, and an applied potential
+difference.
 """
 
-from typing import Any, Iterable, Union
+import logging
+from typing import Any, Union
 import warnings
 
-try:
-    from constvplugin import ConstVLangevinIntegrator
-    FOUND_CONSTVPLUGIN = True
-except:
-    FOUND_CONSTVPLUGIN = False
+import mpmath
 import numpy as np
 import openmm
 from openmm import app, unit
+from scipy import special
 
 from .unit import VACUUM_PERMITTIVITY
-from .. import ArrayLike
+
+try:
+    from openmm_ic import ICLangevinIntegrator
+    FOUND_ICPLUGIN = True
+except ImportError:
+    try:
+        from constvplugin import ConstVLangevinIntegrator as ICLangevinIntegrator
+        FOUND_ICPLUGIN = True
+    except ImportError:
+        FOUND_ICPLUGIN = False
 
 def register_particles(
-        system: openmm.System = None, topology: app.Topology = None,
+        system: openmm.System, topology: app.Topology,
         N: int = 0, mass: Union[float, unit.Quantity] = 0.0, *,
         chain: app.Chain = None, element: app.Element = None, name: str = "",
         resname: str = "", nbforce: openmm.NonbondedForce = None,
         charge: Union[float, unit.Quantity] = 0.0,
         sigma: Union[float, unit.Quantity] = 0.0,
         epsilon: Union[float, unit.Quantity] = 0.0,
-        cnbforces: Union[ArrayLike, dict[openmm.CustomNonbondedForce, 
-                                         Iterable[Any]]] = {}
+        cnbforces: dict[openmm.CustomNonbondedForce, tuple[Any]] = None
     ) -> None:
 
     """
     Sequentially register particles of the same type to the simulation
     system, topology, and nonbonded pair potentials.
 
     Parameters
     ----------
     system : `openmm.System`
-        OpenMM molecular system.
+        OpenMM molecular system. Can be :code:`None` if particles are to
+        be registered to the topology only.
 
     topology : `openmm.app.Topology`
         Topological information about an OpenMM system.
 
     N : `int`, default: :code:`0`
-        Number of atom(s). If not provided, no particles are added.
+        Number of atom(s). If not specified, no particles are added.
 
     mass : `float` or `openmm.unit.Quantity`, default: :code:`0`
-        Molar mass. If not provided, particles have no mass and will not
-        move. 
-        
-        **Reference unit**: :math:`\mathrm{g/mol}`.
+        Molar mass. If not specified, particles are massless and will
+        not move.
+
+        **Reference unit**: :math:`\\mathrm{g/mol}`.
 
     chain : `openmm.app.Chain`, keyword-only, optional
         Chain that the atom(s) should be added to. If not provided,
         a new chain is created for each atom.
 
     element : `openmm.app.Element`, keyword-only, optional
         Chemical element of the atom(s) to add.
-    
+
     name : `str`, keyword-only, optional
         Name of the atom(s) to add.
-    
+
     resname : `str`, keyword-only, optional
-        Name of the residue(s) to add.
+        Name of the residue(s) to add. If not specified, `name` is used
+        if available.
 
     nbforce : `openmm.NonbondedForce`, keyword-only, optional
-        Built-in hybrid pair potential object containing the
+        Standard OpenMM pair potential object implementing the nonbonded
         Lennard-Jones and Coulomb potentials.
-    
+
     charge : `float` or `openmm.unit.Quantity`, keyword-only, \
     default: :code`0`
-        Charge :math:`q` of the atoms for use in the Coulomb potential
-        in `nbforce`. 
-        
-        **Reference unit**: :math:`\mathrm{e}`.
+        Charge :math:`q` of the atom(s) for use in the Coulomb potential
+        in `nbforce`.
+
+        **Reference unit**: :math:`\\mathrm{e}`.
 
     sigma : `float` or `openmm.unit.Quantity`, keyword-only, \
     default: :code`0`
-        :math:`\sigma` parameter of the Lennard-Jones potential in
-        `nbforce`. 
-        
-        **Reference unit**: :math:`\mathrm{nm}`.
+        :math:`\\sigma` parameter of the Lennard-Jones potential in
+        `nbforce`.
+
+        **Reference unit**: :math:`\\mathrm{nm}`.
 
     epsilon : `float` or `openmm.unit.Quantity`, keyword-only, \
     default: :code`0`
-        :math:`\epsilon` parameter of the Lennard-Jones potential in
-        `nbforce`. 
-        
-        **Reference unit**: :math:`\mathrm{kJ/mol}`.
+        :math:`\\epsilon` parameter of the Lennard-Jones potential in
+        `nbforce`.
+
+        **Reference unit**: :math:`\\mathrm{kJ/mol}`.
 
     cnbforces : `dict`, keyword-only, optional
         Custom pair potential objects implementing other non-standard
-        pair potentials and their corresponding per-particle parameters. 
+        pair potentials and their corresponding per-particle parameters.
 
-        **Example**: :code:`{gauss: (0.3 * unit.nanometer,)}`, where 
-        `gauss` is a custom Gaussian potential 
-        :func:`mdhelper.openmm.pair.gauss`.
+        **Example**: :code:`{gauss: (0.3 * unit.nanometer,)}`, where
+        `gauss` is a custom Gaussian potential obtained using
+        :func:`mdhelper.openmm.pair.gauss()`.
     """
 
+    has_nbforce = nbforce is not None
+    has_system = system is not None
     per_chain = chain is None
+    cnbforces = cnbforces or {}
     for _ in range(N):
-        system.addParticle(mass)
+        if has_system:
+            system.addParticle(mass)
         if per_chain:
             chain = topology.addChain()
-        residue = topology.addResidue(resname, chain)
+        residue = topology.addResidue(resname or name, chain)
         topology.addAtom(name, element, residue)
-        if nbforce is not None:
+        if has_nbforce:
             nbforce.addParticle(charge, sigma, epsilon)
         for cnbforce, param in cnbforces.items():
             cnbforce.addParticle(param)
 
-def slab_correction(
+def add_slab_correction(
         system: openmm.System, topology: app.Topology,
         nbforce: Union[openmm.NonbondedForce, openmm.CustomNonbondedForce],
         temp: Union[float, unit.Quantity], fric: Union[float, unit.Quantity],
-        dt: Union[float, unit.Quantity], axis: int = 2, *, 
+        dt: Union[float, unit.Quantity], axis: int = 2, *,
         charge_index: int = 0, z_scale: float = 3, method: str = "force"
     ) -> openmm.Integrator:
 
     r"""
     Implements a slab correction so that efficient three-dimensional
     Ewald methods can continue to be used to evaluate the electrostatics
     for systems that are periodic in the :math:`x`- and
@@ -170,63 +183,64 @@
     system : `openmm.System`
         OpenMM molecular system.
 
     topology : `openmm.app.Topology`
         Topological information about an OpenMM system.
 
     nbforce : `openmm.NonbondedForce` or `openmm.CustomNonbondedForce`
-        Pair potential containing particle charge information. 
-        
+        Pair potential object containing particle charge information.
+
         .. note::
-           
+
            It is assumed that the charge :math:`q` information is the
            first per-particle parameter stored in `nbforce`. If not, the
            index can be specified in `charge_index`.
 
     temp : `float` or `openmm.unit.Quantity`
-        System temperature :math:`T`. 
-        
+        System temperature :math:`T`.
+
         **Reference unit**: :math:`\mathrm{K}`.
-    
+
     fric : `float` or `openmm.unit.Quantity`
         Friction coefficient :math:`\gamma` that couples the system to
         the heat bath.
-        
+
         **Reference unit**: :math:`\mathrm{ps}^{-1}`.
-    
+
     dt : `float` or `openmm.unit.Quantity`
-        Integration step size :math:`\Delta t`. 
-        
+        Integration step size :math:`\Delta t`.
+
         **Reference unit**: :math:`\mathrm{ps}`.
-    
+
     axis : `int`, default: :code:`2`
         Axis along which to apply the slab correction, with :math:`x`
         being :code:`0`, :math:`y` being :code:`1`, and :math:`z` being
-        :code:`2`.
+        :code:`2`. The source code and outputs, if any, will refer to
+        this dimension as :code:`z` regardless of this value.
 
     charge_index : `int`, keyword-only, default: :code:`0`
         Index of charge :math:`q` information in the per-particle
         parameters stored in `nbforce`.
-    
+
     z_scale : `float`, keyword-only, default: :code:`3`
-        :math:`z`-dimension scaling factor.
+        Scaling factor for the dimension specified in `axis`.
 
     method : `str`, keyword-only, default: :code:`"force"`
         Slab correction methodology.
 
         .. container::
 
            **Valid values**:
-            
-           * :code:`"force"`: Collective implementation via 
-             :class:`openmm.openmm.CustomExternalForce` and 
-             :class:`openmm.openmm.CustomCVForce` [3]_. This is 
+
+           * :code:`"force"`: Collective implementation via
+             :class:`openmm.CustomExternalForce` and
+             :class:`openmm.CustomCVForce` [3]_. This is
              generally the most efficient.
            * :code:`"integrator"`: Per-particle implementation via an
-             :class:`openmm.openmm.CustomIntegrator`.
+             :class:`openmm.CustomIntegrator`.
 
     Returns
     -------
     integrator : `openmm.Integrator` or `openmm.CustomIntegrator`
         Integrator that simulates a system using Langevin dynamics, with
         the LFMiddle discretization.
 
@@ -245,16 +259,17 @@
     .. [3] Son, C. Y.; Wang, Z.-G. Image-Charge Effects on Ion
        Adsorption near Aqueous Interfaces. *Proc. Natl. Acad. Sci.
        U.S.A.* **2021**, *118* (19), e2020615118.
        https://doi.org/10.1073/pnas.2020615118.
     """
 
     # Get system dimensions
-    dims = np.array(topology.getUnitCellDimensions() / unit.nanometer) \
-           * unit.nanometer
+    dims = np.array(
+        topology.getUnitCellDimensions().value_in_unit(unit.nanometer)
+    ) * unit.nanometer
     pbv = system.getDefaultPeriodicBoxVectors()
 
     # Scale system z-dimension by specified z-scale
     if z_scale < 2:
         wmsg = ("A z-scaling factor that is less than 2 may introduce "
                 "unwanted slab–slab interactions. The recommended "
                 "value is 3.")
@@ -267,33 +282,38 @@
     pbv[axis] *= z_scale
 
     # Set new system dimensions
     topology.setUnitCellDimensions(dims)
     system.setDefaultPeriodicBoxVectors(*pbv)
 
     # Obtain particle charge information
-    dtype = type(nbforce.getParticleParameters(0)[charge_index])
-    qs = np.fromiter(
-        (nbforce.getParticleParameters(i)[charge_index] / unit.elementary_charge
-         for i in range(nbforce.getNumParticles())) if dtype == unit.Quantity \
-        else (nbforce.getParticleParameters(i)[charge_index]
-              for i in range(nbforce.getNumParticles())),
-        dtype=float
-    )
+    if isinstance(nbforce.getParticleParameters(0)[charge_index], unit.Quantity):
+        qs = np.fromiter(
+            (nbforce.getParticleParameters(i)[charge_index]
+             .value_in_unit(unit.elementary_charge)
+             for i in range(nbforce.getNumParticles())),
+            dtype=float
+        )
+    else:
+        qs = np.fromiter(
+            (nbforce.getParticleParameters(i)[charge_index]
+             for i in range(nbforce.getNumParticles())),
+            dtype=float
+        )
     neutral = qs.min() == qs.max()
     if not neutral:
         q_tot = qs.sum()
         electroneutral = np.isclose(q_tot, 0)
 
     # Calculate coefficient for slab correction
     coef = unit.AVOGADRO_CONSTANT_NA / \
            (2 * VACUUM_PERMITTIVITY * dims[0] * dims[1] * dims[2])
 
     # Get letter representation of axis for formula
-    x = chr(120 + axis)
+    z = chr(120 + axis)
 
     if neutral:
 
         # Instantiate an integrator that simulates a system using
         # Langevin dynamics, with the LFMiddle discretization
         integrator = openmm.LangevinMiddleIntegrator(temp, fric, dt)
 
@@ -323,132 +343,149 @@
             integrator.addPerDofVariable("q", 0)
 
             # Add global dipole moment computation to integrator
             integrator.addComputeSum("M_z", "q*x")
             integrator.addComputeSum("M_zz", "q*x^2")
 
             # Give particle charge information to integrator
-            q_vectors = np.zeros((len(qs), 3), dtype=float)
+            q_vectors = np.zeros((len(qs), 3))
             q_vectors[:, axis] = qs
             integrator.setPerDofVariableByName("q", q_vectors)
 
             # Implement per-particle slab correction
             if electroneutral:
                 slab_corr = openmm.CustomExternalForce(
-                    f"coef*q*({x}*M_z-M_zz/2)"
+                    f"coef*q*({z}*M_z-M_zz/2)"
                 )
             else:
                 slab_corr = openmm.CustomExternalForce(
-                    f"coef*q*({x}*M_z-(M_zz+q_tot*{x}^2)/2-q_tot*dim_z^2/12)"
+                    f"coef*q*({z}*M_z-(M_zz+q_tot*{z}^2)/2-q_tot*dim_z^2/12)"
                 )
                 slab_corr.addGlobalParameter("dim_z", dims[axis])
                 slab_corr.addGlobalParameter("q_tot", q_tot)
             slab_corr.addGlobalParameter("M_z", 0)
             slab_corr.addGlobalParameter("M_zz", 0)
             slab_corr.addGlobalParameter("coef", coef)
             slab_corr.addPerParticleParameter("q")
 
             # Register real particles to the slab correction
             for i, q in enumerate(qs):
                 slab_corr.addParticle(i, (q,))
 
         elif method == "force":
-            
+
             # Instantiate an integrator that simulates a system using
             # Langevin dynamics, with the LFMiddle discretization
             integrator = openmm.LangevinMiddleIntegrator(temp, fric, dt)
 
             # Calculate instantaneous system dipole
-            M_z = openmm.CustomExternalForce(f"q*{x}")
+            M_z = openmm.CustomExternalForce(f"q*{z}")
             M_z.addPerParticleParameter("q")
 
             # Implement collective slab correction
             if electroneutral:
                 slab_corr = openmm.CustomCVForce("coef*M_z^2")
             else:
-                M_zz = openmm.CustomExternalForce(f"q*{x}^2")
+                M_zz = openmm.CustomExternalForce(f"q*{z}^2")
                 M_zz.addPerParticleParameter("q")
                 slab_corr = openmm.CustomCVForce(
                     "coef*(M_z^2-q_tot*M_zz-q_tot^2*dim_z^2/12)"
                 )
                 slab_corr.addCollectiveVariable("M_zz", M_zz)
                 slab_corr.addGlobalParameter("dim_z", dims[axis])
                 slab_corr.addGlobalParameter("q_tot", q_tot)
             slab_corr.addCollectiveVariable("M_z", M_z)
             slab_corr.addGlobalParameter("coef", coef)
-        
+
             # Register real particles to the slab correction
             for i, q in enumerate(qs):
                 M_z.addParticle(i, (q,))
                 if not electroneutral:
                     M_zz.addParticle(i, (q,))
 
         # Register slab correction to the system
         system.addForce(slab_corr)
 
     return integrator
 
-def image_charges(
+def add_image_charges(
         system: openmm.System, topology: app.Topology,
-        positions: Union[np.ndarray, unit.Quantity],
+        positions: Union[np.ndarray[float], unit.Quantity],
         temp: Union[float, unit.Quantity], fric: Union[float, unit.Quantity],
-        dt: Union[float, unit.Quantity], axis: int = 2, *,
-        wall_indices: np.ndarray = None,
-        nbforce: openmm.NonbondedForce = None,
-        cnbforces: Union[Iterable[openmm.CustomNonbondedForce],
-                         dict[openmm.CustomNonbondedForce, Iterable[Any]]] = {},
-        params: Iterable[Iterable[Any]] = ()
+        dt: Union[float, unit.Quantity], *, gamma: float = -1,
+        n_cells: int = 2, nbforce: openmm.NonbondedForce = None,
+        cnbforces: dict[openmm.CustomNonbondedForce, dict[str, Any]] = None,
+        wall_indices: np.ndarray[int] = None, exclude: bool = False
     ) -> tuple[unit.Quantity, openmm.Integrator]:
 
     r"""
-    Implements the method of image charges for perfectly conducting
-    boundaries (with a relative permittivity of
-    :math:`\varepsilon_\mathrm{r}=\infty`).
+    Implements the method of image charges for dielectric boundaries.
+    For more information about the method, see Refs. [1]_, [2]_, and
+    [3]_ for perfectly conducting boundaries, and Refs. [4]_, [5]_, and
+    [6]_ otherwise.
+
+    .. note::
+
+       The boundaries must be in the :math:`xy`-plane and along the
+       :math:`z`-axis.
 
     Parameters
     ----------
     system : `openmm.System`
         OpenMM molecular system.
 
     topology : `openmm.app.Topology`
         Topological information about an OpenMM system.
-    
+
     positions : `numpy.ndarray`
-        Positions of the :math:`N` particles in the real system. 
+        Positions of the :math:`N` particles in the real system.
+
+        **Shape**: :math:`(N,\,3)`.
 
-        **Shape**: :math:`(N,/,3)`.
-        
         **Reference unit**: :math:`\mathrm{nm}`.
 
     temp : `float` or `openmm.unit.Quantity`
-        System temperature :math:`T`. 
-        
+        System temperature :math:`T`.
+
         **Reference unit**: :math:`\mathrm{K}`.
 
     fric : `float` or `openmm.unit.Quantity`
         Friction coefficient :math:`\gamma` that couples the system to
         the heat bath.
-        
+
         **Reference unit**: :math:`\mathrm{ps}^{-1}`.
-    
+
     dt : `float` or `openmm.unit.Quantity`
-        Integration step size :math:`\Delta t`. 
-        
+        Integration step size :math:`\Delta t`.
+
         **Reference unit**: :math:`\mathrm{ps}`.
 
-    axis : `int`, default: :code:`2`
-        Axis along which to apply the method of image charges, with 
-        :math:`x` being :code:`0`, :math:`y` being :code:`1`, and 
-        :math:`z` being :code:`2`.
+    gamma : `float`, keyword-only, default: :code:`-1`
+        Scaled image charge magnitude :math:`\gamma`.
+
+    n_cells : `int`, keyword-only, default: :code:`2`
+        Total number :math:`n_\mathrm{cell}` of cells, with :math:`1`
+        real and :math:`n_\mathrm{cell}-1` image cells.
+
+        .. tip::
+
+           Use :math:`n_\mathrm{cell}>2` to instantiate a
+           highly-confined simulation system with periodic dimensions
+           large enough to satisfy the constraint that the force field
+           cutoff be less than half the box size.
+
+        **Valid values**: Even integers greater than :math:`1` when
+        :math:`\gamma=-1`.
 
     nbforce : `openmm.NonbondedForce`, keyword-only, optional
-        Standard Lennard-Jones (LJ) and Coulomb pair potential used in
-        OpenMM. For the image charges, the charges :math:`q` are flipped
-        while the LJ parameters :math:`\sigma` and :math:`\epsilon` are
-        set to :math:`0`.
+        Standard OpenMM pair potential object implementing the nonbonded
+        Lennard-Jones and Coulomb potentials. For the image charges, the
+        charges :math:`q` have their signs flipped, and the LJ
+        parameters :math:`\sigma` and :math:`\epsilon` are both set to
+        :math:`0`.
 
     cnbforces : `dict`, keyword-only, optional
         Custom pair potential objects implementing other non-standard
         pair potentials. The keys are the potentials and the values are
         the corresponding per-particle parameters to use, which can be
         provided as follows:
 
@@ -457,15 +494,15 @@
            * `None`: All per-particle parameters set to :math:`0`.
            * `dict`: Information on how to transform the real particle
              parameters into those for the image charges. The valid
              (optional) key-value pairs are:
 
              * :code:`"charge"`: Index (`int`) where the charge
                :math:`q` information is stored.
-             * :code:`"zero"`: Index (`int`) or indices (`list`, 
+             * :code:`"zero"`: Index (`int`) or indices (`list`,
                `slice`, or `numpy.ndarray`) of parameters to zero out.
              * :code:`"replace"`: `dict` containing key-value pairs of
                indices (`int`) of parameters to change and their
                replacement value(s). If the value is an `int`, all
                particles receive that value for the current pair
                potential. If the value is another `dict`, the new
                parameter value (value of inner `dict`) is determined by
@@ -476,154 +513,379 @@
         listed above. If one does appear more than once, the order
         in which parameter values are updated follows that of the list
         above.
 
         See the Examples section below for a simple illustration of the
         possibilities outlined above.
 
-    wall_indices : `numpy.ndarray`, keyword-only, optional
+    wall_indices : array-like, keyword-only, optional
         Atom indices corresponding to wall particles. If not provided,
-        the wall particles are guessed using the system dimensions and
-        `axis`.
+        the wall particles are guessed using the system dimensions.
+
+    exclude : `bool`, keyword-only, default: :code:`False`
+        Specifies whether interactions between a wall particle and all
+        image wall particles should be excluded. If :code:`False`, only
+        the interaction between a wall particle and its own image is
+        removed.
+
+        .. tip::
+
+           If you want accurate forces acting on wall particles, set
+           :code:`exclude=True`.
 
     Returns
     -------
     positions : `numpy.ndarray`
-        Positions of the :math:`N` particles in the real system and 
+        Positions of the :math:`N` particles in the real system and
         their images.
 
         **Shape**: :math:`(2N,\,3)`.
 
         **Reference unit**: :math:`\mathrm{nm}`.
-    
+
     integrator : `openmm.Integrator`
         Integrator that simulates a system using Langevin dynamics, with
         the LFMiddle discretization.
 
     Examples
     --------
     Prepare the `cnbforces` `dict` argument for a system with the
     following custom pair potentials:
 
-    * :code:`PairGauss`: Gaussian potential with per-particle
+    * :code:`pair_gauss`: Gaussian potential with per-particle
       parameters `type` and `beta`.
-        
+
       * `type` is the particle type, and is used to look up a
         tabulated function for parameter values. As such, the new
         values will vary and depend on the old ones. For example, for
         a system with :math:`2` types of particles, :math:`0` becomes
         :math:`2` and :math:`1` becomes :math:`3`.
       * `beta` is assumed to be constant, with the value for the real
         particles differing from that for image charges. For this
         example, the new value is :math:`\beta = 42` (arbitrary
         units).
 
-    * :code:`PairWCA`: Weeks–Chander–Andersen potential with per-
+    * :code:`pair_wca`: Weeks–Chander–Andersen potential with per-
       particle parameters `sigma` and `epsilon`, both of which
       should be set to :math:`0` to turn off this potential for
       image charges.
-    * :code:`PairCoulRecip`: Smeared Coulomb potential with per-
+    * :code:`pair_coul_recip`: Smeared Coulomb potential with per-
       particle parameter `charge`, which should be flipped for image
       charges, and `dummy`, a value that should be set to :math:`0`.
 
     .. code::
 
        NEW_BETA_VALUE = 42
        cnbforces = {
-           PairGauss: {"replace": {0: {0: 2, 1: 3}, 1: NEW_BETA_VALUE}},
-           PairWCA: None,
-           PairCoulRecip: {"charge": 0, "zero": 1}
+           pair_gauss: {"replace": {0: {0: 2, 1: 3}, 1: NEW_BETA_VALUE}},
+           pair_wca: None,
+           pair_coul_recip: {"charge": 0, "zero": 1}
        }
+
+    References
+    ----------
+    .. [1] Hautman, J.; Halley, J. W.; Rhee, Y. ‐J. Molecular Dynamics
+       Simulation of Water Beween Two Ideal Classical Metal Walls.
+       *J. Chem. Phys.* **1989**, *91* (1), 467–472.
+       https://doi.org/10.1063/1.457481.
+
+    .. [2] Dwelle, K. A.; Willard, A. P. Constant Potential,
+       Electrochemically Active Boundary Conditions for Electrochemical
+       Simulation. *J. Phys. Chem. C* **2019**, *123* (39), 24095–24103.
+       https://doi.org/10.1021/acs.jpcc.9b06635.
+
+    .. [3] Son, C. Y.; Wang, Z.-G. Image-Charge Effects on Ion
+       Adsorption near Aqueous Interfaces. *Proc. Natl. Acad. Sci.
+       U.S.A.* **2021**, *118* (19), e2020615118.
+       https://doi.org/10.1073/pnas.2020615118.
+
+    .. [4] Dos Santos, A. P.; Girotto, M.; Levin, Y. Simulations of
+       Coulomb Systems with Slab Geometry Using an Efficient 3D Ewald
+       Summation Method. *The Journal of Chemical Physics* **2016**,
+       **144** (14), 144103. https://doi.org/10.1063/1.4945560.
+
+    .. [5] Dos Santos, A. P.; Girotto, M.; Levin, Y. Simulations of
+       Coulomb Systems Confined by Polarizable Surfaces Using Periodic
+       Green Functions. *The Journal of Chemical Physics* **2017**,
+       **147** (18), 184105. https://doi.org/10.1063/1.4997420.
+
+    .. [6] Son, C. Y.; Wang, Z.-G. Manuscript in preparation.
     """
 
-    if not FOUND_CONSTVPLUGIN:
-        emsg = ("The required constant potential MD integrator plugin "
-                "(https://github.com/scychon/openmm_constV) was not found. "
-                "As such, the method of image charges is unavailable.")
+    if not FOUND_ICPLUGIN:
+        emsg = ("An integrator capable of simulating a system with "
+                "image charges was not found. As such, the method of "
+                "image charges is unavailable unless the openmm-ic "
+                "(https://github.com/bbye98/mdhelper/tree/main/lib/openmm-ic-plugin) "
+                "or the constvplugin (https://github.com/scychon/openmm_constV) "
+                "package is installed.")
         raise ImportError(emsg)
 
+    if np.isclose(gamma, 0):
+        emsg = ("Use the slab correction, available via "
+                "mdhelper.openmm.system.slab_correction(), for gamma=0.")
+        raise ValueError(emsg)
+    if not np.isclose(gamma, -1) and n_cells != 2:
+        emsg = ("The method of image charges with gamma != -1 is only "
+                "implemented for n_cells=2.")
+        raise ValueError(emsg)
+
+    def _ic_beta(gamma: float, x: float) -> float:
+
+        r"""
+        Computes the :math:`\beta` value used in the higher-order term
+        correction for the method of image charges with
+        :math:`\gamma\neq\pm1`.
+
+        Parameters
+        ----------
+        gamma : `float`
+            Scaled image charge magnitude :math:`\gamma`.
+
+        x : `float`
+            Scaled :math:`x`-coordinate of the ion.
+
+        Returns
+        -------
+        beta : `float`
+            Approximated :math:`\beta` value.
+        """
+
+        if not 0 <= x <= 1:
+            raise ValueError("'x' must be between 0 and 1.")
+        if np.isclose(x, 0.5):
+            return float(2 * special.zeta(3, 1.5)
+                         - 2 * gamma ** 4 * mpmath.lerchphi(gamma ** 2, 3, 1.5))
+        else:
+            return (
+                special.zeta(2, 2 - x) - special.zeta(2, 1 + x) - gamma ** 4 *
+                float(mpmath.lerchphi(gamma ** 2, 2, 2 - x)
+                      - mpmath.lerchphi(gamma ** 2, 2, 1 + x))
+            ) / (2 * x - 1)
+
     # Get system information
-    dims = np.array(topology.getUnitCellDimensions() / unit.nanometer) \
-           * unit.nanometer
+    dims = np.asarray(
+        topology.getUnitCellDimensions().value_in_unit(unit.nanometer)
+    ) * unit.nanometer
     pbv = system.getDefaultPeriodicBoxVectors()
-    N_real = positions.shape[0]
+    N_real_atoms = positions.shape[0]
     if isinstance(positions, unit.Quantity):
-        positions /= unit.nanometer
+        positions = positions.value_in_unit(unit.nanometer)
 
     # Guess indices of left and right walls if not provided
     if wall_indices is None:
         wall_indices = np.concatenate(
-            ((positions[:, axis] == 0).nonzero()[0],
-            (positions[:, axis] == dims[axis] / unit.nanometer).nonzero()[0])
+            (np.isclose(positions[:, 2], 0).nonzero()[0],
+             np.isclose(positions[:, 2],
+                        dims[2].value_in_unit(unit.nanometer)).nonzero()[0])
         )
 
-    # Mirror particle positions
-    flip = np.ones(3, dtype=int)
-    flip[axis] *= -1
-    positions = np.concatenate((positions, positions * flip)) * unit.nanometer
+    # Find averaged beta value for image charges with gamma =/= +/-1
+    beta = (_ic_beta(gamma, 0) + _ic_beta(gamma, 0.5)) / 2
+
+    # Set up higher-order image charge and slab corrections
+    cv_E_corr = openmm.CustomExternalForce("q*(1-2*z/L)")
+    cv_E_corr.addGlobalParameter("L", dims[2]) # real system z-dimension such
+                                               # that 0 <= (x = z / L_z) <= 1
+    cv_E_corr.addPerParticleParameter("q")
+    cv_M_z = openmm.CustomExternalForce("q*z")
+    cv_M_z.addPerParticleParameter("q")
+    cv_M_zz = openmm.CustomExternalForce("q*z^2")
+    cv_M_zz.addPerParticleParameter("q")
+
+    # Obtain particle charge information and register charges to
+    # corrections
+    if nbforce is None:
+        charge_index = None
+        for force, params in cnbforces:
+            if "charge" in params:
+                charge_index = params["charge"]
+                break
+        if charge_index is None:
+            raise ValueError("No charge information provided.")
+    else:
+        force = nbforce
+        charge_index = 0
+
+    q_tot = 0
+    if isinstance(force.getParticleParameters(0)[charge_index], unit.Quantity):
+        for i in range(force.getNumParticles()):
+            q = (force.getParticleParameters(i)[charge_index]
+                 .value_in_unit(unit.elementary_charge))
+            q_tot += q
+            if not np.isclose(q, 0):
+                cv_E_corr.addParticle(i, (q,))
+                cv_M_z.addParticle(i, (q,))
+                cv_M_zz.addParticle(i, (q,))
+    else:
+        for i in range(force.getNumParticles()):
+            q = force.getParticleParameters(i)[charge_index]
+            q_tot += q
+            if not np.isclose(q, 0):
+                cv_E_corr.addParticle(i, (q,))
+                cv_M_z.addParticle(i, (q,))
+                cv_M_zz.addParticle(i, (q,))
+    electroneutral = np.isclose(q_tot, 0)
 
     # Update and set new system dimensions
-    dims[axis] *= 2
+    dims[2] *= n_cells
     topology.setUnitCellDimensions(dims)
-    pbv[axis] *= 2
+    pbv[2] *= n_cells
     system.setDefaultPeriodicBoxVectors(*pbv)
+    logging.info(f"Increased z-dimension to {dims[2]}.")
+
+    # Determine correction energy expression
+    corr_energy = ""
+    corr = openmm.CustomCVForce(corr_energy)
+    if not np.isclose(beta, 0):
+        corr_energy += "coef1*E_corr*M_z"
+        corr.addCollectiveVariable("E_corr", cv_E_corr)
+        corr.addGlobalParameter(
+            "coef1",
+            (unit.AVOGADRO_CONSTANT_NA * gamma * beta
+             / (4 * np.pi * VACUUM_PERMITTIVITY * dims[2] ** 2))
+            .in_units_of(unit.kilojoule_per_mole /
+                         (unit.elementary_charge ** 2 * unit.nanometer))
+        )
+    if not np.isclose(gamma, -1):
+        corr_energy += "+coef2*M_z^2"
+    if not electroneutral:
+        if np.isclose(gamma, 1):
+            corr_energy += "-coef2*q_tot*M_z*L_z"
+        elif np.isclose(gamma, -1):
+            corr_energy += "+coef2*q_tot*(M_z*L_z-M_zz)"
+        else:
+            corr_energy += "-coef2*q_tot*M_zz"
+        corr.addGlobalParameter("q_tot", q_tot)
+    if "coef2" in corr_energy:
+        corr.addGlobalParameter(
+            "coef2",
+            (unit.AVOGADRO_CONSTANT_NA
+             / (2 * VACUUM_PERMITTIVITY * dims[0] * dims[1] * dims[2]))
+            .in_units_of(unit.kilojoule_per_mole
+                         / (unit.elementary_charge * unit.nanometer) ** 2)
+        )
+    if "L_z" in corr_energy:
+        corr.addGlobalParameter("L_z", dims[2]) # periodic system z-dimension
+    if "M_z" in corr_energy:
+        corr.addCollectiveVariable("M_z", cv_M_z)
+    if "M_zz" in corr_energy:
+        corr.addCollectiveVariable("M_zz", cv_M_zz)
+    if corr_energy:
+        if corr_energy.startswith("+"):
+            corr_energy = corr_energy.lstrip("+")
+        corr.setEnergyFunction(corr_energy)
+        system.addForce(corr)
+        logging.info("Added higher-order image charge and/or slab "
+                     "correction(s).")
+
+    # Mirror particle positions
+    if n_cells == 2:
+        positions = np.concatenate(
+            (positions, positions * np.array((1, 1, -1), dtype=int))
+        ) * unit.nanometer
+    else:
+        positions = np.tile(positions, (n_cells, 1))
+        for cell_index in range(1, n_cells):
+            start = cell_index * N_real_atoms
+            stop = (cell_index + 1) * N_real_atoms
+            positions[start:stop, 2] = (
+                (1 - 2 * (cell_index % 2)) * positions[start:stop, 2]
+                - 2 * np.floor(cell_index / 2)
+                * dims[2].value_in_unit(unit.nanometer)
+            )
+        positions *= unit.nanometer
+    logging.info(f"Replicated {N_real_atoms:,} particles {n_cells - 1} "
+                 "time(s) over the z-axis.")
 
     # Instantiate an integrator that simulates a system using
     # Langevin dynamics and updates the image charge positions
-    integrator = ConstVLangevinIntegrator(temp, fric, dt)
+    integrator = ICLangevinIntegrator(temp, fric, dt, n_cells)
 
     # Register image charges to the system, topology, and force field
-    chains_ic = [topology.addChain() for _ in range(topology.getNumChains())]
-    residues_ic = [topology.addResidue(f"IC_{r.name}", 
-                                       chains_ic[r.chain.index])
-                   for r in list(topology.residues())]
-    for i, atom in enumerate(list(topology.atoms())):
-        system.addParticle(0)
-        topology.addAtom(f"IC_{atom.name}", atom.element,
-                         residues_ic[atom.residue.index])
-        if nbforce is not None:
-            nbforce.addParticle(
-                0 if i in wall_indices
-                else -nbforce.getParticleParameters(i)[0], 0, 0)
-        for force, kwargs in cnbforces.items():
-            params = np.array(force.getParticleParameters(i))
-            if kwargs is None:
-                params[:] = 0
-            else:
-                if "charge" in kwargs:
-                    params[kwargs["charge"]] *= 0 if i in wall_indices else -1
-                if "zero" in kwargs:
-                    params[kwargs["zero"]] = 0
-                if "replace" in kwargs:
-                    for index, value in kwargs["replace"].items():
-                        params[index] = value[params[index]] \
-                                        if isinstance(value, dict) \
-                                        else value
-            force.addParticle(params)
+    cnbforces = cnbforces or {}
+    N_real_chains = topology.getNumChains()
+    atoms = list(topology.atoms())
+    residues = list(topology.residues())
+    coefs = (1, gamma)
+    for c in range(1, n_cells):
+        coef = coefs[c % 2]
+        chains_ic = [topology.addChain() for _ in range(N_real_chains)]
+        residues_ic = [topology.addResidue(f"IC_{r.name}",
+                                           chains_ic[r.chain.index])
+                       for r in residues]
+        for i, atom in enumerate(atoms):
+            system.addParticle(0)
+            topology.addAtom(f"IC_{atom.name}", atom.element,
+                             residues_ic[atom.residue.index])
+            if nbforce is not None:
+                nbforce.addParticle(
+                    0 if i in wall_indices
+                    else coef * nbforce.getParticleParameters(i)[0],
+                    0, 0
+                )
+            for force, kwargs in cnbforces.items():
+                params = np.array(force.getParticleParameters(i))
+                if kwargs is None:
+                    params[:] = 0
+                else:
+                    if "charge" in kwargs:
+                        params[kwargs["charge"]] *= (0 if i in wall_indices
+                                                     else coef)
+                    if "zero" in kwargs:
+                        params[kwargs["zero"]] = 0
+                    if "replace" in kwargs:
+                        for index, value in kwargs["replace"].items():
+                            params[index] = (value[params[index]]
+                                             if isinstance(value, dict)
+                                             else value)
+                force.addParticle(params)
+    logging.info(f"Registered {system.getNumParticles() - N_real_atoms:,} "
+                 "image particles to the force field.")
 
     # Add existing particle exclusions to mirrored image charges
     for i in range(nbforce.getNumExceptions()):
         i1, i2, qq = nbforce.getExceptionParameters(i)[:3]
-        nbforce.addException(N_real + i1, N_real + i2, qq, 0, 0)
-        for force in cnbforces:
-            i1, i2 = force.getExclusionParticles(i)
-            force.addExclusion(N_real + i1, N_real + i2)
-
-    # Prevent wall particles from interacting with their mirrors
-    for i in wall_indices:
-        nbforce.addException(i, N_real + i, 0, 0, 0)
-        for force in cnbforces:
-            force.addExclusion(i, N_real + i)
+        if i1 not in wall_indices and i2 not in wall_indices:
+            for c in range(1, n_cells):
+                nbforce.addException(c * N_real_atoms + i1,
+                                     c * N_real_atoms + i2, qq, 0, 0)
+                for force in cnbforces:
+                    i1, i2 = force.getExclusionParticles(i)
+                    force.addExclusion(c * N_real_atoms + i1,
+                                       c * N_real_atoms + i2)
+    logging.info("Mirrored excluded non-wall image particle–image "
+                 "particle interactions.")
+
+    # Prevent wall particles from interacting with all image wall
+    # particles
+    if exclude:
+        for i in wall_indices:
+            for j in wall_indices:
+                for c in range(1, n_cells):
+                    nbforce.addException(i, c * N_real_atoms + j, 0, 0, 0)
+                    for force in cnbforces:
+                        force.addExclusion(i, c * N_real_atoms + j)
+
+    # Prevent wall particles from interacting their images
+    else:
+        for i in wall_indices:
+            for c in range(1, n_cells):
+                nbforce.addException(i, c * N_real_atoms + i, 0, 0, 0)
+                for force in cnbforces:
+                    force.addExclusion(i, c * N_real_atoms + i)
+    logging.info("Removed wall–image wall interactions.")
 
     return positions, integrator
 
-def electric_field(
+def add_electric_field(
         system: openmm.System, nbforce: openmm.NonbondedForce,
-        efield: Union[float, unit.Quantity,], *, axis: int = 2,
-        charge_index: int = 0, atom_indices: Union[int, Iterable] = None
+        E: Union[float, unit.Quantity], *, axis: int = 2,
+        dielectric: float = 1, charge_index: int = 0,
+        atom_indices: Union[int, np.ndarray[int]] = None
     ) -> None:
 
     r"""
     Adds an electric field to all charged particles by adding a force
     :math:`f_i=q_iE` in the axis specified in `axis`, where :math:`q_i`
     is the per-particle charge and :math:`E` is the electric field.
 
@@ -633,72 +895,217 @@
 
        .. code::
 
           |-| (-) ---> |+|
           |-| <-- E -- |+|
           |-| <--- (+) |+|
 
-       With a positive potential difference 
+       With a positive potential difference
        (:math:`\Delta V>0\;\mathrm{V}`), the electric field is negative
-       (:math:`E<0\;\mathrm{V/m}`) such that it is pointing from the 
-       left (positive) plate to the right (negative) plate. If an ion 
+       (:math:`E<0\;\mathrm{V/m}`) such that it is pointing from the
+       right (positive) plate to the left (negative) plate. If an ion
        has a positive charge (:math:`q_i>0\;\mathrm{e}`), the force will
        be negative, indicating that it will be drawn to the left plate,
        and vice versa.
 
     Parameters
     ----------
     system : `openmm.System`
         OpenMM molecular system.
 
     nbforce : `openmm.NonbondedForce` or `openmm.CustomNonbondedForce`
-        Pair potential containing particle charge information. 
-        
+        Pair potential object containing particle charge information.
+
         .. note::
-           
+
            It is assumed that the charge :math:`q` information is the
            first per-particle parameter stored in `nbforce`. If not, the
            index can be specified in `charge_index`.
-    
-    efield : `float` or `openmm.unit.Quantity`
+
+    E : `float` or `openmm.unit.Quantity`
         Electric field :math:`E`.
 
         **Reference unit**: :math:`\mathrm{kJ/(mol\cdot nm\cdot e)}`.
-    
+
     axis : `int`, keyword-only, default: :code:`2`
         Axis along which the walls are placed. :code:`0`, :code:`1`, and
         :code:`2` correspond to :math:`x`, :math:`y`, and :math:`z`,
         respectively.
 
+    dielectric : `float`, keyword-only, default: :code:`1`
+        Relative permittivity :math:`\varepsilon_\mathrm{r}` of the
+        medium. Used to scale the particle charges by
+        :math:`\sqrt{\varepsilon_\mathrm{r}}` and recover the original
+        values.
+
     charge_index : `int`, keyword-only, default: :code:`0`
         Index of charge :math:`q` information in the per-particle
         parameters stored in `nbforce`.
 
     atom_indices : `int` or array-like, keyword-only, optional
         Indices of atoms to apply the electric field to. By default,
         the electric field is applied to all atoms, but this can be
         computationally expensive when there are charged particles that
-        do not need to be included, such as image charges.
+        do not need to be included, such as image charges. If an `int`
+        is provided, all atoms up to that index are included.
     """
 
     # Get letter representation of axis for formula
-    x = chr(120 + axis)
+    z = chr(120 + axis)
 
     # Get indices of atoms that are affected by the electric field
     if atom_indices is None:
         atom_indices = range(nbforce.getNumParticles())
     elif isinstance(atom_indices, int):
         atom_indices = range(atom_indices)
 
     # Create and register particles to the electric field
-    efield = openmm.CustomExternalForce(f"-q*E*{x}")
-    efield.addGlobalParameter("E", efield)
-    efield.addPerParticleParameter('q')
+    efield = openmm.CustomExternalForce(f"-q*E*{z}")
+    efield.addGlobalParameter("E", E)
+    efield.addPerParticleParameter("q")
 
     for i in atom_indices:
         q = nbforce.getParticleParameters(i)[charge_index]
         if isinstance(q, unit.Quantity):
-            q /= unit.elementary_charge
+            q = q.value_in_unit(unit.elementary_charge)
         if not np.isclose(q, 0):
-            efield.addParticle(i, (q,))
-    
-    system.addForce(efield)
+            efield.addParticle(i, (q * np.sqrt(dielectric),))
+
+    system.addForce(efield)
+
+def estimate_pressure_tensor(
+        context: openmm.Context, dh: float = 1e-5, *, diag: bool = False
+    ) -> np.ndarray[float]:
+
+    r"""
+    Computes the estimated pressure tensor using a central finite
+    difference for the virial contribution.
+
+    The pressure tensor is given by
+
+    .. math::
+
+       \mathbf{p}=\frac{1}{V}\left(
+       \sum_{i=1}^N m_i\mathbf{v}_i^\mathsf{T}\mathbf{v}_i
+       +\mathbf{h}^\mathsf{T}\frac{dU}{d\mathbf{h}}\right)
+
+    where :math:`V` is the volume, :math:`m_i` and :math:`\mathbf{v}_i`
+    are the mass and velocity vector of particle :math:`i`,
+    :math:`\mathbf{h}` is a :math:`3\times 3` matrix where the rows
+    contain the box vectors, and :math:`U` is the total pairwise
+    potential energy.
+
+    To evaluate :math:`dU/d\mathbf{h}`, the box vectors are perturbed by
+    `dh` in each of the six "directions" and the positions are updated
+    accordingly. Then, OpenMM reevaluates the potential
+    energy based on the new periodic box vectors and particle positions,
+    and the difference in potential energy is used in the central finite
+    difference formula to estimate the derivative.
+
+    Parameters
+    ----------
+    context : `openmm.Context`
+        OpenMM simulation context.
+
+    dh : `float`, default: :code:`1e-5`
+        Finite difference step size.
+
+    diag : `bool`, keyword-only, default: :code:`False`
+        Determines whether only the values in the main diagonal of the
+        pressure tensor (i.e., the values that, when summed, gives the
+        system pressure) are calculated.
+
+    Returns
+    -------
+    pres : `numpy.ndarray`
+        Estimated pressure tensor (or diagonal components).
+
+        **Shape**: :math:`(3,)` or :math:`(3,\,3)`.
+
+        **Reference unit**: :math:`\mathrm{atm}`.
+    """
+
+    try:
+        state = context.getState(getPositions=True, getVelocities=True,
+                                 getEnergy=True)
+        box = state.getPeriodicBoxVectors(asNumpy=True)
+        positions = state.getPositions(asNumpy=True)
+        velocities = state.getVelocities(asNumpy=True)
+        volume = box[0, 0] * box[1, 1] * box[2, 2]
+    except openmm.OpenMMException:
+        emsg = ("The simulation context must have information about "
+                "the particle positions and velocities.")
+        raise ValueError(emsg)
+
+    system = context.getSystem()
+    masses = np.fromiter(
+        (system.getParticleMass(i).value_in_unit(unit.dalton)
+         for i in range(system.getNumParticles())),
+        dtype=float
+    ) * unit.dalton
+
+    if diag:
+
+        # Compute the ideal contribution
+        p_kinetic = (masses * velocities ** 2).sum(axis=0)
+
+        # Estimate the virial contribution with a central finite difference
+        p_virial = np.zeros(3) * unit.kilojoule_per_mole
+        for i in range(3):
+            box_ = box.copy()
+            box_[i, i] += dh
+            context.setPeriodicBoxVectors(*box_)
+            context.setPositions(
+                np.dot(positions,
+                       np.divide(box_, box, out=np.zeros_like(box),
+                                 where=box.value_in_unit(unit.nanometer) != 0))
+            )
+            U_plus = context.getState(getEnergy=True).getPotentialEnergy()
+            box_ = box.copy()
+            box_[i, i] -= dh
+            context.setPeriodicBoxVectors(*box_)
+            context.setPositions(
+                np.dot(positions,
+                       np.divide(box_, box, out=np.zeros_like(box),
+                                 where=box.value_in_unit(unit.nanometer) != 0))
+            )
+            U_minus = context.getState(getEnergy=True).getPotentialEnergy()
+            p_virial[i] = U_plus - U_minus
+        p_virial = (p_virial / (2 * dh)).in_units_of(p_kinetic.unit)
+
+    else:
+
+        # Compute the ideal contribution
+        p_kinetic = (masses * velocities * velocities[:, :, None]).sum(axis=0)
+
+        # Estimate the virial contribution with a central finite difference
+        p_virial = np.zeros((3, 3)) * unit.kilojoule_per_mole
+        for i in range(3):
+            for j in range(i + 1):
+                box_ = box.copy()
+                box_[i, j] += dh
+                context.setPeriodicBoxVectors(*box_)
+                context.setPositions(
+                    np.dot(positions,
+                           np.divide(box_, box, out=np.zeros_like(box),
+                                     where=box.value_in_unit(unit.nanometer) != 0))
+                )
+                U_plus = context.getState(getEnergy=True).getPotentialEnergy()
+                box_ = box.copy()
+                box_[i, j] -= dh
+                context.setPeriodicBoxVectors(*box_)
+                context.setPositions(
+                    np.dot(positions,
+                           np.divide(box_, box, out=np.zeros_like(box),
+                                     where=box.value_in_unit(unit.nanometer) != 0))
+                )
+                U_minus = context.getState(getEnergy=True).getPotentialEnergy()
+                p_virial[i, j] = U_plus - U_minus
+        p_virial = (p_virial / (2 * dh)).in_units_of(p_kinetic.unit)
+        p_virial = (
+            p_virial._value + np.tril(p_virial).T
+            - np.diag(np.diag(p_virial))
+        ) * p_virial.unit
+
+    return (
+        (p_kinetic + p_virial) / (unit.AVOGADRO_CONSTANT_NA * volume)
+    ).in_units_of(unit.atmosphere)
```

### Comparing `mdhelper-0.0.2/src/mdhelper/openmm/topology.py` & `mdhelper-1.0.0/src/mdhelper/openmm/topology.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 OpenMM topology transformations
 ===============================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
-This module contains implementations of common OpenMM topology 
+This module contains implementations of common OpenMM topology
 transformations, like the generation of initial particle positions and
 subsetting existing topology objects.
 """
 
+from itertools import repeat
 from typing import Any, Iterable, Union
 
 import numpy as np
 from openmm import app
 
 from ..algorithm import topology as t
 
@@ -23,16 +24,17 @@
     This is an alias function. For more information, see
     :func:`mdhelper.algorithm.topology.create_atoms`.
     """
 
     return t.create_atoms(*args, **kwargs)
 
 def _get_hierarchy_indices(
-        item: Union[app.Atom, app.topology.Bond, app.Residue, app.Chain]
-    ) -> tuple[set, set, set, set]:
+        item: Union[app.Atom, app.topology.Bond, app.Residue, app.Chain],
+        bonds: dict[str, list]
+    ) -> tuple[set[int], set[int], set[int], set[int]]:
 
     """
     Get unique indices of all topology items related to the one passed
     to this function.
 
     For an atom, the indices of itself, the residue it belongs to, and
     the chain that its residue belongs to are returned.
@@ -65,191 +67,193 @@
         Indices of all residues associated with `item`.
 
     chains : `set`
         Indices of all chains associated with `item`.
     """
 
     if isinstance(item, app.Atom):
-        return {item.index}, set(), {item.residue.index}, {item.residue.chain.index}
+        return {item.index}, set(), {item.residue.index}, \
+               {item.residue.chain.index}
 
     elif isinstance(item, app.topology.Bond):
-        return {item.atom1.index, item.atom2.index}, {b.index}, \
+        return {item.atom1.index, item.atom2.index}, {bonds.index(item)}, \
                {item.atom1.residue.index, item.atom2.residue.index}, \
                {item.atom1.residue.chain.index, item.atom2.residue.chain.index}
 
     elif isinstance(item, app.Residue):
         return {a.index for a in item.atoms()}, \
-               {b.index for b in item.bonds()}, {item.index}, {item.chain.index}
+               {bonds.index(b) for b in item.bonds()}, {item.index}, \
+               {item.chain.index}
 
     elif isinstance(item, app.Chain):
-        atoms = set()
-        bonds = set()
-        residues = set()
+        atom_indices = set()
+        bond_indices = set()
+        residue_indices = set()
         for residue in item.residues():
-            a, b, r, _ = _get_hierarchy_indices(residue)
-            atoms |= a
-            bonds |= b
-            residues |= r
-        return atoms, bonds, residues, {item}
+            a, b, r, _ = _get_hierarchy_indices(residue, bonds)
+            atom_indices |= a
+            bond_indices |= b
+            residue_indices |= r
+        return atom_indices, bond_indices, residue_indices, {item.index}
 
 def _is_topology_object(obj: Any):
 
     """
     Check if the argument is a topology item.
 
     Parameters
     ----------
     obj : `Any`
         Any object.
-    
+
     Returns
     -------
     is_topology_object : `bool`
         Boolean value indicating whether `obj` is a topology item.
     """
     return isinstance(obj, (app.Atom, app.topology.Bond, app.Residue, app.Chain))
 
-def subset(
-        topology: app.Topology, positions: np.ndarray = None, *,
-        delete: Iterable[Union[int, app.Atom, app.topology.Bond, app.Residue,
-                               app.Chain]] = None,
-        keep: Iterable[Union[int, app.Atom, app.topology.Bond, app.Residue,
-                             app.Chain]] = None,
+def get_subset(
+        topology: app.Topology, positions: np.ndarray[float], *,
+        delete: list[Any] = None, keep: list[Any] = None,
         types: Union[str, Iterable[str]] = None
-    ) -> Union[app.Topology, np.ndarray]:
+    ) -> Union[app.Topology, np.ndarray[float]]:
 
-    """
-    Creates a topology subset and get its corresponding particle positions.
+    r"""
+    Creates a topology subset and gets its corresponding particle positions.
 
     Parameters
     ----------
     topology : `openmm.app.Topology`
         OpenMM topology.
 
     positions : `numpy.ndarray`
         Positions of the :math:`N` particles in the topology.
 
         **Shape**: :math:`(N,\,3)`.
 
     delete : array-like, keyword-only, optional
-        `openmm.app.Atom`, `openmm.app.Bond`, `openmm.app.Residue`, 
-        and/or `openmm.app.Chain` objects, or the indices of those 
-        objects. If indices are provided, their corresponding object 
+        `openmm.app.Atom`, `openmm.app.Bond`, `openmm.app.Residue`,
+        and/or `openmm.app.Chain` objects, or the indices of those
+        objects. If indices are provided, their corresponding object
         types (:code:`"atom"`, :code:`"residue"`, :code:`"chain"`) must
         be provided in `types`. The specified items will be deleted from
-        the model. 
-        
+        the model.
+
         .. note::
-        
+
            Only one of `delete` and `keep` can be specified.
-    
+
     keep : array-like, keyword-only, optional
-        `openmm.app.Atom`, `openmm.app.Bond`, `openmm.app.Residue`, 
-        and/or `openmm.app.Chain` objects, or the indices of those 
+        `openmm.app.Atom`, `openmm.app.Bond`, `openmm.app.Residue`,
+        and/or `openmm.app.Chain` objects, or the indices of those
         objects. If indices are provided, their corresponding object
         types (:code:`"atom"`, :code:`"residue"`, :code:`"chain"`) must
         be provided in `types`. The specified items will be kept in the
         model.
 
         .. note::
-        
+
            Only one of `delete` and `keep` can be specified.
 
     types : `str` or array-like, keyword-only, optional
-        Object types corresponding to the indices provided in `delete` 
+        Object types corresponding to the indices provided in `delete`
         or `keep`. If a `str` is provided, all items in the array are
-        assumed to have the same object type.
+        assumed to have the same object type. Must be provided if not
+        all items in `delete` or `keep` are OpenMM topology objects.
 
     Returns
     -------
     topology : `openmm.app.Topology`
         OpenMM topology subset.
 
     positions : `numpy.ndarray`
         Positions of the remaining :math:`N_\mathrm{rem}` particles in
         the topology.
 
         **Shape**: :math:`(N_\mathrm{rem},\,3)`.
     """
 
     # Set boolean flags for subroutines below
-    fd, fk = delete is not None, keep is not None
+    found = (delete is not None, keep is not None)
 
     # Check if both delete and keep arguments were provided
-    if fd and fk:
+    if all(found):
         emsg = ("Only specify topology items to either delete or keep. "
                 "When both types are specified, the atoms, bonds, "
                 "residues, and/or chains to be removed from the topology "
                 "become ambiguous.")
         raise ValueError(emsg)
 
-    # Ensure object type(s) are provided
-    if (fd or fk) and types is None:
-        emsg = ("Object types must be provided for the specified "
-                f"topology items to be {'kept' if fk else 'deleted'}.")
+    # Return original topology and positions if no items are specified
+    elif not any(found):
+        return topology, positions
+
+    # Ensure object type(s) are provided if not all items are topology
+    # objects
+    elif types is None \
+            and not all(_is_topology_object(i) for i in
+                        next(a for a in [delete, keep] if a is not None)):
+        emsg = ("Object types must be specified for the topology items "
+                f"to be {'kept' if found[0] else 'deleted'}.")
         raise ValueError(emsg)
 
-    # Create dictionary with topology subitems
-    model = {
-        "atom": np.fromiter(topology.atoms(), dtype=object),
-        "bond": np.fromiter(topology.bonds(), dtype=object),
-        "chain": np.fromiter(topology.chains(), dtype=object),
-        "residue": np.fromiter(topology.residues(), dtype=object)
-    }
-
-    # Create OpenMM modeller
-    Modeller = app.Modeller(topology, positions)
-
-    # If indices and types of objects to be deleted are specified,
-    # create an iterable object of corresponding items from the
-    # dictionary
-    if fd and types is not None:
-        delete = (i if _is_topology_object(i)
-                    else model[types][i]
-                    for i in delete) if isinstance(types, str) \
-                 else (i if _is_topology_object(i) else model[t][i]
-                         for i, t in zip(delete, types))
-
-    elif fk:
-        
-        # Preallocate sets to store indices of atoms, residues, and
-        # chains to delete
-        atoms = set()
-        bonds = set()
-        residues = set()
-        chains = set()
-
-        # Remove items to be kept from the master list of topology
-        # subitems to delete
-        if isinstance(types, str):
-            for item in keep:
-                a, b, r, c = _get_hierarchy_indices(
-                    item if _is_topology_object(item)
-                         else model[types][item]
-                )
-                atoms |= a
-                bonds |= b
-                residues |= r
-                chains |= c   
+    # Create a generator of types if a string is provided
+    elif isinstance(types, str):
+        same = True
+        types = repeat(types)
+    elif types is not None:
+        same = all(t == "atoms" for t in types)
+
+    # Create OpenMM Modeller
+    modeller = app.Modeller(topology, positions)
+
+    if types is not None:
+
+        # Create dictionary with topology subitems
+        model = {
+            "atom": list(topology.atoms()),
+            "bond": list(topology.bonds()),
+            "chain": list(topology.chains()),
+            "residue": list(topology.residues())
+        }
+
+        # If indices and types of objects to be deleted are specified,
+        # create an iterable object of corresponding items from the
+        # dictionary
+        if found[0]:
+            delete = (i if _is_topology_object(i) else model[t][i]
+                    for i, t in zip(delete, types))
         else:
+
+            # Preallocate sets to store indices of atoms, residues, and
+            # chains to keep
+            atoms = set()
+            bonds = set()
+            residues = set()
+            chains = set()
+
+            # Remove items to be kept from the master list of topology
+            # subitems to delete
             for item, item_type in zip(keep, types):
-                a, b, r, c = _get_hierarchy_indices(
-                    item if _is_topology_object(item)
-                         else model[item_type][item]
-                )
+                if not _is_topology_object(item):
+                    item = model[item_type][item]
+                a, b, r, c = _get_hierarchy_indices(item, model["bond"])
                 atoms |= a
                 bonds |= b
                 residues |= r
                 chains |= c
 
-        delete = np.hstack((
-            np.delete(model["atom"], list(atoms)),
-            np.delete(model["bond"], list(bonds)),
-            np.delete(model["residue"], list(residues)),
-            np.delete(model["chain"], list(chains))
-        ))
+            model["atom"] = np.delete(model["atom"], list(atoms))
+            model["residue"] = np.delete(model["residue"], list(residues))
+            model["chain"] = np.delete(model["chain"], list(chains))
+            if not bonds and same:
+                model["bond"] = []
+            else:
+                for i in sorted(bonds, reverse=True):
+                    del model["bond"][i]
+            delete = [i for t in model.values() for i in t]
 
     # Create subset by deleting objects from original topology
-    if delete is not None:
-        Modeller.delete(delete)
+    modeller.delete(delete)
 
-    return Modeller.topology, Modeller.positions
+    return modeller.topology, modeller.positions
```

### Comparing `mdhelper-0.0.2/src/mdhelper/openmm/utility.py` & `mdhelper-1.0.0/src/mdhelper/openmm/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """
 OpenMM utility functions
 ========================
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 This module contains OpenMM-related utility functions.
 """
 
 from datetime import datetime
 import itertools
+import logging
 from typing import Union
 
 import numpy as np
 import openmm
 from openmm import unit
 
-from ..utility import log
-
 def _create_context(
         system: openmm.System, integrator: openmm.Integrator,
-        positions: np.ndarray, platform: openmm.Platform, properties: dict
-    ) -> openmm.Context:
+        positions: np.ndarray[float], platform: openmm.Platform,
+        properties: dict) -> openmm.Context:
 
-    """
+    r"""
     Creates an OpenMM Context by cloning the Integrator passed to this
     function. Useful for benchmarking different simulation systems.
 
     Parameters
     ----------
     system : `openmm.System`
         OpenMM molecular system.
@@ -35,73 +34,73 @@
 
     positions : `np.ndarray` or `unit.Quantity`
         Initial positions of the :math:`N` particles in the system.
 
         **Shape**: :math:`(N,\,3)`.
 
         **Reference unit**: :math:`\mathrm{nm}`.
-    
+
     platform : `openmm.Platform`
         OpenMM platform.
 
     properties : `dict`
         Dictionary of platform-specific properties.
-    
+
     Returns
     -------
     context : `openmm.Context`
         OpenMM simulation context.
     """
 
-    Integrator = openmm.XmlSerializer.clone(integrator)
-    Context = openmm.Context(system, Integrator, platform, properties)
-    Context.setPositions(positions)
-    return Context
+    integrator = openmm.XmlSerializer.clone(integrator)
+    context = openmm.Context(system, integrator, platform, properties)
+    context.setPositions(positions)
+    return context
 
-def _time_integrator(context: openmm.Context, steps: int) -> float:
+def _benchmark_integrator(context: openmm.Context, steps: int) -> float:
 
     """
     Benchmarks the performance of an OpenMM Integrator.
 
     Parameters
     ----------
     context : `openmm.Context`
         OpenMM simulation context.
-    
+
     Returns
     -------
     time : `float`
         Elapsed time, in seconds.
     """
-    
+
     start = datetime.now()
     context.getIntegrator().step(steps)
     return (datetime.now() - start).total_seconds()
 
 def optimize_pme(
         system: openmm.System, integrator: openmm.Integrator,
-        positions: Union[np.ndarray, unit.Quantity],
+        positions: Union[np.ndarray[float], unit.Quantity],
         platform: openmm.Platform, properties: dict,
         min_cutoff: Union[float, unit.Quantity],
         max_cutoff: Union[float, unit.Quantity], *,
         pmeforce: openmm.NonbondedForce = None, cpu_pme: bool = True,
         target: float = 10, target_std: float = None, window: int = 3,
         fastest: int = 5, rerun: int = 2, verbose: bool = True
     ) -> tuple[unit.Quantity, bool]:
-    
+
     """
     Run a series of simulations using different parameters to determine
     the optimal configuration for evaluating electrostatic interactions
     with the particle mesh Ewald (PME) method on a GPU (CUDA or OpenCL).
 
     The cutoff distance for the Coulomb potential can be freely varied
     with no accuracy penalty since OpenMM automatically selects internal
     parameters to satisfy the specified error tolerance. However, it may
     affect the accuracy of other nonbonded interactions, so care must be
-    taken to ensure the optimal Coulomb potential cutoff is compatible 
+    taken to ensure the optimal Coulomb potential cutoff is compatible
     with the other pair potentials in the system.
 
     In certain cases, OpenMM can perform better with the reciprocal
     space calculations being done on the CPU while the direct space
     calculations are being evaluated on the GPU.
 
     Parameters
@@ -111,49 +110,49 @@
 
     integrator : `openmm.Integrator`
         OpenMM integrator or thermostat.
 
     positions : `np.ndarray` or `unit.Quantity`
         Initial positions of the :math:`N` particles in the system.
 
-        **Shape**: :math:`(N,\,3)`.
+        **Shape**: :math:`(N,\\,3)`.
+
+        **Reference unit**: :math:`\\mathrm{nm}`.
 
-        **Reference unit**: :math:`\mathrm{nm}`.
-    
     platform : `openmm.Platform`
         OpenMM platform.
 
     properties : `dict`
         Dictionary of platform-specific properties.
-    
+
     min_cutoff : `float` or `unit.Quantity`
         Minimum cutoff distance to test.
 
-        **Reference unit**: :math:`\mathrm{nm}`.
+        **Reference unit**: :math:`\\mathrm{nm}`.
 
     max_cutoff : `float` or `unit.Quantity`
         Maximum cutoff distance to test.
 
-        **Reference unit**: :math:`\mathrm{nm}`.
+        **Reference unit**: :math:`\\mathrm{nm}`.
 
     pmeforce : `openmm.NonbondedForce` or `openmm.AmoebaMultipoleForce`, \
     keyword-only, optional
         Pair potential with electrostatic interactions that are
         evaluated using PME.
 
     cpu_pme : `bool`, keyword-only, default: :code:`True`
         Determines whether CPU PME should be benchmarked.
 
     target : `float`, keyword-only, default: :code:`10`
-        Target simulation time for each test run, in seconds. 
+        Target simulation time for each test run, in seconds.
 
     target_std : `float`, keyword-only, optional
         Allowed variability for `target`, in seconds. If set to a value
-        that is too small, the target simulation time may never be 
-        satisfied. If not specified, it is set to 10% of `target`. 
+        that is too small, the target simulation time may never be
+        satisfied. If not specified, it is set to 10% of `target`.
 
     window : `int`, keyword-only, default: :code:`3`
         Number of previous runs to look at before deciding whether to
         stop testing larger cutoffs.
 
     fastest : `int`, keyword-only, default: :code:`5`
         Number of fastest configurations to retest before deciding on
@@ -166,21 +165,26 @@
         Determines whether detailed progress is shown.
 
     Returns
     -------
     cutoff : `unit.Quantity`
         Optimal cutoff distance.
 
-        **Reference unit**: :math:`\mathrm{nm}`.
-    
+        **Reference unit**: :math:`\\mathrm{nm}`.
+
     cpu_pme : `bool`
-        Specifies whether to use the CPU to perform reciprocal space 
+        Specifies whether to use the CPU to perform reciprocal space
         calculations.
     """
 
+    # Set up logger
+    logging.basicConfig(format="{asctime} | {levelname:^8s} | {message}",
+                        style="{",
+                        level=logging.INFO if verbose else logging.WARNING)
+
     # Get information about the pair potential of interest
     if pmeforce is None:
         for force in system.getForces():
             if isinstance(force, (openmm.NonbondedForce,
                                   openmm.AmoebaMultipoleForce)):
                 pmeforce = force
                 break
@@ -189,60 +193,57 @@
                         "not being evaluated using the particle mesh "
                         "Ewald (PME) method.")
     cpu_pme &= isinstance(pmeforce, openmm.NonbondedForce) \
                and platform.supportsKernels(["CalcPmeReciprocalForce"])
     tol = pmeforce.getEwaldErrorTolerance()
 
     # Determine the number of timesteps to run for each cutoff distance
-    if verbose:
-        log("Finding reasonable number of timesteps for PME optimizer...")
+    logging.info("Determining a reasonable number of timesteps for PME optimizer...")
     pmeforce.setCutoffDistance(np.sqrt(min_cutoff * max_cutoff))
     properties["UseCpuPme"] = "false"
-    Context = _create_context(system, integrator, positions, platform,
+    context = _create_context(system, integrator, positions, platform,
                               properties)
     if target_std is None:
         target_std = 0.1 * target
     time_width = max(9, np.ceil(np.log10(target)).astype(int) + 7)
     lb, ub = target - target_std, target + target_std
     steps, time = 20, 0
     while True:
-        time = _time_integrator(Context, steps)
-        if verbose:
-            log(f"\tGPU: {steps:14,} ts "
-                f"===> {time:{time_width}.5f} s elapsed")
+        time = _benchmark_integrator(context, steps)
+        logging.info(f"  GPU: {steps:14,} ts "
+                     f"===> {time:{time_width}.5f} s elapsed")
         if lb < time < ub:
             break
         steps = int(target * steps / time)
     if cpu_pme:
         properties["UseCpuPme"] = "true"
-        Context = _create_context(system, integrator, positions, platform,
+        context = _create_context(system, integrator, positions, platform,
                                   properties)
         steps_cpu, time = 20, 0
         while True:
-            time = _time_integrator(Context, steps_cpu)
-            if verbose:
-                log.log(f"\tCPU: {steps_cpu:14,} ts "
-                        f"===> {time:{time_width}.5f} s elapsed")
+            time = _benchmark_integrator(context, steps_cpu)
+            logging.info(f"  CPU: {steps_cpu:14,} ts "
+                         f"===> {time:{time_width}.5f} s elapsed")
             if lb < time < ub:
                 break
             steps_cpu = int(target * steps_cpu / time)
         steps = min(steps, steps_cpu)
     steps = np.round(steps, 2 - np.ceil(np.log10(steps)).astype(int))
-    log(f"Starting PME optimizer (using {steps:,} timesteps)...")
+    logging.info(f"Starting PME optimizer (using {steps:,} timesteps)...")
 
     # Build list of cutoff distances to test
     if isinstance(min_cutoff, unit.Quantity):
-        min_cutoff /= unit.nanometer
+        min_cutoff = min_cutoff.value_in_unit(unit.nanometer)
     if isinstance(max_cutoff, unit.Quantity):
-        max_cutoff /= unit.nanometer
+        max_cutoff = max_cutoff.value_in_unit(unit.nanometer)
     cutoffs = {"gpu": {min_cutoff}}
     if cpu_pme:
         cutoffs["cpu"] = {min_cutoff}
 
-    for dim in [v[i] / unit.nanometer
+    for dim in [v[i].value_in_unit(unit.nanometer)
                 for i, v in enumerate(system.getDefaultPeriodicBoxVectors())]:
 
         # Iterate through possible grid sizes
         for n_mesh in itertools.count(start=5):
 
             # Check if grid size is legal for FFT
             check = n_mesh
@@ -259,62 +260,60 @@
             if cutoff < min_cutoff:
                 break
             if cutoff < max_cutoff:
                 if cpu_pme:
                     cutoffs["cpu"].add(cutoff)
                 if check == 1:
                     cutoffs["gpu"].add(cutoff)
-    
+
     # Get preliminary times for the different architectures and cutoffs
     cutoff_width = max(7, np.ceil(
         np.log10(max(max(v) for v in cutoffs.values()))
     ).astype(int) + 6)
     times = {}
     for arch, cut in cutoffs.items():
-        cutoffs[arch] = np.array(sorted(cut), dtype=float)
-        times[arch] = np.empty(cutoffs[arch].shape, dtype=float)
+        cutoffs[arch] = np.array(sorted(cut))
+        times[arch] = np.empty(cutoffs[arch].shape)
         times[arch][:] = np.nan
         for i, cutoff in enumerate(cutoffs[arch]):
             pmeforce.setCutoffDistance(cutoff)
             properties["UseCpuPme"] = str(arch == "cpu").lower()
-            Context = _create_context(system, integrator, positions, platform,
+            context = _create_context(system, integrator, positions, platform,
                                       properties)
-            times[arch][i] = _time_integrator(Context, steps)
-            if verbose:
-                log(f"\t{arch.upper()}: {cutoff:{cutoff_width}.4f} nm cutoff "
-                    f"===> {times[arch][i]:{time_width}.5f} s elapsed")
+            times[arch][i] = _benchmark_integrator(context, steps)
+            logging.info(f"  {arch.upper()}: {cutoff:{cutoff_width}.4f} nm cutoff "
+                         f"===> {times[arch][i]:{time_width}.5f} s elapsed")
 
             # Stop iteration if simulation is continuously getting slower
-            if i > 3 and np.all(times[arch][i - window:i] > 
-                                times[arch][i - window - 1:i - 1]):
+            if i > window and np.all(times[arch][i - window:i] >
+                                     times[arch][i - window - 1:i - 1]):
                 break
     best = sorted([t, c, a] for a in times.keys()
                             for c, t in zip(cutoffs[a], times[a]))[:fastest]
-    
+
     # Rerun the fastest configurations to ensure correct results
     for i, (time, cutoff, arch) in enumerate(best):
         pmeforce.setCutoffDistance(cutoff)
         properties["UseCpuPme"] = str(arch == "cpu").lower()
-        Context = _create_context(system, integrator, positions, platform,
+        context = _create_context(system, integrator, positions, platform,
                                   properties)
 
         # Replace preliminary time with median time from reruns
         best[i][0] = sorted(
-            (time, *[_time_integrator(Context, steps) for _ in range(rerun)])
+            (time, *[_benchmark_integrator(context, steps) for _ in range(rerun)])
         )[1]
     best.sort()
 
     # Display fastest configurations and timings
     time_width = 8 + 2 * np.ceil(max(0, time_width - 8) // 2).astype(int)
     cutoff_width = 11 + 2 * np.ceil(max(0, cutoff_width - 11) // 2).astype(int)
-    if verbose:
-        log(f"PME optimization completed.\n\t"
-            f" Rank | {'Time (s)':^{time_width}} "
-            f"| {'Cutoff (nm)':^{cutoff_width}} | CPU PME\n\t"
-            f"------|{'-' * (time_width + 2)}"
-            f"|{'-' * (cutoff_width + 2)}|---------\n\t" +
-            "\n\t".join(f" {i + 1:>4} | {time:{time_width}.5f} |"
-                        f" {cutoff:{cutoff_width}.4f} | {arch == 'cpu'}"
-                        for i, (time, cutoff, arch) in enumerate(best)))
+    logging.info(f"PME optimization completed.\n"
+                 f"   Rank | {'Time (s)':^{time_width}} "
+                 f"| {'Cutoff (nm)':^{cutoff_width}} | CPU PME\n"
+                 f"  ------|{'-' * (time_width + 2)}"
+                 f"|{'-' * (cutoff_width + 2)}|---------\n  " +
+                 "\n  ".join(f" {i + 1:>4} | {time:{time_width}.5f} |"
+                             f" {cutoff:{cutoff_width}.4f} | {arch == 'cpu'}"
+                             for i, (time, cutoff, arch) in enumerate(best)))
 
     # Return optimized configuration
     return best[0][1] * unit.nanometer, arch == "cpu"
```

### Comparing `mdhelper-0.0.2/src/mdhelper/plot/axis.py` & `mdhelper-1.0.0/src/mdhelper/plot/axis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 """
 Axis components
 ===============
-.. moduleauthor:: Benjamin B. Ye <bye@caltech.edu>
+.. moduleauthor:: Benjamin Ye <GitHub: @bbye98>
 
 This module provides additional functionality for Matplotlib axes.
 """
 
+from typing import Any
+
 import matplotlib as mpl
 import numpy as np
 
-def tabular_legend(
-        rows: list, cols: list, *, hlabel: str = None, vlabel: str = None,
-        hla: str = "left", vla: str = "top", condense: bool = False,
-        **kwargs: ...) -> tuple[dict, int, int]:
+def set_up_tabular_legend(
+        rows: list[str], cols: list[str], *, hlabel: str = None,
+        vlabel: str = None, hla: str = "left", vla: str = "top",
+        condense: bool = False, **kwargs) -> tuple[dict[str, Any], int, int]:
 
     r"""
     Sets up a tabular legend for a :class:`matplotlib.axes.Axes` object.
-    
+
     Parameters
     ----------
     rows : `tuple` or `list`
         Raw string representations of the row values.
 
     cols : `tuple` or `list`
         Raw string representations of the column values.
 
-    Other parameters
-    ----------------
-    hlabel : `str`, optional
+    hlabel : `str`, keyword-only, optional
         Horizontal label for column values.
 
-    vlabel : `str`, optional
+    vlabel : `str`, keyword-only, optional
         Vertical label for row values.
 
-    hla : `str`, default: :code:`"left"`
+    hla : `str`, keyword-only, default: :code:`"left"`
         Alignment for `hlabel`.
 
         .. container::
 
            **Valid values**:
 
            * :code:`"left"`: Left-aligned text.
            * :code:`"center"`: Horizontally centered text.
 
-    vla : `str`, default: :code:`"top"`
+    vla : `str`, keyword-only, default: :code:`"top"`
         Alignment for `vlabel`.
 
         .. container::
 
            **Valid values**:
 
            * :code:`"top"`: Top-aligned text.
            * :code:`"center"`: Vertically centered text.
 
-    condense : `bool`, default: :code:`False`
+    condense : `bool`, keyword-only, default: :code:`False`
         Condenses the legend by placing `vlabel` in the empty top-left
         corner. Cannot be used when no `vlabel` is specified or in
         conjuction with :code:`vla="center"` (which will take priority).
 
     **kwargs :
         Keyword arguments passed to :meth:`matplotlib.axes.Axes.legend`.
 
@@ -65,17 +65,17 @@
     -------
     properties : `dict`
         Properties of the tabular legend to be unpacked and used in the
         :meth:`matplotlib.axes.Axes.legend` call.
 
         .. container::
 
-           * handles (`list`): :obj:`matplotlib.artist` objects to be 
+           * handles (`list`): :obj:`matplotlib.artist` objects to be
              added to the legend.
-           * labels (`list`): Labels to be shown next to the 
+           * labels (`list`): Labels to be shown next to the
              :obj:`matplotlib.artist` objects in the legend.
            * ncol (`int`): Number of columns in the legend.
            * kwargs (`dict`): Keyword arguments passed to
              :meth:`matplotlib.axes.Axes.legend`.
 
     nrow : `int`
         Number of rows in the legend.
@@ -92,45 +92,47 @@
     shorter values using the width of the largest
     :class:`matplotlib.transforms.Bbox` in the first column. Sample code
     for use in your main script utilizing the outputs of this function is
     provided below:
 
     .. code-block::
 
-        (props, nrow, start) = tabular_legend(..., handletextpad=-5/4)
-        fig, ax = plt.subplots(...)
-        for i, x in enumerate(...):
-            for j, y in enumerate(...):
-                props["handles"][start + i * nrow + j], = ax.plot(...)
-        ax.set_xlabel(...)
-        ax.set_ylabel(...)
-        lgd = ax.legend(**props)
-        fig.canvas.draw()
-        texts = lgd.get_texts()[:nrow]
-        bounds = [t.get_window_extent().bounds[2] / 2 for t in texts]
-        center = max(bounds)
-        for k, t in enumerate(texts):
-            t.set_position((center - bounds[k], 0))
-        plt.show()
+       (props, nrow, start) = tabular_legend(..., handletextpad=-5/4)
+       fig, ax = plt.subplots(...)
+       for i, x in enumerate(...):
+           for j, y in enumerate(...):
+               props["handles"][start + i * nrow + j], = ax.plot(...)
+       ax.set_xlabel(...)
+       ax.set_ylabel(...)
+       lgd = ax.legend(**props)
+       fig.canvas.draw()
+       texts = lgd.get_texts()[:nrow]
+       bounds = [t.get_window_extent().bounds[2] / 2 for t in texts]
+       center = max(bounds)
+       for k, t in enumerate(texts):
+           t.set_position((center - bounds[k], 0))
+       plt.show()
     """
 
     hpad = bool(vlabel) - condense + 1
     vpad = bool(hlabel) + 1
     nrow = len(rows) + vpad
     ncol = len(cols) + hpad
 
     labels = ["" for _ in range(nrow * ncol)]
     if vlabel:
         labels[vpad + (len(rows) // 2 if vla == "center" else -condense)] = vlabel
     iv = vpad + nrow * (bool(vlabel) - condense)
     labels[iv:iv + len(rows)] = rows
     if hlabel:
-        labels[(2 + (hla == "center") * (int(np.ceil(len(cols) / 2)) - 1)) * nrow] = hlabel
+        labels[
+            (2 + (hla == "center") * (int(np.ceil(len(cols) / 2)) - 1)) * nrow
+        ] = hlabel
     labels[hpad * nrow + bool(hlabel)::nrow] = cols
 
     return {
-        "handles": [mpl.patches.Rectangle((0, 0), 0.1, 0.1, ec="none", fill=False) 
+        "handles": [mpl.patches.Rectangle((0, 0), 0.1, 0.1, ec="none", fill=False)
                     for _ in range(len(labels))],
-        "labels": labels, 
+        "labels": labels,
         "ncol": ncol,
         **kwargs
     }, nrow, iv + nrow
```

### Comparing `mdhelper-0.0.2/src/mdhelper.egg-info/PKG-INFO` & `mdhelper-1.0.0/src/mdhelper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mdhelper
-Version: 0.0.2
+Version: 1.0.0
 Summary: A batteries-included toolkit of analysis modules and helper functions 
-Author-email: "Benjamin B. Ye" <bye@caltech.edu>
+Author-email: "Benjamin B. Ye" <bye@caltech.edu>, "Pierre J. Walker" <pjwalker@caltech.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -680,152 +680,91 @@
 Project-URL: Homepage, https://github.com/bbye98/mdhelper
 Project-URL: Bug Tracker, https://github.com/bbye98/mdhelper/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: mdanalysis
+Requires-Dist: netCDF4
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pint
+Requires-Dist: scipy
+Requires-Dist: sympy
+
+<img src="https://raw.githubusercontent.com/bbye98/mdhelper/main/assets/logo.png" align="right" width="256"/>
 
 # MDHelper
 
-MDHelper is a batteries-included toolkit of analysis modules and helper
+[![continuous-integration](https://github.com/bbye98/mdhelper/actions/workflows/ci.yml/badge.svg)](https://github.com/bbye98/mdhelper/actions/workflows/ci.yml)
+
+MDHelper is a toolkit of optimized analysis modules and helper
 functions for molecular dynamics (MD) simulations.
 
 * **Documentation**: https://bbye98.github.io/mdhelper/
+* **Conda**: https://anaconda.org/bbye98/mdhelper
 * **Python Package Index (PyPI)**: https://pypi.org/project/mdhelper/
 
 Note that MDHelper is currently an *experimental* library that has 
 only been tested on Linux and may contain bugs and issues. If you come 
-across one, please 
-[submit a new issue](https://github.com/bbye98/mdhelper/issues/new). If 
-you would like to contribute to MDHelper, please 
-[submit a pull request](https://github.com/bbye98/mdhelper/compare).
+across one or would like to request new features, please 
+[submit a new issue](https://github.com/bbye98/mdhelper/issues/new).
 
 ## Features
 
 * [`algorithm`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/algorithm): 
-Efficient NumPy algorithms for data wrangling and evaluating structural 
-and dynamical properties.
+Efficient NumPy and SciPy algorithms for data wrangling and evaluating 
+structural and dynamical properties.
 * [`analysis`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/analysis): 
 Serial and parallel data analysis tools built on top of the MDAnalysis 
 framework.
 * [`fit`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/fit): 
 Two-dimensional curve fitting models for use with SciPy.
+* [`lammps`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/lammps):
+Helper functions for setting up LAMMPS simulations.
 * [`openmm`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/openmm): 
 Extensions to the high-performance OpenMM toolkit, such as custom 
 bond/pair potentials, support for NetCDF trajectories, and much more.
 * [`plot`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/plot): 
 Settings and additional functionality for Matplotlib figures.
-* [`utility`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/utility): 
-General utility functions.
-
-## Installation and usage
-
-### Prerequisites
-
-If you use pip to manage your Python packages or plan on using OpenMM
-with third-party extensions, such as 
-[`constvplugin`](https://github.com/scychon/openmm_constV) for the
-method of image charges, you must compile and install OpenMM prior to
-installing MDHelper. See the 
-["Compiling OpenMM from Source Code"](http://docs.openmm.org/latest/userguide/library/02_compiling.html) 
-for more section of the OpenMM User Guide for more information. This 
-additional step is necessary since precompiled versions of OpenMM do not
-expose their header files, which are needed to link against custom 
-plugins. Otherwise, the lastest precompiled version of OpenMM on 
-conda-forge will be installed during the installation of MDHelper.
-
-### Virtual environment
-
-It is recommended, but not necessary, that you create a virtual 
-environment to prevent dependency conflicts.
-
-If you are using pip to manage Python packages, use
-
-    virtualenv venv
-    source venv/bin/activate
-
-where `venv` is the name of the new environment.
-
-If you are using Anaconda or Miniconda, use
-
-    conda create --name venv
-    conda activate venv
-
-### Install using pip
-
- 1. Install MDHelper and its dependencies using 
-
-    pip install mdhelper
-
-### Install using Anaconda or Miniconda
-
- 1. Add the conda-forge channel using
-
-        conda config --add channels conda-forge
 
- 2. Install MDHelper and its dependencies using
+## Installation
 
-        conda install mdhelper
+MDHelper requires Python 3.9 or later.
 
-### Build from source
+For the most up-to-date version of MDHelper, clone the repository and install
+the package using pip:
 
- 1. Ensure that the latest version of the Python build frontend, 
-    `build`, is installed:
+    git clone https://github.com/bbye98/mdhelper.git
+    cd mdhelper
+    python -m pip install -e .
 
-        python3 -m pip install --upgrade build
+MDHelper is also available on Conda and PyPI:
 
- 2. Create a local copy of the MDHelper repository on your machine using
+    conda install -c bbye98 mdhelper
+    python -m pip install mdhelper
 
-        git clone https://github.com/bbye98/mdhelper.git
-
- 3. Enter the root directory of MDHelper using
-
-        cd mdhelper
-
- 4. Build the MDHelper wheel using
-
-        python3 -m build
-
-    The Python wheel will be placed in the `dist` directory.
-
- 5. Install MDHelper using
-
-        python3 -m pip install dist/mdhelper-<version>-py3-none-any.whl
-
-    where `<version>` is the version of MDHelper you are installing.
-
-### Portable package
-
- 1. Change to the directory where you want to store a copy of MDHelper using
-
-        cd <directory>
-
-    where `<directory>` is the relative path to the desired directory.
-    
-    If you are already in the correct location, skip this step.
-
- 2. Create a local copy of the MDHelper repository on your machine using
-
-        git clone https://github.com/bbye98/mdhelper.git
-
- 3. Enter the root directory of MDHelper using
-
-        cd mdhelper
-
- 4. Install the dependencies using
+### Prerequisites
 
-        pip install -r requirements.txt
+If you use pip to manage your Python packages, you must compile and 
+install OpenMM prior to installing MDHelper since OpenMM is not 
+available in PyPI. See the 
+["Compiling OpenMM from Source Code"](http://docs.openmm.org/latest/userguide/library/02_compiling.html) 
+section of the OpenMM User Guide for more information.
 
-    or
+If you use Conda, it is recommended that you use the conda-forge 
+channel to install dependencies. To make conda-forge the default 
+channel, use
 
-        conda install --file requirements.txt
+    conda config --add channels conda-forge
 
- 5. Once done, you can use MDHelper by first adding the path to the 
-    `src` directory in your Python scripts:
+### Postrequisites
 
-        import sys
-        sys.path.insert(0, "/path/to/mdhelper/src")
-        import mdhelper
+To use the image of method charges 
+(`mdhelper.openmm.system.add_image_charges()`) in your OpenMM simulations, you must
+compile and install [`constvplugin`](https://github.com/scychon/openmm_constV) or
+[`openmm-ic-plugin`](https://github.com/bbye98/mdhelper/tree/main/lib/openmm-ic-plugin).
```

### Comparing `mdhelper-0.0.2/src/mdhelper.egg-info/SOURCES.txt` & `mdhelper-1.0.0/src/mdhelper.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 LICENSE
 README.md
 pyproject.toml
 src/mdhelper/__init__.py
-src/mdhelper/utility.py
 src/mdhelper.egg-info/PKG-INFO
 src/mdhelper.egg-info/SOURCES.txt
 src/mdhelper.egg-info/dependency_links.txt
 src/mdhelper.egg-info/requires.txt
 src/mdhelper.egg-info/top_level.txt
 src/mdhelper/algorithm/__init__.py
+src/mdhelper/algorithm/accelerated.py
 src/mdhelper/algorithm/correlation.py
 src/mdhelper/algorithm/molecule.py
 src/mdhelper/algorithm/topology.py
+src/mdhelper/algorithm/unit.py
 src/mdhelper/algorithm/utility.py
 src/mdhelper/analysis/__init__.py
 src/mdhelper/analysis/base.py
+src/mdhelper/analysis/electrostatics.py
 src/mdhelper/analysis/polymer.py
 src/mdhelper/analysis/profile.py
 src/mdhelper/analysis/structure.py
+src/mdhelper/analysis/thermodynamics.py
 src/mdhelper/analysis/transport.py
 src/mdhelper/fit/__init__.py
 src/mdhelper/fit/distribution.py
 src/mdhelper/fit/exponential.py
 src/mdhelper/fit/fourier.py
 src/mdhelper/fit/gaussian.py
 src/mdhelper/fit/polynomial.py
 src/mdhelper/fit/power.py
+src/mdhelper/lammps/__init__.py
+src/mdhelper/lammps/topology.py
 src/mdhelper/openmm/__init__.py
 src/mdhelper/openmm/bond.py
 src/mdhelper/openmm/file.py
 src/mdhelper/openmm/pair.py
 src/mdhelper/openmm/reporter.py
 src/mdhelper/openmm/system.py
 src/mdhelper/openmm/topology.py
 src/mdhelper/openmm/unit.py
 src/mdhelper/openmm/utility.py
 src/mdhelper/plot/__init__.py
 src/mdhelper/plot/axis.py
+src/mdhelper/plot/color.py
 src/mdhelper/plot/rcparam.py
 tests/test_algorithm_correlation.py
 tests/test_algorithm_molecule.py
 tests/test_algorithm_topology.py
+tests/test_algorithm_unit.py
 tests/test_algorithm_utility.py
+tests/test_analysis_electrostatics.py
 tests/test_analysis_polymer.py
 tests/test_analysis_profile.py
 tests/test_analysis_structure.py
-tests/test_analysis_transport.py
+tests/test_analysis_transport.py
+tests/test_openmm_file_reporter.py
+tests/test_openmm_topology.py
+tests/test_openmm_unit.py
```

### Comparing `mdhelper-0.0.2/tests/test_algorithm_correlation.py` & `mdhelper-1.0.0/tests/test_algorithm_correlation.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,53 +2,53 @@
 import sys
 
 import numpy as np
 import pytest
 import tidynamics
 
 sys.path.insert(0, f"{pathlib.Path(__file__).parents[1].resolve().as_posix()}/src")
-from mdhelper.algorithm import correlation
+from mdhelper.algorithm import correlation  # noqa: E402
 
 # Generate random times series
 rng = np.random.default_rng()
 shape = (*rng.integers(2, 50, size=3), 3)
 vectors_ones = np.ones(shape)
 vectors_random_1 = rng.random(shape)
 vectors_random_2 = rng.random(shape)
 
 # Calculate reference ACF and CCF for the random time series using
 # tidynamics
 acf_scalar = tidynamics.acf(vectors_random_1[0, :, 0, 0])
-acf_multi_scalar = np.stack(tidynamics.acf(v) 
-                            for v in vectors_random_1[0, :, :, 0].T).T
-acf_block_scalar = np.stack(tidynamics.acf(v) 
-                            for v in vectors_random_1[:, :, 0, 0])
+acf_multi_scalar = np.stack([tidynamics.acf(v)
+                            for v in vectors_random_1[0, :, :, 0].T]).T
+acf_block_scalar = np.stack([tidynamics.acf(v)
+                             for v in vectors_random_1[:, :, 0, 0]])
 acf_vector = tidynamics.acf(vectors_random_1[0, :, 0])
-acf_multi_vector = np.stack(tidynamics.acf(v) 
-                            for v in np.swapaxes(vectors_random_1[0], 0, 1)).T
-acf_block_vector = np.stack(tidynamics.acf(v) 
-                            for v in vectors_random_1[:, :, 0])
-ccf_scalar = tidynamics.correlation(vectors_random_1[0, :, 0, 0], 
+acf_multi_vector = np.stack([tidynamics.acf(v)
+                             for v in np.swapaxes(vectors_random_1[0], 0, 1)]).T
+acf_block_vector = np.stack([tidynamics.acf(v)
+                             for v in vectors_random_1[:, :, 0]])
+ccf_scalar = tidynamics.correlation(vectors_random_1[0, :, 0, 0],
                                     vectors_random_2[0, :, 0, 0])
-ccf_multi_scalar = np.stack(tidynamics.correlation(v1, v2) 
-                            for v1, v2 in zip(vectors_random_1[0, :, :, 0].T, 
-                                              vectors_random_2[0, :, :, 0].T)).T
-ccf_block_scalar = np.stack(tidynamics.correlation(v1, v2) 
-                            for v1, v2 in zip(vectors_random_1[:, :, 0, 0],
-                                              vectors_random_2[:, :, 0, 0]))
-ccf_vector = tidynamics.correlation(vectors_random_1[0, :, 0], 
+ccf_multi_scalar = np.stack([tidynamics.correlation(v1, v2)
+                             for v1, v2 in zip(vectors_random_1[0, :, :, 0].T,
+                                               vectors_random_2[0, :, :, 0].T)]).T
+ccf_block_scalar = np.stack([tidynamics.correlation(v1, v2)
+                             for v1, v2 in zip(vectors_random_1[:, :, 0, 0],
+                                               vectors_random_2[:, :, 0, 0])])
+ccf_vector = tidynamics.correlation(vectors_random_1[0, :, 0],
                                     vectors_random_2[0, :, 0])
-ccf_multi_vector = np.stack(
-    tidynamics.correlation(v1, v2) 
+ccf_multi_vector = np.stack([
+    tidynamics.correlation(v1, v2)
     for v1, v2 in zip(np.swapaxes(vectors_random_1[0], 0, 1),
                       np.swapaxes(vectors_random_2[0], 0, 1))
-).T
-ccf_block_vector = np.stack(tidynamics.correlation(v1, v2) 
-                            for v1, v2 in zip(vectors_random_1[:, :, 0], 
-                                              vectors_random_2[:, :, 0]))
+]).T
+ccf_block_vector = np.stack([tidynamics.correlation(v1, v2)
+                             for v1, v2 in zip(vectors_random_1[:, :, 0],
+                                               vectors_random_2[:, :, 0])])
 
 def test_func_correlation_fft_acf_errors():
 
     # TEST CASE 1: ACF of empty 1D array
     with pytest.raises(ValueError):
         correlation.correlation_fft(np.empty(0))
 
@@ -76,88 +76,88 @@
     assert np.allclose(correlation.correlation_fft(vectors_ones[:, :, 0, 0]), 1)
 
     # TEST CASE 4: ACF of blocked time series of ones for multiple entities
     assert np.allclose(correlation.correlation_fft(vectors_ones[:, :, :, 0]), 1)
 
     # TEST CASE 5: ACF of time series of 1-vectors
     assert np.allclose(
-        correlation.correlation_fft(vectors_ones[0, :, 0], vector=True), 
+        correlation.correlation_fft(vectors_ones[0, :, 0], vector=True),
         shape[-1]
     )
-    
+
     # TEST CASE 6: ACF of time series of 1-vectors for multiple entities
     assert np.allclose(
         correlation.correlation_fft(vectors_ones[0], vector=True),
         shape[-1]
     )
 
     # TEST CASE 7: ACF of blocked time series of 1-vectors
     assert np.allclose(
-        correlation.correlation_fft(vectors_ones[:, :, 0], vector=True), 
+        correlation.correlation_fft(vectors_ones[:, :, 0], vector=True),
         shape[-1]
     )
 
-    # TEST CASE 8: ACF of blocked time series of 1-vectors for multiple 
+    # TEST CASE 8: ACF of blocked time series of 1-vectors for multiple
     # entities
-    assert np.allclose(correlation.correlation_fft(vectors_ones, vector=True), 
+    assert np.allclose(correlation.correlation_fft(vectors_ones, vector=True),
                        shape[-1])
 
 def test_func_correlation_fft_acf_random():
 
     # TEST CASE 1: ACF of time series of random scalars
-    assert np.allclose(correlation.correlation_fft(vectors_random_1[0, :, 0, 0]), 
+    assert np.allclose(correlation.correlation_fft(vectors_random_1[0, :, 0, 0]),
                        acf_scalar)
-    
-    # TEST CASE 2: ACF of time series of random scalars for multiple 
+
+    # TEST CASE 2: ACF of time series of random scalars for multiple
     # entities
     acf = correlation.correlation_fft(vectors_random_1[0, :, :, 0], axis=0)
     assert np.allclose(acf, acf_multi_scalar)
     assert np.allclose(
         correlation.correlation_fft(vectors_random_1[0, :, :, 0], average=True,
                                     axis=0),
         acf.mean(axis=1)
     )
 
     # TEST CASE 3: ACF of blocked time series of random scalars
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[:, :, 0, 0], axis=1), 
+        correlation.correlation_fft(vectors_random_1[:, :, 0, 0], axis=1),
         acf_block_scalar
     )
 
-    # TEST CASE 4: ACF of blocked time series of random scalars for 
+    # TEST CASE 4: ACF of blocked time series of random scalars for
     # multiple entities
     acf = correlation.correlation_fft(vectors_random_1[:, :, :, 0], axis=1)
     assert np.allclose(acf[0], acf_multi_scalar)
     assert np.allclose(acf[:, :, 0], acf_block_scalar)
     assert np.allclose(
         correlation.correlation_fft(vectors_random_1[:, :, :, 0], average=True,
                                     axis=1),
         acf.mean(axis=2)
     )
 
     # TEST CASE 5: ACF of time series of random vectors
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[0, :, 0], axis=0, vector=True), 
+        correlation.correlation_fft(vectors_random_1[0, :, 0], axis=0, vector=True),
         acf_vector
     )
 
-    # TEST CASE 6: ACF of time series of random vectors for multiple 
+    # TEST CASE 6: ACF of time series of random vectors for multiple
     # entities
     assert np.allclose(
         correlation.correlation_fft(vectors_random_1[0], axis=0, vector=True),
         acf_multi_vector
     )
 
     # TEST CASE 7: ACF of blocked time series of random vectors
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[:, :, 0], axis=1, vector=True), 
+        correlation.correlation_fft(vectors_random_1[:, :, 0], axis=1, vector=True),
         acf_block_vector
     )
 
-    # TEST CASE 8: ACF of blocked time series of random vectors for 
+    # TEST CASE 8: ACF of blocked time series of random vectors for
     # multiple entities
     acf = correlation.correlation_fft(vectors_random_1, vector=True)
     assert np.allclose(acf[0], acf_multi_vector)
     assert np.allclose(acf[:, :, 0], acf_block_vector)
 
 def test_func_correlation_shift_acf_errors():
 
@@ -178,62 +178,62 @@
         correlation.correlation_shift(np.empty((2, 2, 2)), axis=2)
 
 def test_func_correlation_shift_acf_random():
 
     # TEST CASE 1: ACF of time series of random scalars
     assert np.allclose(correlation.correlation_shift(vectors_random_1[0, :, 0, 0]),
                        acf_scalar)
-    
-    # TEST CASE 2: ACF of time series of random scalars for multiple 
+
+    # TEST CASE 2: ACF of time series of random scalars for multiple
     # entities
     acf = correlation.correlation_shift(vectors_random_1[0, :, :, 0])
     assert np.allclose(acf, acf_multi_scalar)
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[0, :, :, 0], 
+        correlation.correlation_shift(vectors_random_1[0, :, :, 0],
                                       average=True, axis=0),
         acf.mean(axis=1)
     )
 
     # TEST CASE 3: ACF of blocked time series of random scalars
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[:, :, 0, 0], axis=1), 
+        correlation.correlation_shift(vectors_random_1[:, :, 0, 0], axis=1),
         acf_block_scalar
     )
 
-    # TEST CASE 4: ACF of blocked time series of random scalars for 
+    # TEST CASE 4: ACF of blocked time series of random scalars for
     # multiple entities
     acf = correlation.correlation_shift(vectors_random_1[:, :, :, 0], axis=1)
     assert np.allclose(acf[0], acf_multi_scalar)
     assert np.allclose(acf[:, :, 0], acf_block_scalar)
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[:, :, :, 0], 
+        correlation.correlation_shift(vectors_random_1[:, :, :, 0],
                                       average=True, axis=1),
         acf.mean(axis=2)
     )
 
     # TEST CASE 5: ACF of time series of random vectors
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[0, :, 0], axis=0, vector=True), 
+        correlation.correlation_shift(vectors_random_1[0, :, 0], axis=0, vector=True),
         acf_vector
     )
 
-    # TEST CASE 6: ACF of time series of random vectors for multiple 
+    # TEST CASE 6: ACF of time series of random vectors for multiple
     # entities
     assert np.allclose(
         correlation.correlation_shift(vectors_random_1[0], axis=0, vector=True),
         acf_multi_vector
     )
 
     # TEST CASE 7: ACF of blocked time series of random vectors
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[:, :, 0], axis=1, vector=True), 
+        correlation.correlation_shift(vectors_random_1[:, :, 0], axis=1, vector=True),
         acf_block_vector
     )
 
-    # TEST CASE 8: ACF of blocked time series of random vectors for 
+    # TEST CASE 8: ACF of blocked time series of random vectors for
     # multiple entities
     acf = correlation.correlation_shift(vectors_random_1, vector=True)
     assert np.allclose(acf[0], acf_multi_vector)
     assert np.allclose(acf[:, :, 0], acf_block_vector)
 
 def test_func_correlation_fft_ccf_errors():
 
@@ -243,84 +243,84 @@
 
     # TEST CASE 2: CCF of empty 2D array
     with pytest.raises(ValueError):
         correlation.correlation_fft(np.empty((0, 3)), np.empty((0, 3)))
 
     # TEST CASE 3: CCF of 5D arrays
     with pytest.raises(ValueError):
-        correlation.correlation_fft(np.empty((2, 2, 2, 2, 2)), 
+        correlation.correlation_fft(np.empty((2, 2, 2, 2, 2)),
                                     np.empty((2, 2, 2, 2, 2)))
-        
+
     # TEST CASE 4: CCF of asymmetric 2D arrays
     with pytest.raises(ValueError):
         correlation.correlation_fft(np.empty((2, 3)), np.empty((3, 2)))
 
     # TEST CASE 5: CCF of 3D arrays along invalid axis
     with pytest.raises(ValueError):
-        correlation.correlation_fft(np.empty((2, 2, 2)), np.empty((2, 2, 2)), 
+        correlation.correlation_fft(np.empty((2, 2, 2)), np.empty((2, 2, 2)),
                                     axis=2)
 
 def test_func_correlation_fft_ccf_random():
 
     # TEST CASE 1: CCF of time series of random scalars
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[0, :, 0, 0].tolist(), 
-                                    vectors_random_2[0, :, 0, 0].tolist()), 
+        correlation.correlation_fft(vectors_random_1[0, :, 0, 0].tolist(),
+                                    vectors_random_2[0, :, 0, 0].tolist()),
         ccf_scalar
     )
-    
-    # TEST CASE 2: CCF of time series of random scalars for multiple 
-    # entities   
+
+    # TEST CASE 2: CCF of time series of random scalars for multiple
+    # entities
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[0, :, :, 0], 
-                                    vectors_random_2[0, :, :, 0], axis=0), 
+        correlation.correlation_fft(vectors_random_1[0, :, :, 0],
+                                    vectors_random_2[0, :, :, 0], axis=0),
         ccf_multi_scalar
     )
 
     # TEST CASE 3: CCF of blocked time series of random scalars
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[:, :, 0, 0], 
-                                    vectors_random_2[:, :, 0, 0], axis=1), 
+        correlation.correlation_fft(vectors_random_1[:, :, 0, 0],
+                                    vectors_random_2[:, :, 0, 0], axis=1),
         ccf_block_scalar
     )
 
-    # TEST CASE 4: CCF of blocked time series of random scalars for 
+    # TEST CASE 4: CCF of blocked time series of random scalars for
     # multiple entities
-    ccf = correlation.correlation_fft(vectors_random_1[:, :, :, 0], 
+    ccf = correlation.correlation_fft(vectors_random_1[:, :, :, 0],
                                       vectors_random_2[:, :, :, 0], axis=1)
     assert np.allclose(ccf[0], ccf_multi_scalar)
     assert np.allclose(ccf[:, :, 0], ccf_block_scalar)
 
     # TEST CASE 5: CCF of time series of random vectors
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[0, :, 0], 
-                                    vectors_random_2[0, :, 0], 
-                                    axis=0, vector=True), 
+        correlation.correlation_fft(vectors_random_1[0, :, 0],
+                                    vectors_random_2[0, :, 0],
+                                    axis=0, vector=True),
         ccf_vector
     )
 
-    # TEST CASE 6: CCF of time series of random vectors for multiple 
+    # TEST CASE 6: CCF of time series of random vectors for multiple
     # entities
     assert np.allclose(
         correlation.correlation_fft(vectors_random_1[0], vectors_random_2[0],
                                     axis=0, vector=True),
         ccf_multi_vector
     )
 
     # TEST CASE 7: CCF of blocked time series of random vectors
     assert np.allclose(
-        correlation.correlation_fft(vectors_random_1[:, :, 0], 
-                                    vectors_random_2[:, :, 0], 
-                                    axis=1, vector=True), 
+        correlation.correlation_fft(vectors_random_1[:, :, 0],
+                                    vectors_random_2[:, :, 0],
+                                    axis=1, vector=True),
         ccf_block_vector
     )
 
-    # TEST CASE 8: CCF of blocked time series of random vectors for 
+    # TEST CASE 8: CCF of blocked time series of random vectors for
     # multiple entities
-    ccf = correlation.correlation_fft(vectors_random_1, vectors_random_2, 
+    ccf = correlation.correlation_fft(vectors_random_1, vectors_random_2,
                                       vector=True)
     assert np.allclose(ccf[0], ccf_multi_vector)
     assert np.allclose(ccf[:, :, 0], ccf_block_vector)
 
 def test_func_correlation_shift_ccf_errors():
 
     # TEST CASE 1: CCF of empty 1D arrays
@@ -329,120 +329,120 @@
 
     # TEST CASE 2: CCF of empty 2D array
     with pytest.raises(ValueError):
         correlation.correlation_shift(np.empty((0, 3)), np.empty((0, 3)))
 
     # TEST CASE 3: CCF of 5D arrays
     with pytest.raises(ValueError):
-        correlation.correlation_shift(np.empty((2, 2, 2, 2, 2)), 
+        correlation.correlation_shift(np.empty((2, 2, 2, 2, 2)),
                                       np.empty((2, 2, 2, 2, 2)))
-        
+
     # TEST CASE 4: CCF of asymmetric 2D arrays
     with pytest.raises(ValueError):
         correlation.correlation_shift(np.empty((2, 3)), np.empty((3, 2)))
 
     # TEST CASE 5: CCF of 3D arrays along invalid axis
     with pytest.raises(ValueError):
-        correlation.correlation_shift(np.empty((2, 2, 2)), np.empty((2, 2, 2)), 
+        correlation.correlation_shift(np.empty((2, 2, 2)), np.empty((2, 2, 2)),
                                       axis=2)
 
 def test_func_correlation_shift_ccf_random():
 
     # TEST CASE 1: CCF of time series of random scalars
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[0, :, 0, 0].tolist(), 
-                                      vectors_random_2[0, :, 0, 0].tolist()), 
+        correlation.correlation_shift(vectors_random_1[0, :, 0, 0].tolist(),
+                                      vectors_random_2[0, :, 0, 0].tolist()),
         ccf_scalar
     )
-    
-    # TEST CASE 2: CCF of time series of random scalars for multiple 
+
+    # TEST CASE 2: CCF of time series of random scalars for multiple
     # entities
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[0, :, :, 0], 
-                                      vectors_random_2[0, :, :, 0], axis=0), 
+        correlation.correlation_shift(vectors_random_1[0, :, :, 0],
+                                      vectors_random_2[0, :, :, 0], axis=0),
         ccf_multi_scalar
     )
 
     # TEST CASE 3: CCF of blocked time series of random scalars
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[:, :, 0, 0], 
-                                      vectors_random_2[:, :, 0, 0], axis=1), 
+        correlation.correlation_shift(vectors_random_1[:, :, 0, 0],
+                                      vectors_random_2[:, :, 0, 0], axis=1),
         ccf_block_scalar
     )
 
-    # TEST CASE 4: CCF of blocked time series of random scalars for 
+    # TEST CASE 4: CCF of blocked time series of random scalars for
     # multiple entities
-    ccf = correlation.correlation_shift(vectors_random_1[:, :, :, 0], 
+    ccf = correlation.correlation_shift(vectors_random_1[:, :, :, 0],
                                         vectors_random_2[:, :, :, 0], axis=1)
     assert np.allclose(ccf[0], ccf_multi_scalar)
     assert np.allclose(ccf[:, :, 0], ccf_block_scalar)
 
     # TEST CASE 5: CCF of time series of random vectors
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[0, :, 0], 
-                                      vectors_random_2[0, :, 0], 
-                                      axis=0, vector=True), 
+        correlation.correlation_shift(vectors_random_1[0, :, 0],
+                                      vectors_random_2[0, :, 0],
+                                      axis=0, vector=True),
         ccf_vector
     )
 
-    # TEST CASE 6: CCF of time series of random vectors for multiple 
+    # TEST CASE 6: CCF of time series of random vectors for multiple
     # entities
     assert np.allclose(
         correlation.correlation_shift(vectors_random_1[0], vectors_random_2[0],
                                       axis=0, vector=True),
         ccf_multi_vector
     )
 
     # TEST CASE 7: CCF of blocked time series of random vectors
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[:, :, 0], 
-                                      vectors_random_2[:, :, 0], 
-                                      axis=1, vector=True), 
+        correlation.correlation_shift(vectors_random_1[:, :, 0],
+                                      vectors_random_2[:, :, 0],
+                                      axis=1, vector=True),
         ccf_block_vector
     )
 
-    # TEST CASE 8: CCF of blocked time series of random vectors for 
+    # TEST CASE 8: CCF of blocked time series of random vectors for
     # multiple entities
-    ccf = correlation.correlation_shift(vectors_random_1, vectors_random_2, 
+    ccf = correlation.correlation_shift(vectors_random_1, vectors_random_2,
                                         vector=True)
     assert np.allclose(ccf[0], ccf_multi_vector)
     assert np.allclose(ccf[:, :, 0], ccf_block_vector)
 
 def test_func_correlation_shift_double():
 
     # TEST CASE 1: Doubled ACF for time series of random scalars
     assert np.allclose(
         correlation.correlation_shift(vectors_random_1[0, :, 0, 0], double=True),
         correlation.correlation_shift(vectors_random_1[0, :, 0, 0], double=True)
     )
 
     # TEST CASE 2: Overlapped CCF for time series of random scalars
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[0, :, 0, 0], 
-                                      vectors_random_2[0, :, 0, 0], 
+        correlation.correlation_shift(vectors_random_1[0, :, 0, 0],
+                                      vectors_random_2[0, :, 0, 0],
                                       axis=0, double=True),
-        correlation.correlation_fft(vectors_random_1[0, :, 0, 0], 
-                                    vectors_random_2[0, :, 0, 0], 
+        correlation.correlation_fft(vectors_random_1[0, :, 0, 0],
+                                    vectors_random_2[0, :, 0, 0],
                                     axis=0, double=True)
     )
 
     # TEST CASE 3: Overlapped CCF for blocked time series of random scalars
     assert np.allclose(
-        correlation.correlation_shift(vectors_random_1[:, :, 0, 0], 
-                                      vectors_random_2[:, :, 0, 0], 
+        correlation.correlation_shift(vectors_random_1[:, :, 0, 0],
+                                      vectors_random_2[:, :, 0, 0],
                                       axis=1, double=True),
-        correlation.correlation_fft(vectors_random_1[:, :, 0, 0], 
-                                    vectors_random_2[:, :, 0, 0], 
+        correlation.correlation_fft(vectors_random_1[:, :, 0, 0],
+                                    vectors_random_2[:, :, 0, 0],
                                     axis=1, double=True)
     )
 
 # Generate simple trajectories and calculate their MSDs
-traj_1 = np.array(((0, 0, 0), (1, 1, 1), (2, 2, 2), (3, 3, 3)), dtype=float)
+traj_1 = np.array(((0, 0, 0), (1, 1, 1), (2, 2, 2), (3, 3, 3)))
 msd_1 = np.einsum("td,td->t", traj_1, traj_1)
-traj_2 = np.array(((0, 1, 2), (2, 3, 4), (4, 5, 6), (6, 7, 8)), dtype=float)
+traj_2 = np.array(((0, 1, 2), (2, 3, 4), (4, 5, 6), (6, 7, 8)))
 msd_2 = ((traj_2 - traj_2[0]) ** 2).sum(axis=1)
 cd = (traj_1 * (traj_2 - traj_2[0])).sum(axis=1)
 
 def test_func_msd_fft_errors():
 
     # TEST CASE 1: MSD of empty trajectory
     with pytest.raises(ValueError):
@@ -471,37 +471,37 @@
     # TEST CASE 3: CD of simple trajectories
     assert np.allclose(correlation.msd_fft(traj_1, traj_2.tolist()), cd)
 
     # TEST CASE 4: MSD of first simple trajectory replicated for multiple
     # particles
     assert np.allclose(
         correlation.msd_fft(
-            np.tile(traj_1[:, None], (1, 2, 1)), 
+            np.tile(traj_1[:, None], (1, 2, 1)),
             average=False
-        )[:, 0], 
+        )[:, 0],
         msd_1
     )
 
     # TEST CASE 5: MSD of first simple trajectory replicated for multiple
     # blocks and particles
     assert np.allclose(
         correlation.msd_fft(
-            np.tile(traj_1[None, :, None], (2, 1, 2, 1)), 
+            np.tile(traj_1[None, :, None], (2, 1, 2, 1)),
             average=False
-        )[0, :, 0], 
+        )[0, :, 0],
         msd_1
     )
 
     # TEST CASE 6: CD of simple trajectories replicated for multiple
     # blocks and particles
     assert np.allclose(
         correlation.msd_fft(
-            np.tile(traj_1[None, :, None], (2, 1, 2, 1)), 
+            np.tile(traj_1[None, :, None], (2, 1, 2, 1)),
             np.tile(traj_2[None, :, None], (2, 1, 2, 1))
-        )[0], 
+        )[0],
         cd
     )
 
 def test_func_msd_shift_errors():
 
     # TEST CASE 1: MSD of empty trajectory
     with pytest.raises(ValueError):
@@ -530,32 +530,32 @@
     # TEST CASE 3: CD of simple trajectories
     assert np.allclose(correlation.msd_shift(traj_1, traj_2.tolist()), cd)
 
     # TEST CASE 4: MSD of first simple trajectory replicated for multiple
     # particles
     assert np.allclose(
         correlation.msd_shift(
-            np.tile(traj_1[:, None], (1, 2, 1)), 
+            np.tile(traj_1[:, None], (1, 2, 1)),
             average=False
-        )[:, 0], 
+        )[:, 0],
         msd_1
     )
 
     # TEST CASE 5: MSD of first simple trajectory replicated for multiple
     # blocks and particles
     assert np.allclose(
         correlation.msd_shift(
-            np.tile(traj_1[None, :, None], (2, 1, 2, 1)), 
+            np.tile(traj_1[None, :, None], (2, 1, 2, 1)),
             average=False
-        )[0, :, 0], 
+        )[0, :, 0],
         msd_1
     )
 
     # TEST CASE 6: CD of simple trajectories replicated for multiple
     # blocks and particles
     assert np.allclose(
         correlation.msd_shift(
-            np.tile(traj_1[None, :, None], (2, 1, 2, 1)), 
+            np.tile(traj_1[None, :, None], (2, 1, 2, 1)),
             np.tile(traj_2[None, :, None], (2, 1, 2, 1))
-        )[0], 
+        )[0],
         cd
     )
```

### Comparing `mdhelper-0.0.2/tests/test_algorithm_molecule.py` & `mdhelper-1.0.0/tests/test_algorithm_molecule.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import MDAnalysis as mda
 from MDAnalysis.tests.datafiles import DCD, PSF
 import numpy as np
 import pytest
 
 sys.path.insert(0, f"{pathlib.Path(__file__).parents[1].resolve().as_posix()}/src")
-from mdhelper.algorithm import molecule
+from mdhelper.algorithm import molecule # noqa: E402
 
 universe = mda.Universe(PSF, DCD)
 protein = universe.select_atoms("protein")
 core = universe.select_atoms("protein and (resid 1-29 60-121 160-214)")
 nmp = universe.select_atoms("protein and resid 30-59")
 lid = universe.select_atoms("protein and resid 122-159")
 arg = universe.select_atoms("resname ARG")
@@ -25,29 +25,29 @@
     # TEST CASE 2: Invalid grouping
     with pytest.raises(ValueError):
         molecule.center_of_mass(universe.atoms, "atoms")
 
     # TEST CASE 3: No system dimension information when number of periodic
     # boundary crossings is provided
     with pytest.raises(ValueError):
-        molecule.center_of_mass(universe.atoms, 
+        molecule.center_of_mass(universe.atoms,
                                 images=np.zeros((universe.atoms.n_atoms, 3)))
-        
+
     # TEST CASE 4: Incompatible mass and position arrays
     with pytest.raises(ValueError):
         molecule.center_of_mass(
-            masses=universe.atoms.masses, 
+            masses=universe.atoms.masses,
             positions=[r.atoms.positions for r in universe.residues]
         )
 
 def test_center_of_mass_mda():
 
     """
     Test case 1 is inspired by the example in the "Working with
-    AtomGroups" section of the MDAnalysis Tutorial 
+    AtomGroups" section of the MDAnalysis Tutorial
     (https://www.mdanalysis.org/MDAnalysisTutorial/atomgroups.html).
     """
 
     # TEST CASE 1: Center of mass of domains in AdK
     assert np.allclose(molecule.center_of_mass(core), core.center_of_mass())
     assert np.allclose(molecule.center_of_mass(nmp), nmp.center_of_mass())
     assert np.allclose(molecule.center_of_mass(lid), lid.center_of_mass())
@@ -55,44 +55,44 @@
     # TEST CASE 2: Center of mass of all particles using AtomGroup
     com = universe.atoms.center_of_mass()
     assert np.allclose(molecule.center_of_mass(universe.atoms), com)
 
     # TEST CASE 3: Center of mass of all particles using AtomGroup, but
     # with the masses and unwrapped positions returned
     c, m, p = molecule.center_of_mass(
-        universe.atoms, 
+        universe.atoms,
         images=np.zeros((universe.atoms.n_atoms, 3), dtype=int),
-        dims=np.array((0, 0, 0), dtype=float),
+        dimensions=np.array((0, 0, 0)),
         raw=True
     )
     assert np.allclose(c, com)
     assert np.allclose(m, universe.atoms.masses)
     assert np.allclose(p, universe.atoms.positions)
-    
+
     # TEST CASE 4: Centers of mass of different residues using AtomGroup
-    res_coms = np.array([r.atoms.center_of_mass() 
-                        for r in universe.residues])
+    res_coms = np.array([r.atoms.center_of_mass()
+                         for r in universe.residues])
     assert np.allclose(molecule.center_of_mass(universe.atoms, "residues"),
                        res_coms)
-    
+
     # TEST CASE 5: Centers of mass of different residues using raw masses
     # and positions from AtomGroup
     assert np.allclose(
         molecule.center_of_mass(
             universe.atoms, "residues",
             masses=[r.atoms.masses for r in universe.residues]
         ),
         res_coms
     )
 
-    # TEST CASE 6: Centers of mass of different residues using raw masses 
+    # TEST CASE 6: Centers of mass of different residues using raw masses
     # and positions
     assert np.allclose(
         molecule.center_of_mass(
-            masses=[r.atoms.masses for r in universe.residues], 
+            masses=[r.atoms.masses for r in universe.residues],
             positions=[r.atoms.positions for r in universe.residues]
         ),
         res_coms
     )
 
     # TEST CASE 7: Centers of mass of arginine residues using AtomGroup
     arg_coms = np.array([r.atoms.center_of_mass() for r in arg.residues])
@@ -100,67 +100,67 @@
 
     # TEST CASE 8: Centers of mass of arginine residues using AtomGroup
     # and specified number of residues
     assert np.allclose(molecule.center_of_mass(arg, n_groups=13), arg_coms)
 
     # TEST CASE 9: Centers of mass of arginine residues using raw masses
     # and positions
-    assert np.allclose(molecule.center_of_mass(masses=arg.masses, 
-                                               positions=arg.positions, 
+    assert np.allclose(molecule.center_of_mass(masses=arg.masses,
+                                               positions=arg.positions,
                                                n_groups=13),
                        arg_coms)
-    
+
     # TEST CASE 10: Centers of mass of only segment in AtomGroup
     assert np.allclose(molecule.center_of_mass(universe.atoms, "segments"), com)
 
-    # TEST CASE 11: Centers of mass of only segment in AtomGroup 
+    # TEST CASE 11: Centers of mass of only segment in AtomGroup
     # containing the arginine residues
-    assert np.allclose(molecule.center_of_mass(arg, "segments"), 
+    assert np.allclose(molecule.center_of_mass(arg, "segments"),
                        arg.center_of_mass())
-    
+
 def test_radius_of_gyration_errors():
-    
+
     # TEST CASE 1: Invalid grouping
     with pytest.raises(ValueError):
         molecule.radius_of_gyration(universe.atoms, "atoms")
 
 def test_radius_of_gyration_mda():
 
     """
     The reference implementation is adapted from the "Writing your own
-    trajectory analysis" section of the MDAnalysis User Guide 
+    trajectory analysis" section of the MDAnalysis User Guide
     (https://userguide.mdanalysis.org/stable/examples/analysis/custom_trajectory_analysis.html).
     """
-    
+
     def radius_of_gyration(group):
         positions = group.positions
         masses = group.masses
         center_of_mass = group.center_of_mass()
         r_sq = (positions - center_of_mass) ** 2
         r_ssq = np.array((r_sq.sum(axis=1),
                           (r_sq[:, [1, 2]]).sum(axis=1),
-                          (r_sq[:, [0, 2]]).sum(axis=1), 
+                          (r_sq[:, [0, 2]]).sum(axis=1),
                           (r_sq[:, [0, 1]]).sum(axis=1)))
         return np.sqrt((masses * r_ssq).sum(axis=1) / masses.sum())
-    
+
     # TEST CASE 1: Overall radius of gyration
     ref = radius_of_gyration(universe.atoms)
     assert np.isclose(molecule.radius_of_gyration(universe.atoms), ref[0])
-    assert np.allclose(molecule.radius_of_gyration(universe.atoms, 
+    assert np.allclose(molecule.radius_of_gyration(universe.atoms,
                                                    components=True),
                        ref[1:])
-    
+
     # TEST CASE 2: Radii of gyration of arginine residues
     ref = np.array([radius_of_gyration(g.atoms) for g in arg.residues])
     assert np.allclose(molecule.radius_of_gyration(arg, "residues"),
                        ref[:, 0])
-    assert np.allclose(molecule.radius_of_gyration(arg, "residues", 
+    assert np.allclose(molecule.radius_of_gyration(arg, "residues",
                                                    components=True),
                        ref[:, 1:])
-    
+
     # TEST CASE 3: Radii of gyration of different residues
     ref = np.array([radius_of_gyration(g.atoms) for g in universe.residues])
     assert np.allclose(molecule.radius_of_gyration(universe.atoms, "residues"),
                        ref[:, 0])
-    assert np.allclose(molecule.radius_of_gyration(universe.atoms, "residues", 
+    assert np.allclose(molecule.radius_of_gyration(universe.atoms, "residues",
                                                    components=True),
                        ref[:, 1:])
```

### Comparing `mdhelper-0.0.2/tests/test_algorithm_topology.py` & `mdhelper-1.0.0/tests/test_algorithm_topology.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import sys
 
 import numpy as np
 from openmm import app, unit
 import pytest
 
 sys.path.insert(0, f"{pathlib.Path(__file__).parents[1].resolve().as_posix()}/src")
-from mdhelper.algorithm import topology
+from mdhelper.algorithm import topology # noqa: E402
 
 rng = np.random.default_rng()
-dims = np.array([10, 10, 10], dtype=float)
+dims = np.array((10.0, 10.0, 10.0))
 
 def test_func_create_atoms_error():
 
     # TEST CASE 1: N not specified
     with pytest.raises(ValueError):
         topology.create_atoms(dims)
 
@@ -26,15 +26,15 @@
         topology.create_atoms(dims, N=9000, N_p=9001)
 
     # TEST CASE 4: N not divisible by N_p
     with pytest.raises(ValueError):
         topology.create_atoms(dims, N=10, N_p=3)
 
 def test_func_create_atoms_random():
-    
+
     # TEST CASE 1: Random melt in reduced units
     N = rng.integers(1, 1000)
     pos = topology.create_atoms(dims, N)
     assert pos.shape == (N, 3)
 
     # TEST CASE 2: Random melt with default length unit
     pos = topology.create_atoms(dims * unit.nanometer, N)
@@ -50,37 +50,41 @@
     pos = topology.create_atoms(topo, N)
     assert pos.shape == (N, 3)
 
 def test_func_create_atoms_polymer():
 
     # TEST CASE 1: Random polymer melt
     M = rng.integers(1, 100)
-    N_p = rng.integers(2, 100)
+    N_p = rng.integers(4, 100)
     N = M * N_p
     pos = topology.create_atoms(dims, N, N_p)
     assert pos.shape == (N, 3)
 
-    # TEST CASE 2: Random polymer melt with bond information and wrapped
-    # positions
-    pos, bonds = topology.create_atoms(dims, N, N_p, connectivity=True, 
-                                       randomize=True, wrap=True)
+    # TEST CASE 2: Random polymer melt with bond, angle, and dihedral
+    # nformation and wrapped positions
+    pos, bonds, angles, dihedrals = topology.create_atoms(
+        dims, N, N_p, bonds=True, angles=True, dihedrals=True, randomize=True,
+        wrap=True
+    )
     assert pos.shape == (N, 3)
     assert bonds.shape[0] == N - M
+    assert angles.shape[0] == N - 2 * M
+    assert dihedrals.shape[0] == N - 3 * M
     assert np.all((pos[:, 0] > 0) & (pos[:, 0] < dims[0]))
     assert np.all((pos[:, 1] > 0) & (pos[:, 2] < dims[1]))
     assert np.all((pos[:, 1] > 0) & (pos[:, 2] < dims[2]))
 
 def test_func_create_atoms_lattice():
 
     # TEST CASE 1: FCC lattice with flexible dimensions
     pos, new_dims = topology.create_atoms(dims, lattice="fcc", length=0.8,
                                           flexible=True)
     assert np.allclose(pos[4], 0.8 * np.array((0, np.sqrt(3) / 3, 2 * np.sqrt(6) / 3)))
     assert np.allclose(dims, new_dims, atol=1)
-    
+
     # TEST CASE 2: HCP lattice with flexible dimensions
     pos, new_dims = topology.create_atoms(dims, lattice="hcp", length=0.8,
                                           flexible=True)
     assert np.allclose(pos[1], 0.8 * np.array((0.5, np.sqrt(3) / 2, 0)))
     assert np.allclose(dims, new_dims, atol=1)
 
     # TEST CASE 3: HCP lattice to fill specified dimensions
@@ -90,8 +94,43 @@
 
     # TEST CASE 4: Graphene wall
     pos, new_dims = topology.create_atoms(dims, lattice="honeycomb",
                                           length=0.142 * unit.nanometer,
                                           flexible=True)
     assert pos[1, 1] == 0.142 * unit.nanometer
     assert np.allclose(dims[:2], new_dims[:2], atol=1)
-    assert new_dims[2] == 0 * unit.nanometer
+    assert new_dims[2] == 0 * unit.nanometer
+
+    # TEST CASE 5: Cubic crystal lattice
+    pos, new_dims = topology.create_atoms(dims, lattice="cubic", length=1)
+    assert np.allclose(pos[-1], dims - 1)
+
+def test_func_unwrap():
+
+    pos_old = np.array(((2.0, 2.0, 2.0),))
+    images = np.zeros_like(pos_old, dtype=int)
+    thresholds = dims / 2
+    pos = np.array(((8.0, 8.0, 8.0),))
+
+    # TEST CASE 1: Unwrap not in-place
+    pos_unwrapped, pos_old_updated, images = topology.unwrap(
+        pos, pos_old, dims, thresholds=thresholds, images=images,
+        in_place=False
+    )
+    assert (np.allclose(pos_unwrapped[0], -2)
+            and np.allclose(pos, pos_old_updated))
+
+    # TEST CASE 2: Unwrap in-place
+    topology.unwrap(pos, pos_old, dims)
+    assert np.allclose(pos[0], -2)
+
+def test_func_wrap():
+
+    pos = np.array(((9.0, 10.0, 11.0),))
+
+    # TEST CASE 1: Wrap not in-place
+    pos_wrapped = topology.wrap(pos, dims, in_place=False)
+    assert np.allclose(pos_wrapped[0], (9, 10, 1))
+
+    # TEST CASE 2: Wrap in-place
+    topology.wrap(pos, dims)
+    assert np.allclose(pos[0], (9, 10, 1))
```

### Comparing `mdhelper-0.0.2/tests/test_algorithm_utility.py` & `mdhelper-1.0.0/tests/test_algorithm_utility.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import pathlib
 import sys
 
 import numpy as np
+import pytest
 
 sys.path.insert(0, f"{pathlib.Path(__file__).parents[1].resolve().as_posix()}/src")
-from mdhelper.algorithm import utility
+from mdhelper.algorithm import utility # noqa: E402
 
 rng = np.random.default_rng()
 
 def test_func_closest_factors():
 
     # TEST CASE 1: Cube root of perfect cube
-    factors = utility.closest_factors(1000, 3)
+    factors = utility.get_closest_factors(1000, 3)
     assert np.allclose(factors, 10 * np.ones(3, dtype=int))
 
     # TEST CASE 2: Three closest factors in ascending order
-    factors = utility.closest_factors(35904, 3)
-    assert factors.tolist() == [32, 33, 34] 
+    factors = utility.get_closest_factors(35904, 3)
+    assert factors.tolist() == [32, 33, 34]
 
     # TEST CASE 3: Four closest factors in descending order
-    factors = utility.closest_factors(73440, 4, reverse=True)
+    factors = utility.get_closest_factors(73440, 4, reverse=True)
     assert factors.tolist() == [18, 17, 16, 15]
 
 def test_func_replicate():
 
     # TEST CASE 1: Replicate two vectors
     dims = rng.integers(1, 5, size=3)
     n_cells = rng.integers(2, 10, size=3)
-    pos = utility.replicate(dims, np.array(((0, 0, 0), dims // 2), dtype=float),
-                            n_cells)
+    pos = utility.replicate(dims, np.array(((0, 0, 0), dims // 2)), n_cells)
     assert pos.shape[0] == 2 * n_cells.prod()
     assert np.allclose(pos[2], (dims[0], 0, 0))
 
 def test_func_rebin():
 
     # TEST CASE 1: Rebin 1D array
     arr = np.arange(50)
     ref = np.arange(2, 52, 5)
     assert np.allclose(utility.rebin(arr), ref)
 
     # TEST CASE 2: Rebin 2D array
-    assert np.allclose(utility.rebin(np.tile(arr[None, :], (5, 1))), 
-                       np.tile(ref[None, :], (5, 1)))
+    assert np.allclose(utility.rebin(np.tile(arr[None, :], (5, 1))),
+                       np.tile(ref[None, :], (5, 1)))
+
+    # TEST CASE 3: No factor specified and cannot be determined
+    with pytest.raises(ValueError):
+        utility.rebin(np.empty((17,)))
```

### Comparing `mdhelper-0.0.2/tests/test_analysis_polymer.py` & `mdhelper-1.0.0/tests/test_analysis_polymer.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,39 +3,55 @@
 
 import MDAnalysis as mda
 from MDAnalysis.tests.datafiles import DCD, PSF
 from MDAnalysis.analysis.base import AnalysisFromFunction
 import numpy as np
 
 sys.path.insert(0, f"{pathlib.Path(__file__).parents[1].resolve().as_posix()}/src")
-from mdhelper.analysis import polymer
+from mdhelper.analysis import polymer # noqa: E402
 
+rng = np.random.default_rng()
 universe = mda.Universe(PSF, DCD)
 protein = universe.select_atoms("protein")
 
 def test_class_gyradius():
 
     """
     The reference implementation is adapted from the "Writing your own
-    trajectory analysis" section of the MDAnalysis User Guide 
+    trajectory analysis" section of the MDAnalysis User Guide
     (https://userguide.mdanalysis.org/stable/examples/analysis/custom_trajectory_analysis.html).
     """
 
     def radius_of_gyration(group):
         positions = group.positions
         masses = group.masses
         center_of_mass = group.center_of_mass()
         r_sq = (positions - center_of_mass) ** 2
         r_ssq = np.array((r_sq.sum(axis=1),
                           (r_sq[:, [1, 2]]).sum(axis=1),
-                          (r_sq[:, [0, 2]]).sum(axis=1), 
+                          (r_sq[:, [0, 2]]).sum(axis=1),
                           (r_sq[:, [0, 1]]).sum(axis=1)))
         return np.sqrt((masses * r_ssq).sum(axis=1) / masses.sum())
-    rog = AnalysisFromFunction(radius_of_gyration, universe.trajectory, protein).run()
-    gyradius = polymer.Gyradius(protein, grouping="residues").run()
+
+    rog = AnalysisFromFunction(radius_of_gyration, universe.trajectory,
+                               protein).run()
 
     # TEST CASE 1: Time series of overall radii of gyration
-    assert np.allclose(rog.results["timeseries"][:, 0], gyradius.results.gyradius[0])
+    gyradius = polymer.Gyradius(protein, grouping="residues").run()
+    gyradius_parallel = polymer.Gyradius(
+        protein, grouping="residues", parallel=True
+    ).run()
+    assert np.allclose(rog.results["timeseries"][:, 0],
+                       gyradius.results.gyradii[0])
+    assert np.allclose(rog.results["timeseries"][:, 0],
+                       gyradius_parallel.results.gyradii[0])
 
     # TEST CASE 2: Time series of radius of gyration components
-    gyradius = polymer.Gyradius(protein, grouping="residues", components=True).run()
-    assert np.allclose(rog.results["timeseries"][:, 1:], gyradius.results.gyradius[0])
+    gyradius = polymer.Gyradius(protein, grouping="residues",
+                                components=True).run()
+    gyradius_parallel = polymer.Gyradius(
+        protein, grouping="residues", components=True, parallel=True
+    ).run()
+    assert np.allclose(rog.results["timeseries"][:, 1:],
+                       gyradius.results.gyradii[0])
+    assert np.allclose(rog.results["timeseries"][:, 1:],
+                       gyradius_parallel.results.gyradii[0])
```

### Comparing `mdhelper-0.0.2/tests/test_analysis_transport.py` & `mdhelper-1.0.0/tests/test_analysis_transport.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,86 @@
 import glob
 import os
 import pathlib
 import sys
 import urllib
 
 import MDAnalysis as mda
-from MDAnalysis.tests.datafiles import RANDOM_WALK, RANDOM_WALK_TOPO
 from MDAnalysis.analysis.msd import EinsteinMSD
+from MDAnalysis.tests.datafiles import RANDOM_WALK, RANDOM_WALK_TOPO
 import numpy as np
 from scipy.stats import linregress
 
 sys.path.insert(0, f"{pathlib.Path(__file__).parents[1].resolve().as_posix()}/src")
-from mdhelper.analysis import transport
+from mdhelper.analysis import transport # noqa: E402
 
 def test_class_onsager_msd():
 
     universe = mda.Universe(RANDOM_WALK_TOPO, RANDOM_WALK)
 
     start = 20
     stop = 60
     time = np.arange(universe.trajectory.n_frames)
     msd = EinsteinMSD(universe).run().results.timeseries / 6
     diff = linregress(time[start:stop], msd[start:stop]).slope
 
     # TEST CASE 1: MSD and diffusion coefficients of a random walk
     # calculated using the Einstein relation
-    universe.dimensions = np.array((np.inf, np.inf, np.inf, 90, 90, 90), 
-                                   dtype=float)
+    universe.dimensions = np.array((np.inf, np.inf, np.inf, 90, 90, 90))
     onsager_shift = transport.Onsager(universe.atoms, fft=False, reduced=True).run()
-    onsager_shift.calculate_coefficients(start, stop, scale="linear")
+    onsager_shift.calculate_transport_coefficients(start, stop, scale="linear")
     assert np.allclose(onsager_shift.results.msd_self[0, 0], msd)
     assert np.isclose(diff, onsager_shift.results.D_i[0, 0])
 
     # TEST CASE 2: MSD and diffusion coefficients of a random walk
     # calculated using the FFT-based algorithm
-    universe.dimensions = np.array((np.inf, np.inf, np.inf, 90, 90, 90), 
-                                   dtype=float)
+    universe.dimensions = np.array((np.inf, np.inf, np.inf, 90, 90, 90))
     onsager_fft = transport.Onsager(universe.atoms, reduced=True).run()
-    onsager_fft.calculate_coefficients(start, stop, scale="linear")
+    onsager_fft.calculate_transport_coefficients(start, stop, scale="linear")
     assert np.allclose(onsager_fft.results.msd_self[0, 0], msd)
     assert np.isclose(diff, onsager_fft.results.D_i[0, 0])
 
 def test_class_onsager_transport_coefficients():
 
     """
-    The test cases are adapted from the "Mean Squared Displacement — 
+    The test cases are adapted from the "Mean Squared Displacement —
     :code:`MDAnalysis.analysis.msd`" page from the MDAnalysis User Guide
     (https://docs.mdanalysis.org/stable/documentation_pages/analysis/msd.html)
-    and uses data from the paper "Onsager Transport Coefficients and 
-    Transference Numbers in Polyelectrolyte Solutions and Polymerized 
-    Ionic Liquids" by Fong et al. 
+    and uses data from the paper "Onsager Transport Coefficients and
+    Transference Numbers in Polyelectrolyte Solutions and Polymerized
+    Ionic Liquids" by Fong et al.
     (https://doi.org/10.1021/acs.macromol.0c02001).
     """
 
     def acf_fft(x):
         N = len(x)
-        f = np.fft.fft(x, n=2 * N)  
-        return np.fft.ifft(f * f.conjugate())[:N].real / (N * np.ones(N) 
+        f = np.fft.fft(x, n=2 * N)
+        return np.fft.ifft(f * f.conj())[:N].real / (N * np.ones(N)
                                                           - np.arange(0, N))
 
     def msd_fft(r):
         N = len(r)
-        D = np.append(np.square(r).sum(axis=1), 0) 
+        D = np.append(np.square(r).sum(axis=1), 0)
         Q = 2 * D.sum()
         S1 = np.zeros(N)
         for m in range(N):
             Q = Q - D[m - 1] - D[N - m]
             S1[m] = Q / (N - m)
         return S1 - 2 * sum(acf_fft(r[:, i]) for i in range(r.shape[1]))
 
     def ccf_fft(x, y):
         N = len(x)
         return np.fft.ifft(
-            np.fft.fft(x, n=2 ** (2 * N - 1).bit_length()) 
-            * np.fft.fft(y, n=2 ** (2 * N - 1).bit_length()).conjugate()
+            np.fft.fft(x, n=2 ** (2 * N - 1).bit_length())
+            * np.fft.fft(y, n=2 ** (2 * N - 1).bit_length()).conj()
         )[:N].real / (N * np.ones(N) - np.arange(0, N))
 
     def msd_cross_fft(r, k):
         N = len(r)
-        D = np.append(np.multiply(r, k).sum(axis=1), 0) 
+        D = np.append(np.multiply(r, k).sum(axis=1), 0)
         Q = 2 * D.sum()
         S1 = np.zeros(N)
         for m in range(N):
             Q = Q - D[m - 1] - D[N - m]
             S1[m] = Q / (N - m)
         return S1 - sum(ccf_fft(r[:, i], k[:, i]) for i in range(r.shape[1])) \
                - sum(ccf_fft(k[:, i], r[:, i]) for i in range(k.shape[1]))
@@ -98,37 +96,41 @@
 
     def calc_L_ij(cation_positions, anion_positions):
         return msd_cross_fft(cation_positions.sum(axis=1),
                              anion_positions.sum(axis=1))
 
     def compute_L_ij(anion_positions, cation_positions, volume):
         return np.vstack(
-            ( 
+            (
                 calc_L_ii(anion_positions),
-                calc_L_ij(cation_positions, anion_positions), 
+                calc_L_ij(cation_positions, anion_positions),
                 calc_L_ii(cation_positions),
                 calc_L_ii_self(anion_positions),
                 calc_L_ii_self(cation_positions)
             )
         ) / (6 * volume)
-    
+
     def fit_data(times, f, start, stop):
         return linregress(times[start:stop], f[start:stop])[0]
 
-    url = "https://raw.githubusercontent.com/kdfong/transport-coefficients-MSD/master/example-data"
-
-    if not os.path.isdir("data/onsager"):
-        os.makedirs("data/onsager")
-    os.chdir("data/onsager")
+    path = os.getcwd()
+    if "tests" in path:
+        path_split = path.split("/")
+        path = "/".join(path_split[:path_split.index("tests") + 1])
+    else:
+        path += "/tests"
+    if not os.path.isdir(f"{path}/data/onsager"):
+        os.makedirs(f"{path}/data/onsager")
+    os.chdir(f"{path}/data/onsager")
 
+    url = "https://raw.githubusercontent.com/kdfong/transport-coefficients-MSD/master/example-data"
     if not os.path.isfile("system.data"):
         with urllib.request.urlopen(f"{url}/system.data") as r:
             with open("system.data", "w") as f:
                 f.write(r.read().decode())
-    
     for i in range(1, 6):
         if not os.path.isfile(f"traj_{i}.dcd"):
             with urllib.request.urlopen(f"{url}/traj_{i}.dcd") as r:
                 with open(f"traj_{i}.dcd", "wb") as f:
                     f.write(r.read())
 
     dt = 50
@@ -136,50 +138,51 @@
     fit_start = 2
     fit_stop = 20
     fit_start_self = 20
     fit_stop_self = 50
 
     universe = mda.Universe("system.data", glob.glob("*.dcd"), format="LAMMPS")
     groups = [universe.select_atoms(f"type {i}") for i in range(1, 3)]
-    positions = [np.zeros((universe.trajectory.n_frames - start, g.n_atoms, 3), 
-                          dtype=float) for g in groups]
+    positions = [np.zeros((universe.trajectory.n_frames - start, g.n_atoms, 3))
+                 for g in groups]
     for i, _ in enumerate(universe.trajectory[40:]):
         com = universe.atoms.center_of_mass(wrap=True)
         for g, p in zip(groups, positions):
             p[i] = g.positions - com
     volume = universe.dimensions[:3].prod()
-    times = np.arange(0, (universe.trajectory.n_frames - start) * dt, dt, 
+    times = np.arange(0, (universe.trajectory.n_frames - start) * dt, dt,
                       dtype=int)
     msds = compute_L_ij(*positions, volume)
 
-    onsager = transport.Onsager(groups, temp=1, center=True, com_wrap=True, 
+    onsager = transport.Onsager(groups, temperature=1, center=True,
+                                center_atom=True, center_wrap=True,
                                 reduced=True, dt=dt).run(start=40)
-    onsager.calculate_coefficients(fit_start, fit_stop, 
-                                   start_self=fit_start_self, 
-                                   stop_self=fit_stop_self,
-                                   scale="linear", enforce_linear=False)
+    onsager.calculate_transport_coefficients(fit_start, fit_stop,
+                                             start_self=fit_start_self,
+                                             stop_self=fit_stop_self,
+                                             scale="linear", enforce_linear=False)
 
     L_ij_array = np.triu(onsager.results.L_ij)
     for i, (msd, L_ij) in enumerate(zip(msds, L_ij_array[L_ij_array != 0])):
 
         # TEST CASE 1: Cross displacements of polyelectrolyte system
-        assert np.allclose(msd, onsager.results.msd_cross[i, 0] / volume, 
-                           atol=5e-4)
-        
-        # TEST CASE 2: Onsager transport coefficients of polyelectrolyte 
+        assert np.allclose(msd, onsager.results.msd_cross[i, 0] / volume,
+                           atol=1e-3)
+
+        # TEST CASE 2: Onsager transport coefficients of polyelectrolyte
         # system
         assert np.isclose(fit_data(times, msd, fit_start, fit_stop), L_ij)
 
     for i, (msd, L_ii_self) in enumerate(zip(msds[3:], onsager.results.L_ii_self[0])):
 
         # TEST CASE 1: MSDs of polyelectrolyte system
         assert np.allclose(
-            msd, groups[i].n_atoms * onsager.results.msd_self[i, 0] / volume, 
+            msd, groups[i].n_atoms * onsager.results.msd_self[i, 0] / volume,
             atol=1e-6
         )
 
-        # TEST CASE 2: Self Onsager transport coefficients of 
+        # TEST CASE 2: Self Onsager transport coefficients of
         # polyelectrolyte system
         assert np.isclose(
-            fit_data(times, msd, fit_start_self, fit_stop_self), 
+            fit_data(times, msd, fit_start_self, fit_stop_self),
             L_ii_self
         )
```


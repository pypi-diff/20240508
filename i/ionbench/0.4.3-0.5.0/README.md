# Comparing `tmp/ionbench-0.4.3.tar.gz` & `tmp/ionbench-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionbench-0.4.3.tar", last modified: Thu Apr 11 17:27:16 2024, max compression
+gzip compressed data, was "ionbench-0.5.0.tar", last modified: Wed May  8 13:07:08 2024, max compression
```

## Comparing `ionbench-0.4.3.tar` & `ionbench-0.5.0.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:16.101991 ionbench-0.4.3/
--rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5369 2024-04-11 17:27:16.038478 ionbench-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.185270 ionbench-0.4.3/ionbench/
--rw-rw-rw-   0        0        0     2060 2024-02-19 17:13:07.000000 ionbench-0.4.3/ionbench/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.464520 ionbench-0.4.3/ionbench/benchmarker/
--rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.4.3/ionbench/benchmarker/__init__.py
--rw-rw-rw-   0        0        0    38630 2024-04-11 14:47:04.000000 ionbench-0.4.3/ionbench/benchmarker/benchmarker.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:12.954381 ionbench-0.4.3/ionbench/data/
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.548807 ionbench-0.4.3/ionbench/data/loewe2016/
--rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
--rw-rw-rw-   0        0        0     2929 2024-03-25 13:04:48.000000 ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
--rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.4.3/ionbench/data/loewe2016/ikr.csv
--rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.4.3/ionbench/data/loewe2016/ikur.csv
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.583124 ionbench-0.4.3/ionbench/data/moreno2016/
--rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.4.3/ionbench/data/moreno2016/ina.csv
--rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.4.3/ionbench/data/moreno2016/moreno2016.mmt
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.703981 ionbench-0.4.3/ionbench/data/staircase/
--rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.4.3/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
--rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.4.3/ionbench/data/staircase/dataHH.csv
--rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.4.3/ionbench/data/staircase/dataMM.csv
--rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.4.3/ionbench/data/staircase/fink-2008-ikr-mm.mmt
--rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.4.3/ionbench/data/staircase/staircase-pace.mmt
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.820213 ionbench-0.4.3/ionbench/data/test/
--rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.4.3/ionbench/data/test/data.csv
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.896718 ionbench-0.4.3/ionbench/modification/
--rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.4.3/ionbench/modification/__init__.py
--rw-rw-rw-   0        0        0    16367 2024-03-21 12:50:48.000000 ionbench-0.4.3/ionbench/modification/modification.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.937620 ionbench-0.4.3/ionbench/optimisers/
--rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.4.3/ionbench/optimisers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:14.737033 ionbench-0.4.3/ionbench/optimisers/external_optimisers/
--rw-rw-rw-   0        0        0     6106 2024-04-11 14:14:58.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
--rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Bot2012.py
--rw-rw-rw-   0        0        0     5552 2024-04-11 12:48:07.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
--rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
--rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
--rw-rw-rw-   0        0        0     3223 2024-04-10 19:26:38.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
--rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
--rw-rw-rw-   0        0        0    10669 2024-04-11 13:13:49.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
--rw-rw-rw-   0        0        0     7882 2024-04-11 11:58:47.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
--rw-rw-rw-   0        0        0     9966 2024-04-11 08:50:28.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
--rw-rw-rw-   0        0        0     4293 2024-04-10 19:26:06.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
--rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/__init__.py
--rw-rw-rw-   0        0        0    16043 2024-04-11 16:06:14.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
--rw-rw-rw-   0        0        0     9144 2024-04-11 11:58:59.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     7873 2024-04-10 19:44:28.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5543 2024-04-11 13:02:08.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
--rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
--rw-rw-rw-   0        0        0     6786 2024-04-10 20:06:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
--rw-rw-rw-   0        0        0     4531 2024-04-10 20:06:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
--rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
--rw-rw-rw-   0        0        0     3221 2024-04-05 12:40:19.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.218385 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/
--rw-rw-rw-   0        0        0      311 2023-08-23 14:25:17.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/__init__.py
--rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/cmaes_pints.py
--rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
--rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/pso_pints.py
--rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/snes_pints.py
--rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/xnes_pints.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.464508 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/
--rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/__init__.py
--rw-rw-rw-   0        0        0     2567 2024-04-10 14:53:34.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
--rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/lm_scipy.py
--rw-rw-rw-   0        0        0     2893 2024-04-10 12:52:14.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
--rw-rw-rw-   0        0        0     2898 2024-04-10 19:25:15.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/powell_scipy.py
--rw-rw-rw-   0        0        0     2632 2024-04-10 15:40:25.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
--rw-rw-rw-   0        0        0     1841 2024-04-10 13:20:06.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.575691 ionbench-0.4.3/ionbench/problems/
--rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.4.3/ionbench/problems/__init__.py
--rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.4.3/ionbench/problems/loewe2016.py
--rw-rw-rw-   0        0        0    17417 2024-03-28 13:37:02.000000 ionbench-0.4.3/ionbench/problems/moreno2016.py
--rw-rw-rw-   0        0        0     9604 2024-03-28 13:37:02.000000 ionbench-0.4.3/ionbench/problems/staircase.py
--rw-rw-rw-   0        0        0     5839 2024-03-21 12:50:42.000000 ionbench-0.4.3/ionbench/problems/test.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.610028 ionbench-0.4.3/ionbench/tracker/
--rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.4.3/ionbench/tracker/__init__.py
--rw-rw-rw-   0        0        0    17362 2024-04-10 15:25:47.000000 ionbench-0.4.3/ionbench/tracker/tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.672549 ionbench-0.4.3/ionbench/uncertainty/
--rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.4.3/ionbench/uncertainty/__init__.py
--rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.4.3/ionbench/uncertainty/fim.py
--rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.4.3/ionbench/uncertainty/profile_likelihood.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.857985 ionbench-0.4.3/ionbench/utils/
--rw-rw-rw-   0        0        0      259 2024-03-22 14:22:36.000000 ionbench-0.4.3/ionbench/utils/__init__.py
--rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.4.3/ionbench/utils/autodiff.py
--rw-rw-rw-   0        0        0     1590 2024-03-20 15:36:43.000000 ionbench-0.4.3/ionbench/utils/cache.py
--rw-rw-rw-   0        0        0     4897 2024-04-05 08:53:05.000000 ionbench-0.4.3/ionbench/utils/classes_pints.py
--rw-rw-rw-   0        0        0     1516 2024-02-12 13:34:30.000000 ionbench-0.4.3/ionbench/utils/multistart.py
--rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.4.3/ionbench/utils/particle_optimisers.py
--rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.4.3/ionbench/utils/population_optimisers.py
--rw-rw-rw-   0        0        0     2216 2024-04-10 15:35:53.000000 ionbench-0.4.3/ionbench/utils/scipy_setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:16.026953 ionbench-0.4.3/ionbench.egg-info/
--rw-rw-rw-   0        0        0     5369 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3565 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 17:27:16.140020 ionbench-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     8469 2024-04-11 17:22:24.000000 ionbench-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:27:16.010904 ionbench-0.4.3/test/
--rw-rw-rw-   0        0        0     5403 2024-03-08 13:55:46.000000 ionbench-0.4.3/test/test_modifications.py
--rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.4.3/test/test_multistart.py
--rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.4.3/test/test_optimisers.py
--rw-rw-rw-   0        0        0    29297 2024-04-11 17:20:14.000000 ionbench-0.4.3/test/test_problems.py
--rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.4.3/test/test_uncertainty.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.795995 ionbench-0.5.0/
+-rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5369 2024-05-08 13:07:08.789000 ionbench-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.595162 ionbench-0.5.0/ionbench/
+-rw-rw-rw-   0        0        0     2072 2024-05-01 14:25:47.000000 ionbench-0.5.0/ionbench/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.680689 ionbench-0.5.0/ionbench/benchmarker/
+-rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.5.0/ionbench/benchmarker/__init__.py
+-rw-rw-rw-   0        0        0    39007 2024-05-08 10:48:20.000000 ionbench-0.5.0/ionbench/benchmarker/benchmarker.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.524867 ionbench-0.5.0/ionbench/data/
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.726707 ionbench-0.5.0/ionbench/data/loewe2016/
+-rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.5.0/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
+-rw-rw-rw-   0        0        0     2929 2024-04-24 14:16:20.000000 ionbench-0.5.0/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
+-rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.5.0/ionbench/data/loewe2016/ikr.csv
+-rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.5.0/ionbench/data/loewe2016/ikur.csv
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.745897 ionbench-0.5.0/ionbench/data/moreno2016/
+-rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.5.0/ionbench/data/moreno2016/ina.csv
+-rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.5.0/ionbench/data/moreno2016/moreno2016.mmt
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.802259 ionbench-0.5.0/ionbench/data/staircase/
+-rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.5.0/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
+-rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.5.0/ionbench/data/staircase/dataHH.csv
+-rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.5.0/ionbench/data/staircase/dataMM.csv
+-rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.5.0/ionbench/data/staircase/fink-2008-ikr-mm.mmt
+-rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.5.0/ionbench/data/staircase/staircase-pace.mmt
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.812837 ionbench-0.5.0/ionbench/data/test/
+-rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.5.0/ionbench/data/test/data.csv
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.835169 ionbench-0.5.0/ionbench/modification/
+-rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.5.0/ionbench/modification/__init__.py
+-rw-rw-rw-   0        0        0    16604 2024-05-08 10:41:26.000000 ionbench-0.5.0/ionbench/modification/modification.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:07.852037 ionbench-0.5.0/ionbench/optimisers/
+-rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.5.0/ionbench/optimisers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.197961 ionbench-0.5.0/ionbench/optimisers/external_optimisers/
+-rw-rw-rw-   0        0        0     6106 2024-04-11 14:14:58.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
+-rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Bot2012.py
+-rw-rw-rw-   0        0        0     5552 2024-04-11 12:48:07.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
+-rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
+-rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
+-rw-rw-rw-   0        0        0     3223 2024-04-10 19:26:38.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
+-rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
+-rw-rw-rw-   0        0        0    10669 2024-04-11 13:13:49.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
+-rw-rw-rw-   0        0        0     7882 2024-04-11 11:58:47.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
+-rw-rw-rw-   0        0        0     9966 2024-04-11 08:50:28.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
+-rw-rw-rw-   0        0        0     4293 2024-04-10 19:26:06.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
+-rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/__init__.py
+-rw-rw-rw-   0        0        0    16419 2024-05-08 10:36:44.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
+-rw-rw-rw-   0        0        0     9144 2024-04-11 11:58:59.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     7873 2024-04-10 19:44:28.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5543 2024-04-11 13:02:08.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
+-rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
+-rw-rw-rw-   0        0        0     6786 2024-04-10 20:06:09.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
+-rw-rw-rw-   0        0        0     4531 2024-04-10 20:06:09.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
+-rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
+-rw-rw-rw-   0        0        0     3221 2024-04-05 12:40:19.000000 ionbench-0.5.0/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.303766 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/
+-rw-rw-rw-   0        0        0      373 2024-04-15 16:25:51.000000 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/cmaes_pints.py
+-rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
+-rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/pso_pints.py
+-rw-rw-rw-   0        0        0     1629 2024-05-01 14:27:13.000000 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/rprop_pints.py
+-rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/snes_pints.py
+-rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.5.0/ionbench/optimisers/pints_optimisers/xnes_pints.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.407322 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/
+-rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     2567 2024-04-10 14:53:34.000000 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
+-rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/lm_scipy.py
+-rw-rw-rw-   0        0        0     2893 2024-04-10 12:52:14.000000 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
+-rw-rw-rw-   0        0        0     2898 2024-04-10 19:25:15.000000 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/powell_scipy.py
+-rw-rw-rw-   0        0        0     2580 2024-05-08 10:48:21.000000 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
+-rw-rw-rw-   0        0        0     1841 2024-04-10 13:20:06.000000 ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.474063 ionbench-0.5.0/ionbench/problems/
+-rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.5.0/ionbench/problems/__init__.py
+-rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.5.0/ionbench/problems/loewe2016.py
+-rw-rw-rw-   0        0        0    17442 2024-04-18 13:32:51.000000 ionbench-0.5.0/ionbench/problems/moreno2016.py
+-rw-rw-rw-   0        0        0     9604 2024-05-08 09:44:57.000000 ionbench-0.5.0/ionbench/problems/staircase.py
+-rw-rw-rw-   0        0        0     5818 2024-05-08 09:26:17.000000 ionbench-0.5.0/ionbench/problems/test.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.498014 ionbench-0.5.0/ionbench/tracker/
+-rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.5.0/ionbench/tracker/__init__.py
+-rw-rw-rw-   0        0        0    17279 2024-05-08 10:17:16.000000 ionbench-0.5.0/ionbench/tracker/tracker.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.557248 ionbench-0.5.0/ionbench/uncertainty/
+-rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.5.0/ionbench/uncertainty/__init__.py
+-rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.5.0/ionbench/uncertainty/fim.py
+-rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.5.0/ionbench/uncertainty/profile_likelihood.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.715634 ionbench-0.5.0/ionbench/utils/
+-rw-rw-rw-   0        0        0      301 2024-04-18 14:56:25.000000 ionbench-0.5.0/ionbench/utils/__init__.py
+-rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.5.0/ionbench/utils/autodiff.py
+-rw-rw-rw-   0        0        0     1856 2024-05-01 15:13:07.000000 ionbench-0.5.0/ionbench/utils/cache.py
+-rw-rw-rw-   0        0        0     5456 2024-05-01 14:19:59.000000 ionbench-0.5.0/ionbench/utils/classes_pints.py
+-rw-rw-rw-   0        0        0     1594 2024-05-01 15:12:51.000000 ionbench-0.5.0/ionbench/utils/multistart.py
+-rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.5.0/ionbench/utils/particle_optimisers.py
+-rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.5.0/ionbench/utils/population_optimisers.py
+-rw-rw-rw-   0        0        0     2209 2024-05-08 10:48:21.000000 ionbench-0.5.0/ionbench/utils/scipy_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.782305 ionbench-0.5.0/ionbench.egg-info/
+-rw-rw-rw-   0        0        0     5369 2024-05-08 13:07:07.000000 ionbench-0.5.0/ionbench.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3617 2024-05-08 13:07:07.000000 ionbench-0.5.0/ionbench.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:07:07.000000 ionbench-0.5.0/ionbench.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-08 13:07:07.000000 ionbench-0.5.0/ionbench.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 13:07:07.000000 ionbench-0.5.0/ionbench.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:07:08.796991 ionbench-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     8469 2024-05-08 13:04:18.000000 ionbench-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:07:08.771026 ionbench-0.5.0/test/
+-rw-rw-rw-   0        0        0     5463 2024-05-08 12:44:28.000000 ionbench-0.5.0/test/test_modifications.py
+-rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.5.0/test/test_multistart.py
+-rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.5.0/test/test_optimisers.py
+-rw-rw-rw-   0        0        0    29124 2024-05-08 12:41:12.000000 ionbench-0.5.0/test/test_problems.py
+-rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.5.0/test/test_uncertainty.py
```

### Comparing `ionbench-0.4.3/LICENSE.txt` & `ionbench-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/PKG-INFO` & `ionbench-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.3
+Version: 0.5.0
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: pints>=0.4.1
-Requires-Dist: myokit>=1.34.0
+Requires-Dist: myokit>=1.36.0
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: mygrad>=2.2.0
 Requires-Dist: pymoo>=0.6.0.1
 
 # ionBench
 A benchmarking tool for comparing different parameter optimization algorithms for ion channel models.
```

### Comparing `ionbench-0.4.3/README.md` & `ionbench-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/__init__.py` & `ionbench-0.5.0/ionbench/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 DATA_DIR = os.path.join(ROOT_DIR, "data")
 
 TEST_DIR = os.path.join(os.path.dirname(ROOT_DIR), "test")
 
 OPT_SCIPY = ['ionbench.optimisers.scipy_optimisers.' + st + '_scipy' for st in ['conjugateGD', 'lm', 'nelderMead', 'powell', 'slsqp', 'trustRegionReflective']]
 
-OPT_PINTS = ['ionbench.optimisers.pints_optimisers.' + st + '_pints' for st in ['cmaes', 'nelderMead', 'pso', 'snes', 'xnes']]
+OPT_PINTS = ['ionbench.optimisers.pints_optimisers.' + st + '_pints' for st in ['cmaes', 'nelderMead', 'pso', 'snes', 'xnes', 'rprop']]
 
 OPT_EXT = ['ionbench.optimisers.external_optimisers.' + st for st in ['curvilinearGD_Dokos2004', 'DE_Zhou2009', 'GA_Bot2012', 'GA_Cairns2017', 'GA_Gurkiewicz2007a', 'GA_Gurkiewicz2007b', 'GA_Smirnov2020', 'hybridPSOTRR_Loewe2016', 'hybridPSOTRRTRR_Loewe2016', 'NMPSO_Clausen2020', 'NMPSO_Liu2011', 'patternSearch_Kohjitani2022', 'ppso_Chen2012', 'pso_Cabo2022', 'PSO_Loewe2016', 'pso_Seemann2009', 'PSOTRR_Loewe2016', 'randomSearch_Vanier1999', 'SA_Vanier1999', 'SPSA_Spall1998', 'stochasticSearch_Vanier1999']]
 
 OPT_ALL = OPT_SCIPY + OPT_PINTS + OPT_EXT
 
 N_MOD_SCIPY = [2, 2, 3, 3, 1, 3]
-N_MOD_PINTS = [2, 0, 0, 0, 0]
+N_MOD_PINTS = [2, 0, 0, 0, 0, 0]
 N_MOD_EXT = [3, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
 N_MOD_ALL = N_MOD_SCIPY + N_MOD_PINTS + N_MOD_EXT
 
 APP_SCIPY = []
 for i in range(len(OPT_SCIPY)):
     for j in range(N_MOD_SCIPY[i]):
         APP_SCIPY.append({'module': OPT_SCIPY[i], 'modNum': j + 1, 'kwargs': {}})
```

### Comparing `ionbench-0.4.3/ionbench/benchmarker/benchmarker.py` & `ionbench-0.5.0/ionbench/benchmarker/benchmarker.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,23 @@
             self.WEIGHTS = None
         if not hasattr(self, '_ANALYTICAL_MODEL'):
             self._ANALYTICAL_MODEL = None
         if not hasattr(self, '_RATE_FUNCTIONS'):
             self._RATE_FUNCTIONS = None
 
         self.useScaleFactors = False
-        self.parametersBounded = False  # Should the parameters be bounded
-        self.ratesBounded = False  # Should the rates be bounded
         self.logTransformParams = [False] * self.n_parameters()  # Are any of the parameter log-transformed
+        if 'staircase' in self.NAME:
+            self.add_parameter_bounds()
+            self.add_rate_bounds()
+        else:
+            self.parametersBounded = False  # Should the parameters be bounded
+            self.ratesBounded = False  # Should the rates be bounded
         self.plotter = True  # Should the performance metrics be plotted when evaluate() is called
-        self.tracker = Tracker(self._TRUE_PARAMETERS)  # Tracks the performance metrics
+        self.tracker = Tracker()  # Tracks the performance metrics
         self.V_LOW = -120
         self.V_HIGH = 60
 
         # Set numpy writeable flags
         self._TRUE_PARAMETERS.flags['WRITEABLE'] = False
         self._LOWER_BOUND.flags['WRITEABLE'] = False
         self._UPPER_BOUND.flags['WRITEABLE'] = False
@@ -297,25 +301,29 @@
     def reset(self, fullReset=True):
         """
         Resets the benchmarker. This clears the simulation object and restarts the performance tracker. Optionally, the transforms and bounds can be turned off.
 
         Parameters
         ----------
         fullReset : bool, optional
-            If True, transforms and bounds will be reset (turned off). The default is True.
+            If True, transforms and bounds will be reset (turned off except staircase which will turn bounds on). The default is True.
         """
         self.sim.reset()
         if self.sensitivityCalc:
             self.simSens.reset()
-        self.tracker = Tracker(self._TRUE_PARAMETERS)
+        self.tracker = Tracker()
         if fullReset:
             self.log_transform([False] * self.n_parameters())
             self.useScaleFactors = False
-            self.parametersBounded = False
-            self.ratesBounded = False
+            if 'staircase' in self.NAME:
+                self.add_rate_bounds()
+                self.add_parameter_bounds()
+            else:
+                self.parametersBounded = False
+                self.ratesBounded = False
             self.lb = np.copy(self._LOWER_BOUND)
             self.ub = np.copy(self._UPPER_BOUND)
             self.RATE_MIN = 1.67e-5
             self.RATE_MAX = 1e3
 
     def cost(self, parameters, incrementSolveCounter=True):
         """
@@ -421,17 +429,17 @@
         # Check model is set up to solve for sensitivities
         if not self.sensitivityCalc:
             warnings.warn(
                 "Current benchmarker problem not configured to use derivatives. Will recompile the simulation object with this enabled.")
             self.use_sensitivities()
         # Now to find grad, cost, J (jacobian) and error (residuals)
         # First check if the parameters are out of bounds
-        # Abort solving if the parameters are out of bounds (if staircase, don't check bounded)
-        inParameterBounds = self.in_parameter_bounds(parameters, boundedCheck='staircase' not in self.NAME)
-        inRateBounds = self.in_rate_bounds(parameters, boundedCheck='staircase' not in self.NAME)
+        # Abort solving if the parameters are out of bounds
+        inParameterBounds = self.in_parameter_bounds(parameters)
+        inRateBounds = self.in_rate_bounds(parameters)
         if not inParameterBounds or not inRateBounds:
             # Gradient out of bounds so use penalty function
             # Calculate gradient of penalty function
             parametersMG = [mg.Tensor(p) for p in parameters]
             penalty = self.parameter_penalty(parametersMG) + self.rate_penalty(parametersMG)
             assert penalty.data > 0
             penalty.backward()
@@ -451,15 +459,15 @@
             self.simSens.reset()
             self.set_params(parameters)
             self.set_steady_state(parameters)
             start = time.monotonic()
             try:
                 curr, sens = self.solve_with_sensitivities(times=np.arange(0, self.T_MAX, self.TIMESTEP))
                 sens = np.array(sens)
-            except myokit.SimulationError:
+            except (myokit.SimulationError, np.linalg.LinAlgError):
                 # If the model fails to solve, we will assume the cost is infinite and the jacobian/gradient points back towards good parameters
                 end = time.monotonic()
                 warnings.warn(
                     'Tried to evaluate gradient but model failed to solve, likely poor choice of parameters. ionBench will try to resolve this by assuming infinite cost and a gradient that points back towards good parameters.')
                 self.tracker.update(parameters, incrementSolveCounter=False, solveType='grad',
                                     solveTime=end - start)
                 curr = np.array([np.inf] * len(self.DATA))
@@ -663,15 +671,15 @@
         if continueOnError:
             try:
                 if 'staircase' in self.NAME:
                     log = self.sim.run(self.T_MAX + 1, log=[self._OUTPUT_NAME], log_times=times)
                 else:
                     log = self.sim.run(self.T_MAX + 1, log_times=times)
                 return np.array(log[self._OUTPUT_NAME])
-            except myokit.SimulationError:
+            except (myokit.SimulationError, np.linalg.LinAlgError):
                 warnings.warn("Failed to solve model. Will report infinite output in the hope of continuing the run.")
                 return np.array([np.inf] * len(times))
         else:
             log = self.sim.run(self.T_MAX + 1, log_times=times)
             return np.array(log[self._OUTPUT_NAME])
 
     def simulate(self, parameters, times, continueOnError=True, incrementSolveCounter=True):
@@ -699,17 +707,17 @@
         parameters = self.original_parameter_space(parameters)  # Creates a copy of the parameter vector
 
         # Reset the simulation
         self.sim.reset()
 
         # Abort solving if the parameters are out of bounds
         penalty = 0
-        if self.parametersBounded or 'staircase' in self.NAME:
+        if self.parametersBounded:
             penalty += self.parameter_penalty(parameters)
-        if self.ratesBounded or 'staircase' in self.NAME:
+        if self.ratesBounded:
             penalty += self.rate_penalty(parameters)
         if penalty > 0:
             self.tracker.update(parameters, cost=penalty, incrementSolveCounter=False)
             return np.add(penalty, self.DATA)
 
         # Set the parameters in the simulation object
         self.set_params(parameters)
@@ -815,37 +823,41 @@
         This method reports the performance metrics for the best parameter vector (calling evaluate() does NOT increase the number of cost function evaluations). If benchmarker.plotter = True, then it also plots the performance metrics over the course of the optimisation.
         """
         print('')
         print('========================================')
         print('===      Evaluating Performance      ===')
         print('========================================')
         print('')
-        print('Number of cost evaluations:      ' + str(self.tracker.solveCount))
+        print('Number of cost evaluations:      ' + str(self.tracker.costSolveCount))
         print('Number of grad evaluations:      ' + str(self.tracker.gradSolveCount))
         print('Best cost:                       {0:.6f}'.format(self.tracker.bestCost))
         self.tracker.report_convergence(self.COST_THRESHOLD)
         print('')
         if self.plotter:
-            self.tracker.plot()
-            self.sim.reset()
-            self.set_params(self.tracker.firstParams)
-            self.set_steady_state(self.tracker.firstParams)
-            firstOut = self.solve_model(np.arange(0, self.T_MAX, self.TIMESTEP), continueOnError=True)
-            self.sim.reset()
-            self.set_params(self.original_parameter_space(self.tracker.bestParams))
-            self.set_steady_state(self.original_parameter_space(self.tracker.bestParams))
-            lastOut = self.solve_model(np.arange(0, self.T_MAX, self.TIMESTEP), continueOnError=True)
-            plt.figure()
-            if "moreno" in self.NAME:
-                plt.plot(self.DATA)
-                plt.plot(firstOut)
-                plt.plot(lastOut)
-                plt.ylabel('Summary Statistics')
-            else:
-                plt.plot(np.arange(0, self.T_MAX, self.TIMESTEP), self.DATA)
-                plt.plot(np.arange(0, self.T_MAX, self.TIMESTEP), firstOut)
-                plt.plot(np.arange(0, self.T_MAX, self.TIMESTEP), lastOut)
-                plt.ylabel('Current')
-                plt.xlabel('Time (ms)')
-            plt.legend(['Data', 'First Parameters', 'Best Parameters'])
-            plt.title('Improvement after fitting: ' + self.NAME)
-            plt.show()
+            try:
+                self.tracker.plot()
+                self.sim.reset()
+                self.set_params(self.tracker.firstParams)
+                self.set_steady_state(self.tracker.firstParams)
+                firstOut = self.solve_model(np.arange(0, self.T_MAX, self.TIMESTEP), continueOnError=True)
+                self.sim.reset()
+                self.set_params(self.tracker.bestParams)
+                self.set_steady_state(self.tracker.bestParams)
+                lastOut = self.solve_model(np.arange(0, self.T_MAX, self.TIMESTEP), continueOnError=True)
+                plt.figure()
+                if "moreno" in self.NAME:
+                    plt.plot(self.DATA)
+                    plt.plot(firstOut)
+                    plt.plot(lastOut)
+                    plt.ylabel('Summary Statistics')
+                else:
+                    plt.plot(np.arange(0, self.T_MAX, self.TIMESTEP), self.DATA)
+                    plt.plot(np.arange(0, self.T_MAX, self.TIMESTEP), firstOut)
+                    plt.plot(np.arange(0, self.T_MAX, self.TIMESTEP), lastOut)
+                    plt.ylabel('Current')
+                    plt.xlabel('Time (ms)')
+                plt.legend(['Data', 'First Parameters', 'Best Parameters'])
+                plt.title('Improvement after fitting: ' + self.NAME)
+                plt.show()
+            except IndexError:
+                # If the tracker has no data (e.g. tracker.firstParams is empty), then we can't plot
+                pass
```

### Comparing `ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt` & `ionbench-0.5.0/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt` & `ionbench-0.5.0/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/loewe2016/ikr.csv` & `ionbench-0.5.0/ionbench/data/loewe2016/ikr.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/loewe2016/ikur.csv` & `ionbench-0.5.0/ionbench/data/loewe2016/ikur.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/moreno2016/ina.csv` & `ionbench-0.5.0/ionbench/data/moreno2016/ina.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/moreno2016/moreno2016.mmt` & `ionbench-0.5.0/ionbench/data/moreno2016/moreno2016.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/staircase/beattie-2017-ikr-hh.mmt` & `ionbench-0.5.0/ionbench/data/staircase/beattie-2017-ikr-hh.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/staircase/dataHH.csv` & `ionbench-0.5.0/ionbench/data/staircase/dataHH.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/staircase/dataMM.csv` & `ionbench-0.5.0/ionbench/data/staircase/dataMM.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/staircase/fink-2008-ikr-mm.mmt` & `ionbench-0.5.0/ionbench/data/staircase/fink-2008-ikr-mm.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/data/staircase/staircase-pace.mmt` & `ionbench-0.5.0/ionbench/data/staircase/staircase-pace.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/modification/modification.py` & `ionbench-0.5.0/ionbench/modification/modification.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,18 @@
             bm.add_parameter_bounds()
             bm.lb = self.customBounds[0]
             bm.ub = self.customBounds[1]
         else:
             print(
                 "'" + setting + "' is not a valid option for bounds. Please use either 'off', 'on', or 'Custom'.")
 
+        # If staircase, override with True
+        if 'staircase' in bm.NAME:
+            bm.add_parameter_bounds()
+
     @staticmethod
     def apply_rate_bounds(setting, bm):
         """
         Apply the rate bounds setting to a benchmarker.
 
         Parameters
         ----------
@@ -122,14 +126,18 @@
             bm.ratesBounded = False
         elif setting.lower() == 'on':
             bm.add_rate_bounds()
         else:
             print(
                 "'" + setting + "' is not a valid option for bounds. Please use either 'off', or 'on'.")
 
+        # If staircase, override with True
+        if 'staircase' in bm.NAME:
+            bm.add_rate_bounds()
+
     @staticmethod
     def apply_scale_factors(setting, bm):
         """
         Apply the scale factor setting to a benchmarker.
 
         Parameters
         ----------
@@ -287,15 +295,15 @@
 class Liu2011(Modification):
     def __init__(self):
         super().__init__(name='Liu2011', logTransform='off', parameterBounds='on', scaleFactors='off')
 
 
 class Loewe2016(Modification):
     def __init__(self):
-        super().__init__(name='Loewe2012', logTransform='off', parameterBounds='on', scaleFactors='off')
+        super().__init__(name='Loewe2016', logTransform='off', parameterBounds='on', scaleFactors='off')
 
 
 class Maryak1998(Modification):
     def __init__(self):
         super().__init__(name='Maryak1998', logTransform='off', parameterBounds='off', scaleFactors='off')
```

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/DE_Zhou2009.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/DE_Zhou2009.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Bot2012.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Bot2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Cairns2017.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Cairns2017.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/SA_Vanier1999.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/SA_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/__init__.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/__init__.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,21 +242,27 @@
                 out = scipy.optimize.brent(SSE, brack=(0, 1, 1e9), tol=1e-8, full_output=True)
                 alpha = out[0]
                 falphaNew = out[1]
             except ValueError as e:
                 # Failed. Time to find out why and try to recover
                 # Option 1: NaNs in either SSE(0) or SSE(1e9) but not SSE(1) so step still viable
                 if (np.isnan(SSE(0)) or np.isnan(SSE(1e9))) and not np.isnan(SSE(1)):
-                    # If SSE(1) is NOT WORSE than SSE(0) or SSE(1e9), then we can assume that it is a good step
+                    # If SSE(1) is NOT WORSE than SSE(0) or SSE(1e9) (accounting for SSE(0) or SSE(1e9) being NaN), then we can assume that it is a good step
                     if debug:
                         print(
                             f'NaNs were found. SSE(0): {SSE(0)}, SSE(1): {SSE(1)}, SSE(1e9): {SSE(1e9)}. Will try to continue if possible')
                     if not SSE(1) > SSE(0) and not SSE(1) > SSE(1e9):
                         alpha = 1
                         falphaNew = SSE(alpha)
+                    elif not SSE(1e-6) > SSE(0) and not SSE(1e-6) > SSE(1e9):
+                        alpha = 1e-6
+                        falphaNew = SSE(alpha)
+                    elif not SSE(1e-9) > SSE(0) and not SSE(1e-9) > SSE(1e9):
+                        alpha = 1e-9
+                        falphaNew = SSE(alpha)
                     else:
                         print(f'Failed. SSE(0): {SSE(0)}, SSE(1): {SSE(1)}, SSE(1e9): {SSE(1e9)}')
                         raise e
                 # Option 2: SSE(1e9) is best - take full step
                 elif SSE(1e9) <= SSE(1) and SSE(1e9) <= SSE(0):
                     # SSE(1e9)<SSE(1),SSE(0)
                     alpha = 1e9
```

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/ppso_Chen2012.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/ppso_Chen2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Cabo2022.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/pso_Cabo2022.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Seemann2009.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/pso_Seemann2009.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py` & `ionbench-0.5.0/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/cmaes_pints.py` & `ionbench-0.5.0/ionbench/optimisers/pints_optimisers/cmaes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/nelderMead_pints.py` & `ionbench-0.5.0/ionbench/optimisers/pints_optimisers/nelderMead_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/pso_pints.py` & `ionbench-0.5.0/ionbench/optimisers/pints_optimisers/pso_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/snes_pints.py` & `ionbench-0.5.0/ionbench/optimisers/pints_optimisers/snes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/xnes_pints.py` & `ionbench-0.5.0/ionbench/optimisers/pints_optimisers/xnes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py` & `ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/lm_scipy.py` & `ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/lm_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py` & `ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/powell_scipy.py` & `ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/powell_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py` & `ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     grad = ionbench.utils.cache.get_cached_grad(bm)
 
     if x0 is None:
         x0 = bm.sample()
         if debug:
             print('Sampling x0')
             print(x0)
-    if bm.ratesBounded or 'staircase' in bm.NAME:
+    if bm.ratesBounded:
         constraints = {'type': 'eq', 'fun': lambda p: bm.parameter_penalty(bm.original_parameter_space(p))+bm.rate_penalty(bm.original_parameter_space(p))}
     else:
         constraints = ()
-    if bm.parametersBounded or 'staircase' in bm.NAME:
+    if bm.parametersBounded:
         bounds = minimize_bounds(bm)
         out = scipy.optimize.minimize(cost, x0, jac=grad, method='SLSQP', constraints=constraints, options={'disp': debug, 'maxiter': maxIter}, bounds=bounds)
     else:
         out = scipy.optimize.minimize(cost, x0, jac=grad, method='SLSQP', constraints=constraints, options={'disp': debug, 'maxiter': maxIter})
 
     if debug:
         print(f'Cost of {out.fun} found at:')
```

### Comparing `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py` & `ionbench-0.5.0/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/problems/loewe2016.py` & `ionbench-0.5.0/ionbench/problems/loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/problems/moreno2016.py` & `ionbench-0.5.0/ionbench/problems/moreno2016.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         """
         if continueOnError:
             try:
                 # Run a simulation
                 log = self.sim.run(self.T_MAX + 1, log_times=self._logTimes)
                 # log = self.sim.run(self.T_MAX + 1, log_times=self._logTimes, log=[self._OUTPUT_NAME]) # Setting output name only works for ODE sims, not analytical
                 return self.sum_stats(np.array(log[self._OUTPUT_NAME], dtype='float64'))
-            except myokit.SimulationError:
+            except (myokit.SimulationError, np.linalg.LinAlgError):
                 warnings.warn("Failed to solve model. Will report infinite output in the hope of continuing the run.")
                 return np.array([np.inf] * len(self.DATA), dtype='float64')
         else:
             log = self.sim.run(self.T_MAX + 1, log_times=self._logTimes)
             # log = self.sim.run(self.T_MAX + 1, log_times=self._logTimes, log=[self._OUTPUT_NAME]) # Setting outputName only works for ODE sims, not analytical
             return self.sum_stats(np.array(log[self._OUTPUT_NAME], dtype='float64'))
```

### Comparing `ionbench-0.4.3/ionbench/problems/staircase.py` & `ionbench-0.5.0/ionbench/problems/staircase.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/problems/test.py` & `ionbench-0.5.0/ionbench/problems/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                     grad[i] = np.dot(error, sens[:, i]) / (len(error) * cost)
                 else:
                     grad[i] = 0
 
         return self.map_derivative(J, grad, parameters, inInputSpace, returnCost, residuals, cost, error)
 
     def reset(self, fullReset=True):
-        self.tracker = ionbench.tracker.Tracker(self._TRUE_PARAMETERS)
+        self.tracker = ionbench.tracker.Tracker()
         if fullReset:
             self.log_transform([False] * self.n_parameters())
             self.useScaleFactors = False
             self.parametersBounded = False
             self.ratesBounded = False
             self.lb = np.copy(self._LOWER_BOUND)
             self.ub = np.copy(self._UPPER_BOUND)
```

### Comparing `ionbench-0.4.3/ionbench/tracker/tracker.py` & `ionbench-0.5.0/ionbench/tracker/tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,32 @@
     This class contains two methods: update(), and plot().
 
     update() is called everytime a parameter vector is simulated in the benchmarker (for example, in bm.cost()) and updates the performance metric vectors.
 
     plot() is called during the benchmarker's .evaluate() method. It plots the performance metrics as functions of time (in the order in which parameter vectors were evaluated).
     """
 
-    def __init__(self, trueParams):
-        self.costs = []
-        self.paramRMSRE = []
-        self.paramIdentifiedCount = []
-        self.solveCount = 0
-        self.gradSolveCount = 0
-        self.firstParams = []
-        self.modelSolves = []
-        self.gradSolves = []
-        self._TRUE_PARAMETERS = np.copy(trueParams)
-        self._TRUE_PARAMETERS.flags['WRITEABLE'] = False
-        self.evals = []
-        self.bestParams = []
-        self.bestCost = np.inf
-        self.bestCosts = []
-        self.costTimes = []
-        self.gradTimes = []
+    def __init__(self):
+        # Performance metrics over time
+        self.costs = []  # Cost at evaluation (including from grad calls)
+        self.costSolves = []  # Number of cost solves at a given evaluation
+        self.gradSolves = []  # Number of grad solves at a given evaluation
+        self.evals = []  # (evaluated parameters, solve type) at each evaluation
+        self.bestCosts = []  # Best cost so far at each evaluation
+        self.costTimes = []  # Time taken for cost solves at each evaluation (0 for grad solves)
+        self.gradTimes = []  # Time taken for grad solves at each evaluation (0 for cost solves)
+
+        # Best and first parameters
+        self.bestParams = []  # Best parameters seen so far (lowest cost)
+        self.bestCost = np.inf  # Best cost seen so far (includes cost from grad evaluations)
+        self.firstParams = []  # First parameters, evaluated at the start of the optimisation
+
+        # Counters
+        self.costSolveCount = 0  # Current number of cost evaluations
+        self.gradSolveCount = 0  # Current number of grad evaluations
 
     def update(self, estimatedParams, cost=np.inf, incrementSolveCounter=True, solveType='cost', solveTime=np.NaN):
         """
         This method updates the performance metric tracking vectors with new values. It should only need to be called by a benchmarker class.
 
         Parameters
         ----------
@@ -61,37 +62,46 @@
             A float representing the time, in seconds, it took to solve the model.
 
         Returns
         -------
         None.
 
         """
+        # Cast to numpy array
+        estimatedParams = np.array(estimatedParams)
+
+        # Set first parameters if not already set
         if len(self.firstParams) == 0:
             self.firstParams = np.copy(estimatedParams)
             self.firstParams.flags['WRITEABLE'] = False
-        # Cast to numpy arrays
-        estimatedParams = np.array(estimatedParams)
+
         # Update performance metrics
-        self.paramRMSRE.append(
-            np.sqrt(np.mean(((estimatedParams - self._TRUE_PARAMETERS) / self._TRUE_PARAMETERS) ** 2)))
-        self.paramIdentifiedCount.append(
-            np.sum(np.abs((estimatedParams - self._TRUE_PARAMETERS) / self._TRUE_PARAMETERS) < 0.05))
+        # Update list of costs
         self.costs.append(cost)
+
+        # If the model was solved (anything but penalty function), increment the solve counter
         if incrementSolveCounter:
             if solveType == 'cost':
-                self.solveCount += 1
-                self.costTimes.append(solveTime)
+                self.costSolveCount += 1
             elif solveType == 'grad':
                 self.gradSolveCount += 1
-                self.gradTimes.append(solveTime)
             self.check_repeated_param(estimatedParams, solveType)
         else:
+            # If not solved, set solveTime to 0 and label as unsolved with solveType='none'
+            solveTime = 0
             solveType = 'none'
+        # Update list of times (update with 0 if different solve type)
+        self.costTimes.append(solveTime if solveType == 'cost' else 0)
+        self.gradTimes.append(solveTime if solveType == 'grad' else 0)
+
+        # Update the list of evaluated parameters
         self.evals.append((estimatedParams, solveType))
-        self.modelSolves.append(self.solveCount)
+
+        # Update the list of cost and grad solve counts
+        self.costSolves.append(self.costSolveCount)
         self.gradSolves.append(self.gradSolveCount)
         if cost < self.bestCost:
             self.bestParams = estimatedParams
             self.bestCost = cost
         self.bestCosts.append(self.bestCost)
 
     def plot(self):
@@ -159,56 +169,48 @@
     def save(self, filename):
         """
         Saves the tracked variables. Useful to store results to plot later.
 
         Parameters
         ----------
         filename : string
-            Filename for storing the tracked variables (solveCount, costs, modelSolves, paramRMSRE, paramIdentifiedCount). Variables will be pickled and stored in working directory.
+            Filename for storing the tracked variables. Variables will be pickled and stored in working directory.
 
         Returns
         -------
         None.
 
         """
-        data = {'solveCount': self.solveCount, 'gradSolveCount': self.gradSolveCount, 'costs': self.costs,
-                'modelSolves': self.modelSolves, 'gradSolves': self.gradSolves, 'paramRMSE': self.paramRMSRE,
-                'paramIdentifiedCount': self.paramIdentifiedCount, 'firstParams': self.firstParams, 'evals': self.evals,
-                'bestParams': self.bestParams, 'bestCost': self.bestCost, 'bestCosts': self.bestCosts,
-                'costTimes': self.costTimes,
-                'gradTimes': self.gradTimes}
+        data = {'costSolveCount': self.costSolveCount, 'gradSolveCount': self.gradSolveCount, 'costs': self.costs,
+                'costSolves': self.costSolves, 'gradSolves': self.gradSolves, 'firstParams': self.firstParams,
+                'evals': self.evals, 'bestParams': self.bestParams, 'bestCost': self.bestCost,
+                'bestCosts': self.bestCosts, 'costTimes': self.costTimes, 'gradTimes': self.gradTimes}
         with open(filename, 'wb') as f:
             pickle.dump(data, f)
 
     def load(self, filename):
         """
         Loads the tracked variables. Useful to store results to plot later.
 
         Parameters
         ----------
         filename : string
-            Filename to load the stored tracked variables (solveCount, costs, modelSolves, paramRMSRE, paramIdentifiedCount). Variables will be read for the working directory. Must be saved using the .save() method associated with a tracker.
+            Filename to load the stored tracked variables. Variables will be read for the working directory. Must be saved using the .save() method associated with a tracker.
 
         Returns
         -------
         None.
 
         """
         with open(filename, 'rb') as f:
             data = pickle.load(f)
-        keys = ['solveCount', 'gradSolveCount', 'costs', 'modelSolves', 'gradSolves', 'paramRMSE',
-                'paramIdentifiedCount', 'firstParams', 'evals', 'bestParams', 'bestCost', 'bestCosts', 'costTimes',
+        keys = ['costSolveCount', 'gradSolveCount', 'costs', 'costSolves', 'gradSolves', 'firstParams', 'evals', 'bestParams', 'bestCost', 'bestCosts', 'costTimes',
                 'gradTimes']
-        try:
-            self.solveCount, self.gradSolveCount, self.costs, self.modelSolves, self.gradSolves, self.paramRMSRE, self.paramIdentifiedCount, self.firstParams, self.evals, self.bestParams, self.bestCost, self.bestCosts, self.costTimes, self.gradTimes = [
-                data[key] if key in data.keys() else None for key in keys]
-        except AttributeError:
-            # Assume old (v0.3.4) format
-            self.solveCount, self.gradSolveCount, self.costs, self.modelSolves, self.gradSolves, self.paramRMSRE, self.paramIdentifiedCount, self.firstParams, self.evals, self.bestParams, self.bestCost, self.costTimes, self.gradTimes = data
-            self.bestCosts = np.minimum.accumulate(self.costs)
+        self.costSolveCount, self.gradSolveCount, self.costs, self.costSolves, self.gradSolves, self.firstParams, self.evals, self.bestParams, self.bestCost, self.bestCosts, self.costTimes, self.gradTimes = [
+            data[key] if key in data.keys() else None for key in keys]
 
     def report_convergence(self, threshold):
         """
         Reports the performance metrics at the point of convergence, defined using the two termination criteria: cost threshold and cost unchanged.
 
         Parameters
         ----------
@@ -221,20 +223,20 @@
 
         """
         i = self.when_converged(threshold)
         if i is None:
             print('Convergence reason:              Optimiser terminated early.')
             i = len(self.bestCosts) - 1
         else:
-            print('Convergence reason:              ' + ('Cost threshold' if self.cost_threshold(threshold,
-                                                                                                i) else 'Cost unchanged'))
-        print('Cost evaluations at convergence: ' + str(self.modelSolves[i] if len(self.modelSolves) > 0 else None))
+            print('Convergence reason:              ' + ('Cost threshold' if
+                                                         self.cost_threshold(threshold, i) else 'Cost unchanged'))
+        print('Cost evaluations at convergence: ' + str(self.costSolves[i] if len(self.costSolves) > 0 else None))
         print('Grad evaluations at convergence: ' + str(self.gradSolves[i] if len(self.gradSolves) > 0 else None))
         print('Best cost at convergence:        {0:.6f}'.format(self.bestCosts[i] if len(self.bestCosts) > 0 else self.bestCost))
-        if len(self.modelSolves) > 0:
+        if len(self.costSolves) > 0:
             costTime, gradTime = self.total_solve_time(i)
         else:
             costTime = 0
             gradTime = 0
         print('Model solve time at convergence: {0:.6f}'.format(costTime))
         print('Grad solve time at convergence:  {0:.6f}'.format(gradTime))
 
@@ -337,17 +339,15 @@
         Returns
         -------
         costTime : float
             The total time taken to solve the model (excluding solves with sensitivities) up to (and including) the i-th solve.
         gradTime : float
             The total time taken to solve the model (excluding solves without sensitivities) up to (and including) the i-th solve.
         """
-        gradCount = self.gradSolves[i]
-        costCount = self.modelSolves[i]
-        return np.sum(self.costTimes[:costCount + 1]), np.sum(self.gradTimes[:gradCount + 1])
+        return np.sum(self.costTimes[:i + 1]), np.sum(self.gradTimes[:i + 1])
 
     def check_repeated_param(self, param, solveType):
         """
         Checks if a parameter vector has been evaluated before and reports a warning if it has.
 
         Parameters
         ----------
```

### Comparing `ionbench-0.4.3/ionbench/uncertainty/fim.py` & `ionbench-0.5.0/ionbench/uncertainty/fim.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/uncertainty/profile_likelihood.py` & `ionbench-0.5.0/ionbench/uncertainty/profile_likelihood.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/utils/autodiff.py` & `ionbench-0.5.0/ionbench/utils/autodiff.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/utils/cache.py` & `ionbench-0.5.0/ionbench/utils/cache.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 from functools import lru_cache
+import copy
+
+cachedFunctions = []
+
+
+def cache():
+    def decorator(func):
+        func = lru_cache(maxsize=None)(func)
+        cachedFunctions.append(func)
+        return func
+    return decorator
+
+
+def clear_all_caches():
+    for func in cachedFunctions:
+        func.cache_clear()
 
 
 def get_cached_cost(bm):
     """
     Returns a cached version of the bm.cost() function for the inputted benchmark.
 
     Parameters
@@ -12,15 +28,15 @@
 
     Returns
     -------
     cost_func : function
         Cached cost function.
     """
 
-    @lru_cache(maxsize=None)
+    @cache()
     def cached_func(p):
         return bm.cost(p)
 
     def cost_func(p):
         return cached_func(tuple(p))
 
     return cost_func
@@ -37,15 +53,15 @@
 
     Returns
     -------
     signed_error : function
         Cached signed error (residuals) function.
     """
 
-    @lru_cache(maxsize=None)
+    @cache()
     def cached_func(p):
         return bm.signed_error(p)
 
     def signed_error(p):
         return cached_func(tuple(p))
 
     return signed_error
@@ -64,15 +80,15 @@
 
     Returns
     -------
     grad : function
         Cached grad function.
     """
 
-    @lru_cache(maxsize=None)
+    @cache()
     def cached_func(p):
         return bm.grad(p, **kwargs)
 
     def grad(p):
-        return cached_func(tuple(p))
+        return copy.deepcopy(cached_func(tuple(p)))
 
     return grad
```

### Comparing `ionbench-0.4.3/ionbench/utils/classes_pints.py` & `ionbench-0.5.0/ionbench/utils/classes_pints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pints
 import numpy as np
-from functools import lru_cache
 import ionbench
 
 
 def pints_setup(bm, x0, method, maxIter, debug, forceUnbounded=False):
     """
     Set up a Pints model and optimisation controller for a benchmarker.
     Parameters
@@ -33,15 +32,16 @@
         x0 = bm.sample()
     model = Model(bm)
     if 'moreno' in bm.NAME:
         times = np.arange(len(bm.DATA))
     else:
         times = np.arange(0, bm.T_MAX, bm.TIMESTEP)
     problem = pints.SingleOutputProblem(model, times, model.bm.DATA)
-    error = pints.RootMeanSquaredError(problem)
+    error = ErrorWithGrad(problem, bm)
+
     if bm.parametersBounded and not forceUnbounded:
         if bm.ratesBounded:
             boundaries = AdvancedBoundaries(bm)
         else:
             boundaries = pints.RectangularBoundaries(bm.input_parameter_space(bm.lb), bm.input_parameter_space(bm.ub))
         counter = 1
         while not boundaries.check(x0):
@@ -55,14 +55,29 @@
     opt.set_max_iterations(maxIter)
     opt.set_max_unchanged_iterations(threshold=1e-7)
     if debug:
         opt.set_log_interval(iters=1)
     return model, opt
 
 
+class ErrorWithGrad(pints.RootMeanSquaredError):
+    """
+    Pints error measure that uses RMSE and additionally defines the gradient of the RMSE.
+    """
+    def __init__(self, problem, bm):
+        super().__init__(problem)
+        self.bm = bm
+        self.grad = ionbench.utils.cache.get_cached_grad(bm, returnCost=True)
+
+    def evaluateS1(self, x):
+        if 'moreno' in self.bm.NAME:
+            raise NotImplementedError('Moreno uses weighted RMSE in cost and grad, pints uses unweighted RMSE. No unweighted RMSE grad is available for Moreno.')
+        return self.grad(x)
+
+
 class Model(pints.ForwardModel):
     """
     A Pints forwards model containing a benchmarker class.
     """
 
     def __init__(self, bm):
         """
```

### Comparing `ionbench-0.4.3/ionbench/utils/multistart.py` & `ionbench-0.5.0/ionbench/utils/multistart.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains the multistart function (referenced as ionbench.multistart) which can perform multiple runs of the same optimisation function starting at different initial conditions.
 """
+import ionbench.utils.cache
 
 
 def multistart(opt, bm, initParams, filename, **kwargs):
     """
     Run an optimiser multiple times from different starting location.
 
     Parameters
@@ -29,8 +30,9 @@
     for i in range(len(initParams)):
         out = opt(bm, x0=initParams[i], **kwargs)
         if not filename == '':
             bm.tracker.save(filename + '_run' + str(i) + '.pickle')
         print(out)
         outs.append(out)
         bm.reset(fullReset=False)
+        ionbench.utils.cache.clear_all_caches()
     return outs
```

### Comparing `ionbench-0.4.3/ionbench/utils/particle_optimisers.py` & `ionbench-0.5.0/ionbench/utils/particle_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/utils/population_optimisers.py` & `ionbench-0.5.0/ionbench/utils/population_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/ionbench/utils/scipy_setup.py` & `ionbench-0.5.0/ionbench/utils/scipy_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             print('Sampling x0')
             print(x0)
 
     if debug:
         verbose = 2
     else:
         verbose = 1
-    if bm.parametersBounded or 'staircase' in bm.NAME:
+    if bm.parametersBounded and method != 'lm':
         bounds = minimize_bounds(bm)
     else:
         bounds = (-np.inf, np.inf)
     out = scipy.optimize.least_squares(signed_error, x0, method=method, bounds=bounds, jac=grad, verbose=verbose, max_nfev=maxIter,
                                        **kwargs)
 
     if debug:
```

### Comparing `ionbench-0.4.3/ionbench.egg-info/PKG-INFO` & `ionbench-0.5.0/ionbench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.3
+Version: 0.5.0
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: pints>=0.4.1
-Requires-Dist: myokit>=1.34.0
+Requires-Dist: myokit>=1.36.0
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: mygrad>=2.2.0
 Requires-Dist: pymoo>=0.6.0.1
 
 # ionBench
 A benchmarking tool for comparing different parameter optimization algorithms for ion channel models.
```

### Comparing `ionbench-0.4.3/ionbench.egg-info/SOURCES.txt` & `ionbench-0.5.0/ionbench.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 ionbench/optimisers/external_optimisers/pso_Seemann2009.py
 ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
 ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
 ionbench/optimisers/pints_optimisers/__init__.py
 ionbench/optimisers/pints_optimisers/cmaes_pints.py
 ionbench/optimisers/pints_optimisers/nelderMead_pints.py
 ionbench/optimisers/pints_optimisers/pso_pints.py
+ionbench/optimisers/pints_optimisers/rprop_pints.py
 ionbench/optimisers/pints_optimisers/snes_pints.py
 ionbench/optimisers/pints_optimisers/xnes_pints.py
 ionbench/optimisers/scipy_optimisers/__init__.py
 ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
 ionbench/optimisers/scipy_optimisers/lm_scipy.py
 ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
 ionbench/optimisers/scipy_optimisers/powell_scipy.py
```

### Comparing `ionbench-0.4.3/setup.py` & `ionbench-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     name="ionbench",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.3",  # Required
+    version="0.5.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A benchmarking tool for comparing different parameter optimization algorithms for ion channel models",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -119,15 +119,15 @@
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=["numpy",
                       "pandas",
                       "scipy",
                       "pints>=0.4.1",
-                      "myokit>=1.34.0",
+                      "myokit>=1.36.0",
                       "matplotlib>=3.7.1",
                       "mygrad>=2.2.0",
                       "pymoo>=0.6.0.1"],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
```

### Comparing `ionbench-0.4.3/test/test_modifications.py` & `ionbench-0.5.0/test/test_modifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import ionbench
 from ionbench import modification
 import numpy as np
 import pytest
 
 
 class TestModifications:
-    bm = ionbench.problems.staircase.HH()
+    bm = ionbench.problems.loewe2016.IKr()
 
     @pytest.mark.cheap
     def test_bounds(self):
         # Check bounds are correctly applied for all settings
         # No bounds initially
         assert not self.bm.parametersBounded
         # Sampler
         mod = modification.Modification(parameterBounds='on')
         mod.apply(self.bm)
         assert self.bm.parametersBounded
-        assert all(np.array(self.bm.lb) > 0)
+        assert all(np.array(self.bm.lb) > -np.inf)
         assert all(np.array(self.bm.ub) < np.inf)
         # Custom
         lb = np.random.rand(self.bm.n_parameters())
         ub = np.random.rand(self.bm.n_parameters()) + 1
         mod = modification.Modification(parameterBounds='Custom', customBounds=[lb, ub])
         mod.apply(self.bm)
         assert self.bm.parametersBounded
@@ -108,17 +108,18 @@
         assert any(self.bm.logTransformParams) and not all(self.bm.logTransformParams)
         assert self.bm.useScaleFactors
         assert self.bm.parametersBounded
         assert all(np.array(self.bm.lb) == np.array(lb))
         assert all(np.array(self.bm.ub) == np.array(ub))
 
     @pytest.mark.cheap
-    def test_other_problems(self):
-        # Basic check for another benchmarker
-        mod = modification.Modification(logTransform='on', parameterBounds='on', scaleFactors='On')
-        newbm = ionbench.problems.loewe2016.IKr()
+    def test_staircase(self):
+        # Check staircase problems override bounds
+        mod = modification.Modification(logTransform='on', parameterBounds='off', scaleFactors='On', rateBounds='off')
+        newbm = ionbench.problems.staircase.HH()
         mod.apply(newbm)
         assert newbm.useScaleFactors
         assert all(np.array(newbm.logTransformParams) == np.array(newbm.STANDARD_LOG_TRANSFORM))
         assert any(newbm.logTransformParams)
         assert not all(newbm.logTransformParams)
         assert newbm.parametersBounded
+        assert newbm.ratesBounded
```

### Comparing `ionbench-0.4.3/test/test_multistart.py` & `ionbench-0.5.0/test/test_multistart.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/test/test_optimisers.py` & `ionbench-0.5.0/test/test_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.3/test/test_problems.py` & `ionbench-0.5.0/test/test_problems.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,98 +71,90 @@
         c = self.bm.signed_error(p)[0]
         c2 = self.bm.cost(p)
         assert 1e5 < c < 2e5
         assert 1e5 < c2 < 2e5
         # Check cost is small inside bounds when bounded
         p[0] = self.bm._TRUE_PARAMETERS[0]
         assert self.bm.cost(p) < 1e5
-        # Check parametersBounded = False turns off bounds (unless staircase)
+        # Check parametersBounded = False turns off bounds
         self.bm.parametersBounded = False
         p[0] *= 0.98
-        if 'staircase' in self.bm.NAME:
-            assert self.bm.cost(p) > 1e5
-        else:
-            assert self.bm.cost(p) < 1e5
+        assert self.bm.cost(p) < 1e5
         self.bm.parametersBounded = True
         # Check penalty increases with more bound violations
         p = np.copy(self.bm._TRUE_PARAMETERS) * 0.98
         c = self.bm.signed_error(p)[0]
         assert c > 1e5 * self.bm.n_parameters()
         self.bm.parametersBounded = False
 
     @pytest.mark.cheap
     def test_rate_bounds(self):
         self.bm.reset()
-        assert self.bm.ratesBounded is False
+        if 'staircase' in self.bm.NAME:
+            assert self.bm.ratesBounded is True
+        else:
+            assert self.bm.ratesBounded is False
         self.bm.add_rate_bounds()
         assert self.bm.ratesBounded is True
         tmp = self.bm.RATE_MIN
         # Default params inside rate bounds always
         assert self.bm.cost(self.bm._TRUE_PARAMETERS) < 1e5
         # Move rate bounds so default rates are outside
         self.bm.RATE_MIN = self.bm.RATE_MAX * 2
         assert self.bm.cost(self.bm._TRUE_PARAMETERS) > 1e5
-        # Turn off rate bounds should allow solving again (except for staircase)
+        # Turn off rate bounds should allow solving again
         self.bm.ratesBounded = False
-        assert self.bm.cost(self.bm._TRUE_PARAMETERS) < 1e5 or 'staircase' in self.bm.NAME
-        if 'staircase' in self.bm.NAME:
-            assert self.bm.cost(self.bm._TRUE_PARAMETERS) > 1e5
-            self.bm.RATE_MIN = tmp
-            assert self.bm.cost(self.bm._TRUE_PARAMETERS) < 1e5
+        assert self.bm.cost(self.bm._TRUE_PARAMETERS) < 1e5
         self.bm.RATE_MIN = tmp
 
     @pytest.mark.cheap
     def test_tracker_solve_count(self):
         # Check solve count works with bounds and evaluate
         self.bm.reset()
         # Solve times are empty
         assert len(self.bm.tracker.costTimes) == 0
         assert len(self.bm.tracker.gradTimes) == 0
         # Solve count is 0 after reset
-        assert self.bm.tracker.solveCount == 0
+        assert self.bm.tracker.costSolveCount == 0
         # Solve count increments after solving
         self.bm.cost(self.bm._TRUE_PARAMETERS)
-        assert self.bm.tracker.solveCount == 1
+        assert self.bm.tracker.costSolveCount == 1
         # but not when out of bounds
         self.bm.add_parameter_bounds()
         self.bm.lb = 0.99*self.bm._TRUE_PARAMETERS
         p = np.copy(self.bm._TRUE_PARAMETERS)
         p[0] = 0.98 * self.bm._TRUE_PARAMETERS[0]
         self.bm.cost(p)
-        assert self.bm.tracker.solveCount == 1
+        assert self.bm.tracker.costSolveCount == 1
         self.bm.parametersBounded = False
         if 'ikur' not in self.bm.NAME:
             # or out of rate bounds
             self.bm.add_rate_bounds()
             tmp = self.bm.RATE_MIN
             self.bm.RATE_MIN = self.bm.RATE_MAX
             self.bm.cost(self.bm._TRUE_PARAMETERS)
-            assert self.bm.tracker.solveCount == 1
+            assert self.bm.tracker.costSolveCount == 1
             self.bm.RATE_MIN = tmp
             self.bm.cost(self.bm._TRUE_PARAMETERS)
-            assert self.bm.tracker.solveCount == 2
+            assert self.bm.tracker.costSolveCount == 2
             self.bm.ratesBounded = False
         else:
             self.bm.cost(self.bm._TRUE_PARAMETERS)
         # Solve count doesn't increment when evaluating
         self.bm.evaluate()
-        assert self.bm.tracker.solveCount == 2
-        # Only one cost time and no grad
-        assert len(self.bm.tracker.costTimes) == 2
-        assert len(self.bm.tracker.gradTimes) == 0
+        assert self.bm.tracker.costSolveCount == 2
+        assert self.bm.tracker.gradSolveCount == 0
         # returns to 0 after resetting
         self.bm.reset(fullReset=False)
-        assert self.bm.tracker.solveCount == 0
+        assert self.bm.tracker.costSolveCount == 0
         self.bm.parametersBounded = False
         # grad solve counter increments with grad but not normal solve counter
         self.bm.grad(self.bm._TRUE_PARAMETERS)
-        assert self.bm.tracker.solveCount == 0
+        assert self.bm.tracker.costSolveCount == 0
         assert self.bm.tracker.gradSolveCount == 1
-        assert len(self.bm.tracker.costTimes) == 0
-        assert len(self.bm.tracker.gradTimes) == 1
         self.bm.reset(fullReset=False)
         p1 = self.bm.sample()
         p2 = self.bm.sample()
         c1 = self.bm.cost(p1)
         c2 = self.bm.cost(p2)
         if c1 < c2:
             assert np.abs(c1 - self.bm.tracker.bestCost) < 1e-8
@@ -292,16 +284,16 @@
     @pytest.mark.cheap
     def test_steady_state(self):
         self.bm.reset()
         # Test steady state is right for random parameters
         if 'moreno' not in self.bm.NAME:
             self.bm.reset()
             p = self.bm.sample()
-            assert self.bm.in_parameter_bounds(p, boundedCheck='staircase' not in self.bm.NAME)
-            assert self.bm.in_rate_bounds(p, boundedCheck='staircase' not in self.bm.NAME)
+            assert self.bm.in_parameter_bounds(p)
+            assert self.bm.in_rate_bounds(p)
             out = self.bm.simulate(parameters=p, times=np.arange(0, self.bm.T_MAX, self.bm.TIMESTEP))
             assert np.abs((out[0] - out[1])) < 1e-8
         self.bm.reset()
         p = self.bm.sample()
         self.bm.set_steady_state(p)
         initState = self.bm.sim.state()
         self.bm.set_params(p)
@@ -368,45 +360,53 @@
         assert n == len(self.bm.STANDARD_LOG_TRANSFORM)
         assert n == len(self.bm._LOWER_BOUND)
         assert n == len(self.bm._UPPER_BOUND)
 
     @pytest.mark.cheap
     def test_reset(self):
         self.bm.reset(fullReset=True)
-        assert self.bm.parametersBounded is False
-        assert self.bm.ratesBounded is False
+        if 'staircase' in self.bm.NAME:
+            assert self.bm.parametersBounded is True
+            assert self.bm.ratesBounded is True
+        else:
+            assert self.bm.parametersBounded is False
+            assert self.bm.ratesBounded is False
         assert all([self.bm.logTransformParams[i] is False for i in range(self.bm.n_parameters())])
         assert self.bm.useScaleFactors is False
-        assert self.bm.tracker.solveCount == 0
+        assert self.bm.tracker.costSolveCount == 0
         mod = ionbench.modification.Clerx2019()
         mod.apply(self.bm)
         self.bm.useScaleFactors = True
         if 'ikur' in self.bm.NAME:
             self.bm.ratesBounded = False
             self.bm.cost(self.bm.input_parameter_space(self.bm._TRUE_PARAMETERS))
             self.bm.ratesBounded = True
         else:
             self.bm.cost(self.bm.input_parameter_space(self.bm._TRUE_PARAMETERS))
         assert self.bm.parametersBounded is True
         assert self.bm.ratesBounded is True
         assert any([self.bm.logTransformParams[i] is True for i in range(self.bm.n_parameters())])
         assert self.bm.useScaleFactors is True
-        assert self.bm.tracker.solveCount == 1
+        assert self.bm.tracker.costSolveCount == 1
         self.bm.reset(fullReset=False)
         assert self.bm.parametersBounded is True
         assert self.bm.ratesBounded is True
         assert any([self.bm.logTransformParams[i] is True for i in range(self.bm.n_parameters())])
         assert self.bm.useScaleFactors is True
-        assert self.bm.tracker.solveCount == 0
+        assert self.bm.tracker.costSolveCount == 0
         self.bm.reset()  # Full reset is True by default
-        assert self.bm.parametersBounded is False
-        assert self.bm.ratesBounded is False
+        if 'staircase' in self.bm.NAME:
+            assert self.bm.parametersBounded is True
+            assert self.bm.ratesBounded is True
+        else:
+            assert self.bm.parametersBounded is False
+            assert self.bm.ratesBounded is False
         assert all([self.bm.logTransformParams[i] is False for i in range(self.bm.n_parameters())])
         assert self.bm.useScaleFactors is False
-        assert self.bm.tracker.solveCount == 0
+        assert self.bm.tracker.costSolveCount == 0
 
 
 class Staircase(Problem):
     @pytest.mark.cheap
     def test_sampler(self):
         self.bm.reset()
         # Check sampler is inside the right bounds and doesn't just return default rates, across all transforms
@@ -585,21 +585,21 @@
     bm.plotter = False
     costBound = 0.02  # Accounts for noise
 
 
 class TestLoeweIKr(Loewe):
     bm = ionbench.problems.loewe2016.IKr()
     bm.plotter = False
-    costBound = 0
+    costBound = 1e-16
 
 
 class TestLoeweIKur(Loewe):
     bm = ionbench.problems.loewe2016.IKur()
     bm.plotter = False
-    costBound = 0
+    costBound = 1e-16
 
 
 def sampler_bounds(bm, lb, ub):
     """
     Test function for checking that sampled parameters lie within the expected bounds
     """
     p = bm.sample()
```

### Comparing `ionbench-0.4.3/test/test_uncertainty.py` & `ionbench-0.5.0/test/test_uncertainty.py`

 * *Files identical despite different names*


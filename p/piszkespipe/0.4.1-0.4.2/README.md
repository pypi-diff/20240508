# Comparing `tmp/piszkespipe-0.4.1.tar.gz` & `tmp/piszkespipe-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/piszkespipe-0.4.1.tar", last modified: Tue May  9 14:47:56 2023, max compression
+gzip compressed data, was "dist/piszkespipe-0.4.2.tar", last modified: Wed May  8 17:53:18 2024, max compression
```

## Comparing `piszkespipe-0.4.1.tar` & `piszkespipe-0.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/
--rw-r--r--   0 batty      (501) staff       (20)       66 2021-05-30 18:01:38.000000 piszkespipe-0.4.1/.gitattributes
--rw-r--r--   0 batty      (501) staff       (20)     2046 2020-11-26 15:30:23.000000 piszkespipe-0.4.1/.gitignore
--rw-r--r--   0 batty      (501) staff       (20)    35181 2021-05-29 17:20:45.000000 piszkespipe-0.4.1/LICENCE
--rw-r--r--   0 batty      (501) staff       (20)    16144 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/PKG-INFO
--rw-r--r--   0 batty      (501) staff       (20)    13431 2022-03-08 12:35:42.000000 piszkespipe-0.4.1/README.md
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/examples/
--rw-r--r--   0 batty      (501) staff       (20)     4559 2021-09-02 14:35:10.000000 piszkespipe-0.4.1/examples/run_piszkespipe.ipynb
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/CCF/
--rw-r--r--   0 batty      (501) staff       (20)     4021 2022-03-06 21:22:12.000000 piszkespipe-0.4.1/piszkespipe/CCF/CCF.c
--rw-r--r--   0 batty      (501) staff       (20)     7508 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/CCF/CCF.f90
--rw-r--r--   0 batty      (501) staff       (20)     2244 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/CCF/CCF.pyf
--rw-r--r--   0 batty      (501) staff       (20)   268799 2023-05-09 14:47:54.000000 piszkespipe-0.4.1/piszkespipe/CCF/CCF_pyc.c
--rw-r--r--   0 batty      (501) staff       (20)     2781 2022-03-06 22:09:16.000000 piszkespipe-0.4.1/piszkespipe/CCF/CCF_pyc.pyx
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/Correlation/
--rw-r--r--   0 batty      (501) staff       (20)       47 2021-05-29 18:07:39.000000 piszkespipe-0.4.1/piszkespipe/Correlation/__init__.py
--rw-r--r--   0 batty      (501) staff       (20)   249261 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/Correlation/anchos40000.dat
--rw-r--r--   0 batty      (501) staff       (20)   249429 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/Correlation/anchos50000.dat
--rw-r--r--   0 batty      (501) staff       (20)   251148 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/Correlation/anchos60000.dat
--rw-r--r--   0 batty      (501) staff       (20)    39096 2023-05-09 14:36:16.000000 piszkespipe-0.4.1/piszkespipe/Correlation/correlation.py
--rw-r--r--   0 batty      (501) staff       (20)      330 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/Correlation/lines.dat
--rw-r--r--   0 batty      (501) staff       (20)       32 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/Correlation/lines2.dat
--rw-r--r--   0 batty      (501) staff       (20)      453 2021-05-29 18:48:06.000000 piszkespipe-0.4.1/piszkespipe/Correlation/test.py
--rw-r--r--   0 batty      (501) staff       (20)      897 2021-05-30 15:23:44.000000 piszkespipe-0.4.1/piszkespipe/Correlation/vels.py
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/GLOBALutils/
--rw-r--r--   0 batty      (501) staff       (20)   158603 2021-09-02 01:51:52.000000 piszkespipe-0.4.1/piszkespipe/GLOBALutils/GLOBALutils.py
--rw-r--r--   0 batty      (501) staff       (20)       27 2021-05-29 18:08:12.000000 piszkespipe-0.4.1/piszkespipe/GLOBALutils/__init__.py
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/
--rw-r--r--   0 batty      (501) staff       (20)     7323 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/BTest.py
--rw-r--r--   0 batty      (501) staff       (20)     1369 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/BTestSimple.py
--rw-r--r--   0 batty      (501) staff       (20)    97409 2021-05-12 15:18:03.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/Marsh.c
--rw-r--r--   0 batty      (501) staff       (20)     3920 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/README
--rw-r--r--   0 batty      (501) staff       (20)     7681 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/Test.py
--rw-r--r--   0 batty      (501) staff       (20)     1329 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/TestSimple.py
--rw-r--r--   0 batty      (501) staff       (20)     1055 2021-05-12 14:46:53.000000 piszkespipe-0.4.1/piszkespipe/OptExtract/setup.py
--rwxr-xr-x   0 batty      (501) staff       (20)      128 2021-05-29 20:24:14.000000 piszkespipe-0.4.1/piszkespipe/__init__.py
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/data/
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/data/xc_masks/
--rw-r--r--   0 batty      (501) staff       (20)   116000 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/data/xc_masks/G2.mas
--rw-r--r--   0 batty      (501) staff       (20)   148741 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/data/xc_masks/K5.mas
--rw-r--r--   0 batty      (501) staff       (20)   322762 2020-05-24 11:25:25.000000 piszkespipe-0.4.1/piszkespipe/data/xc_masks/M2.mas
--rw-r--r--   0 batty      (501) staff       (20)    80187 2022-03-08 19:18:36.000000 piszkespipe-0.4.1/piszkespipe/piszkespipe.py
--rw-r--r--   0 batty      (501) staff       (20)    30486 2021-10-24 11:49:35.000000 piszkespipe-0.4.1/piszkespipe/piszkesutils.py
--rw-r--r--   0 batty      (501) staff       (20)       22 2023-05-09 14:38:03.000000 piszkespipe-0.4.1/piszkespipe/version.py
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe/wavcals/
--rw-r--r--   0 batty      (501) staff       (20)      515 2021-05-15 18:48:21.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order00.dat
--rw-r--r--   0 batty      (501) staff       (20)      443 2021-05-14 16:13:42.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order01.dat
--rw-r--r--   0 batty      (501) staff       (20)      638 2021-05-14 19:01:05.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order02.dat
--rw-r--r--   0 batty      (501) staff       (20)      767 2021-05-15 20:46:39.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order03.dat
--rw-r--r--   0 batty      (501) staff       (20)      600 2021-05-14 12:08:49.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order04.dat
--rw-r--r--   0 batty      (501) staff       (20)     1104 2021-05-15 20:48:33.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order05.dat
--rw-r--r--   0 batty      (501) staff       (20)     1183 2021-05-15 20:48:45.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order06.dat
--rw-r--r--   0 batty      (501) staff       (20)     1193 2021-05-15 20:52:12.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order07.dat
--rw-r--r--   0 batty      (501) staff       (20)     1401 2021-05-15 20:54:02.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order08.dat
--rw-r--r--   0 batty      (501) staff       (20)     1312 2021-05-15 20:55:29.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order09.dat
--rw-r--r--   0 batty      (501) staff       (20)     1242 2021-05-15 20:57:10.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order10.dat
--rw-r--r--   0 batty      (501) staff       (20)     1157 2021-05-15 20:59:36.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order11.dat
--rw-r--r--   0 batty      (501) staff       (20)     1401 2021-05-15 21:01:14.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order12.dat
--rw-r--r--   0 batty      (501) staff       (20)     1312 2021-05-15 21:03:17.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order13.dat
--rw-r--r--   0 batty      (501) staff       (20)     1244 2021-05-15 21:05:57.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order14.dat
--rw-r--r--   0 batty      (501) staff       (20)     1242 2021-05-15 21:08:13.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order15.dat
--rw-r--r--   0 batty      (501) staff       (20)     1141 2021-05-15 21:10:44.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order16.dat
--rw-r--r--   0 batty      (501) staff       (20)     1340 2021-05-15 21:14:33.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order17.dat
--rw-r--r--   0 batty      (501) staff       (20)     1335 2021-05-15 21:15:39.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order18.dat
--rw-r--r--   0 batty      (501) staff       (20)     1227 2021-05-15 21:17:05.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order19.dat
--rw-r--r--   0 batty      (501) staff       (20)      936 2021-05-15 21:18:44.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order20.dat
--rw-r--r--   0 batty      (501) staff       (20)     1017 2021-05-15 21:20:30.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order21.dat
--rw-r--r--   0 batty      (501) staff       (20)     1151 2021-05-15 21:22:43.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order22.dat
--rw-r--r--   0 batty      (501) staff       (20)     1152 2021-05-15 21:24:52.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order23.dat
--rw-r--r--   0 batty      (501) staff       (20)      982 2021-05-15 21:26:45.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order24.dat
--rw-r--r--   0 batty      (501) staff       (20)      792 2021-05-15 21:27:26.000000 piszkespipe-0.4.1/piszkespipe/wavcals/order25.dat
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/piszkespipe.egg-info/
--rw-r--r--   0 batty      (501) staff       (20)    16144 2023-05-09 14:47:54.000000 piszkespipe-0.4.1/piszkespipe.egg-info/PKG-INFO
--rw-r--r--   0 batty      (501) staff       (20)     2597 2023-05-09 14:47:55.000000 piszkespipe-0.4.1/piszkespipe.egg-info/SOURCES.txt
--rw-r--r--   0 batty      (501) staff       (20)        1 2023-05-09 14:47:54.000000 piszkespipe-0.4.1/piszkespipe.egg-info/dependency_links.txt
--rw-r--r--   0 batty      (501) staff       (20)       74 2023-05-09 14:47:54.000000 piszkespipe-0.4.1/piszkespipe.egg-info/entry_points.txt
--rw-r--r--   0 batty      (501) staff       (20)      130 2023-05-09 14:47:54.000000 piszkespipe-0.4.1/piszkespipe.egg-info/requires.txt
--rw-r--r--   0 batty      (501) staff       (20)       12 2023-05-09 14:47:54.000000 piszkespipe-0.4.1/piszkespipe.egg-info/top_level.txt
--rw-r--r--   0 batty      (501) staff       (20)      135 2022-09-26 09:32:05.000000 piszkespipe-0.4.1/pyproject.toml
--rw-r--r--   0 batty      (501) staff       (20)      129 2023-04-28 00:00:34.000000 piszkespipe-0.4.1/requirements.txt
--rw-r--r--   0 batty      (501) staff       (20)       38 2023-05-09 14:47:56.000000 piszkespipe-0.4.1/setup.cfg
--rw-r--r--   0 batty      (501) staff       (20)     3025 2022-09-26 09:32:05.000000 piszkespipe-0.4.1/setup.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/
+-rw-r--r--   0 batty      (501) staff       (20)       66 2021-05-30 18:01:38.000000 piszkespipe-0.4.2/.gitattributes
+-rw-r--r--   0 batty      (501) staff       (20)     2063 2024-05-08 17:41:56.000000 piszkespipe-0.4.2/.gitignore
+-rw-r--r--   0 batty      (501) staff       (20)    35181 2021-05-29 17:20:45.000000 piszkespipe-0.4.2/LICENCE
+-rw-r--r--   0 batty      (501) staff       (20)    16088 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/PKG-INFO
+-rw-r--r--   0 batty      (501) staff       (20)    13375 2024-05-08 17:45:16.000000 piszkespipe-0.4.2/README.md
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/examples/
+-rw-r--r--   0 batty      (501) staff       (20)     4531 2024-05-08 17:47:05.000000 piszkespipe-0.4.2/examples/run_piszkespipe.ipynb
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/CCF/
+-rw-r--r--   0 batty      (501) staff       (20)     4021 2022-03-06 21:22:12.000000 piszkespipe-0.4.2/piszkespipe/CCF/CCF.c
+-rw-r--r--   0 batty      (501) staff       (20)     7508 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/CCF/CCF.f90
+-rw-r--r--   0 batty      (501) staff       (20)     2244 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/CCF/CCF.pyf
+-rw-r--r--   0 batty      (501) staff       (20)   268799 2023-05-09 14:47:54.000000 piszkespipe-0.4.2/piszkespipe/CCF/CCF_pyc.c
+-rw-r--r--   0 batty      (501) staff       (20)     2781 2022-03-06 22:09:16.000000 piszkespipe-0.4.2/piszkespipe/CCF/CCF_pyc.pyx
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/Correlation/
+-rw-r--r--   0 batty      (501) staff       (20)       47 2021-05-29 18:07:39.000000 piszkespipe-0.4.2/piszkespipe/Correlation/__init__.py
+-rw-r--r--   0 batty      (501) staff       (20)   249261 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/Correlation/anchos40000.dat
+-rw-r--r--   0 batty      (501) staff       (20)   249429 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/Correlation/anchos50000.dat
+-rw-r--r--   0 batty      (501) staff       (20)   251148 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/Correlation/anchos60000.dat
+-rw-r--r--   0 batty      (501) staff       (20)    39096 2023-05-09 14:36:16.000000 piszkespipe-0.4.2/piszkespipe/Correlation/correlation.py
+-rw-r--r--   0 batty      (501) staff       (20)      330 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/Correlation/lines.dat
+-rw-r--r--   0 batty      (501) staff       (20)       32 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/Correlation/lines2.dat
+-rw-r--r--   0 batty      (501) staff       (20)      453 2021-05-29 18:48:06.000000 piszkespipe-0.4.2/piszkespipe/Correlation/test.py
+-rw-r--r--   0 batty      (501) staff       (20)      897 2021-05-30 15:23:44.000000 piszkespipe-0.4.2/piszkespipe/Correlation/vels.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/GLOBALutils/
+-rw-r--r--   0 batty      (501) staff       (20)   158603 2021-09-02 01:51:52.000000 piszkespipe-0.4.2/piszkespipe/GLOBALutils/GLOBALutils.py
+-rw-r--r--   0 batty      (501) staff       (20)       27 2021-05-29 18:08:12.000000 piszkespipe-0.4.2/piszkespipe/GLOBALutils/__init__.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/
+-rw-r--r--   0 batty      (501) staff       (20)     7323 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/BTest.py
+-rw-r--r--   0 batty      (501) staff       (20)     1369 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/BTestSimple.py
+-rw-r--r--   0 batty      (501) staff       (20)    97409 2021-05-12 15:18:03.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/Marsh.c
+-rw-r--r--   0 batty      (501) staff       (20)     3920 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/README
+-rw-r--r--   0 batty      (501) staff       (20)     7681 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/Test.py
+-rw-r--r--   0 batty      (501) staff       (20)     1329 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/TestSimple.py
+-rw-r--r--   0 batty      (501) staff       (20)     1055 2021-05-12 14:46:53.000000 piszkespipe-0.4.2/piszkespipe/OptExtract/setup.py
+-rwxr-xr-x   0 batty      (501) staff       (20)      128 2021-05-29 20:24:14.000000 piszkespipe-0.4.2/piszkespipe/__init__.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/data/
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/data/xc_masks/
+-rw-r--r--   0 batty      (501) staff       (20)   116000 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/data/xc_masks/G2.mas
+-rw-r--r--   0 batty      (501) staff       (20)   148741 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/data/xc_masks/K5.mas
+-rw-r--r--   0 batty      (501) staff       (20)   322762 2020-05-24 11:25:25.000000 piszkespipe-0.4.2/piszkespipe/data/xc_masks/M2.mas
+-rw-r--r--   0 batty      (501) staff       (20)    80197 2024-05-08 17:45:16.000000 piszkespipe-0.4.2/piszkespipe/piszkespipe.py
+-rw-r--r--   0 batty      (501) staff       (20)    30486 2021-10-24 11:49:35.000000 piszkespipe-0.4.2/piszkespipe/piszkesutils.py
+-rw-r--r--   0 batty      (501) staff       (20)       22 2024-05-08 17:50:00.000000 piszkespipe-0.4.2/piszkespipe/version.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe/wavcals/
+-rw-r--r--   0 batty      (501) staff       (20)      515 2021-05-15 18:48:21.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order00.dat
+-rw-r--r--   0 batty      (501) staff       (20)      443 2021-05-14 16:13:42.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order01.dat
+-rw-r--r--   0 batty      (501) staff       (20)      638 2021-05-14 19:01:05.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order02.dat
+-rw-r--r--   0 batty      (501) staff       (20)      767 2021-05-15 20:46:39.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order03.dat
+-rw-r--r--   0 batty      (501) staff       (20)      600 2021-05-14 12:08:49.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order04.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1104 2021-05-15 20:48:33.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order05.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1183 2021-05-15 20:48:45.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order06.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1193 2021-05-15 20:52:12.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order07.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1401 2021-05-15 20:54:02.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order08.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1312 2021-05-15 20:55:29.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order09.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1242 2021-05-15 20:57:10.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order10.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1157 2021-05-15 20:59:36.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order11.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1401 2021-05-15 21:01:14.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order12.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1312 2021-05-15 21:03:17.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order13.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1244 2021-05-15 21:05:57.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order14.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1242 2021-05-15 21:08:13.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order15.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1141 2021-05-15 21:10:44.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order16.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1340 2021-05-15 21:14:33.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order17.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1335 2021-05-15 21:15:39.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order18.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1227 2021-05-15 21:17:05.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order19.dat
+-rw-r--r--   0 batty      (501) staff       (20)      936 2021-05-15 21:18:44.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order20.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1017 2021-05-15 21:20:30.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order21.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1151 2021-05-15 21:22:43.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order22.dat
+-rw-r--r--   0 batty      (501) staff       (20)     1152 2021-05-15 21:24:52.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order23.dat
+-rw-r--r--   0 batty      (501) staff       (20)      982 2021-05-15 21:26:45.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order24.dat
+-rw-r--r--   0 batty      (501) staff       (20)      792 2021-05-15 21:27:26.000000 piszkespipe-0.4.2/piszkespipe/wavcals/order25.dat
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe.egg-info/
+-rw-r--r--   0 batty      (501) staff       (20)    16088 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe.egg-info/PKG-INFO
+-rw-r--r--   0 batty      (501) staff       (20)     2597 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe.egg-info/SOURCES.txt
+-rw-r--r--   0 batty      (501) staff       (20)        1 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe.egg-info/dependency_links.txt
+-rw-r--r--   0 batty      (501) staff       (20)       74 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe.egg-info/entry_points.txt
+-rw-r--r--   0 batty      (501) staff       (20)      130 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe.egg-info/requires.txt
+-rw-r--r--   0 batty      (501) staff       (20)       12 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/piszkespipe.egg-info/top_level.txt
+-rw-r--r--   0 batty      (501) staff       (20)      135 2022-09-26 09:32:05.000000 piszkespipe-0.4.2/pyproject.toml
+-rw-r--r--   0 batty      (501) staff       (20)      129 2023-04-28 00:00:34.000000 piszkespipe-0.4.2/requirements.txt
+-rw-r--r--   0 batty      (501) staff       (20)       38 2024-05-08 17:53:18.000000 piszkespipe-0.4.2/setup.cfg
+-rw-r--r--   0 batty      (501) staff       (20)     3025 2022-09-26 09:32:05.000000 piszkespipe-0.4.2/setup.py
```

### Comparing `piszkespipe-0.4.1/.gitignore` & `piszkespipe-0.4.2/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
+CCF_pyc.c
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
@@ -134,7 +135,8 @@
 .pyre/
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
+/.idea
```

### Comparing `piszkespipe-0.4.1/LICENCE` & `piszkespipe-0.4.2/LICENCE`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/PKG-INFO` & `piszkespipe-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piszkespipe
-Version: 0.4.1
+Version: 0.4.2
 Summary: A pipeline for reducing echelle spectra obtained in Piszkesteto.
 Home-page: https://github.com/astrobatty/piszkespipe/
 Author: Attila Bodi
 Author-email: astrobatty@gmail.com
 License: UNKNOWN
 Description: [![Image](https://img.shields.io/badge/tutorials-%E2%9C%93-blue.svg)](https://github.com/astrobatty/piszkespipe/tree/main/examples)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astrobatty/piszkespipe/blob/main/examples/run_piszkespipe.ipynb)
@@ -34,15 +34,15 @@
         pkg-config --cflags --libs gsl && gsl-config --version
         ```
         
         ## Installation 1: in a normal python environment (for regular python users)
         
         ``piszkespipe`` can be installed from source:
         ```bash
-        pip install git+https://github.com/astrobatty/piszkespipe.git
+        pip install piszkespipe
         ```
         
         ## Installation 2: in a separate conda environment (for people afraid of python)
         
         The easiest way to separate ``piszkespipe`` from other python packages (and everything else) is to install it in a [conda (see this link for minimal installiation)](https://docs.conda.io/en/latest/miniconda.html) environment:
         ```bash
         conda create -n piszkespipe python=3.7
@@ -51,15 +51,15 @@
         To activate the environment:
         ```bash
         conda activate piszkespipe
         ```
         
         Then the package can be installed:
         ```bash
-        pip install git+https://github.com/astrobatty/piszkespipe.git
+        pip install piszkespipe
         ```
         
         If the code is not used, the environment can be deactivated:
         ```bash
         conda deactivate
         ```
         
@@ -214,20 +214,20 @@
         17- Path to the CCF plot file
         ```
         
         _Note:_ the systematic error in RV can be elliminated by measuring the RV of a standard star and comparing its current value to the literature.
         
         ## Spectral Classification Module
         
-        In order to use the automated spectral classification routines (`-do_class` option), a set of synthetic spectra is required. In particular, the original CERES uses a modified version of the [Coelho et al 2005 models](https://ui.adsabs.harvard.edu/abs/2005A&A...443..735C/abstract), where the models have been reduced in wavelength coverage, degraded in resolution and v*sin(i), and reduced in sampling. This grid of models can be downloaded from [this link](https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz) (2.85 GB; or [from the original source](http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz)) and the $COELHO path to models must be defined:
+        In order to use the automated spectral classification routines (`-do_class` option), a set of synthetic spectra is required. In particular, the original CERES uses a modified version of the [Coelho et al 2005 models](https://ui.adsabs.harvard.edu/abs/2005A&A...443..735C/abstract), where the models have been reduced in wavelength coverage, degraded in resolution and v*sin(i), and reduced in sampling. This grid of models can be downloaded from [this link](https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz) (2.85 GB; or [from the original source](http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz)) and the $COELHO path to models must be defined:
         
         ```bash
         mkdir ~/COELHO_MODELS
         cd ~/COELHO_MODELS
-        wget https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz
+        wget https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz
         # Or from the orignal source:
         # wget http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz
         tar -xf coelho_05_red4_R40.tar.gz
         ```
         
         Then add the location of R_40000b dir to $COELHO path, e.g. by
         ```bash
```

### Comparing `piszkespipe-0.4.1/README.md` & `piszkespipe-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 pkg-config --cflags --libs gsl && gsl-config --version
 ```
 
 ## Installation 1: in a normal python environment (for regular python users)
 
 ``piszkespipe`` can be installed from source:
 ```bash
-pip install git+https://github.com/astrobatty/piszkespipe.git
+pip install piszkespipe
 ```
 
 ## Installation 2: in a separate conda environment (for people afraid of python)
 
 The easiest way to separate ``piszkespipe`` from other python packages (and everything else) is to install it in a [conda (see this link for minimal installiation)](https://docs.conda.io/en/latest/miniconda.html) environment:
 ```bash
 conda create -n piszkespipe python=3.7
@@ -43,15 +43,15 @@
 To activate the environment:
 ```bash
 conda activate piszkespipe
 ```
 
 Then the package can be installed:
 ```bash
-pip install git+https://github.com/astrobatty/piszkespipe.git
+pip install piszkespipe
 ```
 
 If the code is not used, the environment can be deactivated:
 ```bash
 conda deactivate
 ```
 
@@ -206,20 +206,20 @@
 17- Path to the CCF plot file
 ```
 
 _Note:_ the systematic error in RV can be elliminated by measuring the RV of a standard star and comparing its current value to the literature.
 
 ## Spectral Classification Module
 
-In order to use the automated spectral classification routines (`-do_class` option), a set of synthetic spectra is required. In particular, the original CERES uses a modified version of the [Coelho et al 2005 models](https://ui.adsabs.harvard.edu/abs/2005A&A...443..735C/abstract), where the models have been reduced in wavelength coverage, degraded in resolution and v*sin(i), and reduced in sampling. This grid of models can be downloaded from [this link](https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz) (2.85 GB; or [from the original source](http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz)) and the $COELHO path to models must be defined:
+In order to use the automated spectral classification routines (`-do_class` option), a set of synthetic spectra is required. In particular, the original CERES uses a modified version of the [Coelho et al 2005 models](https://ui.adsabs.harvard.edu/abs/2005A&A...443..735C/abstract), where the models have been reduced in wavelength coverage, degraded in resolution and v*sin(i), and reduced in sampling. This grid of models can be downloaded from [this link](https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz) (2.85 GB; or [from the original source](http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz)) and the $COELHO path to models must be defined:
 
 ```bash
 mkdir ~/COELHO_MODELS
 cd ~/COELHO_MODELS
-wget https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz
+wget https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz
 # Or from the orignal source:
 # wget http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz
 tar -xf coelho_05_red4_R40.tar.gz
 ```
 
 Then add the location of R_40000b dir to $COELHO path, e.g. by
 ```bash
```

### Comparing `piszkespipe-0.4.1/examples/run_piszkespipe.ipynb` & `piszkespipe-0.4.2/examples/run_piszkespipe.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988888888888889%*

 * *Differences: {"'cells'": "{4: {'source': ['!pip install piszkespipe']}, 7: {'source': {insert: [(1, '!cd "*

 * *            'COELHO_MODELS; wget '*

 * *            'https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz; tar '*

 * *            "-xf coelho_05_red4_R40.tar.gz\\n')], delete: [1]}}}"}*

```diff
@@ -32,15 +32,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!pip install git+https://github.com/astrobatty/piszkespipe.git"
+                "!pip install piszkespipe"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### __After this step, you may have to restart the runtime.__"
@@ -58,15 +58,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "!mkdir COELHO_MODELS\n",
-                "!cd COELHO_MODELS; wget https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz; tar -xf coelho_05_red4_R40.tar.gz\n",
+                "!cd COELHO_MODELS; wget https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz; tar -xf coelho_05_red4_R40.tar.gz\n",
                 "\n",
                 "import os\n",
                 "os.environ['COELHO'] = '/content/COELHO_MODELS'"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `piszkespipe-0.4.1/piszkespipe/CCF/CCF.c` & `piszkespipe-0.4.2/piszkespipe/CCF/CCF.c`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/CCF/CCF.f90` & `piszkespipe-0.4.2/piszkespipe/CCF/CCF.f90`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/CCF/CCF.pyf` & `piszkespipe-0.4.2/piszkespipe/CCF/CCF.pyf`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/CCF/CCF_pyc.c` & `piszkespipe-0.4.2/piszkespipe/CCF/CCF_pyc.c`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/CCF/CCF_pyc.pyx` & `piszkespipe-0.4.2/piszkespipe/CCF/CCF_pyc.pyx`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/Correlation/anchos40000.dat` & `piszkespipe-0.4.2/piszkespipe/Correlation/anchos40000.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/Correlation/anchos50000.dat` & `piszkespipe-0.4.2/piszkespipe/Correlation/anchos50000.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/Correlation/anchos60000.dat` & `piszkespipe-0.4.2/piszkespipe/Correlation/anchos60000.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/Correlation/correlation.py` & `piszkespipe-0.4.2/piszkespipe/Correlation/correlation.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/Correlation/vels.py` & `piszkespipe-0.4.2/piszkespipe/Correlation/vels.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/GLOBALutils/GLOBALutils.py` & `piszkespipe-0.4.2/piszkespipe/GLOBALutils/GLOBALutils.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/OptExtract/BTest.py` & `piszkespipe-0.4.2/piszkespipe/OptExtract/BTest.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/OptExtract/BTestSimple.py` & `piszkespipe-0.4.2/piszkespipe/OptExtract/BTestSimple.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/OptExtract/Marsh.c` & `piszkespipe-0.4.2/piszkespipe/OptExtract/Marsh.c`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/OptExtract/README` & `piszkespipe-0.4.2/piszkespipe/OptExtract/README`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/OptExtract/Test.py` & `piszkespipe-0.4.2/piszkespipe/OptExtract/Test.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/OptExtract/TestSimple.py` & `piszkespipe-0.4.2/piszkespipe/OptExtract/TestSimple.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/OptExtract/setup.py` & `piszkespipe-0.4.2/piszkespipe/OptExtract/setup.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/data/xc_masks/G2.mas` & `piszkespipe-0.4.2/piszkespipe/data/xc_masks/G2.mas`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/data/xc_masks/K5.mas` & `piszkespipe-0.4.2/piszkespipe/data/xc_masks/K5.mas`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/data/xc_masks/M2.mas` & `piszkespipe-0.4.2/piszkespipe/data/xc_masks/M2.mas`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/piszkespipe.py` & `piszkespipe-0.4.2/piszkespipe/piszkespipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     ###### Path to the synthetic models ######
     if DoClass and os.getenv('COELHO') is None:
         print(bcolors.FAIL + 'COELHO model dir is not found, but -do_class is specified!' + bcolors.ENDC)
         print('Please download the models (2.85 GB), e.g. by')
         print('\tmkdir ~/COELHO_MODELS')
         print('\tcd ~/COELHO_MODELS')
-        print('\twget https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz')
+        print('\twget https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz')
         print('\ttar -xf coelho_05_red4_R40.tar.gz')
         print('And add the location of R_40000b dir to $COELHO path, e.g. by')
         print("\texport COELHO=~/COELHO_MODELS")
         print('Optionally add this line to your .bash_rc file')
         exit()
     elif DoClass:
         models_path = os.path.join( os.getenv('COELHO') , 'R_40000b' )
```

### Comparing `piszkespipe-0.4.1/piszkespipe/piszkesutils.py` & `piszkespipe-0.4.2/piszkespipe/piszkesutils.py`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order00.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order00.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order02.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order02.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order03.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order03.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order04.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order04.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order05.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order05.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order06.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order06.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order07.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order07.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order08.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order08.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order09.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order09.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order10.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order10.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order11.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order11.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order12.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order12.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order13.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order13.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order14.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order14.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order15.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order15.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order16.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order16.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order17.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order17.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order18.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order18.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order19.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order19.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order20.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order20.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order21.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order21.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order22.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order22.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order23.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order23.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order24.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order24.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe/wavcals/order25.dat` & `piszkespipe-0.4.2/piszkespipe/wavcals/order25.dat`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/piszkespipe.egg-info/PKG-INFO` & `piszkespipe-0.4.2/piszkespipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piszkespipe
-Version: 0.4.1
+Version: 0.4.2
 Summary: A pipeline for reducing echelle spectra obtained in Piszkesteto.
 Home-page: https://github.com/astrobatty/piszkespipe/
 Author: Attila Bodi
 Author-email: astrobatty@gmail.com
 License: UNKNOWN
 Description: [![Image](https://img.shields.io/badge/tutorials-%E2%9C%93-blue.svg)](https://github.com/astrobatty/piszkespipe/tree/main/examples)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astrobatty/piszkespipe/blob/main/examples/run_piszkespipe.ipynb)
@@ -34,15 +34,15 @@
         pkg-config --cflags --libs gsl && gsl-config --version
         ```
         
         ## Installation 1: in a normal python environment (for regular python users)
         
         ``piszkespipe`` can be installed from source:
         ```bash
-        pip install git+https://github.com/astrobatty/piszkespipe.git
+        pip install piszkespipe
         ```
         
         ## Installation 2: in a separate conda environment (for people afraid of python)
         
         The easiest way to separate ``piszkespipe`` from other python packages (and everything else) is to install it in a [conda (see this link for minimal installiation)](https://docs.conda.io/en/latest/miniconda.html) environment:
         ```bash
         conda create -n piszkespipe python=3.7
@@ -51,15 +51,15 @@
         To activate the environment:
         ```bash
         conda activate piszkespipe
         ```
         
         Then the package can be installed:
         ```bash
-        pip install git+https://github.com/astrobatty/piszkespipe.git
+        pip install piszkespipe
         ```
         
         If the code is not used, the environment can be deactivated:
         ```bash
         conda deactivate
         ```
         
@@ -214,20 +214,20 @@
         17- Path to the CCF plot file
         ```
         
         _Note:_ the systematic error in RV can be elliminated by measuring the RV of a standard star and comparing its current value to the literature.
         
         ## Spectral Classification Module
         
-        In order to use the automated spectral classification routines (`-do_class` option), a set of synthetic spectra is required. In particular, the original CERES uses a modified version of the [Coelho et al 2005 models](https://ui.adsabs.harvard.edu/abs/2005A&A...443..735C/abstract), where the models have been reduced in wavelength coverage, degraded in resolution and v*sin(i), and reduced in sampling. This grid of models can be downloaded from [this link](https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz) (2.85 GB; or [from the original source](http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz)) and the $COELHO path to models must be defined:
+        In order to use the automated spectral classification routines (`-do_class` option), a set of synthetic spectra is required. In particular, the original CERES uses a modified version of the [Coelho et al 2005 models](https://ui.adsabs.harvard.edu/abs/2005A&A...443..735C/abstract), where the models have been reduced in wavelength coverage, degraded in resolution and v*sin(i), and reduced in sampling. This grid of models can be downloaded from [this link](https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz) (2.85 GB; or [from the original source](http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz)) and the $COELHO path to models must be defined:
         
         ```bash
         mkdir ~/COELHO_MODELS
         cd ~/COELHO_MODELS
-        wget https://www.dropbox.com/s/0ktrptz4bc5bk66/coelho_05_red4_R40.tar.gz
+        wget https://cloud.konkoly.hu/s/taT2qiSjpBwWWDr/download/coelho_05_red4_R40.tar.gz
         # Or from the orignal source:
         # wget http://www.astro.puc.cl/~rbrahm/coelho_05_red4_R40.tar.gz
         tar -xf coelho_05_red4_R40.tar.gz
         ```
         
         Then add the location of R_40000b dir to $COELHO path, e.g. by
         ```bash
```

### Comparing `piszkespipe-0.4.1/piszkespipe.egg-info/SOURCES.txt` & `piszkespipe-0.4.2/piszkespipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piszkespipe-0.4.1/setup.py` & `piszkespipe-0.4.2/setup.py`

 * *Files identical despite different names*


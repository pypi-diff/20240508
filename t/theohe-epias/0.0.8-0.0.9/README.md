# Comparing `tmp/theohe-epias-0.0.8.tar.gz` & `tmp/theohe_epias-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theohe-epias-0.0.8.tar", last modified: Thu Feb 15 12:15:50 2024, max compression
+gzip compressed data, was "theohe_epias-0.0.9.tar", last modified: Wed Apr 17 11:19:41 2024, max compression
```

## Comparing `theohe-epias-0.0.8.tar` & `theohe_epias-0.0.9.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.482647 theohe-epias-0.0.8/
--rw-rw-rw-   0        0        0     1102 2024-01-02 14:20:22.000000 theohe-epias-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2534 2024-02-15 12:15:50.482647 theohe-epias-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2024-01-31 06:32:01.000000 theohe-epias-0.0.8/README.md
--rw-rw-rw-   0        0        0      618 2024-02-15 11:43:13.000000 theohe-epias-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-15 12:15:50.482647 theohe-epias-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.244492 theohe-epias-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.282125 theohe-epias-0.0.8/src/theohe_epias/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.297760 theohe-epias-0.0.8/src/theohe_epias/epys/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/epys/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.297760 theohe-epias-0.0.8/src/theohe_epias/epys/collateral/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/epys/collateral/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.313380 theohe-epias-0.0.8/src/theohe_epias/epys/eligible_customer/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/epys/eligible_customer/__init__.py
--rw-rw-rw-   0        0        0     6154 2024-02-14 11:28:25.000000 theohe-epias-0.0.8/src/theohe_epias/epys/eligible_customer/eligible_customer_meter.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.313380 theohe-epias-0.0.8/src/theohe_epias/epys/invoice/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/epys/invoice/__init__.py
--rw-rw-rw-   0        0        0     3929 2024-01-30 13:26:09.000000 theohe-epias-0.0.8/src/theohe_epias/epys/invoice/data.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.344623 theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/__init__.py
--rw-rw-rw-   0        0        0     4238 2024-01-31 07:54:22.000000 theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/advance.py
--rw-rw-rw-   0        0        0     6357 2024-02-14 11:34:38.000000 theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/imbalance.py
--rw-rw-rw-   0        0        0     9371 2024-01-30 13:26:13.000000 theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/reports.py
--rw-rw-rw-   0        0        0    14555 2024-01-30 13:26:16.000000 theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/settlement.py
--rw-rw-rw-   0        0        0    11363 2024-02-08 10:22:23.000000 theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/settlementdata.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.344623 theohe-epias-0.0.8/src/theohe_epias/epys/registration/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/epys/registration/__init__.py
--rw-rw-rw-   0        0        0    14359 2024-02-15 12:14:58.000000 theohe-epias-0.0.8/src/theohe_epias/epys/registration/registrationmeter.py
--rw-rw-rw-   0        0        0     2775 2024-02-14 11:31:26.000000 theohe-epias-0.0.8/src/theohe_epias/epys/service.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.366751 theohe-epias-0.0.8/src/theohe_epias/epys/utils/
--rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe-epias-0.0.8/src/theohe_epias/epys/utils/__init__.py
--rw-rw-rw-   0        0        0     1784 2024-01-31 07:53:21.000000 theohe-epias-0.0.8/src/theohe_epias/epys/utils/get_time.py
--rw-rw-rw-   0        0        0     1483 2024-01-24 10:50:10.000000 theohe-epias-0.0.8/src/theohe_epias/epys/utils/tgt.py
--rw-rw-rw-   0        0        0     2568 2024-01-24 13:44:04.000000 theohe-epias-0.0.8/src/theohe_epias/epys/utils/time_format.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.366751 theohe-epias-0.0.8/src/theohe_epias/transparency/
--rw-rw-rw-   0        0        0        0 2023-12-22 06:57:44.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.444879 theohe-epias-0.0.8/src/theohe_epias/transparency/data/
--rw-rw-rw-   0        0        0        0 2023-12-22 06:57:44.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/__init__.py
--rw-rw-rw-   0        0        0     7263 2024-01-30 13:26:45.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/ancillary_services.py
--rw-rw-rw-   0        0        0     7181 2024-01-30 13:26:43.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/bilateral_contracts.py
--rw-rw-rw-   0        0        0     7136 2024-01-30 13:26:50.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/bpm.py
--rw-rw-rw-   0        0        0    34681 2024-01-30 13:26:54.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/consumption.py
--rw-rw-rw-   0        0        0    25767 2024-01-30 13:26:57.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/dam.py
--rw-rw-rw-   0        0        0    15698 2024-01-30 13:27:01.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/dams.py
--rw-rw-rw-   0        0        0     5544 2024-01-30 13:32:07.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/general_data.py
--rw-rw-rw-   0        0        0    11556 2024-01-30 13:32:10.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/idm.py
--rw-rw-rw-   0        0        0     8395 2024-01-30 13:32:15.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/imbalance.py
--rw-rw-rw-   0        0        0     8721 2024-01-30 13:32:21.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/mms.py
--rw-rw-rw-   0        0        0    22481 2024-01-30 13:32:25.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/pfm.py
--rw-rw-rw-   0        0        0    18256 2024-01-30 13:32:28.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/production.py
--rw-rw-rw-   0        0        0    28283 2024-01-30 13:32:31.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/renewables.py
--rw-rw-rw-   0        0        0    17089 2024-01-30 13:32:35.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/reports.py
--rw-rw-rw-   0        0        0    20781 2024-01-30 13:32:40.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/transmission.py
--rw-rw-rw-   0        0        0    15315 2024-01-30 13:32:43.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/data/yekg.py
--rw-rw-rw-   0        0        0     1787 2024-01-30 13:33:02.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/service.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.467014 theohe-epias-0.0.8/src/theohe_epias/transparency/utils/
--rw-rw-rw-   0        0        0        0 2023-12-22 06:57:44.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/utils/__init__.py
--rw-rw-rw-   0        0        0     2409 2024-01-02 07:05:20.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/utils/get_time.py
--rw-rw-rw-   0        0        0     1089 2023-12-27 09:14:12.000000 theohe-epias-0.0.8/src/theohe_epias/transparency/utils/time_format.py
-drwxrwxrwx   0        0        0        0 2024-02-15 12:15:50.467014 theohe-epias-0.0.8/src/theohe_epias.egg-info/
--rw-rw-rw-   0        0        0     2534 2024-02-15 12:15:50.000000 theohe-epias-0.0.8/src/theohe_epias.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2165 2024-02-15 12:15:50.000000 theohe-epias-0.0.8/src/theohe_epias.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 12:15:50.000000 theohe-epias-0.0.8/src/theohe_epias.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-02-15 12:15:50.000000 theohe-epias-0.0.8/src/theohe_epias.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-15 12:15:50.000000 theohe-epias-0.0.8/src/theohe_epias.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.753495 theohe_epias-0.0.9/
+-rw-rw-rw-   0        0        0     1100 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3490 2024-04-17 11:19:41.737917 theohe_epias-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2858 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/README.md
+-rw-rw-rw-   0        0        0      618 2024-04-15 12:45:39.000000 theohe_epias-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 11:19:41.753495 theohe_epias-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.537623 theohe_epias-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.559729 theohe_epias-0.0.9/src/theohe_epias/
+-rw-rw-rw-   0        0        0        0 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/src/theohe_epias/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.591067 theohe_epias-0.0.9/src/theohe_epias/epys/
+-rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe_epias-0.0.9/src/theohe_epias/epys/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.591067 theohe_epias-0.0.9/src/theohe_epias/epys/collateral/
+-rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe_epias-0.0.9/src/theohe_epias/epys/collateral/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.591067 theohe_epias-0.0.9/src/theohe_epias/epys/eligible_customer/
+-rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe_epias-0.0.9/src/theohe_epias/epys/eligible_customer/__init__.py
+-rw-rw-rw-   0        0        0     6134 2024-04-15 12:50:19.000000 theohe_epias-0.0.9/src/theohe_epias/epys/eligible_customer/eligible_customer_meter.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.606706 theohe_epias-0.0.9/src/theohe_epias/epys/invoice/
+-rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe_epias-0.0.9/src/theohe_epias/epys/invoice/__init__.py
+-rw-rw-rw-   0        0        0     3909 2024-04-15 12:50:26.000000 theohe_epias-0.0.9/src/theohe_epias/epys/invoice/data.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.622296 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/
+-rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/__init__.py
+-rw-rw-rw-   0        0        0     4218 2024-04-15 12:50:33.000000 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/advance.py
+-rw-rw-rw-   0        0        0     6337 2024-04-15 12:50:38.000000 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/imbalance.py
+-rw-rw-rw-   0        0        0     5054 2024-04-17 11:04:29.000000 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/renewables.py
+-rw-rw-rw-   0        0        0     9351 2024-04-15 12:50:43.000000 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/reports.py
+-rw-rw-rw-   0        0        0    14535 2024-04-15 12:50:51.000000 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/settlement.py
+-rw-rw-rw-   0        0        0    11343 2024-04-15 12:50:56.000000 theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/settlementdata.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.638005 theohe_epias-0.0.9/src/theohe_epias/epys/registration/
+-rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe_epias-0.0.9/src/theohe_epias/epys/registration/__init__.py
+-rw-rw-rw-   0        0        0    19777 2024-04-15 12:51:03.000000 theohe_epias-0.0.9/src/theohe_epias/epys/registration/registrationmeter.py
+-rw-rw-rw-   0        0        0     2811 2024-04-17 11:04:58.000000 theohe_epias-0.0.9/src/theohe_epias/epys/service.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.638005 theohe_epias-0.0.9/src/theohe_epias/epys/unlicensed/
+-rw-rw-rw-   0        0        0        0 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/src/theohe_epias/epys/unlicensed/__init__.py
+-rw-rw-rw-   0        0        0     4321 2024-04-15 12:51:15.000000 theohe_epias-0.0.9/src/theohe_epias/epys/unlicensed/luytob_control.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.659682 theohe_epias-0.0.9/src/theohe_epias/epys/utils/
+-rw-rw-rw-   0        0        0        0 2024-01-02 14:16:48.000000 theohe_epias-0.0.9/src/theohe_epias/epys/utils/__init__.py
+-rw-rw-rw-   0        0        0     1784 2024-01-31 07:53:21.000000 theohe_epias-0.0.9/src/theohe_epias/epys/utils/get_time.py
+-rw-rw-rw-   0        0        0     1483 2024-01-24 10:50:10.000000 theohe_epias-0.0.9/src/theohe_epias/epys/utils/tgt.py
+-rw-rw-rw-   0        0        0     2568 2024-01-24 13:44:04.000000 theohe_epias-0.0.9/src/theohe_epias/epys/utils/time_format.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.659682 theohe_epias-0.0.9/src/theohe_epias/transparency/
+-rw-rw-rw-   0        0        0        0 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.722259 theohe_epias-0.0.9/src/theohe_epias/transparency/data/
+-rw-rw-rw-   0        0        0        0 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/__init__.py
+-rw-rw-rw-   0        0        0     7243 2024-04-15 12:51:37.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/ancillary_services.py
+-rw-rw-rw-   0        0        0     7161 2024-04-15 12:51:41.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/bilateral_contracts.py
+-rw-rw-rw-   0        0        0     7116 2024-04-15 12:51:44.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/bpm.py
+-rw-rw-rw-   0        0        0    34661 2024-04-15 12:51:47.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/consumption.py
+-rw-rw-rw-   0        0        0    25747 2024-04-15 12:51:50.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/dam.py
+-rw-rw-rw-   0        0        0    15678 2024-04-15 12:51:54.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/dams.py
+-rw-rw-rw-   0        0        0     5524 2024-04-15 12:51:57.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/general_data.py
+-rw-rw-rw-   0        0        0    11536 2024-04-15 12:52:00.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/idm.py
+-rw-rw-rw-   0        0        0     8375 2024-04-15 12:52:03.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/imbalance.py
+-rw-rw-rw-   0        0        0     8701 2024-04-15 12:52:05.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/mms.py
+-rw-rw-rw-   0        0        0    22461 2024-04-15 12:52:08.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/pfm.py
+-rw-rw-rw-   0        0        0    18236 2024-04-15 12:52:11.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/production.py
+-rw-rw-rw-   0        0        0    28263 2024-04-15 12:52:14.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/renewables.py
+-rw-rw-rw-   0        0        0    17069 2024-04-15 12:52:16.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/reports.py
+-rw-rw-rw-   0        0        0    20761 2024-04-15 12:52:20.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/transmission.py
+-rw-rw-rw-   0        0        0    15295 2024-04-15 12:52:22.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/data/yekg.py
+-rw-rw-rw-   0        0        0     1611 2024-04-15 12:52:50.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/service.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.737917 theohe_epias-0.0.9/src/theohe_epias/transparency/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/utils/__init__.py
+-rw-rw-rw-   0        0        0     2409 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/utils/get_time.py
+-rw-rw-rw-   0        0        0     1089 2024-03-28 07:48:53.000000 theohe_epias-0.0.9/src/theohe_epias/transparency/utils/time_format.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:19:41.737917 theohe_epias-0.0.9/src/theohe_epias.egg-info/
+-rw-rw-rw-   0        0        0     3490 2024-04-17 11:19:41.000000 theohe_epias-0.0.9/src/theohe_epias.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2312 2024-04-17 11:19:41.000000 theohe_epias-0.0.9/src/theohe_epias.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:19:41.000000 theohe_epias-0.0.9/src/theohe_epias.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-17 11:19:41.000000 theohe_epias-0.0.9/src/theohe_epias.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-17 11:19:41.000000 theohe_epias-0.0.9/src/theohe_epias.egg-info/top_level.txt
```

### Comparing `theohe-epias-0.0.8/LICENSE` & `theohe_epias-0.0.9/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [2024] [Onur Hakkı Eyüboğlu]
+Copyright (c) 2024 Onur Hakkı Eyüboğlu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `theohe-epias-0.0.8/PKG-INFO` & `theohe_epias-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,81 @@
-Metadata-Version: 2.1
-Name: theohe-epias
-Version: 0.0.8
-Summary: Energy Exchange Istanbul (EXIST) or Enerji Piyasaları İşletme A.Ş. (EPİAŞ) by its Turkish name is an energy exchange company.
-Author-email: Onur Hakkı Eyüboğlu <eyubogluo@itu.edu.tr>
-Project-URL: Homepage, https://github.com/onurhakki/exist
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: pandas
-Requires-Dist: pwinput
-
 # Energy Exchange Istanbul (EXIST)
 
-Energy Exchange Istanbul (EXIST) or Enerji Piyasaları İşletme A.Ş. (EPİAŞ) by its Turkish name is an energy exchange company. 
+Energy Exchange Istanbul (EXIST) or Enerji Piyasaları İşletme A.Ş. (EPİAŞ) by its Turkish name is an energy exchange company.
+
+## Services
+
+ - Transparency Platform (Şeffaflık Platformu)
+ - EMMS (Energy Markets Management System) - EPYS (Enerji Piyasaları Yönetim Sistemi)
 
 ### download via pip
+
 ```
 !pip install theohe-epias
 ```
 
 ## Transparency Platform (Şeffaflık Platformu)
 
 Transparency Platform provides necessary data for the transparent, reliable, fair and predictable operation of energy markets. You can access platform from [here](https://seffaflik.epias.com.tr/home).
 
 Also, Transparency API is available for everyone. In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/Transparency%20WebService.ipynb), you can access example details.
 
 ### usage - (example: Market Clearing Price (MCP) - Piyasa Takas Fiyatı (PTF))
+
 ```
 from theohe_epias.transparency.service import WebServiceTransparency
 ws = WebServiceTransparency()
 ws.dam.mcp()
 ```
 
+
 ### usage - between selected dates (example: Market Clearing Price (MCP) - Piyasa Takas Fiyatı (PTF))
+
 ```
 from theohe_epias.transparency.service import WebServiceTransparency
 ws = WebServiceTransparency()
 ws.dam.mcp(startDate=(2023, 12, 1), endDate=(2023, 12, 31), function = "export")
 ```
 
 
+### usage - (example: Market Clearing Price (MCP))
+
+##### 2023 MCP hourly averages on monthly basis
+
+In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/Transparency%20WebService%20(MCP%20-%20SMP%20-%20Direction).ipynb), you can access example details.
+
+
+![mcp_2023](https://github.com/onurhakki/exist/assets/53830179/54c7390c-cc11-4230-9e40-ceda4a1f0592)
+
+
+### usage - (example: System's Direction)
+
+##### 2023 System's Direction averages on monthly basis
+
+In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/Transparency%20WebService%20(MCP%20-%20SMP%20-%20Direction).ipynb), you can access example details.
+
+
+![direction_2023](https://github.com/onurhakki/exist/assets/53830179/8f19d58e-344e-4253-aa69-8217f1b84113)
+
+
 ## EPYS (Enerji Piyasaları Yönetim Sistemi) - EMMS (Energy Markets Management System)
 
 You can access platform from [here](https://epys.epias.com.tr/home).
 
 Also, EPYS is only available for market participants. In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/EPYS%20WebService%20.ipynb), you can access example details.
 
 ### usage - login 
+
 ```
 from theohe_epias.epys.service import WebServiceEPYS
 import warnings
 
 warnings.simplefilter("ignore")
 
 ws = WebServiceEPYS(username = "USERNAME", organizationId = 123456789, test=None)
 ### None for prod
 ### "prp" for test
 ws.login()
 ### or directly use below code
 ### ws.login("password")
 ```
 
-
-
-
-
```

### Comparing `theohe-epias-0.0.8/pyproject.toml` & `theohe_epias-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "theohe-epias"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Onur Hakkı Eyüboğlu", email="eyubogluo@itu.edu.tr" },
 ]
 description = "Energy Exchange Istanbul (EXIST) or Enerji Piyasaları İşletme A.Ş. (EPİAŞ) by its Turkish name is an energy exchange company."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/eligible_customer/eligible_customer_meter.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/eligible_customer/eligible_customer_meter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
-from theohe_epias.epys.utils.time_format import tuple_to_datetime, control_times
+from ...epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
+from ...epys.utils.time_format import tuple_to_datetime, control_times
 from json import dumps
 from requests import request
 
 
 class EligibleCustomerMeter():
     def request_eligiblecustomermeter_data(self, path, payload, octet = False):
         if octet == False:
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/invoice/data.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/invoice/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days
-from theohe_epias.epys.utils.time_format import tuple_to_datetime
+from ...epys.utils.get_time import get_current_settlement_days
+from ...epys.utils.time_format import tuple_to_datetime
 from json import dumps
 from requests import request
 
 class Invoice():
     def request_invoice_data(self, path, payload, octet = False):
         if octet == False:
             service_header ={
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/advance.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/advance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days, get_last_day_of_month, get_current_month
-from theohe_epias.epys.utils.time_format import tuple_to_datetime, control_times
+from ...epys.utils.get_time import get_current_settlement_days, get_last_day_of_month, get_current_month
+from ...epys.utils.time_format import tuple_to_datetime, control_times
 from json import dumps
 from requests import request
 
 
 class Advance():
     def request_advance_data(self, path, payload, octet = False):
         if octet == False:
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/imbalance.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/imbalance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
-from theohe_epias.epys.utils.time_format import tuple_to_datetime, control_times
+from ...epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
+from ...epys.utils.time_format import tuple_to_datetime, control_times
 from json import dumps
 from requests import request
 
 
 class Imbalance():
     def request_imbalance_data(self, path, payload, octet = False):
         if octet == False:
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/reports.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
-from theohe_epias.epys.utils.time_format import tuple_to_datetime, control_times
+from ...epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
+from ...epys.utils.time_format import tuple_to_datetime, control_times
 from json import dumps
 from requests import request
 
 
 class Reports():
     def request_reports_data(self, path, payload, octet = False):
         if octet == False:
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/settlement.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/settlement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
-from theohe_epias.epys.utils.time_format import tuple_to_datetime, control_times
+from ...epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
+from ...epys.utils.time_format import tuple_to_datetime, control_times
 from json import dumps
 from requests import request
 
 
 class Settlement():
     def request_settlement_data(self, path, payload, octet = False):
         if octet == False:
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/reconciliation/settlementdata.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/reconciliation/settlementdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
-from theohe_epias.epys.utils.time_format import tuple_to_datetime, control_times
+from ...epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
+from ...epys.utils.time_format import tuple_to_datetime, control_times
 from json import dumps
 from requests import request
 
 
 class SettlementData():
     def request_data_data(self, path, payload, octet = False):
         if octet == False:
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/registration/registrationmeter.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/registration/registrationmeter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from pandas import ExcelFile
-from theohe_epias.epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
-from theohe_epias.epys.utils.time_format import tuple_to_datetime, control_times
+from ...epys.utils.get_time import get_current_settlement_days, get_last_day_of_month
+from ...epys.utils.time_format import tuple_to_datetime, control_times
 from json import dumps
 from requests import request
 
 
 class RegistrationMeter():
     def request_registrationmeter_data(self, path, payload, octet = False):
         if octet == False:
@@ -343,7 +343,138 @@
             "page": {'number': self.page, 'size': 10000}})
 
         
         if self.final_response != None:
             self.formatted_final_response = self.format_files_registrationmeter(function)
             return self.formatted_final_response
 
+    def registration_powerplant_data(self,
+                        id:int = None,
+                        #idContains: null,
+                        installedPowerMax:float = None,
+                        installedPowerMin:float = None,
+                        licenseNumber:str = None,
+                        licenseTypeIds:list =  [], 
+                        # 11: Üretim Lisansı
+                        # 8 : OSB Üretim Lisansı
+                        # 9 : İletim Lisansı
+                        # 12: Tedarik Lisansı
+                        # 13: Dağıtım Lisansı
+                        # 7 : OSB Dağıtım Lisansı
+                        # 14: Şarj Ağı Lisansı
+
+
+
+                        effectiveDate:tuple = None,
+                        eic:str = None,
+                        name:str = None,
+
+                        recordStatusIds:list = [],
+                        rsmStatusIds:list = [0, 1, 2], # Kayıtlı, Kayıtsız, YEKA
+                        sourceGroupIds:list = [], # [0,1,2] ...
+                        sourceTypeIds:list = [] , # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 31, 32, 33, 41, 43, 44, 48, 49, 50, 53, 54, 141, 12]
+                        trimmingStatusIds:list = [], # 0 , 1
+
+                        statusIds:list = [], 
+                        typeIds:list = [],
+
+                        function = "list"
+):
+
+        
+        """
+        #Registration
+        Santral Listeleme
+        ---------
+        Santrallerin kayıt detaylarını döner.
+
+        İlgili Sayfa
+        ---------
+        https://epys.epias.com.tr/registration-operations/power-plant-operations/power-plant-operation-list
+
+        Parametre 
+        ---------
+         - id:int = None,
+         - effectiveDate:tuple = None,
+         - eic:str = None,
+         - name:str = None,
+         - greenTariffTypeIds:list =  [], ## YETA [1,2,3,4,5,6,7,8,9]
+         - balancingMarketParticipationStatusIds:list =  [], 2 Katılıyor, 3 Katılmıyor
+         - powerPlantEffectiveId:int = None, Santral
+         - recordStatusIds:list = [], # Mevcut Durum: 1 Kullanımda, 2 Kullanım dışı
+         - statusIds:list = [], #Durum: 2 Aktif, 3 Pasif
+         - typeIds:list = [],
+            - typeIds => {
+                0: Sanal
+                1: Dengelemeye Dahil Olmayan Üretim Birimi
+                2: Dengeleme Birimi
+                3: Serbest Tüketici
+                4: Otoproduktor Tüketim Tesisi
+                5: Dağıtım Bölgesi
+                7: Otoproduktor Grup Ortağı
+                8: Santral İç Tüketimi
+                10: İki Bölge Arasında Koridor
+                11: Serbest Tüketici (OSB)
+                12: YEKDEM Kapsamındaki Lisanslı Üretim Birimi
+                13: YEKDEM Kapsamındaki Lisanssız Üretim Birimi
+                14: ST Olmayan Tüketiciler
+                15: Perakende Müşterisi Olan Dağıtımdan Bağlı Serbest Tüketiciler
+                16: Tedarikçiden Perakendeye Dönen Dağıtımdan Bağlı Serbest Tüketiciler
+                17: Perakende Müşterisi Olan İletimden Bağlı Serbest Tüketiciler
+                18: Tedarikçiden Perakendeye Dönen İletimden Bağlı Serbest Tüketiciler
+                20: Sıfır Bakiye Çekişlerinin Tutulduğu UEVÇB
+                21: YEKDEM Dengeleme Birimi
+                22: YEKDEM Üretim Birimi
+                23: LÜY
+                24: TEİAŞ - İç İhtiyaç
+                25: YETA
+                26: İç İhtiyaç – Diğer
+                27: İthalat - İhracat
+                28: TEİAŞ - İSKK
+                29: Aydınlatma
+                }
+
+        Notlar
+        ---------
+         - Yok.
+        """
+
+        if effectiveDate != None:
+            effectiveDate= tuple_to_datetime(effectiveDate)
+            if effectiveDate == False:
+                return
+
+            
+        if function == "list":
+            path = "https://epys{}.epias.com.tr/registration/v1/power-plant/query".format(self.test_coef)
+        else:
+            print("Function is not defined")
+            return
+                    
+        self.request_registrationmeter_data(path, {
+                                    "effectiveDate":effectiveDate,
+                        "eic":eic,
+                        "id":id,
+                        "name":name,
+                        
+                        "installedPowerMax": installedPowerMax,
+                        "installedPowerMin":installedPowerMin,
+                        "licenseNumber":licenseNumber,
+                        "licenseTypeIds": licenseTypeIds,
+
+                        "organizationId":None if self.organizationId == 2 else self.organizationId,
+                        "recordStatusIds":recordStatusIds,
+                        "rsmStatusIds":rsmStatusIds,
+                        "sourceGroupIds": sourceGroupIds,
+                        "sourceTypeIds": sourceTypeIds,
+                        "statusIds":statusIds,
+                        "trimmingStatusIds": trimmingStatusIds,
+                        "typeIds":typeIds,
+
+            "page": {'number': self.page, 'size': 10000}})
+
+        
+        if self.final_response != None:
+            self.formatted_final_response = self.format_files_registrationmeter(function)
+            return self.formatted_final_response
+
+
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/service.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 
-from theohe_epias.epys.utils.tgt import RequestFunctions
+from ..epys.utils.tgt import RequestFunctions
 
-from theohe_epias.epys.invoice.data import Invoice
+from ..epys.invoice.data import Invoice
 
-from theohe_epias.epys.reconciliation.settlement import Settlement
-from theohe_epias.epys.reconciliation.reports import Reports
-from theohe_epias.epys.reconciliation.settlementdata import SettlementData
-from theohe_epias.epys.reconciliation.advance import Advance
-from theohe_epias.epys.reconciliation.imbalance import Imbalance
+from ..epys.reconciliation.settlement import Settlement
+from ..epys.reconciliation.reports import Reports
+from ..epys.reconciliation.settlementdata import SettlementData
+from ..epys.reconciliation.advance import Advance
+from ..epys.reconciliation.imbalance import Imbalance
+from ..epys.reconciliation.renewables import Renewables
 
 
-from theohe_epias.epys.registration.registrationmeter import RegistrationMeter
+from ..epys.registration.registrationmeter import RegistrationMeter
 
-from theohe_epias.epys.eligible_customer.eligible_customer_meter import EligibleCustomerMeter
+from ..epys.eligible_customer.eligible_customer_meter import EligibleCustomerMeter
 
+from ..epys.unlicensed.luytob_control import LUYTOB
 
 
 class WebServiceEPYS(
     RequestFunctions, 
     Invoice, 
-    Settlement, Reports, SettlementData, Advance, Imbalance,
+    Settlement, Reports, SettlementData, Advance, Imbalance, Renewables,
     RegistrationMeter,
-    EligibleCustomerMeter
+    EligibleCustomerMeter,
+    LUYTOB
     ): 
     def __init__(self, username, organizationId, test = None):
         """
         
         If you are tring to list data more than 10000 rows, you have to use page value and request again.
         
         """
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/utils/get_time.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/utils/get_time.py`

 * *Files identical despite different names*

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/utils/tgt.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/utils/tgt.py`

 * *Files identical despite different names*

### Comparing `theohe-epias-0.0.8/src/theohe_epias/epys/utils/time_format.py` & `theohe_epias-0.0.9/src/theohe_epias/epys/utils/time_format.py`

 * *Files identical despite different names*

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/ancillary_services.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/ancillary_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_tomorrow, get_this_month
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_tomorrow, get_this_month
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class AS():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "primary_frequency_capacity_amount": {"list":"markets/ancillary-services/data/primary-frequency-capacity-amount","export":"markets/ancillary-services/export/primary-frequency-capacity-amount"},
 "primary_frequency_capacity_price": {"list":"markets/ancillary-services/data/primary-frequency-capacity-price","export":"markets/ancillary-services/export/primary-frequency-capacity-price"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/bilateral_contracts.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/bilateral_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_year
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_year
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class BC():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "amount_of_bilateral_contracts": {"list":"markets/bilateral-contracts/data/amount-of-bilateral-contracts","export":"markets/bilateral-contracts/export/amount-of-bilateral-contracts"},
 "bilateral_contracts_bid_quantity": {"list":"markets/bilateral-contracts/data/bilateral-contracts-bid-quantity","export":"markets/bilateral-contracts/export/bilateral-contracts-bid-quantity"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/bpm.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/bpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_time_bpm, get_today, get_yesterday, get_this_month
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_time_bpm, get_today, get_yesterday, get_this_month
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class BPM():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "order_summary_down": {"list":"markets/bpm/data/order-summary-down","export":"markets/bpm/export/order-summary-down"},
 "order_summary_up": {"list":"markets/bpm/data/order-summary-up","export":"markets/bpm/export/order-summary-up"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/consumption.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/consumption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_current_settlement_fday, get_current_settlement_lday
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_current_settlement_fday, get_current_settlement_lday
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class Consumption():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "consumer_quantity": {"list":"consumption/data/consumer-quantity","export":"consumption/export/consumer-quantity"},
 "consumer_sector_list": {"list":"consumption/data/consumer-sector-list"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/dam.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/dam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_time_dam
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_time_dam
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class DAM():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
       #      "mcp": {"list":"markets/dam/data/mcp", "export":"markets/dam/export/mcp"},
        #     "interim_mcp": {"list":"markets/dam/data/interim-mcp", "export":"markets/dam/export/interim-mcp"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/dams.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/dams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class Dams():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "active_fullness": {"list":"dams/data/active-fullness","export":"dams/export/active-fullness"},
 "active_volume": {"list":"dams/data/active-volume","export":"dams/export/active-volume"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/general_data.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/general_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_yesterday, get_this_month
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_yesterday, get_this_month
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class GD():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "market_participants": {"list":"markets/general-data/data/market-participants","export":"markets/general-data/export/market-participants"},
 "market_participants_organization_filter_list": {"list":"markets/general-data/data/market-participants-organization-filter-list"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/idm.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/idm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class IDM():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "bid_offer_quantities": {"list":"markets/idm/data/bid-offer-quantities","export":"markets/idm/export/bid-offer-quantities"},
 "matching_quantity": {"list":"markets/idm/data/matching-quantity","export":"markets/idm/export/matching-quantity"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/imbalance.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/imbalance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_current_settlement_day, get_current_settlement_fday, get_current_settlement_lday, get_last_year
+from ...transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_current_settlement_day, get_current_settlement_fday, get_current_settlement_lday, get_last_year
 
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class IB():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "dsg_imbalance_quantity": {"list":"markets/imbalance/data/dsg-imbalance-quantity","export":"markets/imbalance/export/dsg-imbalance-quantity"},
 "dsg_organization_list": {"list":"markets/imbalance/data/dsg-organization-list"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/mms.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/mms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class MMS():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "organization_list": {"list":"generation/data/organization-list"},
 "power_plant_list_by_organization_id": {"list":"markets/data/power-plant-list-by-organization-id"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/pfm.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/pfm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_last_year
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_last_year
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class PFM():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "contract_price_summary": {"list":"markets/pfm/data/contract-price-summary","export":"markets/pfm/export/contract-price-summary"},
 "ggf": {"list":"markets/pfm/data/ggf","export":"markets/pfm/export/ggf"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/production.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/production.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_year, get_tomorrow, get_current_settlement_fday, get_current_settlement_lday, get_last_year
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_year, get_tomorrow, get_current_settlement_fday, get_current_settlement_lday, get_last_year
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class Production():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "aic": {"list":"generation/data/aic","export":"generation/export/aic"},
 "dpp": {"list":"generation/data/dpp","export":"generation/export/dpp"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/renewables.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/renewables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday, get_last_year
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday, get_last_year
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class Renewables():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 #"generation_forecast": {"list":"renewables/data/generation-forecast","export":"renewables/export/generation-forecast"},
 #"imbalance_cost": {"list":"renewables/data/imbalance-cost","export":"renewables/export/imbalance-cost"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/reports.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_yesterday
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_yesterday
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class Reports():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
             "mcp_smp_imbalance": {"list":"data/ptf-smf-sdf", "export":"export/ptf-smf-sdf"},
             "daily_report": {"list":"data/daily-report", "export":"export/daily-report"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/transmission.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/transmission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_year, get_yesterday, get_tomorrow, get_this_month, get_current_settlement_fday, get_current_settlement_lday
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class Transmission():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 
 "capacity_demand": {"list":"transmission/data/capacity-demand","export":"transmission/export/capacity-demand-export"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/data/yekg.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/data/yekg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 
-from theohe_epias.transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_year, get_last_year
-from theohe_epias.transparency.utils.time_format import tuple_to_datetime
+from ...transparency.utils.get_time import get_today, get_yesterday, get_this_month, get_year, get_last_year
+from ...transparency.utils.time_format import tuple_to_datetime
 
 class YEKG():
     def __init__(self):
         self.information = dict()
         self.information["data"] = dict({
 "bilateral_contract_list": {"list":"markets/yek-g/data/bilateral-contract-list","export":"markets/yek-g/export/bilateral-contract-list"},
 "cancelation_quantity": {"list":"markets/yek-g/data/cancelation-quantity","export":"markets/yek-g/export/cancelation-quantity"},
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/utils/get_time.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/utils/get_time.py`

 * *Files identical despite different names*

### Comparing `theohe-epias-0.0.8/src/theohe_epias/transparency/utils/time_format.py` & `theohe_epias-0.0.9/src/theohe_epias/transparency/utils/time_format.py`

 * *Files identical despite different names*

### Comparing `theohe-epias-0.0.8/src/theohe_epias.egg-info/PKG-INFO` & `theohe_epias-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theohe-epias
-Version: 0.0.8
+Version: 0.0.9
 Summary: Energy Exchange Istanbul (EXIST) or Enerji Piyasaları İşletme A.Ş. (EPİAŞ) by its Turkish name is an energy exchange company.
 Author-email: Onur Hakkı Eyüboğlu <eyubogluo@itu.edu.tr>
 Project-URL: Homepage, https://github.com/onurhakki/exist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -12,60 +12,86 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: pwinput
 
 # Energy Exchange Istanbul (EXIST)
 
-Energy Exchange Istanbul (EXIST) or Enerji Piyasaları İşletme A.Ş. (EPİAŞ) by its Turkish name is an energy exchange company. 
+Energy Exchange Istanbul (EXIST) or Enerji Piyasaları İşletme A.Ş. (EPİAŞ) by its Turkish name is an energy exchange company.
+
+## Services
+
+ - Transparency Platform (Şeffaflık Platformu)
+ - EMMS (Energy Markets Management System) - EPYS (Enerji Piyasaları Yönetim Sistemi)
 
 ### download via pip
+
 ```
 !pip install theohe-epias
 ```
 
 ## Transparency Platform (Şeffaflık Platformu)
 
 Transparency Platform provides necessary data for the transparent, reliable, fair and predictable operation of energy markets. You can access platform from [here](https://seffaflik.epias.com.tr/home).
 
 Also, Transparency API is available for everyone. In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/Transparency%20WebService.ipynb), you can access example details.
 
 ### usage - (example: Market Clearing Price (MCP) - Piyasa Takas Fiyatı (PTF))
+
 ```
 from theohe_epias.transparency.service import WebServiceTransparency
 ws = WebServiceTransparency()
 ws.dam.mcp()
 ```
 
+
 ### usage - between selected dates (example: Market Clearing Price (MCP) - Piyasa Takas Fiyatı (PTF))
+
 ```
 from theohe_epias.transparency.service import WebServiceTransparency
 ws = WebServiceTransparency()
 ws.dam.mcp(startDate=(2023, 12, 1), endDate=(2023, 12, 31), function = "export")
 ```
 
 
+### usage - (example: Market Clearing Price (MCP))
+
+##### 2023 MCP hourly averages on monthly basis
+
+In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/Transparency%20WebService%20(MCP%20-%20SMP%20-%20Direction).ipynb), you can access example details.
+
+
+![mcp_2023](https://github.com/onurhakki/exist/assets/53830179/54c7390c-cc11-4230-9e40-ceda4a1f0592)
+
+
+### usage - (example: System's Direction)
+
+##### 2023 System's Direction averages on monthly basis
+
+In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/Transparency%20WebService%20(MCP%20-%20SMP%20-%20Direction).ipynb), you can access example details.
+
+
+![direction_2023](https://github.com/onurhakki/exist/assets/53830179/8f19d58e-344e-4253-aa69-8217f1b84113)
+
+
 ## EPYS (Enerji Piyasaları Yönetim Sistemi) - EMMS (Energy Markets Management System)
 
 You can access platform from [here](https://epys.epias.com.tr/home).
 
 Also, EPYS is only available for market participants. In the [Notebook](https://github.com/onurhakki/exist/blob/main/example-notebooks/EPYS%20WebService%20.ipynb), you can access example details.
 
 ### usage - login 
+
 ```
 from theohe_epias.epys.service import WebServiceEPYS
 import warnings
 
 warnings.simplefilter("ignore")
 
 ws = WebServiceEPYS(username = "USERNAME", organizationId = 123456789, test=None)
 ### None for prod
 ### "prp" for test
 ws.login()
 ### or directly use below code
 ### ws.login("password")
 ```
 
-
-
-
-
```

### Comparing `theohe-epias-0.0.8/src/theohe_epias.egg-info/SOURCES.txt` & `theohe_epias-0.0.9/src/theohe_epias.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 src/theohe_epias/epys/eligible_customer/__init__.py
 src/theohe_epias/epys/eligible_customer/eligible_customer_meter.py
 src/theohe_epias/epys/invoice/__init__.py
 src/theohe_epias/epys/invoice/data.py
 src/theohe_epias/epys/reconciliation/__init__.py
 src/theohe_epias/epys/reconciliation/advance.py
 src/theohe_epias/epys/reconciliation/imbalance.py
+src/theohe_epias/epys/reconciliation/renewables.py
 src/theohe_epias/epys/reconciliation/reports.py
 src/theohe_epias/epys/reconciliation/settlement.py
 src/theohe_epias/epys/reconciliation/settlementdata.py
 src/theohe_epias/epys/registration/__init__.py
 src/theohe_epias/epys/registration/registrationmeter.py
+src/theohe_epias/epys/unlicensed/__init__.py
+src/theohe_epias/epys/unlicensed/luytob_control.py
 src/theohe_epias/epys/utils/__init__.py
 src/theohe_epias/epys/utils/get_time.py
 src/theohe_epias/epys/utils/tgt.py
 src/theohe_epias/epys/utils/time_format.py
 src/theohe_epias/transparency/__init__.py
 src/theohe_epias/transparency/service.py
 src/theohe_epias/transparency/data/__init__.py
```


# Comparing `tmp/mns-scheduler-1.0.4.0.tar.gz` & `tmp/mns-scheduler-1.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.4.0.tar", last modified: Wed May  8 05:56:59 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.4.2.tar", last modified: Wed May  8 10:07:43 2024, max compression
```

## Comparing `mns-scheduler-1.0.4.0.tar` & `mns-scheduler-1.0.4.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.453508 mns-scheduler-1.0.4.0/
--rw-rw-rw-   0        0        0       62 2024-05-08 05:56:59.452511 mns-scheduler-1.0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.415190 mns-scheduler-1.0.4.0/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.417184 mns-scheduler-1.0.4.0/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.418182 mns-scheduler-1.0.4.0/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.420176 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.421174 mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.422171 mns-scheduler-1.0.4.0/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.424166 mns-scheduler-1.0.4.0/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.425163 mns-scheduler-1.0.4.0/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.425163 mns-scheduler-1.0.4.0/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2459 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.426160 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.427157 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.429152 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.431147 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.433143 mns-scheduler-1.0.4.0/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.4.0/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.434512 mns-scheduler-1.0.4.0/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.435033 mns-scheduler-1.0.4.0/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.0/mns_scheduler/finance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.435547 mns-scheduler-1.0.4.0/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.437088 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.438124 mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.438636 mns-scheduler-1.0.4.0/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.439149 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.440191 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-08 05:55:00.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.441240 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.442264 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.444313 mns-scheduler-1.0.4.0/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.446367 mns-scheduler-1.0.4.0/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.446878 mns-scheduler-1.0.4.0/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.450494 mns-scheduler-1.0.4.0/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.451516 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    15508 2024-05-06 09:12:33.000000 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.452511 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3281 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 05:56:59.453508 mns-scheduler-1.0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-08 05:56:57.000000 mns-scheduler-1.0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.638122 mns-scheduler-1.0.4.2/
+-rw-rw-rw-   0        0        0       62 2024-05-08 10:07:43.638122 mns-scheduler-1.0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.602218 mns-scheduler-1.0.4.2/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.604213 mns-scheduler-1.0.4.2/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.605210 mns-scheduler-1.0.4.2/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.607205 mns-scheduler-1.0.4.2/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.608203 mns-scheduler-1.0.4.2/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.609200 mns-scheduler-1.0.4.2/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.610197 mns-scheduler-1.0.4.2/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.611194 mns-scheduler-1.0.4.2/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.612192 mns-scheduler-1.0.4.2/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     5253 2024-05-08 10:01:50.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.612192 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.614186 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.615183 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.617178 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.618176 mns-scheduler-1.0.4.2/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.4.2/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.619173 mns-scheduler-1.0.4.2/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.620170 mns-scheduler-1.0.4.2/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.2/mns_scheduler/finance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.620170 mns-scheduler-1.0.4.2/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.621168 mns-scheduler-1.0.4.2/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.622166 mns-scheduler-1.0.4.2/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.623162 mns-scheduler-1.0.4.2/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.623162 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.625157 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-08 05:55:00.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.626154 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.627152 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.628149 mns-scheduler-1.0.4.2/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.2/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.630144 mns-scheduler-1.0.4.2/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.2/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.2/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.2/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.631142 mns-scheduler-1.0.4.2/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.635131 mns-scheduler-1.0.4.2/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.637125 mns-scheduler-1.0.4.2/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    15511 2024-05-08 10:06:57.000000 mns-scheduler-1.0.4.2/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.2/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:07:43.637125 mns-scheduler-1.0.4.2/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-08 10:07:43.000000 mns-scheduler-1.0.4.2/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3281 2024-05-08 10:07:43.000000 mns-scheduler-1.0.4.2/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:07:43.000000 mns-scheduler-1.0.4.2/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 10:07:43.000000 mns-scheduler-1.0.4.2/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:07:43.638122 mns-scheduler-1.0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-08 10:07:28.000000 mns-scheduler-1.0.4.2/setup.py
```

### Comparing `mns-scheduler-1.0.4.0/README.md` & `mns-scheduler-1.0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.4.2/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.4.2/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.4.2/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.4.2/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.4.2/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.4.2/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.4.2/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.4.2/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
 # 开盘前同步当天交易需要的k线数据
 blockingScheduler.add_job(sync_today_trade_k_line_info, 'cron', hour='08', minute='30')
 
 # 同步十大流通股东信息
 blockingScheduler.add_job(sync_stock_gdfx_free_top_10_one_day, 'cron', hour='08,22', minute='23')
 
 # 更新同花顺概念信息
-blockingScheduler.add_job(ths_concept_info_clean, 'cron', hour='9,18', minute='01')
+blockingScheduler.add_job(ths_concept_info_clean, 'cron', hour='9,12,20', minute='24')
 
 # 更新概念指数下所有股票组成 by 概念代码
 blockingScheduler.add_job(update_one_concept_all_symbol_detail, 'cron', hour='08,18,12', minute='30')
 
 # 同步单只股票下所有概念 by 股票代码
 blockingScheduler.add_job(update_one_symbol_all_concepts, 'cron', hour='09,18,12', minute='15')
```

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.4.2/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.0/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.4.2/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


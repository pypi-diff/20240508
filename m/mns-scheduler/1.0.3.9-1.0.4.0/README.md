# Comparing `tmp/mns-scheduler-1.0.3.9.tar.gz` & `tmp/mns-scheduler-1.0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.3.9.tar", last modified: Sat May  4 10:00:24 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.4.0.tar", last modified: Wed May  8 05:56:59 2024, max compression
```

## Comparing `mns-scheduler-1.0.3.9.tar` & `mns-scheduler-1.0.4.0.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.240760 mns-scheduler-1.0.3.9/
--rw-rw-rw-   0        0        0       62 2024-05-04 10:00:24.239763 mns-scheduler-1.0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.210286 mns-scheduler-1.0.3.9/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.212281 mns-scheduler-1.0.3.9/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.213278 mns-scheduler-1.0.3.9/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.215274 mns-scheduler-1.0.3.9/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.215274 mns-scheduler-1.0.3.9/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.216271 mns-scheduler-1.0.3.9/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.217268 mns-scheduler-1.0.3.9/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.218265 mns-scheduler-1.0.3.9/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.219262 mns-scheduler-1.0.3.9/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2459 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.219262 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.220259 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.222254 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.223251 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.224249 mns-scheduler-1.0.3.9/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.3.9/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.225246 mns-scheduler-1.0.3.9/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.225246 mns-scheduler-1.0.3.9/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.227242 mns-scheduler-1.0.3.9/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.227242 mns-scheduler-1.0.3.9/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.228238 mns-scheduler-1.0.3.9/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.228238 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.229263 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4501 2024-05-04 09:59:40.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.230260 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.231259 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.232255 mns-scheduler-1.0.3.9/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9166 2024-05-04 09:59:40.000000 mns-scheduler-1.0.3.9/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.234223 mns-scheduler-1.0.3.9/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.3.9/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.3.9/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.3.9/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.235267 mns-scheduler-1.0.3.9/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.237769 mns-scheduler-1.0.3.9/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.238766 mns-scheduler-1.0.3.9/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    15508 2024-05-04 09:59:40.000000 mns-scheduler-1.0.3.9/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:00:24.239763 mns-scheduler-1.0.3.9/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-04 10:00:24.000000 mns-scheduler-1.0.3.9/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3247 2024-05-04 10:00:24.000000 mns-scheduler-1.0.3.9/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 10:00:24.000000 mns-scheduler-1.0.3.9/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 10:00:24.000000 mns-scheduler-1.0.3.9/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 10:00:24.240760 mns-scheduler-1.0.3.9/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-04 09:59:40.000000 mns-scheduler-1.0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.453508 mns-scheduler-1.0.4.0/
+-rw-rw-rw-   0        0        0       62 2024-05-08 05:56:59.452511 mns-scheduler-1.0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.415190 mns-scheduler-1.0.4.0/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.417184 mns-scheduler-1.0.4.0/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.418182 mns-scheduler-1.0.4.0/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.420176 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.421174 mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.422171 mns-scheduler-1.0.4.0/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.424166 mns-scheduler-1.0.4.0/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.425163 mns-scheduler-1.0.4.0/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.425163 mns-scheduler-1.0.4.0/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2459 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.426160 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.427157 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.429152 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.431147 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.433143 mns-scheduler-1.0.4.0/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.4.0/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.434512 mns-scheduler-1.0.4.0/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.435033 mns-scheduler-1.0.4.0/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.0/mns_scheduler/finance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.435547 mns-scheduler-1.0.4.0/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.437088 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.438124 mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.438636 mns-scheduler-1.0.4.0/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.439149 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.440191 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-08 05:55:00.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.441240 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.442264 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.444313 mns-scheduler-1.0.4.0/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.446367 mns-scheduler-1.0.4.0/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.0/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.446878 mns-scheduler-1.0.4.0/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.450494 mns-scheduler-1.0.4.0/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.451516 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    15508 2024-05-06 09:12:33.000000 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:56:59.452511 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3281 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 05:56:59.000000 mns-scheduler-1.0.4.0/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 05:56:59.453508 mns-scheduler-1.0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-08 05:56:57.000000 mns-scheduler-1.0.4.0/setup.py
```

### Comparing `mns-scheduler-1.0.3.9/README.md` & `mns-scheduler-1.0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.4.0/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.4.0/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.4.0/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.4.0/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.4.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,18 @@
                                                                          str_day, KPL_MINUTE_BEGIN,
                                                                          end_time)
 
             if data_frame_util.is_empty(kpl_plate_best_index_df):
                 continue
             kpl_plate_best_index_df['number'] = number
             kpl_plate_best_index_df['str_day'] = str_day
+            hour = end_time[0:2]
+            minute = end_time[2:4]
+            str_now_date = str_day + " " + hour + ":" + minute + ":" + "00"
+            kpl_plate_best_index_df['str_now_date'] = str_now_date
             kpl_plate_best_index_df = kpl_plate_best_index_df[[
                 "plate_code",
                 "plate_name",
                 "heat_score",
                 "chg",
                 "speed",
                 "amount",
@@ -74,14 +78,15 @@
                 "super_order_net",
                 "total_mv",
                 "last_reason_organ_add",
                 "ava_pe_now",
                 "ava_pe_next",
                 "number",
                 "str_day",
+                "str_now_date"
 
             ]]
             save_kpl_his_index(kpl_plate_best_index_df, str_day, end_time)
             if end_time == KPL_MINUTE_END:
                 save_kpl_his_daily(kpl_plate_best_index_df, str_day, end_time)
             page_number = page_number + 1
         # 执行下一个时间段
@@ -96,15 +101,15 @@
 
 def save_kpl_his_daily(kpl_plate_best_index_df, str_day, end_time):
     kpl_plate_best_index_df['_id'] = str_day + '-' + end_time + '-' + kpl_plate_best_index_df['plate_code']
     mongodb_util.save_mongo(kpl_plate_best_index_df, db_name_constant.KPL_BEST_CHOOSE_DAILY)
 
 
 def sync_all_days():
-    query = {"_id": {"$gte": '2022-07-22'}, 'trade_date': {"$lte": "2024-04-21"}}
+    query = {"_id": {"$gte": '2024-04-26'}, 'trade_date': {"$lte": "2024-05-07"}}
     trade_date_list = mongodb_util.find_query_data('trade_date_list', query)
     trade_date_list = trade_date_list.sort_values(by=['trade_date'], ascending=False)
     for trade_one in trade_date_list.itertuples():
         sync_best_choose_his_index(trade_one.trade_date)
 
 
 if __name__ == '__main__':
```

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         db_name_constant.REAL_TIME_QUOTES_NOW + '_' + str_day_init, 'number')
     number = number + 1
     realtime_quotes_now_create_db_index_api.create_db_index(str_day_init)
     while True:
         now_date = datetime.datetime.now()
 
         str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
-        if  bool(date_util.is_trade_time(now_date)):
+        if bool(date_util.is_trade_time(now_date)):
             try:
                 real_time_quotes_now = east_money_stock_api.get_real_time_quotes_all_stocks()
                 real_time_quotes_now = handle_init_real_time_quotes_data(real_time_quotes_now.copy(),
                                                                          str_now_date, number)
                 save_real_time_quotes(real_time_quotes_now.copy(), now_date, db_name_constant.REAL_TIME_QUOTES_NOW,
                                       number)
                 try:
```

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.4.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.9/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.4.0/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
 mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
 mns_scheduler/db/__init__.py
 mns_scheduler/db/col_move_service.py
 mns_scheduler/db/db_status.py
 mns_scheduler/dt/__init__.py
 mns_scheduler/dt/stock_dt_pool_sync.py
+mns_scheduler/finance/__init__.py
 mns_scheduler/k_line/__init__.py
 mns_scheduler/k_line/clean/__init__.py
 mns_scheduler/k_line/clean/k_line_info_clean_impl.py
 mns_scheduler/k_line/clean/k_line_info_clean_service.py
 mns_scheduler/k_line/sync/__init__.py
 mns_scheduler/k_line/sync/daily_week_month_line_sync.py
 mns_scheduler/kpl/__init__.py
```


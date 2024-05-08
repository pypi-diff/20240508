# Comparing `tmp/ht_pricing_module-0.3.2.tar.gz` & `tmp/ht_pricing_module-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.3.2.tar", last modified: Mon Jul  3 03:21:10 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.5.1.tar", last modified: Wed May  8 14:23:04 2024, max compression
```

## Comparing `ht_pricing_module-0.3.2.tar` & `ht_pricing_module-0.5.1.tar`

### file list

```diff
@@ -1,122 +1,144 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.157312 ht_pricing_module-0.3.2/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      263 2023-07-03 03:21:10.157312 ht_pricing_module-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-06-30 08:43:11.000000 ht_pricing_module-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.518819 ht_pricing_module-0.3.2/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.3.2/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.543751 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      293 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      558 2023-06-13 01:59:48.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.555719 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.505852 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.581715 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.600665 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    48559 2023-06-29 01:54:18.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3707 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.649533 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0      234 2023-06-27 10:54:41.000000 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     2070 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/crank_nicolson_american.py
--rw-rw-rw-   0        0        0     1007 2023-06-16 01:16:24.000000 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/crank_nicolson_european.py
--rw-rw-rw-   0        0        0     8093 2023-07-03 03:18:02.000000 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py
--rw-rw-rw-   0        0        0     5329 2023-06-27 10:17:12.000000 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
--rw-rw-rw-   0        0        0      693 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/fully_explicit_european.py
--rw-rw-rw-   0        0        0      736 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/fully_implicit_european.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.664493 ht_pricing_module-0.3.2/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-06-19 06:14:01.000000 ht_pricing_module-0.3.2/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.676461 ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.683521 ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.698481 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.847140 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5561 2023-06-07 10:16:58.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
--rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.857113 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.889028 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.964825 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-06-27 02:32:08.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     2393 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py
--rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     2263 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py
--rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     2963 2023-06-26 13:12:34.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py
--rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
--rw-rw-rw-   0        0        0     3503 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.985770 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.024666 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.034639 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     5693 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.046607 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
--rw-rw-rw-   0        0        0     3902 2023-06-05 06:56:38.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.076526 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0      194 2023-06-27 11:31:24.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     5753 2023-06-28 02:47:53.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
--rw-rw-rw-   0        0        0     5077 2023-06-30 11:34:56.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py
--rw-rw-rw-   0        0        0     6870 2023-06-30 09:22:09.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
--rw-rw-rw-   0        0        0     6932 2023-06-30 11:34:43.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py
--rw-rw-rw-   0        0        0     4852 2023-06-29 13:27:41.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.093482 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.138361 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-06-27 02:30:19.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     3801 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py
--rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     3157 2023-06-26 01:22:55.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:10.145357 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-06-13 02:30:48.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    45943 2023-06-28 09:02:37.000000 ht_pricing_module-0.3.2/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:21:09.531783 ht_pricing_module-0.3.2/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-03 03:21:09.000000 ht_pricing_module-0.3.2/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6098 2023-07-03 03:21:09.000000 ht_pricing_module-0.3.2/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 03:21:09.000000 ht_pricing_module-0.3.2/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-03 03:21:09.000000 ht_pricing_module-0.3.2/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-03 03:21:09.000000 ht_pricing_module-0.3.2/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 03:21:10.157312 ht_pricing_module-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1158 2023-07-03 03:21:01.000000 ht_pricing_module-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.271870 ht_pricing_module-0.5.1/
+-rw-rw-rw-   0        0        0       66 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      469 2024-05-08 14:23:04.271870 ht_pricing_module-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.163302 ht_pricing_module-0.5.1/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.174311 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      293 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      753 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      801 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.176707 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.147145 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.178958 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.180966 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    60135 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3741 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.188966 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0      380 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     2071 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_crank_nicolson_american.py
+-rw-rw-rw-   0        0        0     1008 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_crank_nicolson_european.py
+-rw-rw-rw-   0        0        0      689 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_explicit_european.py
+-rw-rw-rw-   0        0        0     5747 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_fd_generator.py
+-rw-rw-rw-   0        0        0     8845 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_fd_generator_parisian_snowball.py
+-rw-rw-rw-   0        0        0     8726 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_fd_generator_snowball.py
+-rw-rw-rw-   0        0        0      732 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_implicit_european.py
+-rw-rw-rw-   0        0        0    14035 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/two_asset_fd_generator_snowball.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.190966 ht_pricing_module-0.5.1/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.192966 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0      156 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.193993 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0       49 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     2229 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/basket/two_asset_basket_as.py
+-rw-rw-rw-   0        0        0     7088 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.197073 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       53 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1547 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/quotient/two_asset_quotient_as.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.201071 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/rainbow/
+-rw-rw-rw-   0        0        0      216 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/rainbow/__init__.py
+-rw-rw-rw-   0        0        0     4664 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/rainbow/three_asset_best_of_as.py
+-rw-rw-rw-   0        0        0     4669 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/rainbow/three_asset_worst_of_as.py
+-rw-rw-rw-   0        0        0     2182 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/rainbow/two_asset_better_of_as.py
+-rw-rw-rw-   0        0        0     2177 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/rainbow/two_asset_worse_of_as.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.203093 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0       57 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     8130 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/snowball/two_asset_snowball_pde.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.206574 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      341 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.221576 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      794 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     3306 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/basket_fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4056 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/basket_fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     3333 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/basket_linear_acc_as.py
+-rw-rw-rw-   0        0        0     4344 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3341 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4124 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     4864 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4211 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     6927 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_fusing_as.py
+-rw-rw-rw-   0        0        0     4271 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3368 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4238 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4318 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5818 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+-rw-rw-rw-   0        0        0     6121 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_close_settle_as.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.222574 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     5120 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.228964 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      232 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3651 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2280 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+-rw-rw-rw-   0        0        0     2780 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/enhanced_asian_as.py
+-rw-rw-rw-   0        0        0     3619 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/enhanced_asian_spread_as.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.237966 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      488 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     6174 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5339 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4870 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/basket_barrier_as.py
+-rw-rw-rw-   0        0        0     4715 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/basket_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1780 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/basket_discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1805 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/basket_discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1982 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1903 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4425 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.240966 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1021 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2316 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.244972 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      166 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0      820 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/basket_binary_as.py
+-rw-rw-rw-   0        0        0     2964 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2320 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2261 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.247054 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     6373 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.252059 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0      128 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2470 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/basket_sharkfin_as.py
+-rw-rw-rw-   0        0        0     2526 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2348 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     2772 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.259374 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0      352 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     7273 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/parisian_snowball_mc.py
+-rw-rw-rw-   0        0        0     6730 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/parisian_snowball_pde.py
+-rw-rw-rw-   0        0        0     5878 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
+-rw-rw-rw-   0        0        0     4855 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py
+-rw-rw-rw-   0        0        0     6995 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+-rw-rw-rw-   0        0        0     6180 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py
+-rw-rw-rw-   0        0        0     3463 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_small_mc.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.262863 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1481 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2414 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.266864 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     1762 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     5949 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.269864 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2278 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    56553 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:23:04.270863 ht_pricing_module-0.5.1/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-05-08 14:23:04.000000 ht_pricing_module-0.5.1/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7571 2024-05-08 14:23:04.000000 ht_pricing_module-0.5.1/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 14:23:04.000000 ht_pricing_module-0.5.1/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-08 14:23:04.000000 ht_pricing_module-0.5.1/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 14:23:04.000000 ht_pricing_module-0.5.1/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 14:23:04.272863 ht_pricing_module-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2024-05-08 13:38:59.000000 ht_pricing_module-0.5.1/setup.py
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
 # 'PAH', 'PAE'
 RebateType = protos_pricer.RebateType
 
 # 'AS', 'MC', 'PDE'
 PricingMethod = protos_pricer.PricingMethod
 
-# 'LINEAR_ACC', 'FIXED_ACC', 'FIXED_ACC_AKO', 'FIXED_ACC_BARRIER', 'LINEAR_ACC_ENHANCED', 'FIXED_ACC_ENHANCED', 'LINEAR_ACC_AKO'
+# 'LINEAR_ACC', 'FIXED_ACC', 'FIXED_ACC_AKO', 'FIXED_ACC_BARRIER', 'LINEAR_ACC_ENHANCED', 'FIXED_ACC_ENHANCED', 'LINEAR_ACC_AKO', 'LINEAR_ACC_FUSING_CLOSE_SETTLE'
 AccumulatorType = protos_pricer.AccumulatorType
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,19 @@
     FIXED_ACC_BARRIER                   = 4;
     LINEAR_ACC_ENHANCED                 = 5;
     FIXED_ACC_ENHANCED                  = 6;
     LINEAR_ACC_AKO                      = 7;
     FIXED_ACC_BARRIER_ENHANCED          = 8;
     LINEAR_ACC_FIXED_ENHANCED           = 9;
     LINEAR_ACC_FUSING                   = 10;
+    FIXED_ACC_FUSING                    = 11;
+    LINEAR_ACC_FUSING_CLOSE_SETTLE      = 12;
+    BASKET_LINEAR_ACC                   = 13;
+    BASKET_FIXED_ACC                    = 14;
+    BASKET_FIXED_ACC_BARRIER            = 15;
 }
 
 enum PriceType {
     UNKNOWN_PRICE_TYPE                  = 0;
     VALUE                               = 1;
     DELTA                               = 2;
     GAMMA                               = 3;
@@ -143,14 +148,27 @@
     DISCRETE_BINARY_MC                  = 34;
     LINEAR_ACC_FUSING_AS                = 35;
 
     QUOTIENT_AS                         = 36;
     SNOWBALL_DISCOUNTED_MC              = 37;
     SNOWBALL_PDE                        = 38;
     SNOWBALL_DISCOUNTED_PDE             = 39;
+
+    ENHANCED_ASIAN_AS                   = 40;
+    ENHANCED_ASIAN_SPREAD_AS            = 41;
+
+    FIXED_ACC_FUSING_AS                 = 42;
+
+    BASKET_BARRIER_AS                   = 43;
+    BASKET_DISCRETE_BARRIER_AS          = 44;
+    LINEAR_ACC_FUSING_CLOSE_SETTLE_AS   = 45;
+
+    BASKET_LINEAR_ACC_AS                = 46;
+    BASKET_FIXED_ACC_AS                 = 47;
+    SNOWBALL_SMALL_MC                   = 48;
 }
 
 message PricerReply {
     PriceType price_type                = 1;
     double result                       = 2;
 }
 
@@ -258,14 +276,67 @@
     double obs_freq                     = 14;
     double base_quantity                = 15;
     double final_position_multiplier    = 16;
     repeated PayoffObservation obs_date = 17; // 观察日序列
 
 }
 
+message LinearAccFusingCloseSettleRequest {
+    PriceType price_type                 = 1;
+    LinearAccFusingCloseSettle param     = 2;
+}
+
+message LinearAccFusingCloseSettle {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3;
+    double strike_price                 = 4;
+    int32 expiry_date                   = 5;
+    double current_date                 = 6;
+    double volatility                   = 7;
+    double riskfree_rate                = 8;
+    double dividend                     = 9;
+    double leverage                     = 10;
+    int32 year_base                     = 11;
+    double payoff                       = 12;
+    double barrier_price                = 13;
+    double obs_freq                     = 14;
+    double base_quantity                = 15;
+    double final_position_multiplier    = 16;
+    repeated PayoffObservation obs_date = 17; // 观察日序列
+
+}
+
+message FixedAccFusingRequest {
+    PriceType price_type                 = 1;
+    FixedAccFusing param                 = 2;
+}
+
+message FixedAccFusing {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3;
+    double strike_price                 = 4;
+    int32 expiry_date                   = 5;
+    double current_date                 = 6;
+    double volatility                   = 7;
+    double riskfree_rate                = 8;
+    double dividend                     = 9;
+    double leverage                     = 10;
+    int32 year_base                     = 11;
+    double payoff                       = 12;   // 区间固定赔付
+    double rebate                       = 13;   // 敲出固定赔付
+    double barrier_price                = 14;
+    double obs_freq                     = 15;
+    double base_quantity                = 16;
+    double final_position_multiplier    = 17;
+    repeated PayoffObservation obs_date = 18; // 观察日序列
+
+}
+
 message FixedAccRequest {
     PriceType price_type                = 1;
     FixedAcc param                      = 2;
 }
 
 message FixedAcc {
     OptionType option_type              = 1; // 期权类型
@@ -280,14 +351,36 @@
     double leverage                     = 10;
     int32 year_base                     = 11;
     double payoff                       = 12;
     repeated PayoffObservation obs_date = 13; // 观察日序列
 
 }
 
+message BasketFixedAccRequest {
+    PriceType price_type                = 1;
+    BasketFixedAcc param                      = 2;
+}
+
+message BasketFixedAcc {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3;
+    double strike_price                 = 4;
+    int32 expiry_date                   = 5;
+    double current_date                 = 6;
+    double volatility                   = 7;
+    double riskfree_rate                = 8;
+    double dividend                     = 9;
+    double leverage                     = 10;
+    int32 year_base                     = 11;
+    double payoff                       = 12;
+    repeated PayoffObservation obs_date = 13; // 观察日序列
+
+}
+
 message FixedAccBarrierRequest {
     PriceType price_type                = 1;
     FixedAccBarrier param               = 2;
 }
 
 message FixedAccBarrier {
     OptionType option_type              = 1; // 期权类型
@@ -348,14 +441,36 @@
     double leverage                     = 10;
     int32 year_base                     = 11;
     double barrier_price                = 12;
     repeated PayoffObservation obs_date = 13; // 观察日序列
 
 }
 
+message BasketLinearAccRequest {
+    PriceType price_type                = 1;
+    BasketLinearAcc param                     = 2;
+}
+
+message BasketLinearAcc {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3;
+    double strike_price                 = 4;
+    int32 expiry_date                   = 5;
+    double current_date                 = 6;
+    double volatility                   = 7;
+    double riskfree_rate                = 8;
+    double dividend                     = 9;
+    double leverage                     = 10;
+    int32 year_base                     = 11;
+    double barrier_price                = 12;
+    repeated PayoffObservation obs_date = 13; // 观察日序列
+
+}
+
 message LinearAccEnhancedRequest {
     PriceType price_type                = 1;
     LinearAccEnhanced param             = 2;
 }
 
 message LinearAccEnhanced {
     OptionType option_type              = 1; // 期权类型
@@ -372,15 +487,15 @@
     double barrier_price                = 12;
     repeated PayoffObservation obs_date = 13; // 观察日序列
 
 }
 
 message FixedAccEnhancedRequest {
     PriceType price_type                = 1;
-    FixedAccEnhanced param             = 2;
+    FixedAccEnhanced param              = 2;
 }
 
 message FixedAccEnhanced {
     OptionType option_type              = 1; // 期权类型
     ExerciseType exercise_type          = 2; // 行权类型
     double spot_price                   = 3;
     double strike_price                 = 4;
@@ -551,14 +666,38 @@
     double barrier_price                = 11;// 障碍价
     BarrierType barrier_type            = 12;// 障碍方向
     KnockType knock_type                = 13;// 敲击类型
     int32 is_knock_in                   = 14;// 是否触发
     double payoff                       = 15;
 }
 
+// BASKET_BARRIER
+message BasketBarrierRequest {
+    PriceType price_type                = 1;
+    BasketBarrier param                 = 2;
+}
+
+message BasketBarrier {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3; // 当前标的价
+    double strike_price                 = 4; // 执行价
+    int32 expiry_date                   = 5; // 到期日离开仓日天数
+    double current_date                 = 6; // 当前日离开仓日天数
+    double volatility                   = 7; // 波动率
+    double riskfree_rate                = 8; // 无风险利率
+    double dividend                     = 9; // 分红率
+    int32 year_base                     = 10;// 年基数
+    double barrier_price                = 11;// 障碍价
+    BarrierType barrier_type            = 12;// 障碍方向
+    KnockType knock_type                = 13;// 敲击类型
+    int32 is_knock_in                   = 14;// 是否触发
+    double rebate                       = 15;// 赔付
+}
+
 message DiscreteBarrierBinaryRequest {
     PriceType price_type                = 1;
     DiscreteBarrierBinary param         = 2;
 }
 
 message DiscreteBarrierBinary {
     OptionType option_type              = 1; // 期权类型
@@ -573,14 +712,15 @@
     int32 year_base                     = 10;// 年基数
     double barrier_price                = 11;// 障碍价
     BarrierType barrier_type            = 12;// 障碍方向
     KnockType knock_type                = 13;// 敲击类型
     int32 is_knock_in                   = 14;// 是否触发
     double payoff                       = 15;
     double obs_freq                     = 16;
+    double adjust_barrier_price         = 17;
 
 }
 
 message DiscreteBarrierRequest {
     PriceType price_type                = 1;
     DiscreteBarrier param               = 2;
 }
@@ -598,14 +738,39 @@
     int32 year_base                     = 10;// 年基数
     double barrier_price                = 11;// 障碍价
     BarrierType barrier_type            = 12;// 障碍方向
     KnockType knock_type                = 13;// 敲击类型
     int32 is_knock_in                   = 14;// 是否触发
     double rebate                       = 15;// 赔付
     double obs_freq                     = 16;//观察频率
+    double adjust_barrier_price         = 17;
+}
+
+message BasketDiscreteBarrierRequest {
+    PriceType price_type                = 1;
+    BasketDiscreteBarrier param               = 2;
+}
+
+message BasketDiscreteBarrier {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3; // 当前标的价
+    double strike_price                 = 4; // 执行价
+    int32 expiry_date                   = 5; // 到期日离开仓日天数
+    double current_date                 = 6; // 当前日离开仓日天数
+    double volatility                   = 7; // 波动率
+    double riskfree_rate                = 8; // 无风险利率
+    double dividend                     = 9; // 分红率
+    int32 year_base                     = 10;// 年基数
+    double barrier_price                = 11;// 障碍价
+    BarrierType barrier_type            = 12;// 障碍方向
+    KnockType knock_type                = 13;// 敲击类型
+    int32 is_knock_in                   = 14;// 是否触发
+    double rebate                       = 15;// 赔付
+    double obs_freq                     = 16;//观察频率
 }
 
 message DiscreteBarrierMcRequest {
     PriceType price_type                = 1;
     DiscreteBarrierMc param             = 2;
 }
 
@@ -645,15 +810,15 @@
     double riskfree_rate                = 8; // 无风险利率
     double dividend                     = 9; // 分红率
     int32 year_base                     = 10;
 }
 
 message BasketVanillaSeriesRequest {
     PriceType price_type                = 1;
-    BasketVanillaSeries param                 = 2;
+    BasketVanillaSeries param           = 2;
 }
 
 message BasketVanillaSeries {
     OptionType option_type              = 1; // 期权类型
     ExerciseType exercise_type          = 2; // 行权类型
     double spot_price                   = 3; // 当前标的价
     double strike_price                 = 4; // 执行价
@@ -807,15 +972,15 @@
     double participation_rate                       = 19;
     double knock_in_strike_price                    = 20;
 }
 
 // SNOWBALL_DISCOUNTED
 message SnowballDiscountedRequest {
     PriceType price_type                = 1;
-    SnowballDiscounted param          = 2;
+    SnowballDiscounted param            = 2;
 }
 
 message SnowballDiscounted {
     double notional                                 = 1; // 单位数量名义金额
     double spot_price                               = 2; // 当前价
     double entrance_price                           = 3; // 入场价
     double knock_in_barrier_price                   = 4; // 敲入价
@@ -832,14 +997,34 @@
     double dividend                                 = 15; // 分红率
     int32 year_base                                 = 16;
     repeated KnockObservation knock_in_obs_date     = 17; // 敲入观察序列
     repeated KnockObservation knock_out_obs_date    = 18; // 敲出观察序列
     double knock_in_strike_price                    = 19;
 }
 
+// SNOWBALL_SMALL
+message SnowballSmallRequest {
+    PriceType price_type                = 1;
+    SnowballSmall param                 = 2;
+}
+
+message SnowballSmall {
+    double notional                                 = 1; // 单位数量名义金额
+    double spot_price                               = 2; // 当前价
+    double knock_out_barrier_price                  = 5; // 敲出价
+    int32 expiry_date                               = 6; // 到日期
+    OptionType option_type                          = 10; // 正向反向雪球方向
+    double current_date                             = 12; // 当前日离开仓日天数
+    double volatility                               = 13; // 波动率
+    double riskfree_rate                            = 14; // 无风险利率
+    double dividend                                 = 15; // 分红率
+    int32 year_base                                 = 16;
+    repeated KnockObservation knock_out_obs_date    = 18; // 敲出观察序列
+}
+
 // RATIO SPREAD
 message RatioSpreadRequest {
     PriceType price_type                = 1;
     RatioSpread param                   = 2;
 }
 
 message RatioSpread {
@@ -914,14 +1099,15 @@
     double barrier_price                = 8;// 障碍价
     BarrierType barrier_type            = 9;// 障碍方向
     KnockType knock_type                = 10;// 敲击类型
     int32 is_knock_in                   = 11;// 是否触发
     double rebate                       = 12;// 赔付
     RebateType rebate_type              = 13;
     double obs_freq                     = 14;
+    double adjust_barrier_price         = 15;
 }
 
 message DoubleOneTouchRequest {
     PriceType price_type                = 1;
     DoubleOneTouch param                = 2;
 }
 
@@ -975,18 +1161,59 @@
     double volatility                   = 7; // 波动率
     double riskfree_rate                = 8; // 无风险利率
     double dividend                     = 9; // 分红率
     repeated PayoffObservation obs_date = 10; // 观察日序列
     int32 year_base                     = 11;
 }
 
+message EnhancedAsianSpreadRequest {
+    PriceType price_type                = 1;
+    EnhancedAsianSpread param           = 2;
+}
+
+message EnhancedAsianSpread {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3; // 当前标的价
+    double strike_price                 = 4; // 执行价
+    double enhanced_strike_price1       = 5; // 增强执行价1
+    double enhanced_strike_price2       = 6; // 增强执行价2
+    int32 expiry_date                   = 7; // 到期日离开仓日天数
+    double current_date                 = 8; // 当前日离开仓日天数
+    double volatility                   = 9; // 波动率
+    double riskfree_rate                = 10; //无风险利率
+    double dividend                     = 11; //分红率
+    int32 year_base                     = 12;
+    repeated PayoffObservation obs_date = 13; // 观察日序列
+}
+
+message EnhancedAsianRequest {
+    PriceType price_type                = 1;
+    EnhancedAsian param                 = 2;
+}
+
+message EnhancedAsian {
+    OptionType option_type              = 1; // 期权类型
+    ExerciseType exercise_type          = 2; // 行权类型
+    double spot_price                   = 3; // 当前标的价
+    double strike_price                 = 4; // 执行价
+    double enhanced_strike_price        = 5; // 增强执行价
+    int32 expiry_date                   = 6; // 到期日离开仓日天数
+    double current_date                 = 7; // 当前日离开仓日天数
+    double volatility                   = 8; // 波动率
+    double riskfree_rate                = 9; //无风险利率
+    double dividend                     = 10; //分红率
+    int32 year_base                     = 11;
+    repeated PayoffObservation obs_date = 12; // 观察日序列
+}
+
 // QUOTIENT
 message QuotientRequest {
     PriceType price_type                = 1;
-    Quotient param                       = 2;
+    Quotient param                      = 2;
 }
 
 message Quotient {
     OptionType option_type              = 1; // 期权类型
     ExerciseType exercise_type          = 2; // 行权类型
     double spot_price1                  = 3; // 当前标的价1
     double spot_price2                  = 4; // 当前标的价2
@@ -1006,15 +1233,16 @@
     int32 obs_index                     = 1; // 观察日离开仓日天数
     double obs_price                    = 2; // 观察价
 }
 
 message KnockObservation {
     int32 obs_index                     = 1; // 观察日离开仓日天数
     double adjust_rate                  = 2; // 观察日调整比率
-    double coupon_rate                  = 3; // 绝对票息率
+    double coupon_rate                  = 3; // 绝对敲出票息率
+    double swap_rate                    = 4; // 绝对互换票息率
 }
 
 service PricerService {
     rpc batchPricer (BatchPricerRequest) returns (BatchPricerReply) {
         option (google.api.http) = {
             post: "/pricer/batch_pricer"
         };
@@ -1040,20 +1268,38 @@
 
     rpc linearAccFusing (LinearAccFusingRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/linear_acc_fusing_as"
         };
     };
 
+    rpc linearAccFusingCloseSettle (LinearAccFusingCloseSettleRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/linear_acc_fusing_close_settle_as"
+        };
+    };
+
+    rpc fixedAccFusing (FixedAccFusingRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/fixed_acc_fusing_as"
+        };
+    };
+
     rpc fixedAcc (FixedAccRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/fixed_acc_as"
         };
     };
 
+    rpc basketFixedAcc (BasketFixedAccRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/basket_fixed_acc_as"
+        };
+    };
+
     rpc fixedAccEnhanced (FixedAccEnhancedRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/fixed_acc_enhanced_as"
         };
     };
 
     rpc fixedAccBarrier (FixedAccBarrierRequest) returns (PricerReply) {
@@ -1070,14 +1316,20 @@
 
     rpc linearAcc (LinearAccRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/linear_acc_as"
         };
     };
 
+    rpc basketLinearAcc (BasketLinearAccRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/basket_linear_acc_as"
+        };
+    };
+
     rpc linearAccEnhanced (LinearAccEnhancedRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/linear_acc_enhanced_as"
         };
     };
 
     rpc linearAccFixedEnhanced (LinearAccFixedEnhancedRequest) returns (PricerReply) {
@@ -1190,20 +1442,26 @@
 
     rpc snowball (SnowballRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/snowball"
         };
     };
 
-        rpc snowballDiscounted (SnowballDiscountedRequest) returns (PricerReply) {
+    rpc snowballDiscounted (SnowballDiscountedRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/snowball_discounted"
         };
     };
 
+    rpc snowballSmall (SnowballSmallRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/snowball_small"
+        };
+    };
+
     rpc ratioSpread (RatioSpreadRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/ratio_spread_as"
         };
     };
 
     rpc ratioSpreadSeries (RatioSpreadSeriesRequest) returns (PricerReply) {
@@ -1238,14 +1496,37 @@
 
     rpc vanillaSeries (VanillaSeriesRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/vanilla_series"
         };
     };
 
+    rpc enhancedAsianSpread (EnhancedAsianSpread) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/enhanced_asian_spread_as"
+        };
+    };
+
+    rpc enhancedAsian (EnhancedAsian) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/enhanced_asian_as"
+        };
+    };
+
+    rpc basketBarrier (BasketBarrierRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/basket_barrier_as"
+        };
+    };
+
+    rpc basketDiscreteBarrier (BasketDiscreteBarrierRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/basket_discrete_barrier_as"
+        };
+    };
+
     rpc quotient (QuotientRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/quotient_as"
         };
     };
 }
-
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.5.1/ht_pricing_module/api_and_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 setattr(struct, k, input[k][i])
             output.append(struct)
         return output
 
 
 class ParamsBase:
     def __init__(self, param):
-        self.param = Struct(param) if isinstance(param, dict) else param
+        self.param = Struct(param) if isinstance(param, dict) and not isinstance(param, Struct) else param
 
 
 def BlackScholesVectorize(S, K, r, q, v, T, t, cp):
     if T - t <= 0 or v == 0:
         return np.maximum(cp * (S - K), 0)
     d1 = (np.log(S / K) + (r - q + v * v / 2) * (T - t)) / (v * np.sqrt(T - t))
     d2 = d1 - v * np.sqrt(T - t)
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/crank_nicolson_american.py` & `ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_crank_nicolson_american.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .fd_grid_generator import FiniteDifference, trigger
+from .one_asset_fd_generator import OneAssetFD, trigger
 from ..api_and_utils import np, tqdm, sp
 
 
-class CrankNicolsonAmerican(FiniteDifference):
+class OneAssetCrankNicolsonAmerican(OneAssetFD):
 
     _theta = 0.5
     _alpha = 0.8
     _epsilon = 1e-6
     _max_iter = 1e4
 
     def _set_matrix_(self):
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/crank_nicolson_european.py` & `ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_crank_nicolson_european.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .fd_grid_generator import FiniteDifference
+from .one_asset_fd_generator import OneAssetFD
 from ..api_and_utils import np, tqdm, sp
 
 
-class CrankNicolsonEuropean(FiniteDifference):
+class OneAssetCrankNicolsonEuropean(OneAssetFD):
     _theta = 0.5
 
     def _set_matrix_(self):
         self._A = sp.diags([self._l[1:], self._c, self._u[:-1]], [-1, 0, 1], format='csc').toarray()
         self._I = sp.eye(self.Ns - 1).toarray()
         self._M1 = self._I + (1 - self._theta) * self.dt * self._A
         self._M2 = self._I - self._theta * self.dt * self._A
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py` & `ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_fd_generator_parisian_snowball.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .fd_grid_generator import interpolate
+from .one_asset_fd_generator import interpolate
 from ..api_and_utils import np, deepcopy, sp, ParamsBase, OptionType
 
 
-class CrankNicolsonSnowball(ParamsBase):
+class OneAssetFDParisianSnowball(ParamsBase):
 
-    def __init__(self, param, Ns=None, theta=1):
+    def __init__(self, param, Ns=None):
         super().__init__(param)
 
         self.Smin = 0 * min(self.param.spot_price, self.param.entrance_price)
         self.Smax = 3 * max(self.param.spot_price, self.param.entrance_price)
 
         self._T0 = round(self.param.current_date, 4)
         self._TT = round(self.param.expiry_date, 4)
@@ -16,16 +16,15 @@
         self._Nt = int(round(self._TT - int(self._T0), 4))
 
         self._Tau = round(self._T0 - int(self._T0), 4)
         self._T_KO = np.array([round(obs.obs_index - int(self._T0), 4) for obs in self.param.knock_out_obs_date])
         self._T_KI = np.array([round(obs.obs_index - int(self._T0), 4) for obs in self.param.knock_in_obs_date])
         self._Rbt_KO = np.array([obs.coupon_rate for obs in self.param.knock_out_obs_date])
 
-        self._theta = theta
-        self.__grid = 'KIgrid' if self.param.is_knock_in else 'NKIgrid'
+        self.__grid = 'KIgrid2nd' if self.param.is_knock_in or self.param.knock_in_times >= 2 else 'KIgrid1st' if self.param.knock_in_times == 1 else 'NKIgrid'
         self.__round = 8
 
         self.__present_value_solved = False
         self.__greeks_solved = False
 
     def _set_direction_(self):
         self._is_call = {OptionType.STANDARD: True, OptionType.REVERSE: False}[self.param.option_type]
@@ -34,18 +33,25 @@
     def _set_spot_vector_(self):
         self.ds = (self.Smax - self.Smin) / max(1, self._Ns)
         self.Svec = np.linspace(self.Smin, self.Smax, self._Ns + 1)
 
     def _set_term_vector_(self):
         self.dt = round(self._TT - int(self._T0), 4) / max(1, self._Nt)
         self.Tvec = np.linspace(0, round(self._TT - int(self._T0), 4), self._Nt + 1)
+        self.Tauvec = self.Tvec.copy()
+        self.Tauvec[1:] = self.Tauvec[1:] - self._Tau
 
     def _set_value_grid_(self):
+        self.KIgrid1st = np.zeros(shape=(self._Ns + 1, self._Nt + 1))
+        self.KIgrid2nd = np.zeros(shape=(self._Ns + 1, self._Nt + 1))
         self.NKIgrid = np.zeros(shape=(self._Ns + 1, self._Nt + 1))
-        self.KIgrid = np.zeros(shape=(self._Ns + 1, self._Nt + 1))
+
+        self.T1KIgrid1st = None
+        self.T1KIgrid2nd = None
+        self.T1NKIgrid = None
 
     def _set_other_vector_(self):
         pass
 
     def _set_initial_vector_grid_(self):
         self._set_direction_()
         self._set_spot_vector_()
@@ -64,18 +70,17 @@
         diffusion_square = (self.param.volatility * self.Svec[1: -1] / self.ds) ** 2
 
         self._l = 0.5 * (diffusion_square - drift)
         self._c = -diffusion_square - self.param.riskfree_rate
         self._u = 0.5 * (diffusion_square + drift)
 
     def _set_matrix_(self):
-        self._A = sp.diags([self._l[1:], self._c, self._u[:-1]], [-1, 0, 1], format='csc').toarray()
-        self._I = sp.eye(self._Ns - 1).toarray()
-        self._M1 = self._I + (1 - self._theta) * self.dt / self.param.year_base * self._A
-        self._M2 = self._I - self._theta * self.dt / self.param.year_base * self._A
+        self._A = sp.diags([self._l[1:], self._c, self._u[:-1]], [-1, 0, 1], format='csc')
+        self._M1 = sp.eye(self._Ns - 1)
+        self._M2 = self._M1 - self.dt / self.param.year_base * self._A
 
     def _solve_(self):
         pass
 
     def _set_grid_delta_(self, grid: str):
         grid = getattr(self, grid)
         grid_delta = np.zeros(shape=(grid.shape[0], grid.shape[1]))
@@ -89,48 +94,53 @@
         grid = getattr(self, grid)
         grid_gamma = np.zeros(shape=(grid.shape[0], grid.shape[1]))
         grid_gamma[1: -1] = (grid[2:] - grid[:-2]) / (2 * self.ds)
         grid_gamma[0] = (grid[1] - grid[0]) / self.ds
         grid_gamma[-1] = (grid[-1] - grid[-2]) / self.ds
         return grid_gamma
 
-    def _set_grid_theta_(self, grid: str, dt: float = 1):
-        grid = getattr(self, grid)
-        T_idx = np.abs(self.Tvec - dt).argmin()
-        grid_theta = (grid[:, T_idx:] - grid[:, :self._Nt - T_idx + 1]) / (dt - self._Tau)
-        return grid_theta
+    def _set_grid_theta_(self, grid: str):
+        T0grid = getattr(self, grid)
+        T1grid = getattr(self, f'T1{grid}')
+        return T1grid - T0grid[:, :max(1, self._Nt)]
 
     def _set_grid_vega_(self, grid: str, dv: float = 0.01):
         pricer_up = deepcopy(self)
         pricer_up.param.volatility = self.param.volatility + dv
         pricer_up.price()
-        grid_vega = getattr(pricer_up, grid) - getattr(self, grid)
-        return grid_vega
+        return getattr(pricer_up, grid) - getattr(self, grid)
+
+    def _set_grid_phi_(self, grid: str, dq: float = 0.001):
+        pricer_up = deepcopy(self)
+        pricer_up.param.dividend = self.param.dividend + dq
+        pricer_up.price()
+        return getattr(pricer_up, grid) - getattr(self, grid)
 
     def _set_grid_rho_(self, grid: str, dr: float = 0.0001):
         pricer_up = deepcopy(self)
         pricer_up.param.riskfree_rate = self.param.riskfree_rate + dr
         pricer_up.price()
-        grid_rho = getattr(pricer_up, grid) - getattr(self, grid)
-        return grid_rho
+        return getattr(pricer_up, grid) - getattr(self, grid)
 
-    def _set_grid_ddeltadt_(self, grid: str, dt: float = 1):
-        grid = getattr(self, grid)
-        T_idx = np.abs(self.Tvec - dt).argmin()
-        grid_ddeltadt = (grid[:, T_idx:] - grid[:, :self._Nt - T_idx + 1]) / (dt - self._Tau)
-        return grid_ddeltadt
+    def _set_grid_ddeltadt_(self, grid: str):
+        T0grid = getattr(self, grid)
+        T1grid = getattr(self, f'T1{grid}')
+        return T1grid - T0grid[:, :max(1, self._Nt)]
 
-    def _set_grid_greeks_(self, grid, include_vega, include_rho):
+    def _set_grid_greeks_(self, grid, include_vega, include_phi, include_rho):
         setattr(self, f'{grid}_delta', self._set_grid_delta_(grid))
+        setattr(self, f'T1{grid}_delta', self._set_grid_delta_(f'T1{grid}'))
         setattr(self, f'{grid}_gamma', self._set_grid_gamma_(f'{grid}_delta'))
         setattr(self, f'{grid}_theta', self._set_grid_theta_(grid))
         setattr(self, f'{grid}_ddeltadt', self._set_grid_ddeltadt_(f'{grid}_delta'))
 
         if include_vega:
             setattr(self, f'{grid}_vega', self._set_grid_vega_(grid))
+        if include_phi:
+            setattr(self, f'{grid}_phi', self._set_grid_phi_(grid))
         if include_rho:
             setattr(self, f'{grid}_rho', self._set_grid_rho_(grid))
 
     def _check_present_value_solved_(self):
         if not self.__present_value_solved:
             self.price()
 
@@ -144,16 +154,17 @@
         self._set_terminal_condition_()
         self._set_boundary_condition_()
         self._set_coefficient_()
         self._set_matrix_()
         self._solve_()
         self.__present_value_solved = True
 
-    def greeks(self, include_vega=True, include_rho=False):
-        self._set_grid_greeks_(grid=self.__grid, include_vega=include_vega, include_rho=include_rho)
+    def greeks(self, include_vega=True, include_phi=False, include_rho=False):
+        self._check_present_value_solved_()
+        self._set_grid_greeks_(grid=self.__grid, include_vega=include_vega, include_phi=include_phi, include_rho=include_rho)
         self.__greeks_solved = True
 
     def present_value(self, S=None):
         self._check_present_value_solved_()
         S = self.param.spot_price if S is None else S
         grid = getattr(self, self.__grid)
         return interpolate(x=self.Svec, y=grid[:, 0])(S).round(self.__round)
@@ -178,14 +189,20 @@
 
     def vega(self, S=None):
         self._check_greeks_solved_()
         S = self.param.spot_price if S is None else S
         grid = getattr(self, f'{self.__grid}_vega')
         return interpolate(x=self.Svec, y=grid[:, 0])(S).round(self.__round)
 
+    def phi(self, S=None):
+        self._check_greeks_solved_()
+        S = self.param.spot_price if S is None else S
+        grid = getattr(self, f'{self.__grid}_phi')
+        return interpolate(x=self.Svec, y=grid[:, 0])(S).round(self.__round)
+
     def rho(self, S=None):
         self._check_greeks_solved_()
         S = self.param.spot_price if S is None else S
         grid = getattr(self, f'{self.__grid}_rho')
         return interpolate(x=self.Svec, y=grid[:, 0])(S).round(self.__round)
 
     def ddeltadt(self, S=None):
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_fd_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,39 +12,42 @@
         noBreak = 0
     elif counter > maxIteration:
         print('结果可能不收敛')
         noBreak = 0
     return noBreak
 
 
-class OptionPricingMethod:
+class OneAssetOption:
 
     def __init__(self, S, K, r, q, t, T, sigma, year_base, option_type):
         self.S = S
         self.K = K
         self.r = r
         self.q = q
         self.t = t
         self.T = T
         self.year_base = year_base
         self.sigma = sigma
         self._is_call = {OptionType.CALL: True, OptionType.PUT: False}[option_type]
         self._omega = 1 if self._is_call else -1
 
 
-class FiniteDifference(OptionPricingMethod):
+class OneAssetFD(OneAssetOption):
 
     def __init__(self, S, K, r, q, t, T, sigma, year_base, option_type, Ns=None, Nt=None, Smin=None, Smax=None):
         super().__init__(S=S, K=K, r=r, q=q, t=t, T=T, sigma=sigma, year_base=year_base, option_type=option_type)
 
         self.Smin = 0 if Smin is None else Smin
         self.Smax = 4 * max(S, K) if Smax is None else Smax
         self.Ns = 1000 if Ns is None else int(Ns)
         self.Nt = int((T - t) * 1) if Nt is None else int(Nt)
 
+        self.__present_value_solved = False
+        self.__greeks_solved = False
+
     def _set_initial_grid_(self):
         self.dS = (self.Smax - self.Smin) / self.Ns * 1.0
         self.dt = self.T / self.year_base / self.Nt * 1.0
         self.Svec = np.linspace(self.Smin, self.Smax, self.Ns + 1)
         self.Tvec = np.linspace(0, (self.T - self.t) / self.year_base, self.Nt + 1)
         self.grid = np.zeros(shape=(self.Ns + 1, self.Nt + 1))
 
@@ -95,28 +98,39 @@
     def _set_grid_vega_(self, dv: float = 0.01):
         pricer_up = deepcopy(self)
         pricer_up.sigma = self.sigma + dv
         pricer_up.price()
         self.grid_vega = pricer_up.grid - self.grid
         self.grid_vega = self.grid_vega.round(8)
 
+    def _check_present_value_solved_(self):
+        if not self.__present_value_solved:
+            self.price()
+
+    def _check_greeks_solved_(self):
+        self._check_present_value_solved_()
+        if not self.__greeks_solved:
+            self.greeks()
+
     def price(self):
         self._set_initial_grid_()
         self._set_terminal_condition_()
         self._set_boundary_condition_()
         self._set_coefficient_()
         self._set_matrix_()
         self._solve_()
+        self.__present_value_solved = True
 
     def greeks(self, include_vega=True):
         self._set_grid_delta_()
         self._set_grid_gamma_()
         self._set_grid_theta_()
         if include_vega:
             self._set_grid_vega_()
+        self.__greeks_solved = True
 
     def present_value(self, S=None):
         S = self.S if S is None else S
         return interpolate(x=self.Svec, y=self.grid[:, 0])(S).round(8)
 
     def delta(self, S=None):
         S = self.S if S is None else S
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/fully_explicit_european.py` & `ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_explicit_european.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .fd_grid_generator import FiniteDifference
+from .one_asset_fd_generator import OneAssetFD
 from ..api_and_utils import np, tqdm, sp
 
 
-class FullyExplicitEuropean(FiniteDifference):
+class OneAssetExplicitEuropean(OneAssetFD):
 
     def _set_matrix_(self):
         self._A = sp.diags([self._l[1:], self._c, self._u[:-1]], [-1, 0, 1], format='csc').toarray()
         self._I = sp.eye(self.Ns - 1).toarray()
         self._M = self._I + self.dt * self._A
 
     def _solve_(self):
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/finite_difference_engine/fully_implicit_european.py` & `ht_pricing_module-0.5.1/ht_pricing_module/finite_difference_engine/one_asset_implicit_european.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .fd_grid_generator import FiniteDifference
+from .one_asset_fd_generator import OneAssetFD
 from ..api_and_utils import np, tqdm, sp
 
 
-class FullyImplicitEuropean(FiniteDifference):
+class OneAssetImplicitEuropean(OneAssetFD):
 
     def _set_matrix_(self):
         self._A = sp.diags([self._l[1:], self._c, self._u[:-1]], [-1, 0, 1], format='csc').toarray()
         self._I = sp.eye(self.Ns - 1).toarray()
         self._M = self._I - self.dt * self._A
 
     def _solve_(self):
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.5.1/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,9 +66,9 @@
           将返回矩阵乘以当前价格即可得到价格路径。
           """
 
         drift = riskfree_rate - dividend - 0.5 * volatility ** 2
         t_arr = np.arange(1, expiry_date + 1, 1) - intraday
         t_arr = np.hstack([0, t_arr])
         dt_arr = (t_arr[1:] - t_arr[:-1]) / year_base
-        gmb_trn = generate_randn(qmc_flag, antithetic_flag, random_seed, path_num, drift, volatility, dt_arr)
-        return gmb_trn
+        gmb_rtn = generate_randn(qmc_flag, antithetic_flag, random_seed, path_num, drift, volatility, dt_arr)
+        return gmb_rtn
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,73 @@
 from ..monte_carlo_engine import *
 from ..api_and_utils import *
+from ..finite_difference_engine import *
 
 
-class MultiAssetOptionBase:
+class OneAssetOptionBase(ParamsBase):
 
     def __init__(self, param):
-        self.param = Params(param) if isinstance(param, dict) else param
+        super().__init__(param)
 
     def __calculate_present_value__(self) -> float:
         raise NotImplementedError()
 
     @lru_cache(maxsize=10)
     def present_value(self) -> float:
         return self.__calculate_present_value__()
 
     @lru_cache(maxsize=10)
-    def delta(self, leg: int, step: float = 0.001) -> float:
-        spot_price = f'spot_price{leg}'
-        time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
-        if time_to_expiry <= 0:
-            return 0.0
-
-        if hasattr(self.param, spot_price):
-            spot_up = getattr(self.param, spot_price) * (1 + step)
-            spot_down = getattr(self.param, spot_price) * (1 - step)
-            pricer_up = deepcopy(self)
-            setattr(pricer_up.param, spot_price, spot_up)
-            pricer_down = deepcopy(self)
-            setattr(pricer_down.param, spot_price, spot_down)
-            return (pricer_up.present_value() - pricer_down.present_value()) / (spot_up - spot_down)
+    def delta(self, step: float = 0.001) -> float:
+        if hasattr(self.param, 'expiry_date') and hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
+            if self.param.expiry_date - self.param.current_date <= 0:
+                return 0.0
+            else:
+                spot_up = self.param.spot_price * (1 + step)
+                spot_down = self.param.spot_price * (1 - step)
+                pricer_up, pricer_down = deepcopy(self), deepcopy(self)
+                pricer_up.param.spot_price = spot_up
+                pricer_down.param.spot_price = spot_down
+                return (pricer_up.present_value() - pricer_down.present_value()) / (spot_up - spot_down)
         return 0.0
 
     @lru_cache(maxsize=10)
-    def gamma(self, leg: int, step: float = 0.001) -> float:
-        spot_price = f'spot_price{leg}'
-        if hasattr(self.param, spot_price):
-            spot_up = getattr(self.param, spot_price) * (1 + step)
-            spot_down = getattr(self.param, spot_price) * (1 - step)
-            pricer_up = deepcopy(self)
-            setattr(pricer_up.param, spot_price, spot_up)
-            pricer_down = deepcopy(self)
-            setattr(pricer_down.param, spot_price, spot_down)
+    def moddelta(self, step: float = 0.001) -> float:
+        if hasattr(self.param, 'expiry_date') and hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
+            if 0 < self.param.expiry_date - self.param.current_date <= 1:
+                mod_step = 0.0001
+                mod_current = self.param.expiry_date - mod_step
+                spot_up = self.param.spot_price * (1 + step)
+                spot_down = self.param.spot_price * (1 - step)
+                mod_pricer_up, mod_pricer_down = deepcopy(self), deepcopy(self)
+                mod_pricer_up.param.spot_price = spot_up
+                mod_pricer_down.param.spot_price = spot_down
+                mod_pricer_up.param.current_date = mod_current
+                mod_pricer_down.param.current_date = mod_current
+                return (mod_pricer_up.present_value() - mod_pricer_down.present_value()) / (spot_up - spot_down)
+            else:
+                return self.delta(step=step)
+        return 0.0
+
+    @lru_cache(maxsize=10)
+    def gamma(self, step: float = 0.001) -> float:
+        if hasattr(self.param, 'spot_price'):
+            spot_up = self.param.spot_price * (1 + step)
+            spot_down = self.param.spot_price * (1 - step)
+            pricer_up, pricer_down = deepcopy(self), deepcopy(self)
+            pricer_up.param.spot_price = spot_up
+            pricer_down.param.spot_price = spot_down
             return (pricer_up.present_value() + pricer_down.present_value() - 2 * self.present_value()) / pow((spot_up - spot_down) / 2, 2) 
         return 0.0
 
     @lru_cache(maxsize=10)
-    def vega(self, leg: int, step: float = 0.01) -> float:
-        volatility = f'volatility{leg}'
-        if hasattr(self.param, volatility):
-            vol_up = getattr(self.param, volatility) + step
+    def vega(self, step: float = 0.01) -> float:
+        if hasattr(self.param, 'volatility'):
+            vol_up = self.param.volatility + step
             pricer_up = deepcopy(self)
-            setattr(pricer_up.param, volatility, vol_up)
+            pricer_up.param.volatility = vol_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
@@ -62,43 +75,59 @@
             pricer_up.param.current_date = current_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
     def rho(self, step: float = 0.0001) -> float:
         if hasattr(self.param, 'riskfree_rate'):
-            current_up = self.param.riskfree_rate + step
+            rate_up = self.param.riskfree_rate + step
             pricer_up = deepcopy(self)
-            pricer_up.param.riskfree_rate = current_up
+            pricer_up.param.riskfree_rate = rate_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
-    def dpvdcorr(self, step: float = 0.01) -> float:
-        if hasattr(self.param, 'correlation'):
-            corr_up = self.param.correlation + step
-            corr_down = self.param.correlation - step
+    def phi(self, step: float = 0.001) -> float:
+        if hasattr(self.param, 'dividend'):
+            div_up = self.param.dividend + step
             pricer_up = deepcopy(self)
-            pricer_up.param.correlation = corr_up
-            pricer_down = deepcopy(self)
-            pricer_down.param.correlation = corr_down
-            return (pricer_up.present_value() - pricer_down.present_value()) / 2
+            pricer_up.param.dividend = div_up
+            return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
-    def ddeltadt(self, leg: int, time_step: float = 1, price_step: float = 0.001):
-        if hasattr(self.param, 'current_date'):
+    def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+        if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
-            return pricer_up.delta(leg=leg, step=price_step) - self.delta(leg=leg, step=price_step)
+            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+        return 0.0
+
+    @lru_cache(maxsize=10)
+    def modddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+        if hasattr(self.param, 'expiry_date') and hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
+            if 0 < self.param.expiry_date - self.param.current_date <= 1:
+                mod_step = 0.0001
+                mod_current = self.param.expiry_date - mod_step
+                mod_current_up = mod_current + time_step
+                mod_pricer, mod_pricer_up = deepcopy(self), deepcopy(self)
+                mod_pricer.param.current_date = mod_current
+                mod_pricer_up.param.current_date = mod_current_up
+                return mod_pricer_up.delta(step=price_step) - mod_pricer.delta(step=price_step)
+            elif 1 < self.param.expiry_date - self.param.current_date <= 2:
+                current_up = self.param.current_date + time_step
+                pricer_up = deepcopy(self)
+                pricer_up.param.current_date = current_up
+                return pricer_up.moddelta(step=price_step) - self.delta(step=price_step)
+            else:
+                return self.ddeltadt(time_step=time_step, price_step=price_step)
         return 0.0
 
     @lru_cache(maxsize=10)
-    def ddeltadv(self, leg: int, vol_step: float = 0.01, price_step: float = 0.001):
-        volatility = f'volatility{leg}'
-        if hasattr(self.param, volatility):
-            vol_up = getattr(self.param, volatility) + vol_step
+    def ddeltadv(self, vol_step: float = 0.01, price_step: float = 0.001):
+        if hasattr(self.param, 'volatility') and hasattr(self.param, 'spot_price'):
+            vol_up = self.param.volatility + vol_step
             pricer_up = deepcopy(self)
-            setattr(pricer_up.param, volatility, vol_up)
-            return pricer_up.delta(leg=leg, step=price_step) - self.delta(leg=leg, step=price_step)
+            pricer_up.param.volatility = vol_up
+            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
         return 0.0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/quotient/two_asset_quotient_as.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..multi_asset_option_base import *
 
 
-class Quotient(MultiAssetOptionBase):
+class TwoAssetQuotient(MultiAssetOptionBase):
 
     def __calculate_present_value__(self):
         rst = 0
         cp = {OptionType.CALL: 1, OptionType.PUT: -1}[self.param.option_type]
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         s1_d_s2 = self.param.spot_price1 / self.param.spot_price2
         if time_to_expiry <= 0 or (self.param.volatility1 == 0 and self.param.volatility2 == 0):
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,8 +4,12 @@
 from .fixed_acc_ako_as import FixedAccAko
 from .linear_acc_enhanced_as import LinearAccEnhanced
 from .fixed_acc_enhanced_as import FixedAccEnhanced
 from .linear_acc_ako_as import LinearAccAko
 from .fixed_acc_barrier_enhanced_as import FixedAccBarrierEnhanced
 from .linear_acc_fixed_enhanced_as import LinearAccFixedEnhanced
 from .linear_acc_fusing_as import LinearAccFusing
-from .linear_acc_fusing_trans_forward_as import LinearAccFusingTransForward
+from .linear_acc_fusing_close_settle_as import LinearAccFusingCloseSettle
+from .fixed_acc_fusing_as import FixedAccFusing
+from .basket_linear_acc_as import BasketLinearAcc
+from .basket_fixed_acc_as import BasketFixedAcc
+from .basket_fixed_acc_barrier_as import BasketFixedAccBarrier
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,23 @@
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+
+        cp = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
-            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
+            if cp * (self.param.spot_price - self.param.barrier_price) >= 0:
+                return 0 - self.delta(step=price_step)
+            else:
+                return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
         return 0.0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..one_asset_option_base import *
-from ..vanilla import Vanilla
-from ..binary import Binary
+from ..vanilla.vanilla_as import Vanilla
+from ..binary.binary_as import Binary
 
 
 class FixedAcc(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..one_asset_option_base import *
-from ..vanilla import Vanilla
-from ..binary import Binary
+from ..vanilla.vanilla_as import Vanilla
+from ..binary.binary_as import Binary
 
 
 class FixedAccBarrier(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..one_asset_option_base import *
-from ..vanilla import Vanilla
-from ..binary import Binary
+from ..vanilla.vanilla_as import Vanilla
+from ..binary.binary_as import Binary
 
 
 class FixedAccBarrierEnhanced(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..one_asset_option_base import *
-from ..vanilla import Vanilla
-from ..binary import Binary
+from ..vanilla.vanilla_as import Vanilla
+from ..binary.binary_as import Binary
 
 
 class FixedAccEnhanced(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,16 +63,23 @@
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+
+        cp = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
-            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
+            if cp * (self.param.spot_price - self.param.barrier_price) >= 0:
+                return 0 - self.delta(step=price_step)
+            else:
+                return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
         return 0.0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,22 +84,29 @@
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+
+        cp = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
-            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
+            if cp * (self.param.spot_price - self.param.barrier_price) >= 0:
+                return 0 - self.delta(step=price_step)
+            else:
+                return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
         return 0.0
 
     @lru_cache(maxsize=10)
     def remain_value(self) -> float:
         phi = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
         rst = 0
         for obs in self.param.obs_date:
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_close_settle_as.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from ..one_asset_option_base import *
 from ..barrier.discrete_barrier_as import DiscreteBarrier
 from ..forward import Forward
 from ..touch import DiscreteOneTouch
 
 
-class LinearAccFusingTransForward(OneAssetOptionBase):
+class LinearAccFusingCloseSettle(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
         cp = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
+        entrance_price = self.param.barrier_price - cp * self.param.payoff
 
         for obs in self.param.obs_date:
             param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
@@ -42,21 +43,21 @@
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['year_base'] = self.param.year_base
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate_type'] = RebateType.PAH
-            param['rebate'] = cp * (self.param.entrance_price - self.param.strike_price)
+            param['rebate'] = cp * (entrance_price - self.param.strike_price)
             param['obs_freq'] = self.param.obs_freq
             touch2 = DiscreteOneTouch(param)
 
             param = Params()
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
-            param['strike_price'] = self.param.entrance_price
+            param['strike_price'] = entrance_price
             forward3 = Forward(param)
 
             rst = rst + self.param.base_quantity * (-(self.param.leverage - 1) * barrier1.present_value() + touch2.present_value() + cp * forward3.present_value())
 
         param = Params()
         param['option_type'] = option_type1
         param['exercise_type'] = self.param.exercise_type
@@ -89,16 +90,36 @@
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
     @lru_cache(maxsize=10)
     def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+
+        cp = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
         if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             for obs in pricer_up.param.obs_date:
                 if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
                     obs.obs_price = pricer_up.param.spot_price
-            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
+            if cp * (self.param.spot_price - self.param.barrier_price) >= 0:
+                return 0 - self.delta(step=price_step)
+            else:
+                return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+
         return 0.0
+
+    @lru_cache(maxsize=10)
+    def remain_value(self) -> float:
+        phi = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
+        rst = 0
+        for obs in self.param.obs_date:
+            if obs.obs_index > self.param.current_date:
+                break
+            payoff = phi * (obs.obs_price - self.param.strike_price)
+            if payoff <= 0:
+                payoff = self.param.leverage * payoff
+            rst = rst + self.param.base_quantity * payoff
+        return self.present_value() - rst
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..one_asset_option_base import *
-from ..barrier import DiscreteBarrier
-from ..forward import Forward
+from ..barrier.discrete_barrier_as import DiscreteBarrier
+from ..forward.forward_as import Forward
 
 
 class Airbag(OneAssetOptionBase):
 
     def __calculate_present_value__(self):
         phi = {OptionType.STANDARD: 1, OptionType.REVERSE: -1}[self.param.option_type]
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
             if self.param.running_avg > n / m * X:
                 if self.param.option_type == OptionType.PUT:
                     return 0
                 else:
                     RA_hat = self.param.running_avg * m / n + EA * (n - m) / n
                     return np.exp(-self.param.riskfree_rate * T) * (RA_hat - X)
 
-        vA = np.sqrt((np.log(EA2) - 2 * np.log(EA)) / T)
+        vA = np.sqrt(max(np.log(EA2) - 2 * np.log(EA), 0) / T)
 
         if m > 0:
             X = n / (n - m) * X - m / (n - m) * self.param.running_avg
 
         d1 = (np.log(EA / X) + vA * vA / 2 * T) / (vA * np.sqrt(T))
         d2 = d1 - vA * np.sqrt(T)
         rst = np.exp(-self.param.riskfree_rate * T) * (cp * EA * norm.cdf(cp * d1) - cp * X * norm.cdf(cp * d2))
-        return rst * (n - m) / n
+        return rst * (n - m) / n
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,13 @@
             du = {BarrierType.DOWN: 'd', BarrierType.UP: 'u'}[self.param.barrier_type]
             io = {KnockType.IN: 'i', KnockType.OUT: 'o'}[self.param.knock_type]
 
             rst = {'cdi': B3 if self.param.strike_price >= self.param.barrier_price else B1 - B2 + B4,
                    'cui': B1 if self.param.strike_price >= self.param.barrier_price else B2 - B3 + B4,
                    'pdi': B2 - B3 + B4 if self.param.strike_price >= self.param.barrier_price else B1,
                    'pui': B1 - B2 + B4 if self.param.strike_price >= self.param.barrier_price else B3,
-                   'cdo': B1 - B3 if self.param.strike_price >= self.param.strike_price else B2 - B4,
+                   'cdo': B1 - B3 if self.param.strike_price >= self.param.barrier_price else B2 - B4,
                    'cuo': 0 if self.param.strike_price >= self.param.barrier_price else B1 - B2 + B3 - B4,
                    'pdo': B1 - B2 + B3 - B4 if self.param.strike_price >= self.param.barrier_price else 0,
                    'puo': B2 - B4 if self.param.strike_price >= self.param.barrier_price else B1 - B3}[f'{cp}{du}{io}']
         return rst
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from ..one_asset_option_base import *
-from ..barrier.barrier_as import Barrier
+from ..barrier.barrier_binary_as import BarrierBinary
 
 
-class DiscreteBarrier(OneAssetOptionBase):
+class DiscreteBarrierBinary(OneAssetOptionBase):
     """
-    离散障碍近似解析解
-    reference: The Complete Guide to Option Pricing Formulas, 2nd ed. L164
-    :param obs_freq 观测频率
+    离散二元障碍近似解析解
     """
 
     def __init__(self, param):
         super().__init__(param)
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         dt = self.param.obs_freq / self.param.year_base
         adjust = 0.5826 * self.param.volatility * math.sqrt(dt)
         if self.param.barrier_type == BarrierType.UP and time_to_expiry > 0:
-            self.param.barrier_price = self.param.barrier_price * np.exp(adjust)
+            self.param.adjust_barrier_price = self.param.barrier_price * np.exp(adjust)
         elif self.param.barrier_type == BarrierType.DOWN and time_to_expiry > 0:
-            self.param.barrier_price = self.param.barrier_price * np.exp(-adjust)
+            self.param.adjust_barrier_price = self.param.barrier_price * np.exp(-adjust)
+        else:
+            self.param.adjust_barrier_price = self.param.barrier_price
 
     def __calculate_present_value__(self) -> float:
         param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
-        param['barrier_price'] = self.param.barrier_price
+        param['barrier_price'] = self.param.adjust_barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['volatility'] = self.param.volatility
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['year_base'] = self.param.year_base
         param['barrier_type'] = self.param.barrier_type
         param['knock_type'] = self.param.knock_type
         param['is_knock_in'] = self.param.is_knock_in
-        param['rebate'] = self.param.rebate
-        pricer = Barrier(param)
+        param['payoff'] = self.param.payoff
+        pricer = BarrierBinary(param)
         return pricer.present_value()
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from ..one_asset_option_base import *
-from ..barrier.barrier_binary_as import BarrierBinary
+from ..touch.one_touch_as import OneTouch
 
 
-class DiscreteBarrierBinary(OneAssetOptionBase):
+class DiscreteOneTouch(OneAssetOptionBase):
     """
-    离散二元障碍近似解析解
+    离散单触碰期权解析解
     """
 
     def __init__(self, param):
         super().__init__(param)
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         dt = self.param.obs_freq / self.param.year_base
         adjust = 0.5826 * self.param.volatility * math.sqrt(dt)
         if self.param.barrier_type == BarrierType.UP and time_to_expiry > 0:
-            self.param.barrier_price = self.param.barrier_price * np.exp(adjust)
+            self.param.adjust_barrier_price = self.param.barrier_price * np.exp(adjust)
         elif self.param.barrier_type == BarrierType.DOWN and time_to_expiry > 0:
-            self.param.barrier_price = self.param.barrier_price * np.exp(-adjust)
+            self.param.adjust_barrier_price = self.param.barrier_price * np.exp(-adjust)
+        else:
+            self.param.adjust_barrier_price = self.param.barrier_price
 
     def __calculate_present_value__(self) -> float:
         param = Params()
-        param['option_type'] = self.param.option_type
-        param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
-        param['strike_price'] = self.param.strike_price
-        param['barrier_price'] = self.param.barrier_price
+        param['barrier_price'] = self.param.adjust_barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['volatility'] = self.param.volatility
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['year_base'] = self.param.year_base
         param['barrier_type'] = self.param.barrier_type
         param['knock_type'] = self.param.knock_type
         param['is_knock_in'] = self.param.is_knock_in
-        param['payoff'] = self.param.payoff
-        pricer = BarrierBinary(param)
+        param['rebate_type'] = self.param.rebate_type
+        param['rebate'] = self.param.rebate
+        pricer = OneTouch(param)
         return pricer.present_value()
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,17 @@
     Bachelier model
     """
     def __calculate_present_value__(self) -> float:
 
         def __norm_pdf__(x):
             return 1 / math.sqrt(2 * math.pi) * math.exp(-1 * pow(x, 2) / 2)
 
-        rst = 0
         cp = {OptionType.CALL: 1, OptionType.PUT: -1}[self.param.option_type]
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         if time_to_expiry <= 0:
             rst = max(cp * (self.param.spot_price - self.param.strike_price), 0)
         else:
-            b = self.param.riskfree_rate - self.param.dividend
-            f0 = self.param.spot_price * math.exp(b * time_to_expiry)
             t_adj_vol = self.param.volatility * math.sqrt(time_to_expiry)
             discount_factor = math.exp(-1 * self.param.riskfree_rate * time_to_expiry)
-            d = (f0 - self.param.strike_price) / t_adj_vol
-            rst = discount_factor * (t_adj_vol * __norm_pdf__(d) + cp * (f0 - self.param.strike_price) * norm.cdf(cp * d))
+            d = (self.param.spot_price - self.param.strike_price) / t_adj_vol
+            rst = discount_factor * (t_adj_vol * __norm_pdf__(d) + cp * (self.param.spot_price - self.param.strike_price) * norm.cdf(cp * d))
         return rst
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,15 @@
             drift = self.param.riskfree_rate - self.param.dividend
             d1 = (math.log(self.param.spot_price / self.param.strike_price) + (drift + math.pow(self.param.volatility, 2) / 2.0) * time_to_expiry) / t_adj_vol
             d2 = d1 - t_adj_vol
             rst = self.param.payoff * math.exp(-1 * self.param.riskfree_rate * time_to_expiry) * norm.cdf(cp * d2)
         return rst
 
     def __american(self):
-        """美式(待验证)"""
-        # TODO: 验证
+        """美式, One Touch解析解"""
         rst = 0
         cp = {OptionType.CALL: 1, OptionType.PUT: -1}[self.param.option_type]
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         if time_to_expiry <= 0:
             rst = self.param.payoff if cp * (self.param.spot_price - self.param.strike_price) >= 0 else 0
         elif cp * (self.param.spot_price - self.param.strike_price) >= 0:
             rst = self.param.payoff
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/accumulator/basket_fixed_acc_barrier_as.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,77 @@
-from ht_pricing_module.one_asset_pricing_module.one_asset_option_base import *
-from ht_pricing_module.one_asset_pricing_module.binary.binary_as import Binary
-from ht_pricing_module.one_asset_pricing_module.vanilla.vanilla_as import Vanilla
-
-
-class SharkfinYield(OneAssetOptionBase):
-
-    def __calculate_present_value__(self):
-        time_to_expiry = (self.param.expiry_date - self.param.entrance_date) / self.param.year_base
-        participation_rate = (self.param.max_yield_annual - self.param.min_yield_annual) * time_to_expiry / abs((self.param.strike_price - self.param.barrier_price) / self.param.entrance_price)
-
-        param = Params()
-        param['option_type'] = self.param.option_type
-        param['exercise_type'] = self.param.exercise_type
-        param['spot_price'] = self.param.spot_price / self.param.entrance_price
-        param['strike_price'] = self.param.strike_price / self.param.entrance_price
-        param['expiry_date'] = self.param.expiry_date
-        param['current_date'] = self.param.current_date
-        param['volatility'] = self.param.volatility
-        param['riskfree_rate'] = self.param.riskfree_rate
-        param['dividend'] = self.param.dividend
-        param['year_base'] = self.param.year_base
-        vanilla1 = Vanilla(param)
-
-        param = Params()
-        param['option_type'] = self.param.option_type
-        param['exercise_type'] = self.param.exercise_type
-        param['spot_price'] = self.param.spot_price / self.param.entrance_price
-        param['strike_price'] = self.param.barrier_price / self.param.entrance_price
-        param['expiry_date'] = self.param.expiry_date
-        param['current_date'] = self.param.current_date
-        param['volatility'] = self.param.volatility
-        param['riskfree_rate'] = self.param.riskfree_rate
-        param['dividend'] = self.param.dividend
-        param['year_base'] = self.param.year_base
-        vanilla2 = Vanilla(param)
-
-        param = Params()
-        param['option_type'] = self.param.option_type
-        param['exercise_type'] = self.param.exercise_type
-        param['spot_price'] = self.param.spot_price / self.param.entrance_price
-        param['strike_price'] = self.param.barrier_price / self.param.entrance_price
-        param['expiry_date'] = self.param.expiry_date
-        param['current_date'] = self.param.current_date
-        param['volatility'] = self.param.volatility
-        param['riskfree_rate'] = self.param.riskfree_rate
-        param['dividend'] = self.param.dividend
-        param['payoff'] = self.param.rebate_annual * time_to_expiry
-        param['year_base'] = self.param.year_base
-        binary3 = Binary(param)
-
-        return self.param.notional * (participation_rate * (vanilla1.present_value() - vanilla2.present_value()) - binary3.present_value() + self.param.min_yield_annual * time_to_expiry)
-
-
-if __name__ == '__main__':
-    param = Params()
-    param['option_type'] = OptionType.PUT
-    param['exercise_type'] = ExerciseType.EUROPEAN
-    param['notional'] = 1
-    param['spot_price'] = 100
-    param['entrance_price'] = 100
-    param['strike_price'] = 95
-    param['barrier_price'] = 90
-    param['expiry_date'] = 245
-    param['current_date'] = 245
-    param['entrance_date'] = 0
-    param['volatility'] = 0.14
-    param['riskfree_rate'] = 0.03
-    param['dividend'] = 0.03
-    param['year_base'] = 245
-    param['rebate_annual'] = 0.07
-    param['min_yield_annual'] = 0.02
-    param['max_yield_annual'] = 0.14
-
-    pricer = SharkfinYield(param=param)
-    print(pricer.present_value())
-    import matplotlib.pyplot as plt
-    spot_ls = np.arange(85, 100, 0.1)
-    pv_ls = []
-    for spot in spot_ls:
-        param['spot_price'] = spot
-        pricer = SharkfinYield(param=param)
-        pv_ls.append(pricer.present_value())
-    plt.plot(spot_ls, pv_ls)
-    plt.show()
+from ..one_asset_option_base import *
+from ..basket.basket_vanilla_as import BasketVanilla
+from ..binary.basket_binary_as import BasketBinary
+
+
+class BasketFixedAccBarrier(OneAssetOptionBase):
+
+    def __calculate_present_value__(self) -> float:
+        rst = 0
+
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+
+        for obs in self.param.obs_date:
+            param = Params()
+            param['option_type'] = option_type1
+            param['exercise_type'] = self.param.exercise_type
+            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
+            param['strike_price'] = self.param.strike_price
+            param['expiry_date'] = obs.obs_index
+            param['current_date'] = self.param.current_date
+            param['volatility'] = self.param.volatility
+            param['riskfree_rate'] = self.param.riskfree_rate
+            param['year_base'] = self.param.year_base
+            basket_vanilla1 = BasketVanilla(param)
+
+            param = Params()
+            param['option_type'] = option_type2
+            param['exercise_type'] = self.param.exercise_type
+            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
+            param['strike_price'] = self.param.strike_price
+            param['expiry_date'] = obs.obs_index
+            param['current_date'] = self.param.current_date
+            param['volatility'] = self.param.volatility
+            param['riskfree_rate'] = self.param.riskfree_rate
+            param['payoff'] = self.param.payoff
+            param['year_base'] = self.param.year_base
+            basket_binary2 = BasketBinary(param)
+
+            param = Params()
+            param['option_type'] = option_type2
+            param['exercise_type'] = self.param.exercise_type
+            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
+            param['strike_price'] = self.param.barrier_price
+            param['expiry_date'] = obs.obs_index
+            param['current_date'] = self.param.current_date
+            param['volatility'] = self.param.volatility
+            param['riskfree_rate'] = self.param.riskfree_rate
+            param['payoff'] = self.param.payoff
+            param['year_base'] = self.param.year_base
+            basket_binary3 = BasketBinary(param)
+            rst = rst + (-self.param.leverage * basket_vanilla1.present_value() + basket_binary2.present_value() - basket_binary3.present_value())
+        return rst
+
+    @lru_cache(maxsize=10)
+    def theta(self, step: float = 1) -> float:
+        if hasattr(self.param, 'current_date'):
+            current_up = self.param.current_date + step
+            pricer_up = deepcopy(self)
+            pricer_up.param.current_date = current_up
+            for obs in pricer_up.param.obs_date:
+                if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
+                    obs.obs_price = pricer_up.param.spot_price
+            return pricer_up.present_value() - self.present_value()
+        return 0.0
+
+    @lru_cache(maxsize=10)
+    def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+        if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
+            current_up = self.param.current_date + time_step
+            pricer_up = deepcopy(self)
+            pricer_up.param.current_date = current_up
+            for obs in pricer_up.param.obs_date:
+                if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
+                    obs.obs_price = pricer_up.param.spot_price
+            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
+        return 0.0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         return notional * rst
 
     intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
     price = spot_price * McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
                                                   intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
     M = len(price)
 
-    ki_obs_idx = np.where(knock_in_obs['obs_index'] >= 0)
+    ki_obs_idx = np.where(knock_in_obs['obs_index'] >= 0) if intraday == 0 else np.where(knock_in_obs['obs_index'] > 0)
     ki_obs_idx = knock_in_obs['obs_index'][ki_obs_idx].astype(int)
 
-    ko_obs_idx = np.where(knock_out_obs['obs_index'] >= 0)
+    ko_obs_idx = np.where(knock_out_obs['obs_index'] >= 0) if intraday == 0 else np.where(knock_out_obs['obs_index'] > 0)
     ko_coupon = knock_out_obs['coupon_rate'][ko_obs_idx]
     ko_obs_idx = knock_out_obs['obs_index'][ko_obs_idx].astype(int)
 
     t_arr = np.hstack([0, np.arange(1, expiry_date + 1, 1) - intraday])
     assert round(expiry_date - intraday, 4) == round(t_arr[-1], 4)
 
     ki_mat_flag = np.zeros((M, 1), dtype=bool) if len(ki_obs_idx) == 0 else phi * (price[:, ki_obs_idx] - knock_in_barrier_price) <= 0
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from ..one_asset_option_base import interpolate, np, CrankNicolsonSnowball, tqdm
+from ..one_asset_option_base import interpolate, np, sp, spilu, OneAssetFDSnowball
 
 
-class SnowballDiscountedPde(CrankNicolsonSnowball):
+class SnowballDiscountedPde(OneAssetFDSnowball):
 
     def _set_other_vector_(self):
-        self._IntVec = self.param.margin_rate * (np.exp(self.param.riskfree_rate * self.Tvec / self.param.year_base) - 1)
+        self._IntVec = self.param.margin_rate * (np.exp(self.param.riskfree_rate * self.Tauvec / self.param.year_base) - 1)
         self._S_KO = self._omega * (self.Svec - self.param.knock_out_barrier_price) >= 0
         self._S_KI = self._omega * (self.Svec - self.param.knock_in_barrier_price) <= 0
 
     def _set_terminal_condition_(self):
         S_NKI_NKO = ~(self._S_KO | self._S_KI)
 
         self.KIgrid[:, -1] = (self._omega * ((self.Svec - self.param.knock_in_strike_price) / self.param.entrance_price) - self._IntVec[-1]) * self.param.notional
@@ -35,44 +35,46 @@
             if not np.isscalar(self._Rbt_KO) and len(self._Rbt_KO) > 1:
                 f1 = interpolate(x=self._T_KO, y=self._Rbt_KO, kind='next', bounds_error=False, fill_value=(self._Rbt_KO[0], self._Rbt_KO[-1]))
                 f2 = interpolate(x=self._T_KO, y=self._T_KO, kind='next', bounds_error=False, fill_value=(self._T_KO[0], self._T_KO[-1]))
                 self.NKIgrid[0, :] = (f1(self.Tvec) - self._IntVec) * self.param.notional * np.exp(-self.param.riskfree_rate * (f2(self.Tvec) - self.Tvec) / self.param.year_base)
             else:
                 self.NKIgrid[0, :] = (self._Rbt_KO - self._IntVec) * self.param.notional * DFr
 
+    def _solve_intraday_(self, idx, KIgrid, NKIgrid):
+        if self._Tau > 0 and self._Nt > 0:
+            dt = round(1 - self._Tau, 4)
+            M2 = self._M1 - dt / self.param.year_base * self._A
+            iluM = spilu(sp.csc_matrix(M2), drop_tol=1e-10, fill_factor=100)
+
+            U = NKIgrid[1: -1, idx + 1].copy()
+            U[0] += self._l[0] * dt / self.param.year_base * NKIgrid[0, idx]
+            U[-1] += self._u[-1] * dt / self.param.year_base * NKIgrid[-1, idx]
+            NKIgrid[1: -1, idx] = iluM.solve(U)
+        return KIgrid, NKIgrid
+
     def _solve_(self):
-        invM = np.linalg.inv(self._M2)
+        iluM = spilu(sp.csc_matrix(self._M2), drop_tol=1e-10, fill_factor=100)
 
         KO_idx = np.searchsorted(self.Tvec, self._T_KO)
         KI_idx = np.searchsorted(self.Tvec, self._T_KI)
 
-        for j in tqdm(list(reversed(np.arange(self._Nt))), leave=False):
+        for j in list(reversed(np.arange(self._Nt))):
 
             self.KIgrid[1: -1, j] = self.KIgrid[1: -1, j + 1]
 
             if j + 1 in KO_idx:
                 self.NKIgrid[self._S_KO, j + 1] = (self._Rbt_KO[np.where(KO_idx == j + 1)] - self._IntVec[j + 1]) * self.param.notional
 
             if j + 1 in KI_idx:
                 self.NKIgrid[self._S_KI, j + 1] = self.KIgrid[self._S_KI, j + 1]
 
-            U = self._M1.dot(self.NKIgrid[1: -1, j + 1])
-            U[0] += self._theta * self._l[0] * self.dt / self.param.year_base * self.NKIgrid[0, j] + (1 - self._theta) * self._l[0] * self.dt / self.param.year_base * self.NKIgrid[0, j + 1]
-            U[-1] += self._theta * self._u[-1] * self.dt / self.param.year_base * self.NKIgrid[-1, j] + (1 - self._theta) * self._u[-1] * self.dt / self.param.year_base * self.NKIgrid[-1, j + 1]
-            self.NKIgrid[1: -1, j] = np.dot(invM, U)
-
-            # if j in KO_idx:
-            #     self.NKIgrid[self._S_KO, j] = (self._Rbt_KO[np.where(KO_idx == j)] - self._IntVec[j]) * self.param.notional
-            #
-            # if j in KI_idx:
-            #     self.NKIgrid[self._S_KI, j] = self.KIgrid[self._S_KI, j]
+            U = self.NKIgrid[1: -1, j + 1].copy()
+            U[0] += self._l[0] * self.dt / self.param.year_base * self.NKIgrid[0, j]
+            U[-1] += self._u[-1] * self.dt / self.param.year_base * self.NKIgrid[-1, j]
+            self.NKIgrid[1: -1, j] = iluM.solve(U)
 
-        if self._Tau > 0 and self._Nt > 0:
-            dt = 1 - self._Tau
-            M1 = self._I + (1 - self._theta) * dt / self.param.year_base * self._A
-            M2 = self._I - self._theta * dt / self.param.year_base * self._A
-            invM = np.linalg.inv(M2)
-
-            U = M1.dot(self.NKIgrid[1: -1, 1])
-            U[0] += self._theta * self._l[0] * dt / self.param.year_base * self.NKIgrid[0, 0] + (1 - self._theta) * self._l[0] * dt / self.param.year_base * self.NKIgrid[0, 1]
-            U[-1] += self._theta * self._u[-1] * dt / self.param.year_base * self.NKIgrid[-1, 0] + (1 - self._theta) * self._u[-1] * dt / self.param.year_base * self.NKIgrid[-1, 1]
-            self.NKIgrid[1: -1, 0] = np.dot(invM, U)
+        self.KIgrid, self.NKIgrid = self._solve_intraday_(idx=0, KIgrid=self.KIgrid.copy(), NKIgrid=self.NKIgrid.copy())
+
+        if self._Nt > 1:
+            self.T1KIgrid, self.T1NKIgrid = self._solve_intraday_(idx=0, KIgrid=self.KIgrid[:, 1:].copy(), NKIgrid=self.NKIgrid[:, 1:].copy())
+        else:
+            self.T1KIgrid, self.T1NKIgrid = self.KIgrid[:, self._Nt:].copy(), self.NKIgrid[:, self._Nt:].copy()
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         return rst
 
     intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
     price = spot_price * McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
                                                   intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
     M = len(price)
 
-    ki_obs_idx = np.where(knock_in_obs['obs_index'] >= 0)
+    ki_obs_idx = np.where(knock_in_obs['obs_index'] >= 0) if intraday == 0 else np.where(knock_in_obs['obs_index'] > 0)
     ki_adj = knock_in_obs['adjust_rate'][ki_obs_idx]
     ki_obs_idx = knock_in_obs['obs_index'][ki_obs_idx].astype(int)
 
-    ko_obs_idx = np.where(knock_out_obs['obs_index'] >= 0)
+    ko_obs_idx = np.where(knock_out_obs['obs_index'] >= 0) if intraday == 0 else np.where(knock_out_obs['obs_index'] > 0)
     ko_adj = knock_out_obs['adjust_rate'][ko_obs_idx]
     ko_coupon = knock_out_obs['coupon_rate'][ko_obs_idx]
     ko_obs_idx = knock_out_obs['obs_index'][ko_obs_idx].astype(int)
 
     t_arr = np.hstack([0, np.arange(1, expiry_date + 1, 1) - intraday])
     assert round(expiry_date - intraday, 4) == round(t_arr[-1], 4)
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py` & `ht_pricing_module-0.5.1/ht_pricing_module/multi_asset_pricing_module/snowball/two_asset_snowball_pde.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,125 @@
-from ..one_asset_option_base import interpolate, np, tqdm, CrankNicolsonSnowball
+from ..multi_asset_option_base import TwoAssetFDSnowball, interpolate, np, spilu, sp, tqdm
 
 
-class SnowballPde(CrankNicolsonSnowball):
-
+class TwoAssetSnowballPde(TwoAssetFDSnowball):
+    
     def _set_other_vector_(self):
-        self._IntVec = self.param.margin_rate * (np.exp(self.param.riskfree_rate * self.Tvec / self.param.year_base) - 1)
-        self._EnhVec = np.maximum(self._omega * self.param.participation_rate * ((self.Svec - self.param.knock_out_barrier_price) / self.param.entrance_price), 0)
-        self._S_KO = self._omega * (self.Svec - self.param.knock_out_barrier_price) >= 0
-        self._S_KI = self._omega * (self.Svec - self.param.knock_in_barrier_price) <= 0
+        self._S1Rtn = self._omega * (self.S1vec - self.param.entrance_price1) / self.param.entrance_price1
+        self._S2Rtn = self._omega * (self.S2vec - self.param.entrance_price2) / self.param.entrance_price2
+        self._S1Rtn, self._S2Rtn = np.meshgrid(self._S1Rtn, self._S2Rtn)
+        S1_d_S2_u = self._S1Rtn - self._S2Rtn <= 0
+        self._Min_S1Rtn_S2Rtn = np.minimum(self._S1Rtn * S1_d_S2_u + self._S2Rtn * np.logical_not(S1_d_S2_u), 0)
+
+        self._S1_KO = self._omega * (self.S1vec - self.param.knock_out_barrier_price1) >= 0
+        self._S2_KO = self._omega * (self.S2vec - self.param.knock_out_barrier_price2) >= 0
+        self._S1_KI = self._omega * (self.S1vec - self.param.knock_in_barrier_price1) <= 0
+        self._S2_KI = self._omega * (self.S2vec - self.param.knock_in_barrier_price2) <= 0
 
     def _set_terminal_condition_(self):
-        S_NKI_NKO = ~(self._S_KO | self._S_KI)
-
-        self.KIgrid[self._S_KO, -1] = (self.param.bonus_rate - self._IntVec[-1] + self._EnhVec[self._S_KO]) * self.param.notional
-        self.KIgrid[self._S_KI, -1] = (np.maximum((self.param.floor_rate - 1), np.minimum(self._omega * (self.Svec[self._S_KI] - self.param.knock_in_strike_price) / self.param.entrance_price, 0)) - self._IntVec[-1]) * self.param.notional
-        self.KIgrid[S_NKI_NKO, -1] = (np.maximum((self.param.floor_rate - 1), np.minimum(self._omega * (self.Svec[S_NKI_NKO] - self.param.knock_in_strike_price) / self.param.entrance_price, 0)) - self._IntVec[-1]) * self.param.notional
-
-        self.NKIgrid[self._S_KO, -1] = self.KIgrid[self._S_KO, -1]
-        self.NKIgrid[self._S_KI, -1] = self.KIgrid[self._S_KI, -1]
-        self.NKIgrid[S_NKI_NKO, -1] = (self.param.bonus_rate - self._IntVec[-1]) * self.param.notional
+        self._S_KO = np.logical_and(*np.meshgrid(self._S1_KO, self._S2_KO))
+        self._S_KI = np.logical_or(*np.meshgrid(self._S1_KI, self._S2_KI))
+        self._S_NKI_NKO = np.logical_not(np.logical_or(self._S_KO, self._S_KI))
+
+        self.KIgrid[self._S_KO] = self.param.bonus_rate * self.param.notional
+        self.KIgrid[self._S_KI] = self._Min_S1Rtn_S2Rtn[self._S_KI] * self.param.notional
+        self.KIgrid[self._S_NKI_NKO] = self._Min_S1Rtn_S2Rtn[self._S_NKI_NKO] * self.param.notional
+
+        self.NKIgrid[self._S_KO] = self.KIgrid[self._S_KO]
+        self.NKIgrid[self._S_KI] = self.KIgrid[self._S_KI]
+        self.NKIgrid[self._S_NKI_NKO] = self.param.bonus_rate * self.param.notional
 
     def _set_boundary_condition_(self):
         DFr = np.exp(-self.param.riskfree_rate * (self.Tvec[-1] - self.Tvec) / self.param.year_base)
 
         if self._is_call:
-            self.KIgrid[0, :] = (np.maximum((self.param.floor_rate - 1), np.minimum(self._omega * (self.Svec[0] - self.param.knock_in_strike_price) / self.param.entrance_price, 0)) - self._IntVec) * self.param.notional * DFr
+            self._BC_1d_2 = np.outer(DFr, self._Min_S1Rtn_S2Rtn[:, 0]) * self.param.notional
+            self._BC_1_2d = np.outer(DFr, self._Min_S1Rtn_S2Rtn[0, :]) * self.param.notional
+            self._BC_1u_2 = np.outer(DFr, self._Min_S1Rtn_S2Rtn[:, -1]) * self.param.notional
+            self._BC_1_2u = np.outer(DFr, self._Min_S1Rtn_S2Rtn[-1, :]) * self.param.notional
+
             if not np.isscalar(self._Rbt_KO) and len(self._Rbt_KO) > 1:
                 f1 = interpolate(x=self._T_KO, y=self._Rbt_KO, kind='next', bounds_error=False, fill_value=(self._Rbt_KO[0], self._Rbt_KO[-1]))
                 f2 = interpolate(x=self._T_KO, y=self._T_KO, kind='next', bounds_error=False, fill_value=(self._T_KO[0], self._T_KO[-1]))
-                self.KIgrid[-1, :] = (f1(self.Tvec) - self._IntVec + self._EnhVec[-1]) * self.param.notional * np.exp(-self.param.riskfree_rate * (f2(self.Tvec) - self.Tvec) / self.param.year_base)
+                DFRbt = f1(self.Tvec) * np.exp(-self.param.riskfree_rate * (f2(self.Tvec) - self.Tvec) / self.param.year_base) * self.param.notional
+                self._BC_1u_2[:, self._S2_KO] = DFRbt.reshape(self._Nt + 1, -1)
+                self._BC_1_2u[:, self._S1_KO] = DFRbt.reshape(self._Nt + 1, -1)
             else:
-                self.KIgrid[-1, :] = (self._Rbt_KO - self._IntVec + self._EnhVec[-1]) * self.param.notional * DFr
+                self._BC_1u_2[:, self._S2_KO] = (self._Rbt_KO * self.param.notional * DFr).reshape(self._Nt + 1, -1)
+                self._BC_1_2u[:, self._S1_KO] = (self._Rbt_KO * self.param.notional * DFr).reshape(self._Nt + 1, -1)
         else:
-            self.KIgrid[-1, :] = (np.maximum((self.param.floor_rate - 1), np.minimum(self._omega * (self.Svec[-1] - self.param.knock_in_strike_price) / self.param.entrance_price, 0)) - self._IntVec) * self.param.notional * DFr
+            self._BC_1d_2 = np.outer(DFr, self._Min_S1Rtn_S2Rtn[:, 0]) * self.param.notional
+            self._BC_1_2d = np.outer(DFr, self._Min_S1Rtn_S2Rtn[0, :]) * self.param.notional
+            self._BC_1u_2 = np.outer(DFr, self._Min_S1Rtn_S2Rtn[:, -1]) * self.param.notional
+            self._BC_1_2u = np.outer(DFr, self._Min_S1Rtn_S2Rtn[-1, :]) * self.param.notional
+
             if not np.isscalar(self._Rbt_KO) and len(self._Rbt_KO) > 1:
                 f1 = interpolate(x=self._T_KO, y=self._Rbt_KO, kind='next', bounds_error=False, fill_value=(self._Rbt_KO[0], self._Rbt_KO[-1]))
                 f2 = interpolate(x=self._T_KO, y=self._T_KO, kind='next', bounds_error=False, fill_value=(self._T_KO[0], self._T_KO[-1]))
-                self.KIgrid[0, :] = (f1(self.Tvec) - self._IntVec + self._EnhVec[0]) * self.param.notional * np.exp(-self.param.riskfree_rate * (f2(self.Tvec) - self.Tvec) / self.param.year_base)
+                DFRbt = f1(self.Tvec) * np.exp(-self.param.riskfree_rate * (f2(self.Tvec) - self.Tvec) / self.param.year_base) * self.param.notional
+                self._BC_1d_2[:, self._S2_KO] = DFRbt.reshape(self._Nt + 1, -1)
+                self._BC_1_2d[:, self._S1_KO] = DFRbt.reshape(self._Nt + 1, -1)
             else:
-                self.KIgrid[0, :] = (self._Rbt_KO - self._IntVec + self._EnhVec[0]) * self.param.notional * DFr
+                self._BC_1d_2[:, self._S2_KO] = (self._Rbt_KO * self.param.notional * DFr).reshape(self._Nt + 1, -1)
+                self._BC_1_2d[:, self._S1_KO] = (self._Rbt_KO * self.param.notional * DFr).reshape(self._Nt + 1, -1)
 
-        self.NKIgrid[0, :] = self.KIgrid[0, :]
-        self.NKIgrid[-1, :] = self.KIgrid[-1, :]
+    def _solve_intraday_(self, idx, KIcube, NKIcube):
+        if self._Tau > 0 and self._Nt > 0:
+            dt = round(1 - self._Tau, 4)
+            m1, m2 = self._Ns1 - 1, self._Ns2 - 1
+            M = sp.eye(m1 * m2) - dt / self.param.year_base * self._A
+            iluA = spilu(M, drop_tol=1e-10, fill_factor=100)
+
+            KIgrid = KIcube[idx + 1].copy()
+            KIgrid[:, 0], KIgrid[:, -1] = self._BC_1d_2[idx, :], self._BC_1u_2[idx, :]
+            KIgrid[0, :], KIgrid[-1, :] = self._BC_1_2d[idx, :], self._BC_1_2u[idx, :]
+            U = np.reshape(KIgrid[1:-1, 1:-1], (m1 * m2, 1), order='F') + dt / self.param.year_base * self._update_boundary_(KIgrid)
+            KIgrid[1:-1, 1:-1] = np.reshape(iluA.solve(U), (m2, m1), order='F')
+
+            NKIgrid = NKIcube[idx + 1].copy()
+            NKIgrid[:, 0], NKIgrid[:, -1] = self._BC_1d_2[idx, :], self._BC_1u_2[idx, :]
+            NKIgrid[0, :], NKIgrid[-1, :] = self._BC_1_2d[idx, :], self._BC_1_2u[idx, :]
+            U = np.reshape(NKIgrid[1:-1, 1:-1], (m1 * m2, 1), order='F') + dt / self.param.year_base * self._update_boundary_(NKIgrid)
+            NKIgrid[1:-1, 1:-1] = np.reshape(iluA.solve(U), (m2, m1), order='F')
+
+            NKIcube[idx] = NKIgrid
+        return KIcube, NKIcube
 
     def _solve_(self):
-        invM = np.linalg.inv(self._M2)
+        m1, m2 = self._Ns1 - 1, self._Ns2 - 1
+        iluA = spilu(self._M, drop_tol=1e-10, fill_factor=100)
 
         KO_idx = np.searchsorted(self.Tvec, self._T_KO)
         KI_idx = np.searchsorted(self.Tvec, self._T_KI)
 
+        self.KIcube, self.NKIcube = [self.KIgrid.copy()], [self.NKIgrid.copy()]
         for j in tqdm(list(reversed(np.arange(self._Nt))), leave=False):
 
             if j + 1 in KO_idx:
-                self.KIgrid[self._S_KO, j + 1] = (self._Rbt_KO[np.where(KO_idx == j + 1)] - self._IntVec[j + 1] + self._EnhVec[self._S_KO]) * self.param.notional
-                self.NKIgrid[self._S_KO, j + 1] = self.KIgrid[self._S_KO, j + 1]
+                self.KIgrid[self._S_KO] = (self._Rbt_KO[np.where(KO_idx == j + 1)]) * self.param.notional
+                self.NKIgrid[self._S_KO] = self.KIgrid[self._S_KO]
 
-            U = self._M1.dot(self.KIgrid[1: -1, j + 1])
-            U[0] += self._theta * self._l[0] * self.dt / self.param.year_base * self.KIgrid[0, j] + (1 - self._theta) * self._l[0] * self.dt / self.param.year_base * self.KIgrid[0, j + 1]
-            U[-1] += self._theta * self._u[-1] * self.dt / self.param.year_base * self.KIgrid[-1, j] + (1 - self._theta) * self._u[-1] * self.dt / self.param.year_base * self.KIgrid[-1, j + 1]
-            self.KIgrid[1: -1, j] = np.dot(invM, U)
+            self.KIgrid[:, 0], self.KIgrid[:, -1] = self._BC_1d_2[j, :], self._BC_1u_2[j, :]
+            self.KIgrid[0, :], self.KIgrid[-1, :] = self._BC_1_2d[j, :], self._BC_1_2u[j, :]
+            U = np.reshape(self.KIgrid[1:-1, 1:-1], (m1 * m2, 1), order='F') + self.dt / self.param.year_base * self._update_boundary_(self.KIgrid)
+            self.KIgrid[1:-1, 1:-1] = np.reshape(iluA.solve(U), (m2, m1), order='F')
 
             if j + 1 in KI_idx:
-                self.NKIgrid[self._S_KI, j + 1] = self.KIgrid[self._S_KI, j + 1]
+                self.NKIgrid[self._S_KI] = self.KIgrid[self._S_KI]
 
-            U = self._M1.dot(self.NKIgrid[1: -1, j + 1])
-            U[0] += self._theta * self._l[0] * self.dt / self.param.year_base * self.NKIgrid[0, j] + (1 - self._theta) * self._l[0] * self.dt / self.param.year_base * self.NKIgrid[0, j + 1]
-            U[-1] += self._theta * self._u[-1] * self.dt / self.param.year_base * self.NKIgrid[-1, j] + (1 - self._theta) * self._u[-1] * self.dt / self.param.year_base * self.NKIgrid[-1, j + 1]
-            self.NKIgrid[1: -1, j] = np.dot(invM, U)
-
-            # if j in KO_idx:
-            #     self.KIgrid[self._S_KO, j] = (self._Rbt_KO[np.where(KO_idx == j)] - self._IntVec[j] + self._EnhVec[self._S_KO]) * self.param.notional
-            #     self.NKIgrid[self._S_KO, j] = self.KIgrid[self._S_KO, j]
-            #
-            # if j in KI_idx:
-            #     self.NKIgrid[self._S_KI, j] = self.KIgrid[self._S_KI, j]
+            self.NKIgrid[:, 0], self.NKIgrid[:, -1] = self._BC_1d_2[j, :], self._BC_1u_2[j, :]
+            self.NKIgrid[0, :], self.NKIgrid[-1, :] = self._BC_1_2d[j, :], self._BC_1_2u[j, :]
+            U = np.reshape(self.NKIgrid[1:-1, 1:-1], (m1 * m2, 1), order='F') + self.dt / self.param.year_base * self._update_boundary_(self.NKIgrid)
+            self.NKIgrid[1:-1, 1:-1] = np.reshape(iluA.solve(U), (m2, m1), order='F')
+
+            self.KIcube.append(self.KIgrid.copy())
+            self.NKIcube.append(self.NKIgrid.copy())
+
+        self.KIcube, self.NKIcube = np.array(self.KIcube[::-1]), np.array(self.NKIcube[::-1])
+        self.KIcube, self.NKIcube = self._solve_intraday_(idx=0, KIcube=self.KIcube, NKIcube=self.NKIcube)
+        self.KIgrid, self.NKIgrid = self.KIcube[0], self.NKIcube[0]
 
-        if self._Tau > 0 and self._Nt > 0:
-            dt = 1 - self._Tau
-            M1 = self._I + (1 - self._theta) * dt / self.param.year_base * self._A
-            M2 = self._I - self._theta * dt / self.param.year_base * self._A
-            invM = np.linalg.inv(M2)
-
-            U = M1.dot(self.KIgrid[1: -1, 1])
-            U[0] += self._theta * self._l[0] * dt / self.param.year_base * self.KIgrid[0, 0] + (1 - self._theta) * self._l[0] * dt / self.param.year_base * self.KIgrid[0, 1]
-            U[-1] += self._theta * self._u[-1] * dt / self.param.year_base * self.KIgrid[-1, 0] + (1 - self._theta) * self._u[-1] * dt / self.param.year_base * self.KIgrid[-1, 1]
-            self.KIgrid[1: -1, 0] = np.dot(invM, U)
-
-            U = self._M1.dot(self.NKIgrid[1: -1, 1])
-            U[0] += self._theta * self._l[0] * dt / self.param.year_base * self.NKIgrid[0, 0] + (1 - self._theta) * self._l[0] * dt / self.param.year_base * self.NKIgrid[0, 1]
-            U[-1] += self._theta * self._u[-1] * dt / self.param.year_base * self.NKIgrid[-1, 0] + (1 - self._theta) * self._u[-1] * dt / self.param.year_base * self.NKIgrid[-1, 1]
-            self.NKIgrid[1: -1, 0] = np.dot(invM, U)
+        if self._Nt > 1:
+            TempKIcube, TempNKIcube = self._solve_intraday_(idx=0, KIcube=self.KIcube[1:], NKIcube=self.NKIcube[1:])
+        else:
+            TempKIcube, TempNKIcube = self.KIcube[self._Nt:], self.NKIcube[self._Nt:]
+        self.T1KIgrid, self.T1NKIgrid = TempKIcube[0], TempNKIcube[0]
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/barrier/basket_discrete_barrier_binary_as.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from ..one_asset_option_base import *
-from ..touch.one_touch_as import OneTouch
+from ..barrier.basket_barrier_binary_as import BasketBarrierBinary
 
 
-class DiscreteOneTouch(OneAssetOptionBase):
-    """
-    离散单触碰期权解析解
-    """
+class BasketDiscreteBarrierBinary(OneAssetOptionBase):
 
     def __init__(self, param):
         super().__init__(param)
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         dt = self.param.obs_freq / self.param.year_base
         adjust = 0.5826 * self.param.volatility * math.sqrt(dt)
         if self.param.barrier_type == BarrierType.UP and time_to_expiry > 0:
-            self.param.barrier_price = self.param.barrier_price * np.exp(adjust)
+            self.param.adjust_barrier_price = self.param.barrier_price + adjust
         elif self.param.barrier_type == BarrierType.DOWN and time_to_expiry > 0:
-            self.param.barrier_price = self.param.barrier_price * np.exp(-adjust)
+            self.param.adjust_barrier_price = self.param.barrier_price - adjust
+        else:
+            self.param.adjust_barrier_price = self.param.barrier_price
 
     def __calculate_present_value__(self) -> float:
         param = Params()
+        param['option_type'] = self.param.option_type
+        param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
-        param['barrier_price'] = self.param.barrier_price
+        param['strike_price'] = self.param.strike_price
+        param['barrier_price'] = self.param.adjust_barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
-        param['dividend'] = self.param.dividend
         param['volatility'] = self.param.volatility
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['year_base'] = self.param.year_base
         param['barrier_type'] = self.param.barrier_type
         param['knock_type'] = self.param.knock_type
         param['is_knock_in'] = self.param.is_knock_in
-        param['rebate_type'] = self.param.rebate_type
-        param['rebate'] = self.param.rebate
-        pricer = OneTouch(param)
+        param['payoff'] = self.param.payoff
+        pricer = BasketBarrierBinary(param)
         return pricer.present_value()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.5.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.2/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.5.1/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,81 +15,100 @@
 ht_pricing_module/api_and_utils/protos/__init__.py
 ht_pricing_module/api_and_utils/protos/pricer.proto
 ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
 ht_pricing_module/api_and_utils/protos/google/api/http.proto
 ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
 ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
 ht_pricing_module/finite_difference_engine/__init__.py
-ht_pricing_module/finite_difference_engine/crank_nicolson_american.py
-ht_pricing_module/finite_difference_engine/crank_nicolson_european.py
-ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py
-ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-ht_pricing_module/finite_difference_engine/fully_explicit_european.py
-ht_pricing_module/finite_difference_engine/fully_implicit_european.py
+ht_pricing_module/finite_difference_engine/one_asset_crank_nicolson_american.py
+ht_pricing_module/finite_difference_engine/one_asset_crank_nicolson_european.py
+ht_pricing_module/finite_difference_engine/one_asset_explicit_european.py
+ht_pricing_module/finite_difference_engine/one_asset_fd_generator.py
+ht_pricing_module/finite_difference_engine/one_asset_fd_generator_parisian_snowball.py
+ht_pricing_module/finite_difference_engine/one_asset_fd_generator_snowball.py
+ht_pricing_module/finite_difference_engine/one_asset_implicit_european.py
+ht_pricing_module/finite_difference_engine/two_asset_fd_generator_snowball.py
 ht_pricing_module/monte_carlo_engine/__init__.py
 ht_pricing_module/monte_carlo_engine/mc_path_generator.py
 ht_pricing_module/multi_asset_pricing_module/__init__.py
 ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+ht_pricing_module/multi_asset_pricing_module/basket/__init__.py
+ht_pricing_module/multi_asset_pricing_module/basket/two_asset_basket_as.py
 ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
-ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+ht_pricing_module/multi_asset_pricing_module/quotient/two_asset_quotient_as.py
+ht_pricing_module/multi_asset_pricing_module/rainbow/__init__.py
+ht_pricing_module/multi_asset_pricing_module/rainbow/three_asset_best_of_as.py
+ht_pricing_module/multi_asset_pricing_module/rainbow/three_asset_worst_of_as.py
+ht_pricing_module/multi_asset_pricing_module/rainbow/two_asset_better_of_as.py
+ht_pricing_module/multi_asset_pricing_module/rainbow/two_asset_worse_of_as.py
+ht_pricing_module/multi_asset_pricing_module/snowball/__init__.py
+ht_pricing_module/multi_asset_pricing_module/snowball/two_asset_snowball_pde.py
 ht_pricing_module/one_asset_pricing_module/__init__.py
 ht_pricing_module/one_asset_pricing_module/exceptions.py
 ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
 ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+ht_pricing_module/one_asset_pricing_module/accumulator/basket_fixed_acc_as.py
+ht_pricing_module/one_asset_pricing_module/accumulator/basket_fixed_acc_barrier_as.py
+ht_pricing_module/one_asset_pricing_module/accumulator/basket_linear_acc_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_fusing_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
-ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
+ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_close_settle_as.py
 ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
 ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
 ht_pricing_module/one_asset_pricing_module/asian/__init__.py
 ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
 ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
 ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+ht_pricing_module/one_asset_pricing_module/asian/enhanced_asian_as.py
+ht_pricing_module/one_asset_pricing_module/asian/enhanced_asian_spread_as.py
 ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
-ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py
 ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
 ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
-ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py
+ht_pricing_module/one_asset_pricing_module/barrier/basket_barrier_as.py
+ht_pricing_module/one_asset_pricing_module/barrier/basket_barrier_binary_as.py
+ht_pricing_module/one_asset_pricing_module/barrier/basket_discrete_barrier_as.py
+ht_pricing_module/one_asset_pricing_module/barrier/basket_discrete_barrier_binary_as.py
 ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
 ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
-ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py
 ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py
 ht_pricing_module/one_asset_pricing_module/basket/__init__.py
 ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
 ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
 ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+ht_pricing_module/one_asset_pricing_module/binary/basket_binary_as.py
 ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
 ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
 ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
 ht_pricing_module/one_asset_pricing_module/forward/__init__.py
 ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+ht_pricing_module/one_asset_pricing_module/sharkfin/basket_sharkfin_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
 ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+ht_pricing_module/one_asset_pricing_module/snowball/parisian_snowball_mc.py
+ht_pricing_module/one_asset_pricing_module/snowball/parisian_snowball_pde.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py
-ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py
+ht_pricing_module/one_asset_pricing_module/snowball/snowball_small_mc.py
 ht_pricing_module/one_asset_pricing_module/spread/__init__.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
 ht_pricing_module/one_asset_pricing_module/touch/__init__.py
-ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py
 ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
-ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py
 ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
 ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
 ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
 ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
 ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
```

### Comparing `ht_pricing_module-0.3.2/setup.py` & `ht_pricing_module-0.5.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.3.2"
+VERSION = "0.5.1"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
@@ -25,13 +25,11 @@
       packages=filter_package(),
       include_package_data=True,
       platforms="any",
       install_requires=['numpy', 'scipy', 'pandas', 'grpcio==1.38.0', 'grpcio-status==1.38.0',
                         'grpcio-tools==1.38.0', 'protobuf==3.17.3']
       )
 
+# user, pypi2023
 # py -m build
-# python .\setup.py bdist_egg
-# py -m twine upload .\dist\*
-# py -m twine upload --repository testpypi dist/*
-# pip install --upgrade ht-pricing-module -i https://pypi.python.org/simple
-# pip install ht-pricing-module -i https://test.pypi.org/simple/
+# py -m twine upload .\dist\* --repository-url=http://10.17.75.129:9001
+# pip install ht-pricing-module --upgrade -i http://10.17.75.129:9001 --trusted-host 10.17.75.129
```


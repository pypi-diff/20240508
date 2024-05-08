# Comparing `tmp/buildz-0.5.3.tar.gz` & `tmp/buildz-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.5.3.tar", last modified: Sun Apr 28 15:57:38 2024, max compression
+gzip compressed data, was "buildz-0.5.4.tar", last modified: Wed May  8 03:06:37 2024, max compression
```

## Comparing `buildz-0.5.3.tar` & `buildz-0.5.4.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2705 2024-04-28 15:57:38.417507 buildz-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.323733 buildz-0.5.3/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.3/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.3/buildz/__main__.py
--rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.5.3/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.3/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.3/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.5.3/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.3/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.3/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.3/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.3/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.3/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.3/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.3/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.3/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.3/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.3/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.3/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.3/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.3/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.3/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.3/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.3/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.3/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/fz/
--rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.3/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.3/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.5.3/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.3/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.3/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.3/buildz/ioc/base.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.3/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.354985 buildz-0.5.3/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.3/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.3/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.3/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.370605 buildz-0.5.3/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.3/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.386231 buildz-0.5.3/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/deal_lists.js
--rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/xfile_defaults.js
--rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.3/buildz/ioc/ioc_deal/conf/xfile_lists.js
--rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/deal.py
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.3/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      828 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      932 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1021 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     6134 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1087 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.3/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1082 2024-04-25 13:54:58.000000 buildz-0.5.3/buildz/ioc/ioc_deal/xfile.py
--rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.3/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.386231 buildz-0.5.3/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.3/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.3/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.386231 buildz-0.5.3/buildz/xf/
--rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.3/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.3/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0      960 2024-04-25 14:34:17.000000 buildz-0.5.3/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.401853 buildz-0.5.3/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.3/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.3/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.401853 buildz-0.5.3/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.3/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.3/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.3/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.3/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.3/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.3/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.3/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.3/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.3/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.3/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.3/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.3/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.3/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.3/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.401853 buildz-0.5.3/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.3/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.3/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.3/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     2055 2024-04-26 07:39:31.000000 buildz-0.5.3/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.3/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.3/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.3/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.3/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.3/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.3/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.3/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.5.3/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.3/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.3/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     3515 2024-04-26 08:09:20.000000 buildz-0.5.3/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.3/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.3/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.3/buildz/xf/loaderz/test1.py
--rw-rw-rw-   0        0        0     2009 2024-04-23 09:07:57.000000 buildz-0.5.3/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.3/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2746 2024-04-25 17:36:02.000000 buildz-0.5.3/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.3/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1477 2024-04-25 14:36:40.000000 buildz-0.5.3/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.3/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.3/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.417507 buildz-0.5.3/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.3/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.3/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.3/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.3/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.3/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.3/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.3/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.3/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:57:38.339356 buildz-0.5.3/buildz.egg-info/
--rw-rw-rw-   0        0        0     2705 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3751 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 15:57:38.000000 buildz-0.5.3/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 15:57:38.417507 buildz-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-04-28 15:56:06.000000 buildz-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2823 2024-05-08 03:06:37.033407 buildz-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.924044 buildz-0.5.4/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.4/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.4/buildz/__main__.py
+-rw-rw-rw-   0        0        0     2944 2024-05-07 11:40:11.000000 buildz-0.5.4/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.4/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.4/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.4/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.4/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.4/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.4/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.4/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.4/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.4/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.4/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.4/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.4/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.4/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.4/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.4/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.4/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.4/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.4/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.4/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.4/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/fz/
+-rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.4/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.4/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      629 2024-05-03 05:05:00.000000 buildz-0.5.4/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.4/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.4/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.4/buildz/ioc/base.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.4/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.4/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.4/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.4/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.986537 buildz-0.5.4/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.4/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.002166 buildz-0.5.4/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.4/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0     1038 2024-05-06 14:06:01.000000 buildz-0.5.4/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 08:29:26.000000 buildz-0.5.4/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1021 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6134 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1087 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.4/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.4/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.4/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.002166 buildz-0.5.4/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.4/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.4/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.002166 buildz-0.5.4/buildz/xf/
+-rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.4/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.4/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0      960 2024-05-03 05:07:16.000000 buildz-0.5.4/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.017784 buildz-0.5.4/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.4/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.4/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.017784 buildz-0.5.4/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.4/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.4/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.4/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.4/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.4/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.4/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.4/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.4/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.4/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.4/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.4/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.4/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.4/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.4/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.017784 buildz-0.5.4/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.4/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.4/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.4/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     2056 2024-05-07 13:50:27.000000 buildz-0.5.4/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.4/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.4/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.4/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.4/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.4/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.4/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.4/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     3313 2024-05-07 12:00:45.000000 buildz-0.5.4/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.4/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.4/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     3515 2024-04-26 08:09:20.000000 buildz-0.5.4/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.4/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.4/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.4/buildz/xf/loaderz/test1.py
+-rw-rw-rw-   0        0        0     2600 2024-05-06 14:14:08.000000 buildz-0.5.4/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.4/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2746 2024-05-07 11:58:30.000000 buildz-0.5.4/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.4/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.4/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.4/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.4/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.4/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.4/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.4/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.4/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.4/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.4/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.4/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.4/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2823 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3751 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:06:37.033407 buildz-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-05-08 03:04:03.000000 buildz-0.5.4/setup.py
```

### Comparing `buildz-0.5.3/LICENSE` & `buildz-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/PKG-INFO` & `buildz-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.3
-Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
+Version: 0.5.4
+Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
 Description-Content-Type: text/markdown
@@ -24,14 +24,16 @@
 代码关系:
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
     buildz.ioc需要buildz.xf和buildz.pyz
     buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
+持续更新中。。。
+
 PS: 对比了下json.loads（修改了下json的scanner.py，让它在纯python下运行，不然json.loads会更快）和目前的xf.loads(buildz.xf.readz.loads)的速度，xf.loads比json.loads慢7倍，可能是读字符串更频繁，方法调用更多（为了代码更结构化和容易修改），其实有一版更慢(buildz.xf.read.loads，废弃代码，后面看情况删掉)，慢100倍，因为只考虑结构化，没考虑列表增减开销
 
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
@@ -41,9 +43,11 @@
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
     buildz.ioc use buildz.xf and buildz.pyz
     buildz.tz: some tools, only contains "myerse diff algorithm" now
     buildz.demo use all other modules
 
 run python -m buildz to see help
 
+continue updating...
+
 PS: testing speed on json.loads(has modified scanner.py in json module to make it purely run on Python, which make it run slower) and xf.loads(real func is buildz.xf.readz.loads), xf.loads takes 7 times longer than json.loads, it may cost by more func calls and more string cutting and reading(to make codes more structuring and easier to update)
 ```
```

### Comparing `buildz-0.5.3/README.md` & `buildz-0.5.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 代码关系:
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
     buildz.ioc需要buildz.xf和buildz.pyz
     buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
+持续更新中。。。
+
 PS: 对比了下json.loads（修改了下json的scanner.py，让它在纯python下运行，不然json.loads会更快）和目前的xf.loads(buildz.xf.readz.loads)的速度，xf.loads比json.loads慢7倍，可能是读字符串更频繁，方法调用更多（为了代码更结构化和容易修改），其实有一版更慢(buildz.xf.read.loads，废弃代码，后面看情况删掉)，慢100倍，因为只考虑结构化，没考虑列表增减开销
 
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
@@ -28,9 +30,11 @@
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
     buildz.ioc use buildz.xf and buildz.pyz
     buildz.tz: some tools, only contains "myerse diff algorithm" now
     buildz.demo use all other modules
 
 run python -m buildz to see help
 
+continue updating...
+
 PS: testing speed on json.loads(has modified scanner.py in json module to make it purely run on Python, which make it run slower) and xf.loads(real func is buildz.xf.readz.loads), xf.loads takes 7 times longer than json.loads, it may cost by more func calls and more string cutting and reading(to make codes more structuring and easier to update)
 ```
```

### Comparing `buildz-0.5.3/buildz/argx.py` & `buildz-0.5.4/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/ioc/deal.py` & `buildz-0.5.4/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/ioc/help.py` & `buildz-0.5.4/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/myers/deal.py` & `buildz-0.5.4/buildz/demo/myers/deal.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,26 @@
             else:
                 for stp in stps:
                     c = stp[-1]
                     if type(c)==bytes:
                         stp[-1] = c.decode()
                 stps = "t"+xf.dumps(stps)
                 stps = stps.encode()
-            fz.write(fp_step, stps)
+            fz.write(stps, fp_step)
             print("done diff")
         elif opt == 'update':
             bs1 = fz.read(fp1).decode("utf-8")
             bs_step = fz.read(fp_step)
             mark_encode = bs_step[:1] == b'e'
             bs_step= bs_step[1:]
             if mark_encode:
                 stps = tz.m_decode(bs_step)
             else:
                 stps = xf.loads(bs_step.decode())
             bs2 = tz.m_update(bs1, stps,split=spt).encode("utf-8")
-            fz.write(fp2, bs2)
+            fz.write(bs2, fp2)
             print("done update")
         else:
             print(f"unexpect opt: {opt}")
     pass
 
 pass
```

### Comparing `buildz-0.5.3/buildz/demo/res/conf/main.js` & `buildz-0.5.4/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/res/help/ioc.js` & `buildz-0.5.4/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/res/help/myers.js` & `buildz-0.5.4/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/res/help/search.js` & `buildz-0.5.4/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/res/help/xf.js` & `buildz-0.5.4/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/res/test.js` & `buildz-0.5.4/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/search/deal.py` & `buildz-0.5.4/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/demo/test.py` & `buildz-0.5.4/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/fz/dirz.py` & `buildz-0.5.4/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/fz/fio.py` & `buildz-0.5.4/buildz/fz/fio.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,20 @@
             if len(bs)==0:
                 break
             yield bs
 
 pass
 reads=freads
 
-def fwrite(fp, ct, mode = 'wb'):
+def fwrite(ct, fp, mode = 'wb'):
     with open(fp, mode) as f:
         f.write(ct)
 
 pass
 write = fwrite
-def fwrites(fp, cts, mode = 'wb'):
+def fwrites(cts, fp, mode = 'wb'):
     with open(fp, mode) as f:
         for ct in cts:
             f.write(ct)
 
 pass
 writes = fwrites
```

### Comparing `buildz-0.5.3/buildz/fz/lsf.py` & `buildz-0.5.4/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc/base.py` & `buildz-0.5.4/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc/conf.py` & `buildz-0.5.4/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc/confs.py` & `buildz-0.5.4/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.4/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/deal.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/ioc/ioc_deal/xfile.py` & `buildz-0.5.4/buildz/ioc/ioc_deal/xfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 join = os.path.join
 class XfileDeal(FormatDeal):
     """
     配置文件载入xfile/xf:
         {
             id:id
             type:xfile
-            filepath: fp 
-            # or fp: fp
+            filepath: item_conf(fp) 
+            # or fp: item_conf(fp)
         }
     简写:
         [[id, xfile], fp]
         [xfile, fp]
         [xf, fp]
     例:
         [xfile, test.js]
+        [xfile, [val, test.js]]
     """
     def init(self, fp_lists = None, fp_defaults = None):
         self.singles = {}
         self.sources = {}
         super().init("XfileDeal", fp_lists, fp_defaults, 
             join(dp, "conf", "xfile_lists.js"),
             join(dp, "conf", "xfile_defaults.js"))
@@ -31,11 +32,12 @@
         sid = edata.sid
         data = edata.data
         conf = edata.conf
         data = self.format(data)
         fp = xf.g(data, filepath=None)
         if fp is None:
             fp = xf.g(data, fp = fp)
+        fp = self.get_obj(fp, conf)
         rst = xf.loads(xf.fread(fp))
         return rst
 
 pass
```

### Comparing `buildz-0.5.3/buildz/pyz.py` & `buildz-0.5.4/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/tz/myers_diff.py` & `buildz-0.5.4/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/file.py` & `buildz-0.5.4/buildz/xf/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,12 +36,12 @@
 pass
 def fread_c(filepath, coding = 'utf-8'):
     s = bread(filepath)
     return decode_c(s, coding)
 
 pass
 
-def fwrite(filepath, content, mode = 'w'):
+def fwrite(content, filepath, mode = 'w'):
     with open(filepath, mode) as f:
         f.write(content)
 
 pass
```

### Comparing `buildz-0.5.3/buildz/xf/loader/base.py` & `buildz-0.5.4/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/buffer.py` & `buildz-0.5.4/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/listz.py` & `buildz-0.5.4/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/lr.py` & `buildz-0.5.4/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.4/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.4/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.4/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/reval.py` & `buildz-0.5.4/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/setz.py` & `buildz-0.5.4/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/spt.py` & `buildz-0.5.4/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/deal/strz.py` & `buildz-0.5.4/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/item.py` & `buildz-0.5.4/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/mg.py` & `buildz-0.5.4/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loader/pos.py` & `buildz-0.5.4/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/base.py` & `buildz-0.5.4/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/buffer.py` & `buildz-0.5.4/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/lr.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         cl = buffer.read(self.ll)
         if self.left!=cl:
             return False
         _arr = []
         rm = buffer.full().strip()
         buffer.clean2read(self.ll)
         if len(rm)>0:
-            arr.append(item.Item(rm, type="", is_val=False))
+            _arr.append(item.Item(rm, type="", is_val=False))
         while True:
             cr = buffer.read(self.lr)
             if cr == self.right:
                 rm = buffer.full().strip()
                 buffer.clean2read(self.lr)
                 break
             if not mg.deal(buffer, _arr):
```

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/lrval.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/mapz.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/nextz.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/deal/strz.py` & `buildz-0.5.4/buildz/xf/loaderz/deal/strz.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         while True:
             if do_judge and self.right == buffer.rget(self.lr):
                 break
             c = buffer.read_cache(1)
             if do_judge and c == self.label_et:
                 mark_et += 1
             if len(c)==0:
+                if self.single_line and self.note:
+                    break
                 raise Exception(f"unexcept string end while reading str")
             do_judge = 1
             if c == self.label_l2:
                 mark_l2 = 1
                 do_judge = 0
                 c = buffer.read_cache(1)
                 if len(c)==0:
```

### Comparing `buildz-0.5.3/buildz/xf/loaderz/item.py` & `buildz-0.5.4/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/mg.py` & `buildz-0.5.4/buildz/xf/loaderz/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/pos.py` & `buildz-0.5.4/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/loaderz/test.py` & `buildz-0.5.4/buildz/xf/loaderz/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/mapz.py` & `buildz-0.5.4/buildz/xf/mapz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,163 @@
 00000000: 0d0a 6465 6620 6765 7428 6f62 6a2c 206b  ..def get(obj, k
 00000010: 6579 2c20 6465 6661 756c 743d 4e6f 6e65  ey, default=None
 00000020: 293a 0d0a 2020 2020 6966 206b 6579 206e  ):..    if key n
 00000030: 6f74 2069 6e20 6f62 6a3a 0d0a 2020 2020  ot in obj:..    
 00000040: 2020 2020 7265 7475 726e 2064 6566 6175      return defau
 00000050: 6c74 0d0a 2020 2020 7265 7475 726e 206f  lt..    return o
 00000060: 626a 5b6b 6579 5d0d 0a0d 0a70 6173 730d  bj[key]....pass.
-00000070: 0a64 6566 2067 286f 626a 2c20 2a2a 6d61  .def g(obj, **ma
-00000080: 7073 293a 0d0a 2020 2020 7273 7420 3d20  ps):..    rst = 
-00000090: 5b5d 0d0a 2020 2020 666f 7220 6b20 696e  []..    for k in
-000000a0: 206d 6170 733a 0d0a 2020 2020 2020 2020   maps:..        
-000000b0: 7620 3d20 6d61 7073 5b6b 5d0d 0a20 2020  v = maps[k]..   
-000000c0: 2020 2020 2069 6620 6b20 696e 206f 626a       if k in obj
-000000d0: 3a0d 0a20 2020 2020 2020 2020 2020 2076  :..            v
-000000e0: 203d 206f 626a 5b6b 5d0d 0a20 2020 2020   = obj[k]..     
-000000f0: 2020 2072 7374 2e61 7070 656e 6428 7629     rst.append(v)
-00000100: 0d0a 2020 2020 6966 206c 656e 2872 7374  ..    if len(rst
-00000110: 293d 3d31 3a0d 0a20 2020 2020 2020 2072  )==1:..        r
-00000120: 7374 203d 2072 7374 5b30 5d0d 0a20 2020  st = rst[0]..   
-00000130: 2072 6574 7572 6e20 7273 740d 0a0d 0a70   return rst....p
-00000140: 6173 730d 0a64 6566 2073 286f 626a 2c20  ass..def s(obj, 
-00000150: 2a2a 6d61 7073 293a 0d0a 2020 2020 666f  **maps):..    fo
-00000160: 7220 6b20 696e 206d 6170 733a 0d0a 2020  r k in maps:..  
-00000170: 2020 2020 2020 7620 3d20 6d61 7073 5b6b        v = maps[k
-00000180: 5d0d 0a20 2020 2020 2020 206f 626a 5b6b  ]..        obj[k
-00000190: 5d20 3d20 760d 0a0d 0a70 6173 730d 0a64  ] = v....pass..d
-000001a0: 6566 2073 6574 7328 6d61 7073 2c20 6b65  ef sets(maps, ke
-000001b0: 7973 2c20 7661 6c29 3a0d 0a20 2020 2069  ys, val):..    i
-000001c0: 6620 7479 7065 286b 6579 7329 2021 3d20  f type(keys) != 
-000001d0: 6c69 7374 3a0d 0a20 2020 2020 2020 206b  list:..        k
-000001e0: 6579 7320 3d20 5b6b 6579 735d 0d0a 2020  eys = [keys]..  
-000001f0: 2020 666f 7220 6b65 7920 696e 206b 6579    for key in key
-00000200: 735b 3a2d 315d 3a0d 0a20 2020 2020 2020  s[:-1]:..       
-00000210: 2069 6620 6b65 7920 6e6f 7420 696e 206d   if key not in m
-00000220: 6170 733a 0d0a 2020 2020 2020 2020 2020  aps:..          
-00000230: 2020 6d61 7073 5b6b 6579 5d20 3d20 7b7d    maps[key] = {}
-00000240: 0d0a 2020 2020 2020 2020 6d61 7073 203d  ..        maps =
-00000250: 206d 6170 735b 6b65 795d 0d0a 2020 2020   maps[key]..    
-00000260: 6d61 7073 5b6b 6579 735b 2d31 5d5d 203d  maps[keys[-1]] =
-00000270: 2076 616c 0d0a 0d0a 7061 7373 0d0a 6465   val....pass..de
-00000280: 6620 6765 7473 286d 6170 732c 206b 6579  f gets(maps, key
-00000290: 732c 2064 6566 6175 6c74 203d 204e 6f6e  s, default = Non
-000002a0: 6529 3a0d 0a20 2020 2069 6620 7479 7065  e):..    if type
-000002b0: 286b 6579 7329 2021 3d20 6c69 7374 3a0d  (keys) != list:.
-000002c0: 0a20 2020 2020 2020 206b 6579 7320 3d20  .        keys = 
-000002d0: 5b6b 6579 735d 0d0a 2020 2020 666f 7220  [keys]..    for 
-000002e0: 6b65 7920 696e 206b 6579 733a 0d0a 2020  key in keys:..  
-000002f0: 2020 2020 2020 6966 206b 6579 206e 6f74        if key not
-00000300: 2069 6e20 6d61 7073 3a0d 0a20 2020 2020   in maps:..     
-00000310: 2020 2020 2020 2072 6574 7572 6e20 6465         return de
-00000320: 6661 756c 740d 0a20 2020 2020 2020 206d  fault..        m
-00000330: 6170 7320 3d20 6d61 7073 5b6b 6579 5d0d  aps = maps[key].
-00000340: 0a20 2020 2072 6574 7572 6e20 6d61 7073  .    return maps
-00000350: 0d0a 0d0a 7061 7373 0d0a 6465 6620 7265  ....pass..def re
-00000360: 6d6f 7665 7328 6d61 7073 2c20 6b65 7973  moves(maps, keys
-00000370: 293a 0d0a 2020 2020 6966 2074 7970 6528  ):..    if type(
-00000380: 6b65 7973 2920 213d 206c 6973 743a 0d0a  keys) != list:..
-00000390: 2020 2020 2020 2020 6b65 7973 203d 205b          keys = [
-000003a0: 6b65 7973 5d0d 0a20 2020 2061 7272 203d  keys]..    arr =
-000003b0: 205b 5d0d 0a20 2020 2066 6f72 206b 6579   []..    for key
-000003c0: 2069 6e20 6b65 7973 3a0d 0a20 2020 2020   in keys:..     
-000003d0: 2020 2069 6620 6b65 7920 6e6f 7420 696e     if key not in
-000003e0: 206d 6170 733a 0d0a 2020 2020 2020 2020   maps:..        
-000003f0: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
-00000400: 2020 2061 7272 2e61 7070 656e 6428 5b6d     arr.append([m
-00000410: 6170 732c 206b 6579 5d29 0d0a 2020 2020  aps, key])..    
-00000420: 2020 2020 6d61 7073 203d 206d 6170 735b      maps = maps[
-00000430: 6b65 795d 0d0a 2020 2020 6172 722e 7265  key]..    arr.re
-00000440: 7665 7273 6528 290d 0a20 2020 2066 6972  verse()..    fir
-00000450: 7374 3d31 0d0a 2020 2020 666f 7220 6d61  st=1..    for ma
-00000460: 7073 2c6b 6579 2069 6e20 6172 723a 0d0a  ps,key in arr:..
-00000470: 2020 2020 2020 2020 6966 2066 6972 7374          if first
-00000480: 206f 7220 6c65 6e28 6d61 7073 5b6b 6579   or len(maps[key
-00000490: 5d29 3d3d 303a 0d0a 2020 2020 2020 2020  ])==0:..        
-000004a0: 2020 2020 6465 6c20 6d61 7073 5b6b 6579      del maps[key
-000004b0: 5d0d 0a20 2020 2020 2020 2066 6972 7374  ]..        first
-000004c0: 3d30 0d0a 2020 2020 7265 7475 726e 204e  =0..    return N
-000004d0: 6f6e 650d 0a0d 0a70 6173 730d 0a64 6566  one....pass..def
-000004e0: 206c 326d 2861 7272 2c20 2a2a 6d61 7073   l2m(arr, **maps
-000004f0: 293a 0d0a 2020 2020 7273 7420 3d20 7b7d  ):..    rst = {}
-00000500: 0d0a 2020 2020 6920 3d20 300d 0a20 2020  ..    i = 0..   
-00000510: 2066 6f72 206b 2069 6e20 6d61 7073 3a0d   for k in maps:.
-00000520: 0a20 2020 2020 2020 2069 6620 693c 6c65  .        if i<le
-00000530: 6e28 6172 7229 3a0d 0a20 2020 2020 2020  n(arr):..       
-00000540: 2020 2020 2076 616c 203d 2061 7272 5b69       val = arr[i
-00000550: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
-00000560: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00000570: 6c20 3d20 6d61 7073 5b6b 5d0d 0a20 2020  l = maps[k]..   
-00000580: 2020 2020 2072 7374 5b6b 5d20 3d20 7661       rst[k] = va
-00000590: 6c0d 0a20 2020 2020 2020 2069 2b3d 310d  l..        i+=1.
-000005a0: 0a20 2020 2072 6574 7572 6e20 7273 740d  .    return rst.
-000005b0: 0a0d 0a70 6173 730d 0a0d 0a64 6566 2064  ...pass....def d
-000005c0: 6565 705f 7570 6461 7465 2874 6172 6765  eep_update(targe
-000005d0: 742c 2073 7263 2c20 7265 706c 6163 653d  t, src, replace=
-000005e0: 3129 3a0d 0a20 2020 2022 2222 0d0a 2020  1):..    """..  
-000005f0: 2020 2020 2020 6469 6374 e6b7 b1e5 b182        dict......
-00000600: e69b b4e6 96b0 efbc 8c73 7263 5b6b 6579  .........src[key
-00000610: 5de6 98af 6469 6374 e5b0 b1e6 b7b1 e585  ]...dict........
-00000620: a5e6 9bb4 e696 b0ef bc8c e590 a6e5 8899  ................
-00000630: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00000640: 7263 e69c 89e8 808c 6d61 7073 e6b2 a1e6  rc......maps....
-00000650: 9c89 e5b0 b1e6 9bbf e68d a2ef bc8c e590  ................
-00000660: a6e5 8899 efbc 9a0d 0a20 2020 2020 2020  .........       
-00000670: 2020 2020 2020 2020 2072 6570 6c61 6365           replace
-00000680: 3d31 e5b0 b1e6 9bbf e68d a20d 0a20 2020  =1...........   
-00000690: 2022 2222 0d0a 2020 2020 666f 7220 6b20   """..    for k 
-000006a0: 696e 2073 7263 3a0d 0a20 2020 2020 2020  in src:..       
-000006b0: 2076 616c 203d 2073 7263 5b6b 5d0d 0a20   val = src[k].. 
-000006c0: 2020 2020 2020 2069 6620 6b20 6e6f 7420         if k not 
-000006d0: 696e 2074 6172 6765 743a 0d0a 2020 2020  in target:..    
-000006e0: 2020 2020 2020 2020 7461 7267 6574 5b6b          target[k
-000006f0: 5d20 3d20 7661 6c0d 0a20 2020 2020 2020  ] = val..       
-00000700: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00000710: 2020 2020 2020 206d 7661 6c20 3d20 7461         mval = ta
-00000720: 7267 6574 5b6b 5d0d 0a20 2020 2020 2020  rget[k]..       
-00000730: 2069 6620 7479 7065 286d 7661 6c29 203d   if type(mval) =
-00000740: 3d20 6469 6374 2061 6e64 2074 7970 6528  = dict and type(
-00000750: 7661 6c29 3d3d 6469 6374 3a0d 0a20 2020  val)==dict:..   
-00000760: 2020 2020 2020 2020 2064 6565 705f 7570           deep_up
-00000770: 6461 7465 286d 7661 6c2c 2076 616c 2c20  date(mval, val, 
-00000780: 7265 706c 6163 6529 0d0a 2020 2020 2020  replace)..      
-00000790: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000007a0: 2020 2020 2069 6620 7265 706c 6163 653a       if replace:
-000007b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000007c0: 2020 7461 7267 6574 5b6b 5d20 3d20 7661    target[k] = va
-000007d0: 6c0d 0a0d 0a70 6173 73                   l....pass
+00000070: 0a64 6566 2067 6574 6628 6f62 6a2c 206b  .def getf(obj, k
+00000080: 6579 2c20 6663 293a 0d0a 2020 2020 6966  ey, fc):..    if
+00000090: 206b 6579 206e 6f74 2069 6e20 6f62 6a3a   key not in obj:
+000000a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000000b0: 2066 6328 290d 0a20 2020 2072 6574 7572   fc()..    retur
+000000c0: 6e20 6f62 6a5b 6b65 795d 0d0a 0d0a 7061  n obj[key]....pa
+000000d0: 7373 0d0a 6465 6620 6766 6e28 6f62 6a2c  ss..def gfn(obj,
+000000e0: 202a 2a6d 6170 7329 3a0d 0a20 2020 2072   **maps):..    r
+000000f0: 7374 203d 205b 5d0d 0a20 2020 2066 6f72  st = []..    for
+00000100: 206b 2069 6e20 6d61 7073 3a0d 0a20 2020   k in maps:..   
+00000110: 2020 2020 2069 6620 6b20 696e 206f 626a       if k in obj
+00000120: 2061 6e64 206f 626a 5b6b 5d20 6973 206e   and obj[k] is n
+00000130: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00000140: 2020 2020 2020 7620 3d20 6f62 6a5b 6b5d        v = obj[k]
+00000150: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00000160: 0a20 2020 2020 2020 2020 2020 2076 203d  .            v =
+00000170: 206d 6170 735b 6b5d 2829 0d0a 2020 2020   maps[k]()..    
+00000180: 2020 2020 7273 742e 6170 7065 6e64 2876      rst.append(v
+00000190: 290d 0a20 2020 2069 6620 6c65 6e28 7273  )..    if len(rs
+000001a0: 7429 3d3d 313a 0d0a 2020 2020 2020 2020  t)==1:..        
+000001b0: 7273 7420 3d20 7273 745b 305d 0d0a 2020  rst = rst[0]..  
+000001c0: 2020 7265 7475 726e 2072 7374 0d0a 0d0a    return rst....
+000001d0: 7061 7373 0d0a 6465 6620 6766 286f 626a  pass..def gf(obj
+000001e0: 2c20 2a2a 6d61 7073 293a 0d0a 2020 2020  , **maps):..    
+000001f0: 7273 7420 3d20 5b5d 0d0a 2020 2020 666f  rst = []..    fo
+00000200: 7220 6b20 696e 206d 6170 733a 0d0a 2020  r k in maps:..  
+00000210: 2020 2020 2020 6966 206b 2069 6e20 6f62        if k in ob
+00000220: 6a3a 0d0a 2020 2020 2020 2020 2020 2020  j:..            
+00000230: 7620 3d20 6f62 6a5b 6b5d 0d0a 2020 2020  v = obj[k]..    
+00000240: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000250: 2020 2020 2020 2076 203d 206d 6170 735b         v = maps[
+00000260: 6b5d 2829 0d0a 2020 2020 2020 2020 7273  k]()..        rs
+00000270: 742e 6170 7065 6e64 2876 290d 0a20 2020  t.append(v)..   
+00000280: 2069 6620 6c65 6e28 7273 7429 3d3d 313a   if len(rst)==1:
+00000290: 0d0a 2020 2020 2020 2020 7273 7420 3d20  ..        rst = 
+000002a0: 7273 745b 305d 0d0a 2020 2020 7265 7475  rst[0]..    retu
+000002b0: 726e 2072 7374 0d0a 0d0a 7061 7373 0d0a  rn rst....pass..
+000002c0: 6465 6620 6728 6f62 6a2c 202a 2a6d 6170  def g(obj, **map
+000002d0: 7329 3a0d 0a20 2020 2072 7374 203d 205b  s):..    rst = [
+000002e0: 5d0d 0a20 2020 2066 6f72 206b 2069 6e20  ]..    for k in 
+000002f0: 6d61 7073 3a0d 0a20 2020 2020 2020 2076  maps:..        v
+00000300: 203d 206d 6170 735b 6b5d 0d0a 2020 2020   = maps[k]..    
+00000310: 2020 2020 6966 206b 2069 6e20 6f62 6a3a      if k in obj:
+00000320: 0d0a 2020 2020 2020 2020 2020 2020 7620  ..            v 
+00000330: 3d20 6f62 6a5b 6b5d 0d0a 2020 2020 2020  = obj[k]..      
+00000340: 2020 7273 742e 6170 7065 6e64 2876 290d    rst.append(v).
+00000350: 0a20 2020 2069 6620 6c65 6e28 7273 7429  .    if len(rst)
+00000360: 3d3d 313a 0d0a 2020 2020 2020 2020 7273  ==1:..        rs
+00000370: 7420 3d20 7273 745b 305d 0d0a 2020 2020  t = rst[0]..    
+00000380: 7265 7475 726e 2072 7374 0d0a 0d0a 7061  return rst....pa
+00000390: 7373 0d0a 6465 6620 7328 6f62 6a2c 202a  ss..def s(obj, *
+000003a0: 2a6d 6170 7329 3a0d 0a20 2020 2066 6f72  *maps):..    for
+000003b0: 206b 2069 6e20 6d61 7073 3a0d 0a20 2020   k in maps:..   
+000003c0: 2020 2020 2076 203d 206d 6170 735b 6b5d       v = maps[k]
+000003d0: 0d0a 2020 2020 2020 2020 6f62 6a5b 6b5d  ..        obj[k]
+000003e0: 203d 2076 0d0a 0d0a 7061 7373 0d0a 6465   = v....pass..de
+000003f0: 6620 7365 7473 286d 6170 732c 206b 6579  f sets(maps, key
+00000400: 732c 2076 616c 293a 0d0a 2020 2020 6966  s, val):..    if
+00000410: 2074 7970 6528 6b65 7973 2920 213d 206c   type(keys) != l
+00000420: 6973 743a 0d0a 2020 2020 2020 2020 6b65  ist:..        ke
+00000430: 7973 203d 205b 6b65 7973 5d0d 0a20 2020  ys = [keys]..   
+00000440: 2066 6f72 206b 6579 2069 6e20 6b65 7973   for key in keys
+00000450: 5b3a 2d31 5d3a 0d0a 2020 2020 2020 2020  [:-1]:..        
+00000460: 6966 206b 6579 206e 6f74 2069 6e20 6d61  if key not in ma
+00000470: 7073 3a0d 0a20 2020 2020 2020 2020 2020  ps:..           
+00000480: 206d 6170 735b 6b65 795d 203d 207b 7d0d   maps[key] = {}.
+00000490: 0a20 2020 2020 2020 206d 6170 7320 3d20  .        maps = 
+000004a0: 6d61 7073 5b6b 6579 5d0d 0a20 2020 206d  maps[key]..    m
+000004b0: 6170 735b 6b65 7973 5b2d 315d 5d20 3d20  aps[keys[-1]] = 
+000004c0: 7661 6c0d 0a0d 0a70 6173 730d 0a64 6566  val....pass..def
+000004d0: 2067 6574 7328 6d61 7073 2c20 6b65 7973   gets(maps, keys
+000004e0: 2c20 6465 6661 756c 7420 3d20 4e6f 6e65  , default = None
+000004f0: 293a 0d0a 2020 2020 6966 2074 7970 6528  ):..    if type(
+00000500: 6b65 7973 2920 213d 206c 6973 743a 0d0a  keys) != list:..
+00000510: 2020 2020 2020 2020 6b65 7973 203d 205b          keys = [
+00000520: 6b65 7973 5d0d 0a20 2020 2066 6f72 206b  keys]..    for k
+00000530: 6579 2069 6e20 6b65 7973 3a0d 0a20 2020  ey in keys:..   
+00000540: 2020 2020 2069 6620 6b65 7920 6e6f 7420       if key not 
+00000550: 696e 206d 6170 733a 0d0a 2020 2020 2020  in maps:..      
+00000560: 2020 2020 2020 7265 7475 726e 2064 6566        return def
+00000570: 6175 6c74 0d0a 2020 2020 2020 2020 6d61  ault..        ma
+00000580: 7073 203d 206d 6170 735b 6b65 795d 0d0a  ps = maps[key]..
+00000590: 2020 2020 7265 7475 726e 206d 6170 730d      return maps.
+000005a0: 0a0d 0a70 6173 730d 0a64 6566 2072 656d  ...pass..def rem
+000005b0: 6f76 6573 286d 6170 732c 206b 6579 7329  oves(maps, keys)
+000005c0: 3a0d 0a20 2020 2069 6620 7479 7065 286b  :..    if type(k
+000005d0: 6579 7329 2021 3d20 6c69 7374 3a0d 0a20  eys) != list:.. 
+000005e0: 2020 2020 2020 206b 6579 7320 3d20 5b6b         keys = [k
+000005f0: 6579 735d 0d0a 2020 2020 6172 7220 3d20  eys]..    arr = 
+00000600: 5b5d 0d0a 2020 2020 666f 7220 6b65 7920  []..    for key 
+00000610: 696e 206b 6579 733a 0d0a 2020 2020 2020  in keys:..      
+00000620: 2020 6966 206b 6579 206e 6f74 2069 6e20    if key not in 
+00000630: 6d61 7073 3a0d 0a20 2020 2020 2020 2020  maps:..         
+00000640: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
+00000650: 2020 6172 722e 6170 7065 6e64 285b 6d61    arr.append([ma
+00000660: 7073 2c20 6b65 795d 290d 0a20 2020 2020  ps, key])..     
+00000670: 2020 206d 6170 7320 3d20 6d61 7073 5b6b     maps = maps[k
+00000680: 6579 5d0d 0a20 2020 2061 7272 2e72 6576  ey]..    arr.rev
+00000690: 6572 7365 2829 0d0a 2020 2020 6669 7273  erse()..    firs
+000006a0: 743d 310d 0a20 2020 2066 6f72 206d 6170  t=1..    for map
+000006b0: 732c 6b65 7920 696e 2061 7272 3a0d 0a20  s,key in arr:.. 
+000006c0: 2020 2020 2020 2069 6620 6669 7273 7420         if first 
+000006d0: 6f72 206c 656e 286d 6170 735b 6b65 795d  or len(maps[key]
+000006e0: 293d 3d30 3a0d 0a20 2020 2020 2020 2020  )==0:..         
+000006f0: 2020 2064 656c 206d 6170 735b 6b65 795d     del maps[key]
+00000700: 0d0a 2020 2020 2020 2020 6669 7273 743d  ..        first=
+00000710: 300d 0a20 2020 2072 6574 7572 6e20 4e6f  0..    return No
+00000720: 6e65 0d0a 0d0a 7061 7373 0d0a 6465 6620  ne....pass..def 
+00000730: 6c32 6d28 6172 722c 202a 2a6d 6170 7329  l2m(arr, **maps)
+00000740: 3a0d 0a20 2020 2072 7374 203d 207b 7d0d  :..    rst = {}.
+00000750: 0a20 2020 2069 203d 2030 0d0a 2020 2020  .    i = 0..    
+00000760: 666f 7220 6b20 696e 206d 6170 733a 0d0a  for k in maps:..
+00000770: 2020 2020 2020 2020 6966 2069 3c6c 656e          if i<len
+00000780: 2861 7272 293a 0d0a 2020 2020 2020 2020  (arr):..        
+00000790: 2020 2020 7661 6c20 3d20 6172 725b 695d      val = arr[i]
+000007a0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+000007b0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+000007c0: 203d 206d 6170 735b 6b5d 0d0a 2020 2020   = maps[k]..    
+000007d0: 2020 2020 7273 745b 6b5d 203d 2076 616c      rst[k] = val
+000007e0: 0d0a 2020 2020 2020 2020 692b 3d31 0d0a  ..        i+=1..
+000007f0: 2020 2020 7265 7475 726e 2072 7374 0d0a      return rst..
+00000800: 0d0a 7061 7373 0d0a 0d0a 6465 6620 6465  ..pass....def de
+00000810: 6570 5f75 7064 6174 6528 7461 7267 6574  ep_update(target
+00000820: 2c20 7372 632c 2072 6570 6c61 6365 3d31  , src, replace=1
+00000830: 293a 0d0a 2020 2020 2222 220d 0a20 2020  ):..    """..   
+00000840: 2020 2020 2064 6963 74e6 b7b1 e5b1 82e6       dict.......
+00000850: 9bb4 e696 b0ef bc8c 7372 635b 6b65 795d  ........src[key]
+00000860: e698 af64 6963 74e5 b0b1 e6b7 b1e5 85a5  ...dict.........
+00000870: e69b b4e6 96b0 efbc 8ce5 90a6 e588 993a  ...............:
+00000880: 0d0a 2020 2020 2020 2020 2020 2020 7372  ..            sr
+00000890: 63e6 9c89 e880 8c6d 6170 73e6 b2a1 e69c  c......maps.....
+000008a0: 89e5 b0b1 e69b bfe6 8da2 efbc 8ce5 90a6  ................
+000008b0: e588 99ef bc9a 0d0a 2020 2020 2020 2020  ........        
+000008c0: 2020 2020 2020 2020 7265 706c 6163 653d          replace=
+000008d0: 31e5 b0b1 e69b bfe6 8da2 0d0a 2020 2020  1...........    
+000008e0: 2222 220d 0a20 2020 2066 6f72 206b 2069  """..    for k i
+000008f0: 6e20 7372 633a 0d0a 2020 2020 2020 2020  n src:..        
+00000900: 7661 6c20 3d20 7372 635b 6b5d 0d0a 2020  val = src[k]..  
+00000910: 2020 2020 2020 6966 206b 206e 6f74 2069        if k not i
+00000920: 6e20 7461 7267 6574 3a0d 0a20 2020 2020  n target:..     
+00000930: 2020 2020 2020 2074 6172 6765 745b 6b5d         target[k]
+00000940: 203d 2076 616c 0d0a 2020 2020 2020 2020   = val..        
+00000950: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+00000960: 2020 2020 2020 6d76 616c 203d 2074 6172        mval = tar
+00000970: 6765 745b 6b5d 0d0a 2020 2020 2020 2020  get[k]..        
+00000980: 6966 2074 7970 6528 6d76 616c 2920 3d3d  if type(mval) ==
+00000990: 2064 6963 7420 616e 6420 7479 7065 2876   dict and type(v
+000009a0: 616c 293d 3d64 6963 743a 0d0a 2020 2020  al)==dict:..    
+000009b0: 2020 2020 2020 2020 6465 6570 5f75 7064          deep_upd
+000009c0: 6174 6528 6d76 616c 2c20 7661 6c2c 2072  ate(mval, val, r
+000009d0: 6570 6c61 6365 290d 0a20 2020 2020 2020  eplace)..       
+000009e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000009f0: 2020 2020 6966 2072 6570 6c61 6365 3a0d      if replace:.
+00000a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a10: 2074 6172 6765 745b 6b5d 203d 2076 616c   target[k] = val
+00000a20: 0d0a 0d0a 7061 7373                      ....pass
```

### Comparing `buildz-0.5.3/buildz/xf/read.py` & `buildz-0.5.4/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/readz.py` & `buildz-0.5.4/buildz/xf/readz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/stack.py` & `buildz-0.5.4/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/write.py` & `buildz-0.5.4/buildz/xf/write.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     else:
         cf.set(set=1, prev=1)
     mgs = build(json_format)
     return mgs.dump(obj, cf)
 
 pass
 
-def dumpf(filepath, obj, bytes = 0, format = 0, deep = 0, json_format= 0, mode = 'w'):
+def dumpf(obj, filepath, bytes = 0, format = 0, deep = 0, json_format= 0, mode = 'w'):
     s = dumps(obj, bytes = bytes, format = format, deep = deep, json_format= json_format)
-    file.fwrite(filepath, s, mode)
+    file.fwrite(s, filepath, mode)
 
 pass
 
 def dump(output, obj, *argv, **maps):
     rs = dumps(obj, *argv, **maps)
     output(rs)
```

### Comparing `buildz-0.5.3/buildz/xf/writer/base.py` & `buildz-0.5.4/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/writer/conf.py` & `buildz-0.5.4/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/writer/deal/listz.py` & `buildz-0.5.4/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.4/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/writer/deal/strz.py` & `buildz-0.5.4/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/writer/itemz.py` & `buildz-0.5.4/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/writer/mg.py` & `buildz-0.5.4/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz/xf/xargs.py` & `buildz-0.5.4/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/buildz.egg-info/PKG-INFO` & `buildz-0.5.4/buildz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.3
-Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
+Version: 0.5.4
+Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
 Description-Content-Type: text/markdown
@@ -24,14 +24,16 @@
 代码关系:
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
     buildz.ioc需要buildz.xf和buildz.pyz
     buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
+持续更新中。。。
+
 PS: 对比了下json.loads（修改了下json的scanner.py，让它在纯python下运行，不然json.loads会更快）和目前的xf.loads(buildz.xf.readz.loads)的速度，xf.loads比json.loads慢7倍，可能是读字符串更频繁，方法调用更多（为了代码更结构化和容易修改），其实有一版更慢(buildz.xf.read.loads，废弃代码，后面看情况删掉)，慢100倍，因为只考虑结构化，没考虑列表增减开销
 
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
@@ -41,9 +43,11 @@
     buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
     buildz.ioc use buildz.xf and buildz.pyz
     buildz.tz: some tools, only contains "myerse diff algorithm" now
     buildz.demo use all other modules
 
 run python -m buildz to see help
 
+continue updating...
+
 PS: testing speed on json.loads(has modified scanner.py in json module to make it purely run on Python, which make it run slower) and xf.loads(real func is buildz.xf.readz.loads), xf.loads takes 7 times longer than json.loads, it may cost by more func calls and more string cutting and reading(to make codes more structuring and easier to update)
 ```
```

### Comparing `buildz-0.5.3/buildz.egg-info/SOURCES.txt` & `buildz-0.5.4/buildz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildz-0.5.3/setup.py` & `buildz-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.5.3',
+    version = '0.5.4',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
-    description = "a json-base file format's read and write code by python, and codes to read and product object from configure file in such format",
+    description = "配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
     author_email = '1309458652@qq.com',
     packages = find_packages(),
     include_package_data = True,
     platforms = 'any',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


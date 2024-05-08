# Comparing `tmp/gotrackit-0.2.3.tar.gz` & `tmp/gotrackit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.2.3.tar", last modified: Tue May  7 06:29:21 2024, max compression
+gzip compressed data, was "gotrackit-0.2.4.tar", last modified: Wed May  8 07:31:42 2024, max compression
```

## Comparing `gotrackit-0.2.3.tar` & `gotrackit-0.2.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.036558 gotrackit-0.2.3/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     7782 2024-05-07 06:29:21.036558 gotrackit-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     7036 2024-05-07 06:17:50.000000 gotrackit-0.2.3/README.md
--rw-rw-rw-   0        0        0      795 2024-05-07 06:20:09.000000 gotrackit-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 06:29:21.036558 gotrackit-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.953780 gotrackit-0.2.3/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.958766 gotrackit-0.2.3/src/gotrackit/
--rw-rw-rw-   0        0        0    15805 2024-04-29 14:02:05.000000 gotrackit-0.2.3/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0    17874 2024-05-07 03:22:33.000000 gotrackit-0.2.3/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.3/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.3/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.966745 gotrackit-0.2.3/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.3/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.3/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.971732 gotrackit-0.2.3/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4275 2024-04-30 05:17:12.000000 gotrackit-0.2.3/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     8007 2024-04-14 02:50:11.000000 gotrackit-0.2.3/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.3/src/gotrackit/gps/GpsXfer.py
--rw-rw-rw-   0        0        0    22763 2024-05-07 03:27:27.000000 gotrackit-0.2.3/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.974724 gotrackit-0.2.3/src/gotrackit/map/
--rw-rw-rw-   0        0        0    19143 2024-05-07 03:27:27.000000 gotrackit-0.2.3/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    38187 2024-05-07 05:58:17.000000 gotrackit-0.2.3/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4848 2024-05-07 05:58:17.000000 gotrackit-0.2.3/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.975721 gotrackit-0.2.3/src/gotrackit/model/
--rw-rw-rw-   0        0        0    65946 2024-05-07 05:18:41.000000 gotrackit-0.2.3/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.981706 gotrackit-0.2.3/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.3/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    27388 2024-05-07 03:33:38.000000 gotrackit-0.2.3/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.983700 gotrackit-0.2.3/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.988686 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.990681 gotrackit-0.2.3/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.992676 gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.995668 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.001652 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.003646 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.007635 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.012627 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.014617 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.019604 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.020601 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    21421 2024-04-30 12:21:10.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.023593 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.024590 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     5758 2024-04-20 03:45:37.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.3/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.3/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.028581 gotrackit-0.2.3/src/gotrackit/netxfer/
--rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.3/src/gotrackit/netxfer/SumoConvert.py
--rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.3/src/gotrackit/netxfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.030575 gotrackit-0.2.3/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9156 2024-04-21 05:56:15.000000 gotrackit-0.2.3/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.034564 gotrackit-0.2.3/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.3/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.3/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    12123 2024-05-06 03:34:25.000000 gotrackit-0.2.3/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.3/src/gotrackit/tools/group.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.3/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.3/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.035561 gotrackit-0.2.3/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     7782 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3695 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.077210 gotrackit-0.2.4/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     7990 2024-05-08 07:31:42.076213 gotrackit-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7244 2024-05-08 07:07:22.000000 gotrackit-0.2.4/README.md
+-rw-rw-rw-   0        0        0      795 2024-05-08 07:22:19.000000 gotrackit-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:31:42.077210 gotrackit-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.000415 gotrackit-0.2.4/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.004404 gotrackit-0.2.4/src/gotrackit/
+-rw-rw-rw-   0        0        0    15805 2024-04-29 14:02:05.000000 gotrackit-0.2.4/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    17874 2024-05-07 03:22:33.000000 gotrackit-0.2.4/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.4/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.4/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.012383 gotrackit-0.2.4/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.4/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.4/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.016373 gotrackit-0.2.4/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4275 2024-04-30 05:17:12.000000 gotrackit-0.2.4/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0     8333 2024-05-07 13:58:22.000000 gotrackit-0.2.4/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.4/src/gotrackit/gps/GpsXfer.py
+-rw-rw-rw-   0        0        0    22763 2024-05-07 03:27:27.000000 gotrackit-0.2.4/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.019364 gotrackit-0.2.4/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    19826 2024-05-08 05:02:02.000000 gotrackit-0.2.4/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    38784 2024-05-08 07:13:14.000000 gotrackit-0.2.4/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4848 2024-05-07 05:58:17.000000 gotrackit-0.2.4/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.023353 gotrackit-0.2.4/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    53479 2024-05-08 07:15:53.000000 gotrackit-0.2.4/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.027343 gotrackit-0.2.4/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.4/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    27388 2024-05-07 03:33:38.000000 gotrackit-0.2.4/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.029338 gotrackit-0.2.4/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.033327 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.035322 gotrackit-0.2.4/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.036319 gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.042305 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.047290 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.048287 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.051279 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.056266 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.058261 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.062250 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.063248 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    21421 2024-04-30 12:21:10.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.065242 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.066239 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5758 2024-04-20 03:45:37.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.4/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.4/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.067237 gotrackit-0.2.4/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.4/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.4/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.071225 gotrackit-0.2.4/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9156 2024-05-07 23:25:32.000000 gotrackit-0.2.4/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.075216 gotrackit-0.2.4/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.4/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.4/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12123 2024-05-06 03:34:25.000000 gotrackit-0.2.4/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.4/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.4/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.4/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.076213 gotrackit-0.2.4/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     7990 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3695 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.2.3/LICENSE` & `gotrackit-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/PKG-INFO` & `gotrackit-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,55 +45,58 @@
 
 
 **版本状态：05.07已经更新: v0.2.3**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
 
-- 效率优化, 相较于v0.2.2小幅度提升
+- 地图匹配接口效率优化, 相较于v0.2.2小幅度提升
 
-- crs判断BUG修复、境外路网构建失败BUG修复
+- 地图匹配接口报错机制优化
 
-- 报错机制优化
+- 地图匹配接口移除html_fldr参数, 使用out_fldr替代
 
-- 输出文件目录指定参数html_fldr废除, 改为out_fldr
+- 地图匹配接口增加即时输出开关instant_output, 打开后, 每匹配完一条轨迹马上进行结果存储
 
-- 增加环路处理功能
-    
-- 增加匹配结果即时输出参数, 每匹配完一条轨迹可马上进行结果存储
+- 路网构建: crs判断BUG修复、境外路网构建失败BUG修复
+
+- 增加 环路 处理功能
+
+
+**不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.2效率将大幅度提升, 最高可以提升10倍的性能 !~
+~ v0.2.4(相较于0.2.1)效率将大幅度提升, 最高可以提升10倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.2版解算时间 |
-|----------------|----------|----------------|------------------|---------|------------|-------------|-----------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **3.3秒**  |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **1.7秒**    |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.4版解算时间 |
+|----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
+| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.87秒**   |
+| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.89秒**   |
 
 
-v0.2.2多核效率对比:
+v0.2.4多核效率对比:
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快96s解算完150条轨迹，平均每条轨迹0.64s，相较于1.7s再次提升了60%，在车辆数较多时，多核的效率提升很明显。
+基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快89s解算完150条轨迹，平均每条轨迹0.59s，相较于0.89s再次提升了30%，在车辆数较多时，多核的效率提升很明显。
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.2解算时间 |
+| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 300.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 139.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 120.3秒     |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 104.9秒     | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 96.4秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.5秒      | 
+| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 290.0秒     | 
+| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 130.6秒     |
+| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 113.3秒     |
+| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.3秒      | 
+| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 89.4秒      | 
+| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 91.5秒      | 
 
 
 <br>
 
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
```

### Comparing `gotrackit-0.2.3/README.md` & `gotrackit-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,55 +23,58 @@
 
 
 **版本状态：05.07已经更新: v0.2.3**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
 
-- 效率优化, 相较于v0.2.2小幅度提升
+- 地图匹配接口效率优化, 相较于v0.2.2小幅度提升
 
-- crs判断BUG修复、境外路网构建失败BUG修复
+- 地图匹配接口报错机制优化
 
-- 报错机制优化
+- 地图匹配接口移除html_fldr参数, 使用out_fldr替代
 
-- 输出文件目录指定参数html_fldr废除, 改为out_fldr
+- 地图匹配接口增加即时输出开关instant_output, 打开后, 每匹配完一条轨迹马上进行结果存储
 
-- 增加环路处理功能
-    
-- 增加匹配结果即时输出参数, 每匹配完一条轨迹可马上进行结果存储
+- 路网构建: crs判断BUG修复、境外路网构建失败BUG修复
+
+- 增加 环路 处理功能
+
+
+**不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.2效率将大幅度提升, 最高可以提升10倍的性能 !~
+~ v0.2.4(相较于0.2.1)效率将大幅度提升, 最高可以提升10倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.2版解算时间 |
-|----------------|----------|----------------|------------------|---------|------------|-------------|-----------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **3.3秒**  |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **1.7秒**    |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.4版解算时间 |
+|----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
+| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.87秒**   |
+| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.89秒**   |
 
 
-v0.2.2多核效率对比:
+v0.2.4多核效率对比:
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快96s解算完150条轨迹，平均每条轨迹0.64s，相较于1.7s再次提升了60%，在车辆数较多时，多核的效率提升很明显。
+基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快89s解算完150条轨迹，平均每条轨迹0.59s，相较于0.89s再次提升了30%，在车辆数较多时，多核的效率提升很明显。
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.2解算时间 |
+| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 300.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 139.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 120.3秒     |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 104.9秒     | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 96.4秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.5秒      | 
+| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 290.0秒     | 
+| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 130.6秒     |
+| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 113.3秒     |
+| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.3秒      | 
+| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 89.4秒      | 
+| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 91.5秒      | 
 
 
 <br>
 
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
```

### Comparing `gotrackit-0.2.3/pyproject.toml` & `gotrackit-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.2.3/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.4/src/gotrackit/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/MapMatch.py` & `gotrackit-0.2.4/src/gotrackit/MapMatch.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.4/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.4/src/gotrackit/generation/GpsGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.4/src/gotrackit/gps/GpsArray.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/gps/GpsTrip.py` & `gotrackit-0.2.4/src/gotrackit/gps/GpsTrip.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,18 +53,21 @@
         print(rf'{car_num} vehicles, cutting group...')
         for agent_id, group_gps_gdf in self.gps_points_gdf.groupby(agent_field):
             group_gps_gdf.sort_values(by=time_field, ascending=True, inplace=True)
 
             # 时间差和距离差
             group_gps_gdf[next_time_field] = group_gps_gdf[time_field].shift(-1).fillna(group_gps_gdf[time_field])
             group_gps_gdf[next_p_field] = group_gps_gdf[geometry_field].shift(-1).fillna(group_gps_gdf[geometry_field])
-            group_gps_gdf[time_gap_field] = group_gps_gdf.apply(
-                lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
-            group_gps_gdf[dis_gap_field] = group_gps_gdf.apply(
-                lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
+            group_gps_gdf[time_gap_field] = group_gps_gdf[next_time_field] - group_gps_gdf[time_field]
+            group_gps_gdf[time_gap_field] = group_gps_gdf[time_gap_field].apply(lambda t: t.seconds)
+            group_gps_gdf[dis_gap_field] = group_gps_gdf[next_p_field].distance(group_gps_gdf[geometry_field])
+            # group_gps_gdf[time_gap_field] = group_gps_gdf.apply(
+            #     lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
+            # group_gps_gdf[dis_gap_field] = group_gps_gdf.apply(
+            #     lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
 
             # 切分主行程
             group_gps_gdf['main_label'] = (group_gps_gdf[time_gap_field] > self.group_gap_threshold).astype(int)
             self.add_group(label_field='main_label', df=group_gps_gdf, agent_id=agent_id)
             group_gps_gdf.drop(columns=['main_label'], axis=1, inplace=True)
 
             for _, _gps_df in group_gps_gdf.groupby(group_field):
```

### Comparing `gotrackit-0.2.3/src/gotrackit/gps/GpsXfer.py` & `gotrackit-0.2.4/src/gotrackit/gps/GpsXfer.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.4/src/gotrackit/gps/LocGps.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/map/Link.py` & `gotrackit-0.2.4/src/gotrackit/map/Link.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         self.__double_single_mapping: dict[int, tuple[int, int, int, int]] = dict()
         self.__ft_link_mapping: dict[tuple[int, int], int] = dict()
 
         self.__graph = nx.DiGraph()
         self.__ud_graph = nx.Graph()
         self.__one_out_degree_nodes = None
         self.__link_ft_mapping: dict[int, tuple[int, int]] = dict()
+        self.__link_f_mapping: dict[int, int] = dict()
+        self.__link_t_mapping: dict[int, int] = dict()
         self.done_link_vec = False
 
     def check(self):
         assert self.link_gdf.crs.srs.upper() == self.geo_crs, \
             rf'Link层数据必须为WGS84 - EPSG:4326, 实际输入: {self.link_gdf.crs.srs}'
         gap_set = {net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                    net_field.TO_NODE_FIELD, net_field.DIRECTION_FIELD, self.weight_field,
@@ -90,22 +92,25 @@
         self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD] = list(self.__single_link_gdf.index)
 
     def renew_length(self):
         self.link_gdf[length_field] = self.link_gdf[geometry_field].length
 
     def init_link_from_existing_single_link(self, single_link_gdf: gpd.GeoDataFrame = None,
                                             ft_link_mapping: dict = None,
-                                            double_single_mapping: dict = None, link_ft_mapping: dict = None):
+                                            double_single_mapping: dict = None, link_ft_mapping: dict = None,
+                                            link_t_mapping: dict = None, link_f_mapping: dict = None):
         """通过给定的single_link_gdf初始化link, 用在子net的初始化上"""
         self.__single_link_gdf = single_link_gdf.copy()
 
         self.__double_single_mapping = double_single_mapping
         self.__ft_link_mapping = ft_link_mapping
         # single_link: (f, t)
         self.__link_ft_mapping = link_ft_mapping
+        self.__link_t_mapping = link_t_mapping
+        self.__link_f_mapping = link_f_mapping
 
     def create_single_link(self, link_gdf: gpd.GeoDataFrame):
         """
         基于原来路网创建单向路网, 并且建立映射表
         :return:
         """
         link_gdf[net_field.DIRECTION_FIELD] = link_gdf[net_field.DIRECTION_FIELD].astype(int)
@@ -131,14 +136,16 @@
                                             self.__single_link_gdf[net_field.DIRECTION_FIELD],
                                             self.__single_link_gdf[net_field.FROM_NODE_FIELD],
                                             self.__single_link_gdf[net_field.TO_NODE_FIELD])}
         self.__ft_link_mapping = {(f, t): single_link for f, t, single_link in
                                   zip(self.__single_link_gdf[net_field.FROM_NODE_FIELD],
                                       self.__single_link_gdf[net_field.TO_NODE_FIELD],
                                       self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD])}
+        self.__link_f_mapping = {v: k[0] for k, v in self.__ft_link_mapping.items()}
+        self.__link_t_mapping = {v: k[1] for k, v in self.__ft_link_mapping.items()}
 
     def create_graph(self, weight_field: str = None):
         """
         创建有向图
         :return:
         """
         edge_list = [(f, t, {weight_field: l}) for f, t, l in
@@ -390,13 +397,21 @@
     def link_series(self, link_id: int = None) -> gpd.GeoSeries:
         return self.link_gdf.loc[link_id, :].copy()
 
     @property
     def link_ft_map(self) -> dict[int, tuple[int, int]]:
         return self.__link_ft_mapping
 
+    @property
+    def link_f_map(self) -> dict[int, int]:
+        return self.__link_f_mapping
+
+    @property
+    def link_t_map(self) -> dict[int, int]:
+        return self.__link_t_mapping
+
     def vertex_degree(self, node: int = None) -> int:
         """无向图的节点度"""
         return self.__ud_graph.degree[node]
 
     def used_node(self) -> set[int]:
         return set(self.link_gdf[from_node_field]) | set(self.link_gdf[to_node_field])
```

### Comparing `gotrackit-0.2.3/src/gotrackit/map/Net.py` & `gotrackit-0.2.4/src/gotrackit/map/Net.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 class Net(object):
 
     @function_time_cost
     def __init__(self, link_path: str = None, node_path: str = None, link_gdf: gpd.GeoDataFrame = None,
                  node_gdf: gpd.GeoDataFrame = None, weight_field: str = 'length', init_from_existing: bool = False,
                  is_check: bool = True, create_single: bool = True, search_method: str = 'dijkstra',
                  ft_link_mapping: dict = None, double_single_mapping: dict = None, link_ft_mapping: dict = None,
+                 link_t_mapping: dict = None, link_f_mapping: dict = None,
                  not_conn_cost: float = 999.0, cache_path: bool = True, cache_id: bool = True,
                  is_sub_net: bool = False, fmm_cache: bool = False, cache_cn: int = 2, cache_slice: int = None,
                  fmm_cache_fldr: str = None,
                  cache_name: str = 'cache', recalc_cache: bool = True,
                  cut_off: float = 1200.0, max_cut_off: float = 5000.0, delete_circle: bool = True):
         """
         创建Net类
@@ -60,14 +61,16 @@
         :param node_gdf: 若指定了该参数, 则直接从内存中的gdf创建Net点层
         :param weight_field: 搜路权重字段
         :param create_single: 是否在初始化的时候创建single层
         :param search_method: 路径搜索方法, 'dijkstra'
         :param init_from_existing: 是否直接从内存中的gdf创建single_link_gdf, 该参数用于类内部创建子net, 用户不用关心该参数, 使用默认值即可
         :param double_single_mapping:
         :param link_ft_mapping:
+        :param link_f_mapping:
+        :param link_t_mapping:
         :param ft_link_mapping:
         :param not_conn_cost: 不连通路径的阻抗(m), 默认999.0米
         :param is_sub_net: 是否是子网络, 默认False
         :param fmm_cache: 是否启用路径预存储, 默认False
         :param cache_cn: 使用几个核能进行路径预计算, 默认2
         :param fmm_cache_fldr: 存储路径预处理结果的文件目录, 默认./
         :param recalc_cache: 是否重新计算FMM路径缓存, 默认True
@@ -131,15 +134,17 @@
                 self.__link.init_link()
         else:
             if create_single:
                 # for sub net
                 self.__link.init_link_from_existing_single_link(single_link_gdf=link_gdf,
                                                                 double_single_mapping=double_single_mapping,
                                                                 ft_link_mapping=ft_link_mapping,
-                                                                link_ft_mapping=link_ft_mapping)
+                                                                link_ft_mapping=link_ft_mapping,
+                                                                link_t_mapping=link_t_mapping,
+                                                                link_f_mapping=link_f_mapping)
         if is_check:
             self.check()
 
     @property
     def planar_crs(self):
         return self.__planar_crs
 
@@ -312,14 +317,22 @@
         return self.__link.bilateral_unidirectional_mapping
 
     @property
     def link_ft_map(self) -> dict[int, tuple[int, int]]:
         return self.__link.link_ft_map
 
     @property
+    def link_t_map(self) -> dict[int, int]:
+        return self.__link.link_t_map
+
+    @property
+    def link_f_map(self) -> dict[int, int]:
+        return self.__link.link_f_map
+
+    @property
     def available_link_id(self) -> int:
         return self.__link.available_link_id
 
     def get_ft_node_link_mapping(self):
         return self.__link.get_ft_link_mapping()
 
     @function_time_cost
@@ -351,15 +364,15 @@
         sub_node_gdf = self.__node.get_node_data().loc[sub_node_list, :].copy()
         sub_net = Net(link_gdf=sub_single_link_gdf,
                       node_gdf=sub_node_gdf,
                       weight_field=weight_field,
                       init_from_existing=True, is_check=False, cache_path=cache_path, cache_id=cache_id,
                       not_conn_cost=not_conn_cost, is_sub_net=True, fmm_cache=fmm_cache,
                       ft_link_mapping=self.get_ft_node_link_mapping(),
-                      link_ft_mapping=self.link_ft_map,
+                      link_ft_mapping=self.link_ft_map, link_f_mapping=self.link_f_map, link_t_mapping=self.link_t_map,
                       double_single_mapping=self.bilateral_unidirectional_mapping, cut_off=self.cut_off,
                       delete_circle=False)
         sub_net.init_net(stp_cost_cache_df=self.get_path_cache(), cache_prj_inf=self.get_prj_cache())
         return sub_net
 
     @property
     def graph(self) -> nx.DiGraph:
@@ -642,15 +655,15 @@
                 result = pool.apply_async(self.single_source_cache,
                                           args=(node_group[i], g, self.cut_off, self.weight_field, self.cache_slice))
                 result_list.append(result)
             pool.close()
             pool.join()
             for res in result_list:
                 done_stp_cost_df = pd.concat([done_stp_cost_df, res.get()])
-            done_stp_cost_df.reset_index(inplace=True, drop=False)
+            done_stp_cost_df.reset_index(inplace=True, drop=True)
         _ = self.__link.get_link_data()[[net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD,
                                          self.weight_field]].rename(
             columns={net_field.FROM_NODE_FIELD: o_node_field, net_field.TO_NODE_FIELD: d_node_field,
                      self.weight_field: cost_field})
         _[path_field] = _.apply(lambda row: [int(row[o_node_field]), int(row[d_node_field])], axis=1)
         done_stp_cost_df = pd.concat([_, done_stp_cost_df])
         del _
```

### Comparing `gotrackit-0.2.3/src/gotrackit/map/Node.py` & `gotrackit-0.2.4/src/gotrackit/map/Node.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/model/Markov.py` & `gotrackit-0.2.4/src/gotrackit/model/Markov.py`

 * *Files 13% similar despite different names*

```diff
@@ -269,22 +269,23 @@
                 cache_prj_info = self.net.get_prj_cache()
             else:
                 done_stp_cost_df = pd.DataFrame()
                 cache_prj_info = dict()
         else:
             done_stp_cost_df = self.net.get_path_cache()
             cache_prj_info = self.net.get_prj_cache()
-
+        single_link_f_map, single_link_t_map = self.net.link_f_map, self.net.link_t_map
         adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, prj_done_df, \
             done_stp_cost_df = \
             self.generate_transition_mat_beta(single_link_ft_df, self.gps_candidate_link,
                                               gps_pre_next_dis_df, g, self.net.search_method,
                                               self.net.weight_field, self.net.cache_path, self.net.not_conn_cost,
                                               done_stp_cost_df, is_sub_net, fmm_cache,
-                                              cut_off, max_cut_off, cache_prj_info, add_single_ft)
+                                              cut_off, max_cut_off, cache_prj_info, add_single_ft, single_link_f_map,
+                                              single_link_t_map)
         # print(len(done_stp_cost_df))
         ft_idx_map.reset_index(inplace=True, drop=True)
         s2s_route_l.reset_index(inplace=True, drop=True)
         self.__adj_seq_path_dict = adj_seq_path_dict
         self.__ft_idx_map = ft_idx_map
         self.__ft_transition_dict = ft_transition_dict
         self.__s2s_route_l = s2s_route_l
@@ -299,84 +300,67 @@
                                      gps_pre_next_dis_df: pd.DataFrame = None,
                                      g: nx.DiGraph = None,
                                      method: str = None, weight_field: str = 'length',
                                      cache_path: bool = True, not_conn_cost: float = 999.0,
                                      done_stp_cost_df: pd.DataFrame = None,
                                      is_sub_net: bool = True, fmm_cache: bool = False, cut_off: float = 600.0,
                                      max_cut_off: float = 2000.0, cache_prj_inf: dict = None,
-                                     add_single_ft: list[bool] = None) -> \
+                                     add_single_ft: list[bool] = None, link_f_map: dict = None,
+                                     link_t_map: dict = None) -> \
             tuple[dict, dict, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
         # K候选
         seq_k_candidate_info = \
             self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate, using_cache=fmm_cache,
                                      top_k=self.top_k, cache_prj_inf=cache_prj_inf)
         # print(rf'{len(seq_k_candidate_info)}个候选路段...')
         seq_k_candidate_info.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
+        now_source_node = set(seq_k_candidate_info[net_field.FROM_NODE_FIELD])
 
         seq_k_candidate_info['idx'] = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD)[
                                           net_field.SINGLE_LINK_ID_FIELD].rank(method='min').astype(int) - 1
 
         ft_idx_map = seq_k_candidate_info[[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'idx']].copy()
 
-        # ft_idx_map.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
         del seq_k_candidate_info['idx']
         del pre_seq_candidate
-
         seq_k_candidate = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD).agg(
             {net_field.SINGLE_LINK_ID_FIELD: list, gps_field.POINT_SEQ_FIELD: list,
-             net_field.FROM_NODE_FIELD: 'count'}).rename(
+             'route_dis': list, net_field.FROM_NODE_FIELD: 'count'}).rename(
             columns={gps_field.POINT_SEQ_FIELD: 'g_s', net_field.FROM_NODE_FIELD: 'count'})
         seq_len_dict = {s: l for s, l in zip(seq_k_candidate.index, seq_k_candidate['count'])}
-        gps_match_link_route_dis = seq_k_candidate_info[
-            [gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'route_dis']].copy()
         seq_k_candidate.rename(columns={net_field.SINGLE_LINK_ID_FIELD: markov_field.FROM_STATE,
+                                        'route_dis': 'from_route_dis',
                                         'g_s': gps_field.FROM_GPS_SEQ}, inplace=True)
 
         seq_k_candidate[markov_field.TO_STATE] = seq_k_candidate[markov_field.FROM_STATE].shift(-1)
         seq_k_candidate[gps_field.TO_GPS_SEQ] = seq_k_candidate[gps_field.FROM_GPS_SEQ].shift(-1)
-
+        seq_k_candidate['to_route_dis'] = seq_k_candidate['from_route_dis'].shift(-1)
         seq_k_candidate.dropna(subset=[markov_field.TO_STATE], inplace=True)
 
-        from_state = seq_k_candidate[[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ]].reset_index(drop=False).rename(
+        from_state = seq_k_candidate[[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ, 'from_route_dis']].reset_index(
+            drop=False).rename(
             columns={gps_field.POINT_SEQ_FIELD: 'g'}).explode(
-            column=[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ], ignore_index=True)
-
+            column=[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ, 'from_route_dis'], ignore_index=True)
         to_state = seq_k_candidate[
-            [markov_field.TO_STATE, gps_field.TO_GPS_SEQ]].reset_index(drop=False).rename(
-            columns={gps_field.POINT_SEQ_FIELD: 'g'}).explode(column=[markov_field.TO_STATE, gps_field.TO_GPS_SEQ],
-                                                              ignore_index=True)
+            [markov_field.TO_STATE, gps_field.TO_GPS_SEQ, 'to_route_dis']].reset_index(drop=False).rename(
+            columns={gps_field.POINT_SEQ_FIELD: 'g'}).explode(
+            column=[markov_field.TO_STATE, gps_field.TO_GPS_SEQ, 'to_route_dis'],
+            ignore_index=True)
+        from_state['from_route_dis'] = from_state['from_route_dis'].astype(float)
+        to_state['to_route_dis'] = to_state['to_route_dis'].astype(float)
 
         transition_df = pd.merge(from_state, to_state, on='g', how='outer')
         transition_df.reset_index(inplace=True, drop=True)
         # print(rf'{len(transition_df)}次状态转移...')
-        transition_df = self.diy_merge(left_df=transition_df,
-                                       right_df=single_link_ft_df[
-                                           [net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
-                                            net_field.TO_NODE_FIELD]],
-                                       left_key=markov_field.FROM_STATE, right_key=net_field.SINGLE_LINK_ID_FIELD,
-                                       label='from')
-        transition_df = self.diy_merge(left_df=transition_df,
-                                       right_df=single_link_ft_df[
-                                           [net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
-                                            net_field.TO_NODE_FIELD]],
-                                       left_key=markov_field.TO_STATE, right_key=net_field.SINGLE_LINK_ID_FIELD,
-                                       label='to')
-        transition_df = self.diy_merge(left_df=transition_df,
-                                       right_df=gps_match_link_route_dis,
-                                       left_key=[gps_field.FROM_GPS_SEQ, markov_field.FROM_STATE],
-                                       right_key=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
-                                       label='from', merge_type='prj')
-        transition_df = self.diy_merge(left_df=transition_df,
-                                       right_df=gps_match_link_route_dis,
-                                       left_key=[gps_field.TO_GPS_SEQ, markov_field.TO_STATE],
-                                       right_key=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
-                                       label='to', merge_type='prj')
-        del gps_match_link_route_dis
+        transition_df['from_link_f'] = transition_df[markov_field.FROM_STATE].map(link_f_map)
+        transition_df['from_link_t'] = transition_df[markov_field.FROM_STATE].map(link_t_map)
+        transition_df['to_link_f'] = transition_df[markov_field.TO_STATE].map(link_f_map)
+        transition_df['to_link_t'] = transition_df[markov_field.TO_STATE].map(link_t_map)
 
-        now_source_node = set(transition_df['from_link_f'])
+        # now_source_node = set(transition_df['from_link_f'])
         if not fmm_cache:
             # 先计算所有要计算的path
             if o_node_field in done_stp_cost_df.columns:
                 already_cache_node = set(done_stp_cost_df[o_node_field])
             else:
                 already_cache_node = set()
             gap = now_source_node - already_cache_node
@@ -387,16 +371,19 @@
                 done_stp_cost_df = self.add_path_cache(done_stp_cost_df=done_stp_cost_df,
                                                        source_node_list=gap, cut_off=cut_off,
                                                        single_link_ft_path_df=single_link_ft_df,
                                                        weight_field=weight_field, method=method, g=g,
                                                        add_single_ft=add_single_ft)
         del single_link_ft_df, g
 
-        transition_df = pd.merge(transition_df, done_stp_cost_df, left_on=['from_link_f', 'to_link_f'],
+        _done_stp_cost_df = done_stp_cost_df[done_stp_cost_df[o_node_field].isin(now_source_node) &
+                                             done_stp_cost_df[d_node_field].isin(now_source_node)].copy()
+        transition_df = pd.merge(transition_df, _done_stp_cost_df, left_on=['from_link_f', 'to_link_f'],
                                  right_on=[o_node_field, d_node_field], how='left')
+        del _done_stp_cost_df
         del transition_df[o_node_field], transition_df[d_node_field]
         # sub_net do not share path within different agents
         if is_sub_net or fmm_cache or not cache_path:
             del done_stp_cost_df
             done_stp_cost_df = pd.DataFrame()
 
         transition_df[cost_field] = transition_df[cost_field].fillna(0)
@@ -412,16 +399,15 @@
                                  _[cost_field]) if c > 0}
         same_link_idx = transition_df[markov_field.FROM_STATE] == transition_df[markov_field.TO_STATE]
         transition_df.loc[same_link_idx, markov_field.ROUTE_LENGTH] = \
             np.abs(transition_df.loc[same_link_idx, :]['from_route_dis'] -
                    transition_df.loc[same_link_idx, :]['to_route_dis'])
         transition_df['2nd_node'] = -1
         transition_df['-2nd_node'] = -1
-        # normal_path_idx_a = transition_df[cost_field] > 0
-        # normal_path_idx_a可能全是False
+        # normal_path_idx_a = transition_df[cost_field] > 0, normal_path_idx_a可能全是False
         try:
             transition_df.loc[normal_path_idx_a, '2nd_node'] = transition_df.loc[normal_path_idx_a, :][
                 path_field].apply(
                 lambda x: x[1])
             transition_df.loc[normal_path_idx_a, '-2nd_node'] = transition_df.loc[normal_path_idx_a, :][
                 path_field].apply(
                 lambda x: x[-2])
@@ -444,19 +430,14 @@
             -transition_df[markov_field.ROUTE_LENGTH] + transition_df[gps_field.ADJ_DIS])
 
         s2s_route_l = transition_df[[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ, markov_field.ROUTE_LENGTH,
                                      markov_field.FROM_STATE, markov_field.TO_STATE]].copy()
         transition_df['trans_values'] = \
             self.transition_probability(self.beta, transition_df[markov_field.DIS_GAP].values, self.dis_para)
 
-        # ft_transition_dict = {f_gps_seq: df[
-        #     [markov_field.FROM_STATE, markov_field.TO_STATE, 'trans_values']].set_index(
-        #     [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values for (f_gps_seq, t_gps_seq), df in
-        #                       transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
-
         ft_transition_dict = {f_gps_seq: df['trans_values'].values.reshape(seq_len_dict[f_gps_seq],
                                                                            int(len(df) / seq_len_dict[f_gps_seq])) for
                               (f_gps_seq, t_gps_seq), df in
                               transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
 
         return adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, seq_k_candidate_info, done_stp_cost_df
 
@@ -502,30 +483,14 @@
             cost_df[cost_field] = np.around(cost_df[cost_field], decimals=1)
             stp_cost_df = pd.merge(stp_df, cost_df, on=[o_node_field, d_node_field])
             del stp_df, cost_df
             stp_cost_df.reset_index(inplace=True, drop=True)
         return stp_cost_df
 
     @staticmethod
-    def diy_merge(left_df: pd.DataFrame, right_df: pd.DataFrame or gpd.GeoDataFrame = None,
-                  left_key: str or list[str] = None,
-                  right_key: str or list[str] = None, label: str = 'from', merge_type: str = 'ft'):
-        df = pd.merge(left_df, right_df, left_on=left_key, right_on=right_key, how='left')
-
-        if merge_type == 'ft':
-            df.rename(columns={net_field.FROM_NODE_FIELD: label + '_link_f',
-                               net_field.TO_NODE_FIELD: label + '_link_t'}, inplace=True)
-
-            df.drop(columns=[right_key], axis=1, inplace=True)
-        else:
-            df.rename(columns={'route_dis': label + '_route_dis'}, inplace=True)
-            df.drop(columns=right_key, axis=1, inplace=True)
-        return df
-
-    @staticmethod
     def _single_source_path_alpha(g: nx.DiGraph = None, source: int = None, method: str = 'dijkstra',
                                   weight_field: str = None, cut_off: float = 600.0) -> \
             tuple[dict[int, int], dict[int, list]]:
         if method == 'dijkstra':
             return nx.single_source_dijkstra(g, source, weight=weight_field, cutoff=cut_off)
         else:
             return nx.single_source_bellman_ford(g, source, weight=weight_field)
@@ -896,185 +861,13 @@
 
     def format_war_info(self):
         if self.warn_info['from_ft']:
             self.format_warn_info = pd.DataFrame(self.warn_info)
         del self.warn_info
 
 
-    # @function_time_cost
-    # def generate_transition_mat_beta1(self, gps_ft_list: list = None, single_link_ft_df: pd.DataFrame = None,
-    #                                   pre_seq_candidate: pd.DataFrame = None,
-    #                                   gps_pre_next_dis_df: pd.DataFrame = None,
-    #                                   g: nx.DiGraph = None,
-    #                                   method: str = None, weight_field: str = 'length',
-    #                                   cache_path: bool = True, not_conn_cost: float = 999.0,
-    #                                   done_stp_cost_df: pd.DataFrame = None,
-    #                                   is_sub_net: bool = True, fmm_cache: bool = False, cut_off: float = 600.0,
-    #                                   max_cut_off: float = 2000.0, cache_prj_inf: dict = None) -> \
-    #         tuple[dict, dict, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
-    #     gps_ft_df = pd.DataFrame(gps_ft_list, columns=['f_gps_seq', 't_gps_seq'])
-    #     used_gps_seq = list(set(gps_ft_df['f_gps_seq']) | set(gps_ft_df['t_gps_seq']))
-    #
-    #     # 确定最终的top_k候选
-    #     pre_seq_candidate = pre_seq_candidate[
-    #         pre_seq_candidate[gps_field.POINT_SEQ_FIELD].isin(used_gps_seq)].copy()
-    #     seq_k_candidate_info = self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate,
-    #                                                     top_k=self.top_k, cache_prj_inf=cache_prj_inf)
-    #
-    #     # 存储状态的索引和状态序列的映射
-    #     seq_k_candidate_info['idx'] = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD)[
-    #                                       net_field.SINGLE_LINK_ID_FIELD].rank(method='min').astype(int) - 1
-    #     ft_idx_map = seq_k_candidate_info[[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'idx']].copy()
-    #     ft_idx_map.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
-    #     del seq_k_candidate_info['idx']
-    #
-    #     del pre_seq_candidate
-    #     del used_gps_seq
-    #
-    #     s = time.time()
-    #     # 构造状态转移表
-    #     seq_k_candidate = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD).agg(
-    #         {net_field.SINGLE_LINK_ID_FIELD: list, gps_field.POINT_SEQ_FIELD: list,
-    #          net_field.FROM_NODE_FIELD: list, net_field.TO_NODE_FIELD: list, 'route_dis': list}).rename(
-    #         columns={gps_field.POINT_SEQ_FIELD: gps_field.FROM_GPS_SEQ,
-    #                  net_field.SINGLE_LINK_ID_FIELD: markov_field.FROM_STATE,
-    #                  net_field.FROM_NODE_FIELD: 'from_link_f', net_field.TO_NODE_FIELD: 'from_link_t',
-    #                  'route_dis': 'from_route_dis'})
-    #
-    #     seq_k_candidate[[gps_field.TO_GPS_SEQ, markov_field.TO_STATE, 'to_link_f', 'to_link_t', 'to_route_dis']] = \
-    #         seq_k_candidate[[gps_field.FROM_GPS_SEQ, markov_field.FROM_STATE, 'from_link_f', 'from_link_t',
-    #                          'from_route_dis']].shift(-1)
-    #     seq_k_candidate.dropna(subset=[markov_field.TO_STATE], inplace=True)
-    #
-    #     from_state = seq_k_candidate[
-    #         [markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ,
-    #          'from_link_f', 'from_link_t', 'from_route_dis']].reset_index(drop=False).explode(
-    #         column=[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ, 'from_link_f', 'from_link_t',
-    #                 'from_route_dis'], ignore_index=True)
-    #
-    #     to_state = seq_k_candidate[
-    #         [markov_field.TO_STATE, gps_field.TO_GPS_SEQ, 'to_link_f', 'to_link_t', 'to_route_dis']].reset_index(
-    #         drop=False).explode(
-    #         column=[markov_field.TO_STATE, gps_field.TO_GPS_SEQ, 'to_link_f', 'to_link_t', 'to_route_dis'],
-    #         ignore_index=True)
-    #     del seq_k_candidate
-    #     transition_df = pd.merge(from_state, to_state, on=gps_field.POINT_SEQ_FIELD, how='outer')
-    #     del transition_df[gps_field.POINT_SEQ_FIELD]
-    #     del from_state, to_state
-    #     transition_df.reset_index(inplace=True, drop=True)
-    #     print(rf'构造: {time.time() - s}')
-    #     t = time.time()
-    #     del single_link_ft_df
-    #
-    #     now_source_node = set(transition_df['from_link_f'])
-    #     if not fmm_cache:
-    #         # 先计算所有要计算的path
-    #         already_cache_node = set(done_stp_cost_df['o_node'])
-    #         gap = now_source_node - already_cache_node
-    #         if not gap:
-    #             done_stp_cost_df = self.add_path_cache(done_stp_cost_df=done_stp_cost_df,
-    #                                                    source_node_list=gap, cut_off=cut_off,
-    #                                                    weight_field=weight_field, method=method, g=g)
-    #             now_source_node = set(done_stp_cost_df['o_node'])
-    #
-    #     # 如果某些点除开自身-自身没有其他点, 则加一个5km搜索
-    #     done_stp_cost_df.drop(index=done_stp_cost_df[done_stp_cost_df['o_node'] == done_stp_cost_df['d_node']].index,
-    #                           inplace=True)
-    #     no_path_node = now_source_node - set(done_stp_cost_df['o_node'])
-    #     if no_path_node:
-    #         done_stp_cost_df = self.add_path_cache(done_stp_cost_df=done_stp_cost_df,
-    #                                                source_node_list=no_path_node, cut_off=max_cut_off,
-    #                                                weight_field=weight_field, method=method, g=g)
-    #     del g
-    #
-    #     # transition_df['from_route_dis'] = transition_df['from_route_dis'].astype(float)
-    #     # transition_df['to_route_dis'] = transition_df['to_route_dis'].astype(float)
-    #
-    #     transition_df = pd.merge(transition_df, done_stp_cost_df, left_on=['from_link_f', 'to_link_f'],
-    #                              right_on=['o_node', 'd_node'], how='left')
-    #     del transition_df['o_node'], transition_df['d_node']
-    #     # sub_net do not share path within different agents
-    #     if is_sub_net or fmm_cache or not cache_path:
-    #         del done_stp_cost_df
-    #         done_stp_cost_df = pd.DataFrame()
-    #
-    #     transition_df['cost'] = transition_df['cost'].fillna(0)
-    #     transition_df.reset_index(inplace=True, drop=True)
-    #     transition_df[markov_field.ROUTE_LENGTH] = not_conn_cost * 1.0
-    #
-    #     _ = transition_df[transition_df['cost'] > 0]
-    #     adj_seq_path_dict = {(int(f_state), int(t_state)): node_path for f_state, t_state, node_path, c in
-    #                          zip(_[markov_field.FROM_STATE],
-    #                              _[markov_field.TO_STATE],
-    #                              _['path'],
-    #                              _['cost']) if c > 0}
-    #     z = time.time()
-    #     same_link_idx = transition_df[markov_field.FROM_STATE] == transition_df[markov_field.TO_STATE]
-    #     transition_df.loc[same_link_idx, markov_field.ROUTE_LENGTH] = \
-    #         np.abs(transition_df.loc[same_link_idx, :]['from_route_dis'].values.astype(float) -
-    #                transition_df.loc[same_link_idx, :]['to_route_dis'].values.astype(float))
-    #     transition_df['2nd_node'] = -1
-    #     transition_df['-2nd_node'] = -1
-    #     normal_path_idx_a = transition_df['cost'] > 0
-    #     t2 = time.time()
-    #     transition_df.loc[normal_path_idx_a, '2nd_node'] = transition_df.loc[normal_path_idx_a, :]['path'].apply(
-    #         lambda x: x[1])
-    #     transition_df.loc[normal_path_idx_a, '-2nd_node'] = transition_df.loc[normal_path_idx_a, :]['path'].apply(
-    #         lambda x: x[-2])
-    #     t3 = time.time()
-    #     normal_path_idx_b = (normal_path_idx_a & \
-    #                          (transition_df['2nd_node'] == transition_df['from_link_t']) & \
-    #                          (transition_df['-2nd_node'] != transition_df['to_link_t'])) | \
-    #                         ((transition_df['from_link_f'] == transition_df['to_link_t']) &
-    #                          (transition_df['from_link_t'] == transition_df['to_link_f']))
-    #
-    #     transition_df.loc[normal_path_idx_b, markov_field.ROUTE_LENGTH] = \
-    #         np.abs(transition_df.loc[normal_path_idx_b, :]['cost'].values -
-    #                transition_df.loc[normal_path_idx_b, :]['from_route_dis'].values.astype(float) +
-    #                transition_df.loc[normal_path_idx_b, :]['to_route_dis'].values.astype(float))
-    #     print(rf'cache_len: {len(done_stp_cost_df)}')
-    #
-    #     transition_df = pd.merge(transition_df, gps_pre_next_dis_df, on=[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ],
-    #                              how='left')
-    #
-    #     transition_df[markov_field.DIS_GAP] = np.abs(
-    #         -transition_df[markov_field.ROUTE_LENGTH] + transition_df[gps_field.ADJ_DIS])
-    #     t4 = time.time()
-    #     # print(transition_df[markov_field.DIS_GAP])
-    #     print(rf'向量化总时间: {t4 - z}')
-    #     print(rf'apply: {t3 - t2}')
-    #     print(rf'总计算: {t4 - t}')
-    #
-    #     s2s_route_l = transition_df[[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ, markov_field.ROUTE_LENGTH,
-    #                                  markov_field.FROM_STATE, markov_field.TO_STATE]].copy()
-    #
-    #     transition_df['trans_values'] = \
-    #         self.transition_probability(self.beta, transition_df[markov_field.DIS_GAP].values, self.dis_para)
-    #
-    #     ft_transition_dict = {f_gps_seq: df[
-    #         [markov_field.FROM_STATE, markov_field.TO_STATE, 'trans_values']].set_index(
-    #         [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values for (f_gps_seq, t_gps_seq), df in
-    #                           transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
-    #     print(rf'归并mat: {time.time() - t4}')
-    #
-    #     return adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, seq_k_candidate_info, done_stp_cost_df
-
-
 if __name__ == '__main__':
     pass
-    # a = LineString([(0, 0), (0, 1)])
-    # z = a.segmentize(1/3 + 0.1 * 1/ 3)
-    # print(z)
-
-    # x = pd.DataFrame({'a': [1,2,3], 'b': [4,5,6]})
-    # print(x)
-    # x.loc[x['a'] >= 2, ['a', 'b']] = [[12, 11], [121,344]]
-    # print(x)
-    #
-    # x = datetime.datetime.now()
-    # time.sleep(2)
-    # x1 = datetime.datetime.now()
-    # print((x1 - x).total_seconds())
```

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/NetGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/Request/request_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.4/src/gotrackit/netreverse/format_od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/netxfer/SumoConvert.py` & `gotrackit-0.2.4/src/gotrackit/netxfer/SumoConvert.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.4/src/gotrackit/solver/Viterbi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.4/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/tools/geo_process.py` & `gotrackit-0.2.4/src/gotrackit/tools/geo_process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/tools/group.py` & `gotrackit-0.2.4/src/gotrackit/tools/group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.4/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit/visualization.py` & `gotrackit-0.2.4/src/gotrackit/visualization.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.3/src/gotrackit.egg-info/PKG-INFO` & `gotrackit-0.2.4/src/gotrackit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,55 +45,58 @@
 
 
 **版本状态：05.07已经更新: v0.2.3**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
 
-- 效率优化, 相较于v0.2.2小幅度提升
+- 地图匹配接口效率优化, 相较于v0.2.2小幅度提升
 
-- crs判断BUG修复、境外路网构建失败BUG修复
+- 地图匹配接口报错机制优化
 
-- 报错机制优化
+- 地图匹配接口移除html_fldr参数, 使用out_fldr替代
 
-- 输出文件目录指定参数html_fldr废除, 改为out_fldr
+- 地图匹配接口增加即时输出开关instant_output, 打开后, 每匹配完一条轨迹马上进行结果存储
 
-- 增加环路处理功能
-    
-- 增加匹配结果即时输出参数, 每匹配完一条轨迹可马上进行结果存储
+- 路网构建: crs判断BUG修复、境外路网构建失败BUG修复
+
+- 增加 环路 处理功能
+
+
+**不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.2效率将大幅度提升, 最高可以提升10倍的性能 !~
+~ v0.2.4(相较于0.2.1)效率将大幅度提升, 最高可以提升10倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.2版解算时间 |
-|----------------|----------|----------------|------------------|---------|------------|-------------|-----------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **3.3秒**  |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **1.7秒**    |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.4版解算时间 |
+|----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
+| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.87秒**   |
+| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.89秒**   |
 
 
-v0.2.2多核效率对比:
+v0.2.4多核效率对比:
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快96s解算完150条轨迹，平均每条轨迹0.64s，相较于1.7s再次提升了60%，在车辆数较多时，多核的效率提升很明显。
+基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快89s解算完150条轨迹，平均每条轨迹0.59s，相较于0.89s再次提升了30%，在车辆数较多时，多核的效率提升很明显。
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.2解算时间 |
+| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 300.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 139.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 120.3秒     |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 104.9秒     | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 96.4秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.5秒      | 
+| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 290.0秒     | 
+| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 130.6秒     |
+| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 113.3秒     |
+| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.3秒      | 
+| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 89.4秒      | 
+| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 91.5秒      | 
 
 
 <br>
 
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
```

### Comparing `gotrackit-0.2.3/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.4/src/gotrackit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


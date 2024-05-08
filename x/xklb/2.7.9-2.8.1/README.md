# Comparing `tmp/xklb-2.7.9.tar.gz` & `tmp/xklb-2.8.1.tar.gz`

## Comparing `xklb-2.7.9.tar` & `xklb-2.8.1.tar`

### file list

```diff
@@ -1,135 +1,138 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.7.9/.gitattributes
--rw-r--r--   0        0        0   216289 2020-02-02 00:00:00.000000 xklb-2.7.9/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/__init__.py
--rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/lb.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/media_printer.py
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/readme.py
--rw-r--r--   0        0        0   112269 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/__init__.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/av.py
--rw-r--r--   0        0        0    21197 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/fs_add.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/gallery_add.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/gallery_backend.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/hn_add.py
--rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/links_add.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/places_import.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/reddit_add.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/row_add.py
--rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/site_add.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/substack.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/subtitle.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tabs_add.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tildes.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tube_add.py
--rw-r--r--   0        0        0    20265 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/tube_backend.py
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/createdb/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/__init__.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/dedupe_db.py
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/dedupe_media.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/merge_online_local.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/mpv_watchlater.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/pushshift.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/editdb/reddit_selftext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/christen.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/sample_compare.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/sample_hash.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/files/similar_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/__init__.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/merge_folders.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/mount_stats.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/move_list.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/rel_mv.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/scatter.py
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/folders/similar_folders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/__init__.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/big_dirs.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/disk_usage.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/fsdb/search_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/__init__.py
--rw-r--r--   0        0        0    11660 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/block.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/db_history.py
--rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/db_playlists.py
--rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/download.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/download_status.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/history.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/history_add.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/optimize_db.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/playlists.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/redownload.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/search.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediadb/stats.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediafiles/media_check.py
--rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediafiles/process_ffmpeg.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/mediafiles/process_image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/misc/__init__.py
--rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/misc/dedupe_czkawka.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/misc/export_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/multidb/__init__.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/multidb/copy_play_counts.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/multidb/merge_dbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/__init__.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/links_open.py
--rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/media_player.py
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/play_actions.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/playback_control.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/post_actions.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/surf.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/playback/tabs_open.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/__init__.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/eda.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/incremental_diff.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/tablefiles/mcda.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/cluster_sort.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/extract_links.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/extract_text.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/markdown_links.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/text/nouns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/__init__.py
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    17737 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/consts.py
--rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/devices.py
--rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/nums.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/objects.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/printing.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/processes.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/strings.py
--rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/utils/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/assets/__init__.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.7.9/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.7.9/.gitignore
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 xklb-2.7.9/pyproject.toml
--rw-r--r--   0        0        0   156009 2020-02-02 00:00:00.000000 xklb-2.7.9/.github/README.md
--rw-r--r--   0        0        0   159790 2020-02-02 00:00:00.000000 xklb-2.7.9/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.8.1/.gitattributes
+-rw-r--r--   0        0        0   216289 2020-02-02 00:00:00.000000 xklb-2.8.1/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/__init__.py
+-rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/lb.py
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/media_printer.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/readme.py
+-rw-r--r--   0        0        0   112366 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/av.py
+-rw-r--r--   0        0        0    20488 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/data/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    18964 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/files/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/files/christen.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/files/similar_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/big_dirs.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/mount_stats.py
+-rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/scatter.py
+-rw-r--r--   0        0        0     8348 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/folders/similar_folders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/block.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/db_history.py
+-rw-r--r--   0        0        0    19107 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/db_media.py
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/db_playlists.py
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/history.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/history_add.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediadb/stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediafiles/__init__.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/surf.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/text/__init__.py
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/consts.py
+-rw-r--r--   0        0        0     9380 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/nums.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/processes.py
+-rw-r--r--   0        0        0    13007 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/sqlgroups.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/strings.py
+-rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.8.1/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.8.1/.gitignore
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 xklb-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0   156082 2020-02-02 00:00:00.000000 xklb-2.8.1/.github/README.md
+-rw-r--r--   0        0        0   159863 2020-02-02 00:00:00.000000 xklb-2.8.1/PKG-INFO
```

### Comparing `xklb-2.7.9/pdm.lock` & `xklb-2.8.1/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -982,20 +982,20 @@
 files = [
     {file = "jedi-0.19.1-py2.py3-none-any.whl", hash = "sha256:e983c654fe5c02867aef4cdfce5a2fbb4a50adc0af145f70504238f18ef5e7e0"},
     {file = "jedi-0.19.1.tar.gz", hash = "sha256:cf0496f3651bc65d7174ac1b7d043eff454892c708a87d1b683e57b569927ffd"},
 ]
 
 [[package]]
 name = "joblib"
-version = "1.4.0"
+version = "1.4.2"
 requires_python = ">=3.8"
 summary = "Lightweight pipelining with Python functions"
 files = [
-    {file = "joblib-1.4.0-py3-none-any.whl", hash = "sha256:42942470d4062537be4d54c83511186da1fc14ba354961a2114da91efa9a4ed7"},
-    {file = "joblib-1.4.0.tar.gz", hash = "sha256:1eb0dc091919cd384490de890cb5dfd538410a6d4b3b54eef09fb8c50b409b1c"},
+    {file = "joblib-1.4.2-py3-none-any.whl", hash = "sha256:06d478d5674cbc267e7496a410ee875abd68e4340feff4490bcb7afb88060ae6"},
+    {file = "joblib-1.4.2.tar.gz", hash = "sha256:2382c5816b2636fbd20a09e0f4e9dad4736765fdfb7dca582943b9c1366b3f0e"},
 ]
 
 [[package]]
 name = "kaitaistruct"
 version = "0.10"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7"
 summary = "Kaitai Struct declarative parser generator for binary data: runtime library for Python"
```

### Comparing `xklb-2.7.9/.github/LICENSE` & `xklb-2.8.1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/.github/Windows.md` & `xklb-2.8.1/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/.github/examples/art.avif` & `xklb-2.8.1/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/.github/examples/extract.svg` & `xklb-2.8.1/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/.github/examples/tubeadd.svg` & `xklb-2.8.1/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/.github/workflows/push.yaml` & `xklb-2.8.1/.github/workflows/push.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,49 @@
 name: PyTest and Publish
 
 on:
   push:
     tags: ['v[0-9].[0-9]+.[0-9]+']
 
 jobs:
-  test:
+  test1:
+    runs-on: ubuntu-latest
+    timeout-minutes: 20
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+
+      - name: Setup Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.10"
+
+      - uses: FedericoCarboni/setup-ffmpeg@v3
+
+      - name: Install pdm
+        run: |
+          python -m pip install pdm
+          pdm install --no-editable -G test
+
+      - name: Run missing modules test
+        run: pdm run pytest tests/test_modules.py  # should run before deluxe deps installed
+
+      - name: Run deluxe pytest
+        run: |
+          pdm install --no-editable -G deluxe
+          pdm run pytest
+
+  test2:
+    needs: test1
     strategy:
       fail-fast: false
       max-parallel: 8
       matrix:
-        nv: [ {os: windows-latest, py: "3.10"}, {os: macos-13, py: "3.11"}, {os: ubuntu-latest, py: "3.12"} ]
+        nv: [ {os: windows-latest, py: "3.11"}, {os: macos-13, py: "3.12"} ]
 
     runs-on: ${{ matrix.nv.os }}
     timeout-minutes: 20
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.nv.py }}
@@ -23,27 +52,23 @@
           python-version: ${{ matrix.nv.py }}
 
       - uses: FedericoCarboni/setup-ffmpeg@v3
 
       - name: Install Dependencies
         run: |
           python -m pip install pdm
-
-      - name: Run missing modules test
-        run: |
           pdm install --no-editable -G test
-          pdm run pytest tests/test_modules.py
 
       - name: Run deluxe pytest
         run: |
           pdm install --no-editable -G deluxe
           pdm run pytest
 
   publish:
-    needs: test
+    needs: [test1, test2]
     runs-on: ubuntu-latest
     timeout-minutes: 20
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
 
@@ -55,15 +80,15 @@
       - name: Install pdm
         run: python -m pip install pdm
 
       - name: Build and publish
         run: pdm publish -u __token__ -P ${{ secrets.PYPI_TOKEN }}
 
   release:
-    needs: [test, publish]
+    needs: publish
     runs-on: ubuntu-latest
     timeout-minutes: 20
 
     steps:
       - uses: chapmanjacobd/create-release-node16@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `xklb-2.7.9/xklb/lb.py` & `xklb-2.8.1/xklb/lb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse, importlib, sys, textwrap
 
 from tabulate import tabulate
 
 from xklb import __version__
-from xklb.utils import iterables
+from xklb.utils import argparse_utils, iterables
 from xklb.utils.log_utils import log
 
 progs = {
     "Create database subcommands": {
         "fs_add": "Add local media",
         "tube_add": "Add online video media (yt-dlp)",
         "web_add": "Add open-directory media",
@@ -127,15 +127,15 @@
 
 def print_help(parser) -> None:
     print(usage())
     print(parser.epilog)
 
 
 def create_subcommands_parser() -> argparse.ArgumentParser:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="lb",
         description="xk media library",
         epilog="Report bugs here: https://github.com/chapmanjacobd/library/issues/new/choose",
         add_help=False,
     )
     subparsers = parser.add_subparsers()
 
@@ -207,15 +207,15 @@
     add_parser(subparsers, "xklb.files.similar_files.similar_files")
     add_parser(subparsers, "xklb.folders.merge_folders.merge_folders", ["merge-folder", "mv"])
     add_parser(subparsers, "xklb.folders.move_list.move_list", ["mv-list"])
     add_parser(subparsers, "xklb.folders.rel_mv.rel_mv", ["relmv", "mv-rel", "mvrel"])
     add_parser(subparsers, "xklb.folders.scatter.scatter")
     add_parser(subparsers, "xklb.folders.similar_folders.similar_folders")
     add_parser(subparsers, "xklb.folders.mount_stats.mount_stats", ["mu", "mount-usage"])
-    add_parser(subparsers, "xklb.fsdb.big_dirs.big_dirs", ["large-folders"])
+    add_parser(subparsers, "xklb.folders.big_dirs.big_dirs", ["large-folders"])
     add_parser(subparsers, "xklb.fsdb.disk_usage.disk_usage", ["du", "usage"])
     add_parser(subparsers, "xklb.fsdb.search_db.search_db", ["s", "sdb", "search-dbs"])
     add_parser(subparsers, "xklb.mediadb.block.block")
     add_parser(subparsers, "xklb.mediadb.download.dl_download", ["dl", "download"])
     add_parser(subparsers, "xklb.mediadb.download_status.download_status", ["ds", "dl-status"])
     add_parser(subparsers, "xklb.mediadb.history.history", ["hi", "log"])
     add_parser(subparsers, "xklb.mediadb.history_add.history_add", ["add-history"])
```

### Comparing `xklb-2.7.9/xklb/media_printer.py` & `xklb-2.8.1/xklb/media_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,22 @@
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
+def should_align_right(k, v):
+    if k.endswith(("size", "ratio")) or k.startswith("percent"):
+        return True
+    if isinstance(v, (int, float)):
+        return True
+    return None
+
+
 def media_printer(args, data, units=None, media_len=None) -> None:
     if units is None:
         units = "media"
 
     action = getattr(args, "action", "")
     print_args = getattr(args, "print", "")
     cols = getattr(args, "cols", [])
@@ -101,15 +109,18 @@
 
     if not media:
         processes.no_media_found()
 
     if "f" not in print_args and "limit" in getattr(args, "defaults", []):
         media.reverse()
 
-    tables = args.db.table_names()
+    try:
+        tables = args.db.table_names()
+    except AttributeError:
+        tables = []
 
     duration = sum(m.get("duration") or 0 for m in media)
     if "a" in print_args and ("Aggregate" not in media[0].get("path") or ""):
         if "count" in media[0]:
             D = {"path": "Aggregate", "count": sum(d.get("count") or 0 for d in media)}
         elif "exists" in media[0]:
             D = {"path": "Aggregate", "count": sum(d.get("exists") or 0 for d in media)}
@@ -173,42 +184,39 @@
         and "time_downloaded" in m_columns
     ):
         for m in media:
             m["download_duration"] = cadence_adjusted_items(
                 args, m["never_downloaded"] + m["retry_queued"], time_column="time_downloaded"
             )  # TODO where= p.extractor_key, or try to use SQL
 
-    for k, v in list(media[0].items()):
-        if k.endswith("size"):
-            printing.col_naturalsize(media, k)
-        elif k.endswith("duration") or k in ("playhead",):
-            printing.col_duration(media, k)
-        elif k.startswith("time_") or "_time_" in k:
-            printing.col_naturaltime(media, k)
-        elif k == "title_path":
-            media = [{"title_path": "\n".join(iterables.concat(d["title"], d["path"])), **d} for d in media]
-            media = [{k: v for k, v in d.items() if k not in ("title", "path")} for d in media]
-        elif k.startswith("percent") or k.endswith("ratio"):
-            for d in media:
-                d[k] = strings.safe_percent(d[k])
-        # elif isinstance(v, (int, float)):
-        #     for d in media:
-        #         if d[k] is not None:
-        #             d[k] = f'{d[k]:n}'  # TODO add locale comma separators
-
-    def should_align_right(k, v):
-        if k.endswith(("size", "ratio")) or k.startswith("percent"):
-            return True
-        if isinstance(v, (int, float)):
-            return True
-        return None
+    if not any([args.to_json, "f" in print_args]):
+        for k, v in list(media[0].items()):
+            if k.endswith("size"):
+                printing.col_naturalsize(media, k)
+            elif k.endswith("duration") or k in ("playhead",):
+                printing.col_duration(media, k)
+            elif k.startswith("time_") or "_time_" in k:
+                printing.col_naturaltime(media, k)
+            elif k == "title_path":
+                media = [{"title_path": "\n".join(iterables.concat(d["title"], d["path"])), **d} for d in media]
+                media = [{k: v for k, v in d.items() if k not in ("title", "path")} for d in media]
+            elif k.startswith("percent") or k.endswith("ratio"):
+                for d in media:
+                    d[k] = strings.safe_percent(d[k])
+            # elif isinstance(v, (int, float)):
+            #     for d in media:
+            #         if d[k] is not None:
+            #             d[k] = f'{d[k]:n}'  # TODO add locale comma separators
 
     media = iterables.list_dict_filter_bool(media)
 
-    if "f" in print_args:
+    if args.to_json:
+        printing.pipe_lines(json.dumps(m) + "\n" for m in media)
+
+    elif "f" in print_args:
         if len(media) <= 1000 and getattr(args, "action", "") not in [consts.SC.links_open]:
             media, deleted_paths = filter_deleted(media)
             db_media.mark_media_deleted(args, deleted_paths)
             if len(media) == 0:
                 raise FileNotFoundError
 
         if not cols:
```

### Comparing `xklb-2.7.9/xklb/readme.py` & `xklb-2.8.1/xklb/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     [Unit]
     Description=xklb daily browser tabs
 
     [Service]
     Type=simple
     RemainAfterExit=no
     Environment="DISPLAY=:0"
-    ExecStart="/usr/bin/fish" "-c" "lb tabs /home/xk/lb/tabs.db"
+    ExecStart=library tabs /home/my/tabs.db
 
     tee ~/.config/systemd/user/tabs.timer
     [Unit]
     Description=xklb daily browser tabs timer
 
     [Timer]
     Persistent=yes
```

### Comparing `xklb-2.7.9/xklb/usage.py` & `xklb-2.8.1/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,17 @@
         as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
         library {action} -RRCO
 
         You can even sort the items within each cluster by auto-MCDA ~LOL~
         library {action} -B --sort-groups-by 'mcda median_size,-deleted'
         library {action} -C --sort-groups-by 'mcda median_size,-deleted'
 
+    Filter media by playlist:
+        library {action} --playlists URL1 URL2
+
     Filter media by file siblings of parent directory:
         library {action} --sibling   # only include files which have more than or equal to one sibling
         library {action} --solo      # only include files which are alone by themselves
 
         `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
         library {action} --sibling --solo      # you will always get zero records here
         library {action} --lower 2 --upper 1   # equivalent
@@ -1834,16 +1837,17 @@
         using the ask-keep action will mark a video as deleted when you 'quit 4' and it will mark a video as watched when you 'quit'.
 
         For example, here I bind "'" to "KEEP" and  "j" to "DELETE"
 
             ' quit
             j quit 4
 
-        This is pretty intuitive after you use it a few times but writing this out I realize this might seem a bit opaque.
-        Instead of using built-in post-actions (example above) you could also do something like
+        This is pretty intuitive after you use it a few times but another option is to
+        define your own post-actions:
+
             `--cmd5 'echo {} >> keep.txt' --cmd6 'echo {} >> rejected.txt'`
 
         But you will still bind keys in mpv input.conf:
 
             k quit 5  # goes to keep.txt
             r quit 6  # goes to rejected.txt
 
@@ -1920,15 +1924,15 @@
 
     Find similar files based on ONLY size
 
         $ library similar-files --no-filter-names ~/d/
 
     Read paths from dbs
 
-        $ library similar-files --dbs db1.db db2.db
+        $ lb fs audio.db --cols path,duration,size,time_deleted --to-json | lb similar-files --from-json -v
 
 """
 
 similar_folders = """library similar-folders PATH ...
 
     Find similar folders based on foldernames, similar size, and similar number of files
 
@@ -1953,15 +1957,15 @@
 
     Find similar folders based on ONLY total size
 
         $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
 
     Read paths from dbs
 
-        $ library similar-folders --dbs db1.db db2.db
+        $ lb fs audio.db --cols path,duration,size,time_deleted --to-json | lb similar-folders --from-json -v
 
     Print only paths
 
         $ library similar-folders ~/d/ -pf
         /home/xk/d/dump/datasets/vector/output/
         /home/xk/d/dump/datasets/vector/output2/
 """
```

### Comparing `xklb-2.7.9/xklb/createdb/av.py` & `xklb-2.8.1/xklb/createdb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/createdb/fs_add.py` & `xklb-2.8.1/xklb/createdb/fs_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
 
 from xklb import usage
 from xklb.createdb import av
 from xklb.files import sample_hash
+from xklb.folders import rel_mv
 from xklb.mediadb import db_media, db_playlists, playlists
 from xklb.mediafiles import process_ffmpeg, process_image
 from xklb.utils import (
     arg_utils,
     arggroups,
     argparse_utils,
     consts,
@@ -28,18 +29,17 @@
 from xklb.utils.consts import SC, DBType
 from xklb.utils.log_utils import log
 
 REGEX_SENTENCE_ENDS = re.compile(r";|,|\.|\*|\n|\t")
 
 
 def parse_args(action, usage):
-    parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
+    parser = argparse_utils.ArgumentParser(prog="library " + action, usage=usage)
     arggroups.db_profiles(parser)
-    arggroups.capability_simulate(parser)
-    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
+    arggroups.simulate(parser)
 
     parser.add_argument(
         "--io-multiplier",
         type=float,
         default=1.0,
         help="Especially useful for text, image, filesystem db types",
     )
@@ -48,15 +48,14 @@
     parser.add_argument("--scan-subtitles", "--scan-subtitle", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--hash", action="store_true")
     parser.add_argument("--move")
 
     parser.add_argument("--process", action="store_true", help=argparse.SUPPRESS)
     arggroups.process_ffmpeg(parser)
-    parser.add_argument("--delete-unplayable", action="store_true")
 
     parser.add_argument("--check-corrupt", "--check-corruption", action="store_true")
     arggroups.media_check(parser)
     parser.set_defaults(gap="0.10")
 
     parser.add_argument(
         "--force", "-f", action="store_true", help="Mark all subpath files as deleted if no files found"
@@ -68,37 +67,28 @@
         parser.add_argument("paths", nargs="+")
     args = parser.parse_intermixed_args()
 
     if not args.profiles:
         args.profiles = [DBType.video]
 
     if args.move:
-        args.move = str(Path(args.move).expanduser().resolve())
-
-    args.gap = nums.float_from_percent(args.gap)
-    if args.delete_corrupt:
-        args.delete_corrupt = nums.float_from_percent(args.delete_corrupt)
-    if args.full_scan_if_corrupt:
-        args.full_scan_if_corrupt = nums.float_from_percent(args.full_scan_if_corrupt)
-
-    args.split_longer_than = nums.human_to_seconds(args.split_longer_than)
-    args.min_split_segment = nums.human_to_seconds(args.min_split_segment)
-
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
+        args.move = Path(args.move).expanduser().resolve()
 
     if hasattr(args, "paths"):
         args.paths = iterables.conform(args.paths)
-    log.info(objects.dict_filter_bool(args.__dict__))
 
     if not which("ffprobe") and (DBType.audio in args.profiles or DBType.video in args.profiles):
         log.error("ffmpeg is not installed. Install it with your package manager.")
         raise SystemExit(3)
 
-    return args, parser
+    arggroups.process_ffmpeg_post(args)
+    arggroups.media_check_post(args)
+
+    arggroups.args_post(args, parser, create_db=action == SC.fs_add)
+    return args
 
 
 def munge_book_tags(path) -> dict:
     try:
         import textract  # type: ignore
     except ModuleNotFoundError:
         print(
@@ -115,15 +105,15 @@
     return {"tags": strings.combine(tags)}
 
 
 munge_book_tags_fast = processes.with_timeout(70)(munge_book_tags)
 munge_book_tags_slow = processes.with_timeout(350)(munge_book_tags)
 
 
-def extract_metadata(mp_args, path) -> dict[str, int] | None:
+def extract_metadata(mp_args, path) -> dict[str, str | int | None] | None:
     try:
         path.encode()
     except UnicodeEncodeError:
         log.error("Could not encode file path as UTF-8. Skipping %s", path)
         return None
 
     try:
@@ -181,16 +171,16 @@
         else:
             log.debug(f"{timer()-start} {path}")
 
     if getattr(mp_args, "hash", False) and media["type"] != "directory" and media["size"] > 0:
         media["hash"] = sample_hash.sample_hash_file(path)
 
     if getattr(mp_args, "move", False) and not file_utils.is_file_open(path):
-        dest_path = bytes(Path(mp_args.move) / Path(path).relative_to(mp_args.playlist_path))
-        dest_path = path_utils.clean_path(dest_path)
+        dest_path = rel_mv.gen_rel_path(path, mp_args.move)
+        dest_path = path_utils.clean_path(bytes(dest_path))
         file_utils.rename_move_file(path, dest_path, simulate=mp_args.simulate)
         path = media["path"] = dest_path
 
     if getattr(mp_args, "process", False):
         if objects.is_profile(mp_args, DBType.audio) and Path(path).suffix not in [".opus", ".mka"]:
             result = process_ffmpeg.process_path(
                 mp_args,
@@ -373,16 +363,16 @@
         if description:
             tags += "\n" + description
         if tags:
             caption["captions_t0"] = {"time": 0, "text": tags}
 
         captions.append(caption)
 
-    media = [{"playlists_id": args.playlists_id, **d} for d in media]
     media = iterables.list_dict_filter_bool(media)
+    media = [{"playlists_id": args.playlists_id, **d} for d in media]
     args.db["media"].insert_all(media, pk="id", alter=True, replace=True)
 
     for d in captions:
         media_id = args.db.pop("select id from media where path = ?", [d["path"]])
         if len(d["chapters"]) > 0:
             args.db["captions"].insert_all([{**d, "media_id": media_id} for d in d["chapters"]], alter=True)
         if len(d["subtitles"]) > 0:
@@ -514,17 +504,15 @@
     elif args.io_multiplier != 1.0:
         n_jobs = max(1, int(max(os.cpu_count() or 4, 4) * args.io_multiplier))
 
     threadsafe = [DBType.audio, DBType.video, DBType.filesystem]
 
     info = {
         "extractor_key": "Local",
-        "extractor_config": objects.dict_filter_bool(
-            {k: v for k, v in args.__dict__.items() if k not in ["db", "database", "verbose", "force", "paths"]}
-        ),
+        "extractor_config": args.extractor_config,
         "time_deleted": 0,
     }
     args.playlists_id = db_playlists.add(args, str(path), info, check_subpath=True)
 
     print(f"[{path}] Building file list...")
     new_files = find_new_files(args, path)
     if new_files:
@@ -571,23 +559,23 @@
         db_utils.optimize(args)
 
 
 def fs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args, _parser = parse_args(SC.fs_add, usage.fs_add)
+    args = parse_args(SC.fs_add, usage.fs_add)
     extractor(args, args.paths)
 
 
 def fs_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args, parser = parse_args(SC.fs_update, usage.fs_update)
+    args = parse_args(SC.fs_update, usage.fs_update)
 
     fs_playlists = list(
         args.db.query(
             f"""
             SELECT *
             FROM playlists
             WHERE extractor_key = 'Local'
@@ -596,10 +584,10 @@
                 , path
             """,
         ),
     )
 
     for playlist in fs_playlists:
         extractor_config = json.loads(playlist.get("extractor_config") or "{}")
-        args_env = arg_utils.override_config(parser, extractor_config, args)
+        args_env = arg_utils.override_config(args, extractor_config)
 
         extractor(args_env, [playlist["path"]])
```

### Comparing `xklb-2.7.9/xklb/createdb/gallery_backend.py` & `xklb-2.8.1/xklb/createdb/gallery_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/createdb/hn_add.py` & `xklb-2.8.1/xklb/createdb/hn_add.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse, asyncio, queue, sqlite3, threading
-from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, db_utils, objects, web
+from xklb.utils import arggroups, argparse_utils, db_utils, objects, web
 from xklb.utils.log_utils import log
 
 """
 My understanding of aiohttp is stolen
 from ashish01's excellent https://github.com/ashish01/hn-data-dumps/blob/main/hn_async2.py
 
 MIT License
@@ -30,25 +29,22 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
 def parse_args(prog, usage) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog, usage)
+    parser = argparse_utils.ArgumentParser(prog, usage)
     parser.add_argument("--oldest", action="store_true")
     arggroups.requests(parser)
     arggroups.debug(parser)
     arggroups.database(parser)
     args = parser.parse_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
-
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def db_worker(args, input_queue):
     conn = sqlite3.connect(args.database, isolation_level=None)
     db_conn = db_utils.connect(args, conn)
     while True:
```

### Comparing `xklb-2.7.9/xklb/createdb/links_add.py` & `xklb-2.8.1/xklb/createdb/links_add.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import argparse, json, random, time
-from pathlib import Path
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
 from xklb import usage
 from xklb.mediadb import db_media, db_playlists
 from xklb.text import extract_links
-from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, printing, strings, web
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, db_utils, objects, printing, strings, web
 from xklb.utils.log_utils import log
 
 
-def parse_args(**kwargs):
-    parser = argparse.ArgumentParser(**kwargs)
+def parse_args(action, **kwargs):
+    parser = argparse_utils.ArgumentParser(**kwargs)
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
 
     parser.add_argument("--max-pages", type=int)
     parser.add_argument("--fixed-pages", type=int)
     parser.add_argument("--backfill-pages", "--backfill", type=int)
 
     parser.add_argument("--stop-pages-no-match", "--stop-no-match", type=int, default=4)
     parser.add_argument("--stop-pages-no-new", "--stop-no-new", type=int, default=10)
     parser.add_argument("--stop-new", type=int)
     parser.add_argument("--stop-known", type=int)
     parser.add_argument("--stop-link")
 
     parser.add_argument("--page-replace")
     parser.add_argument("--page-key", default="page")
-    parser.add_argument("--page-step", "--step", "-S", type=int, default=1)
+    parser.add_argument("--page-step", "--step", type=int, default=1)
     parser.add_argument("--page-start", "--start-page", "--start", type=int)
 
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
 
     arggroups.filter_links(parser)
 
     arggroups.requests(parser)
@@ -37,56 +36,38 @@
     arggroups.extractor(parser)
 
     parser.add_argument("--force", action="store_true")
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    if "add" in kwargs["prog"]:
+    if "add" in action:
         arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
 
     if args.auto_pager:
         args.fixed_pages = 1
 
-    if args.scroll:
-        args.selenium = True
+    arggroups.extractor_post(args)
+    arggroups.filter_links_post(args)
+    arggroups.selenium_post(args)
 
-    if not args.case_sensitive:
-        args.before_include = [s.lower() for s in args.before_include]
-        args.path_include = [s.lower() for s in args.path_include]
-        args.text_include = [s.lower() for s in args.text_include]
-        args.after_include = [s.lower() for s in args.after_include]
-        args.before_exclude = [s.lower() for s in args.before_exclude]
-        args.path_exclude = [s.lower() for s in args.path_exclude]
-        args.text_exclude = [s.lower() for s in args.text_exclude]
-        args.after_exclude = [s.lower() for s in args.after_exclude]
-
-    if not args.no_url_decode:
-        args.path_include = [web.url_decode(s) for s in args.path_include]
-        args.path_exclude = [web.url_decode(s) for s in args.path_exclude]
-
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
-    return args, parser
+    arggroups.args_post(args, parser, create_db=True)
+    return args
 
 
 def add_playlist(args, path):
     info = {
         "hostname": urlparse(path).hostname,
         "category": getattr(args, "category", None) or "Uncategorized",
         "time_created": consts.APPLICATION_START,
-        "extractor_config": {
-            k: v for k, v in args.__dict__.items() if k not in ["db", "database", "verbose", "paths", "backfill_pages"]
-        },
+        "extractor_config": args.extractor_config,
         "time_deleted": 0,
     }
-    args.playlists_id = db_playlists.add(args, str(path), info)
+    return db_playlists.add(args, str(path), info)
 
 
 def consolidate_media(args, path: str) -> dict:
     return {
         "path": path,
         "category": getattr(args, "category", None) or "Uncategorized",
         "time_created": consts.APPLICATION_START,
@@ -243,15 +224,15 @@
     print(
         f"{len(new_media)} new [{len(known_media)} known] in {page_count} pages (avg {len(new_media) // page_count} new [{len(known_media) // page_count} known])"
     )
     return len(new_media)
 
 
 def links_add() -> None:
-    args, _parser = parse_args(prog="library links-add", usage=usage.links_add)
+    args = parse_args(consts.SC.links_add, usage=usage.links_add)
 
     if args.insert_only:
         media_new = set()
         media_known = set()
         for p in arg_utils.gen_paths(args):
             if db_media.exists(args, p):
                 media_known.add(p)
@@ -263,15 +244,15 @@
             printing.print_overwrite(f"Link import: {len(media_new)} new [{len(media_known)} known]")
     else:
         if args.selenium:
             web.load_selenium(args)
         try:
             playlist_count = 0
             for playlist_path in arg_utils.gen_paths(args):
-                add_playlist(args, playlist_path)
+                args.playlists_id = add_playlist(args, playlist_path)
                 extractor(args, playlist_path)
 
                 if playlist_count > 3:
                     time.sleep(random.uniform(0.05, 2))
                 playlist_count += 1
 
         finally:
@@ -279,15 +260,15 @@
                 web.quit_selenium(args)
 
     if not args.db["media"].detect_fts():
         db_utils.optimize(args)
 
 
 def links_update() -> None:
-    args, parser = parse_args(prog="library links-update", usage=usage.links_update)
+    args = parse_args(consts.SC.links_update, usage=usage.links_update)
 
     link_playlists = db_playlists.get_all(
         args,
         order_by="""length(path)-length(REPLACE(path, '/', '')) desc
         , random()
         """,
     )
@@ -296,15 +277,15 @@
     if selenium_needed:
         web.load_selenium(args)
 
     try:
         playlist_count = 0
         for playlist in link_playlists:
             extractor_config = json.loads(playlist.get("extractor_config") or "{}")
-            args_env = arg_utils.override_config(parser, extractor_config, args)
+            args_env = arg_utils.override_config(args, extractor_config)
 
             new_media = extractor(args_env, playlist["path"])
 
             if new_media > 0:
                 db_playlists.decrease_update_delay(args, playlist["path"])
             else:
                 db_playlists.increase_update_delay(args, playlist["path"])
```

### Comparing `xklb-2.7.9/xklb/createdb/places_import.py` & `xklb-2.8.1/xklb/createdb/places_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import argparse
 from pathlib import Path
 
 from xklb import usage
 from xklb.mediadb import db_media
-from xklb.utils import arggroups, consts, db_utils, nums, objects
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, consts, nums, objects
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library places-import", usage=usage.places_import)
+    parser = argparse_utils.ArgumentParser(prog="library places-import", usage=usage.places_import)
     arggroups.database(parser)
     parser.add_argument("paths", nargs="+")
     arggroups.debug(parser)
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def google_maps_takeout(df):
     import pandas as pd
 
     new_df = pd.DataFrame()
```

### Comparing `xklb-2.7.9/xklb/createdb/reddit_add.py` & `xklb-2.8.1/xklb/createdb/reddit_add.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import argparse
 import datetime as dt
 import sys
 from functools import partial
 from itertools import takewhile
-from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import prawcore
 
 from xklb import usage
 from xklb.mediadb import db_media, db_playlists
-from xklb.utils import arggroups, consts, db_utils, iterables, objects
+from xklb.utils import arggroups, argparse_utils, consts, db_utils, iterables, objects
 from xklb.utils.log_utils import log
 
 PRAW_SETUP_INSTRUCTIONS = r"""
 You will need your Reddit user login info, client id, and secret.
 See https://www.reddit.com/wiki/api for client id / secret.
 
 Then create a praw.ini file:
@@ -38,15 +37,15 @@
 
 
 if TYPE_CHECKING:
     import praw
 
 
 def parse_args(action, usage) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library " + action,
         usage=usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--force", "-f", action="store_true")
     parser.add_argument("--limit", default=1000, type=int)
     parser.add_argument("--lookback", default=4, type=int, help="Number of days to look back")
@@ -60,27 +59,23 @@
     if action == "redditadd":
         parser.add_argument("paths", nargs="+")
     args = parser.parse_intermixed_args()
 
     if action == "redditadd":
         args.paths = iterables.conform(args.paths)
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
     try:
         import praw
 
         args.reddit = praw.Reddit(args.praw_site, config_interpolation="basic")
     except Exception as e:
         print(PRAW_SETUP_INSTRUCTIONS)
         raise SystemExit(e) from e
 
-    log.info(objects.dict_filter_bool(args.__dict__))
-
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 """
 Catherine Devlin's reddit-to-sqlite project was very helpful in understanding
 how to work with praw. Any lines of code which can be attributed to that person
 should be.
@@ -333,15 +328,17 @@
 
         db_playlists._add(
             args,
             objects.dict_filter_bool(
                 {
                     "path": path,
                     "extractor_playlist_id": name,
-                    "extractor_config": objects.filter_namespace(args, ["limit", "lookback", "praw_site"]),
+                    "extractor_config": objects.filter_namespace(
+                        args.extractor_config, ["limit", "lookback", "praw_site"]
+                    ),
                     "extractor_key": extractor_key,
                     "time_modified": consts.now(),
                     "time_deleted": 0,
                 },
             ),
         )
```

### Comparing `xklb-2.7.9/xklb/createdb/row_add.py` & `xklb-2.8.1/xklb/createdb/row_add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import argparse
-from pathlib import Path
-
 from xklb import usage
-from xklb.utils import arggroups, db_utils, nums
+from xklb.utils import arggroups, argparse_utils, nums
 
 
 def parse_unknown_args_to_dict(unknown_args):
     kwargs = {}
     key = None
     values = []
 
@@ -29,19 +26,18 @@
     if len(values) > 0:
         kwargs[key] = get_val()
 
     return kwargs
 
 
 def row_add():
-    parser = argparse.ArgumentParser(description="Add arbitrary rows to a SQLITE db", usage=usage.row_add)
+    parser = argparse_utils.ArgumentParser(description="Add arbitrary rows to a SQLITE db", usage=usage.row_add)
     parser.add_argument("--table-name", "--table", "-t", default="media")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args, unknown_args = parser.parse_known_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
+    arggroups.args_post(args, parser, create_db=True)
 
     kwargs = parse_unknown_args_to_dict(unknown_args)
     args.db[args.table_name].insert(kwargs, alter=True)  # type: ignore
```

### Comparing `xklb-2.7.9/xklb/createdb/site_add.py` & `xklb-2.8.1/xklb/createdb/site_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import argparse, json
 from collections import defaultdict
 from io import StringIO
-from pathlib import Path
 
 from bs4 import BeautifulSoup, element
 
 from xklb import usage
 from xklb.text import extract_text
-from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, web
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, db_utils, iterables, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library site-add", usage=usage.site_add)
+    parser = argparse_utils.ArgumentParser(prog="library site-add", usage=usage.site_add)
     arggroups.selenium(parser)
     parser.set_defaults(selenium=True)
 
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
     parser.add_argument(
         "--extract-html-table", action="store_true", help="Extract data from HTML tables within the page"
     )
@@ -24,19 +23,17 @@
     parser.add_argument("--extract-xml", action="store_true", help="Extract data from XML")
 
     arggroups.debug(parser)
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.selenium_post(args)
 
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def extract_tables(dict_, table_name):
     dict_ = objects.flatten_dict_single_parents(dict_)
     dict_ = objects.flatten_grandparents(dict_)
 
@@ -269,15 +266,15 @@
         request = None
         response = None  # tell selenium-wire to not keep the response... idk if this works
 
     args.driver.response_interceptor = response_interceptor  # type: ignore
 
 
 def load_page(args, path):
-    if args.local_file:
+    if args.local_html:
         path = "file://" + path
 
     from selenium.common.exceptions import WebDriverException
 
     attach_interceptors(args)
     web.selenium_get_page(args, path)
```

### Comparing `xklb-2.7.9/xklb/createdb/substack.py` & `xklb-2.8.1/xklb/createdb/substack.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import argparse
-from pathlib import Path
 
 from bs4 import BeautifulSoup
 
 from xklb import usage
 from xklb.mediadb import db_media
-from xklb.utils import arggroups, db_utils, nums, objects, web
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, nums, web
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library substack", usage=usage.substack)
+    parser = argparse_utils.ArgumentParser(prog="library substack", usage=usage.substack)
     arggroups.requests(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("paths", nargs="+", help="Substack path to extract article for")
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def save_page(args, url):
     response = web.get(args, url)
     if response:
         soup = BeautifulSoup(response.text, "lxml")
```

### Comparing `xklb-2.7.9/xklb/createdb/subtitle.py` & `xklb-2.8.1/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/createdb/tabs_add.py` & `xklb-2.8.1/xklb/createdb/tabs_add.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 import argparse, sys
 from datetime import datetime, timedelta
-from pathlib import Path
 from random import randint
 
 from xklb import usage
 from xklb.mediadb import db_history, db_media
-from xklb.utils import arggroups, consts, db_utils, iterables, objects, path_utils, strings
+from xklb.utils import arggroups, argparse_utils, consts, iterables
 from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library tabs-add", usage=usage.tabs_add)
+    parser = argparse_utils.ArgumentParser(prog="library tabs-add", usage=usage.tabs_add)
     arggroups.extractor(parser)
     arggroups.frequency(parser)
 
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
     parser.add_argument("--allow-immediate", action="store_true")
     arggroups.debug(parser)
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
 
-    args.frequency = strings.partial_startswith(args.frequency, consts.frequency)
-
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.extractor_post(args)
+    arggroups.frequency_post(args)
 
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def get_days(frequency):
     d = {"weekly": 7, "monthly": 30, "quarterly": 89, "yearly": 364, "decadally": 3640}
     return d.get(frequency, 7)
 
 
-def get_new_paths(args) -> list[str]:
-    if not args.no_sanitize:
-        args.paths = [path_utils.sanitize_url(args, path) for path in args.paths]
-
+def get_new_paths(args, paths) -> list[str]:
     if args.category is None:
         qb = (
-            "select path from media where path in (" + ",".join(["?"] * len(args.paths)) + ")",
-            (*args.paths,),
+            "select path from media where path in (" + ",".join(["?"] * len(paths)) + ")",
+            (*paths,),
         )
     else:
         qb = (
-            "select path from media where category = ? and path in (" + ",".join(["?"] * len(args.paths)) + ")",
-            (args.category, *args.paths),
+            "select path from media where category = ? and path in (" + ",".join(["?"] * len(paths)) + ")",
+            (args.category, *paths),
         )
 
     try:
         existing = {d["path"] for d in args.db.query(*qb)}
     except Exception as e:
         log.debug(e)
     else:
@@ -62,16 +55,16 @@
             with args.db.conn:  # type: ignore
                 for p in list(existing):
                     args.db.conn.execute(  # type: ignore
                         "DELETE from history WHERE media_id = (select id from media where path = ?)", [p]
                     )
             db_media.mark_media_deleted(args, list(existing))
 
-    args.paths = iterables.conform([path.strip() for path in args.paths])
-    return args.paths
+    paths = iterables.conform([path.strip() for path in paths])
+    return paths
 
 
 def consolidate_url(args, path: str) -> dict:
     from urllib.parse import urlparse
 
     hostname = urlparse(path).hostname or ""
 
@@ -85,17 +78,17 @@
     }
 
 
 def tabs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
     args = parse_args()
-    args.paths = list(gen_paths(args))
+    paths = list(gen_paths(args))
 
-    tabs = iterables.list_dict_filter_bool([consolidate_url(args, path) for path in get_new_paths(args)])
+    tabs = iterables.list_dict_filter_bool([consolidate_url(args, path) for path in get_new_paths(args, paths)])
     for tab in tabs:
         db_media.add(args, tab)
     if not args.allow_immediate and args.frequency != "daily":
         # prevent immediately opening -- pick a random day within the week
         min_date = datetime.today() - timedelta(days=get_days(args.frequency) - 2)  # at least two days away
         max_date = datetime.today()
 
@@ -104,31 +97,27 @@
 
         for d in tabs:
             time_played = randint(min_time, max_time)
             db_history.add(args, [d["path"]], time_played=time_played, mark_done=True)
 
 
 def tabs_shuffle() -> None:
-    parser = argparse.ArgumentParser(prog="library tabs-shuffle", usage=usage.tabs_shuffle)
+    parser = argparse_utils.ArgumentParser(prog="library tabs-shuffle", usage=usage.tabs_shuffle)
     parser.add_argument("--days", "-d", type=int, default=7)
     parser.add_argument(
         "--frequency",
         "-f",
         type=str.lower,
         help=f"One of: {', '.join(consts.frequency)} (default: %(default)s)",
     )
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_intermixed_args()
-
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser)
 
     tabs = list(
         args.db.query(
             f"""
         WITH m as (
             SELECT
                 media.id
```

### Comparing `xklb-2.7.9/xklb/createdb/tildes.py` & `xklb-2.8.1/xklb/createdb/tildes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import argparse
 from datetime import datetime
-from pathlib import Path
 from time import sleep
 
 from bs4 import BeautifulSoup
 from dateutil import parser
 
 from xklb import usage
 from xklb.mediadb import db_media
-from xklb.utils import arggroups, db_utils, nums, objects, web
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, nums, web
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library tildes", usage=usage.tildes)
+    parser = argparse_utils.ArgumentParser(prog="library tildes", usage=usage.tildes)
     arggroups.requests(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("username", help="Tildes.net user to extract comments for")
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def save_page(args, text):
     soup = BeautifulSoup(text, "lxml")
 
     comment_elements = soup.find_all("article", class_="comment")
```

### Comparing `xklb-2.7.9/xklb/createdb/tube_add.py` & `xklb-2.8.1/xklb/createdb/tube_add.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,80 @@
 import argparse, sys
 from pathlib import Path
 
 from xklb import usage
 from xklb.createdb import tube_backend
 from xklb.mediadb import db_media, db_playlists
-from xklb.utils import arggroups, argparse_utils, consts, db_utils, iterables, objects, path_utils, processes
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, db_utils
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library " + action,
         usage=usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     arggroups.extractor(parser)
     arggroups.download(parser)
     arggroups.download_subtitle(parser)
     parser.set_defaults(download_archive=str(Path("~/.local/share/yt_archive.txt").expanduser().resolve()))
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     if action == SC.tube_add:
-        parser.add_argument(
-            "playlists", nargs="*", default=argparse_utils.STDIN_DASH, action=argparse_utils.ArgparseArgsOrStdin
-        )
+        arggroups.paths_or_stdin(parser)
 
     args = parser.parse_intermixed_args()
     args.action = action
 
-    if action == SC.tube_add:
-        Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    if hasattr(args, "playlists"):
-        args.playlists = list({s.strip() for s in args.playlists})
-        if not args.no_sanitize:
-            args.playlists = [path_utils.sanitize_url(args, p) for p in args.playlists]
-        args.playlists = iterables.conform(args.playlists)
-
-    processes.timeout(args.timeout)
+    arggroups.extractor_post(args)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser, create_db=action == SC.tube_add)
     return args
 
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
 
     args = parse_args(SC.tube_add, usage=usage.tube_add)
+    paths = arg_utils.gen_paths(args)
 
     if args.insert_only:
         args.db["media"].insert_all(
             [
                 {
                     "path": p,
                     "time_created": consts.APPLICATION_START,
                     "time_modified": 0,
                     "time_deleted": 0,
                 }
-                for p in args.playlists
+                for p in paths
             ],
             alter=True,
             ignore=True,
             pk="id",
         )
     elif args.insert_only_playlists:
         args.db["playlists"].insert_all(
-            [{"path": p, "time_created": consts.APPLICATION_START} for p in args.playlists],
+            [{"path": p, "time_created": consts.APPLICATION_START} for p in paths],
             alter=True,
             ignore=True,
             pk="path",
         )
     else:
+        paths = list(paths)
         known_playlists = set()
-        if not args.force and len(args.playlists) > 9:
+        if not args.force and len(paths) > 9:
             known_playlists = db_media.get_paths(args)
 
-        for path in args.playlists:
+        for path in paths:
             if args.safe and not tube_backend.is_supported(path):
                 log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
                 continue
 
             if path in known_playlists:
                 log.info("[%s]: Already added. Skipping!", path)
                 continue
```

### Comparing `xklb-2.7.9/xklb/createdb/tube_backend.py` & `xklb-2.8.1/xklb/createdb/tube_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 from pprint import pprint
 from subprocess import CalledProcessError
 from types import ModuleType
 
 from xklb.createdb import subtitle
 from xklb.data.yt_dlp_errors import (
-    prefix_unrecoverable_errors,
+    environment_errors,
     yt_meaningless_errors,
     yt_recoverable_errors,
     yt_unrecoverable_errors,
 )
 from xklb.mediadb import db_media, db_playlists
 from xklb.mediafiles import media_check
-from xklb.utils import consts, db_utils, iterables, objects, path_utils, printing, sql_utils, strings
-from xklb.utils.consts import DBType
+from xklb.utils import consts, db_utils, iterables, objects, printing, sql_utils, strings
+from xklb.utils.consts import DBType, DLStatus
 from xklb.utils.log_utils import Timer, log
 
 yt_dlp = None
 yt_archive = set()
 
 
 def load_module_level_yt_dlp() -> ModuleType:
@@ -70,17 +70,14 @@
     if args.verbose >= consts.LOG_DEBUG:
         all_opts.update(ignoreerrors=False, quiet=False)
     if args.ignore_errors:
         all_opts.update(ignoreerrors=True)
 
     log.debug(objects.dict_filter_bool(all_opts))
 
-    if hasattr(args, "playlists") and args.playlists and hasattr(args, "no_sanitize") and not args.no_sanitize:
-        args.playlists = [path_utils.sanitize_url(args, path) for path in args.playlists]
-
     return all_opts
 
 
 def is_supported(url) -> bool:  # thank you @dbr
     if consts.REGEX_V_REDD_IT.match(url):
         return True
 
@@ -309,14 +306,41 @@
         entry = ydl.extract_info(playlist_path, download=False)
         if entry and "entries" in entry:
             entries = entry.pop("entries")[0]
             entry = {**entry, **entries}
         return entry
 
 
+def log_error(ydl_log, webpath):
+    ydl_full_log = ydl_log["error"] + ydl_log["warning"] + ydl_log["info"]
+    ydl_errors = [
+        line for log_entry in ydl_full_log for line in log_entry.splitlines() if not yt_meaningless_errors.match(line)
+    ]
+    ydl_errors_txt = "\n".join(ydl_errors)
+
+    matched_error = strings.combine([line for line in ydl_errors if environment_errors.match(line)])
+    if matched_error:
+        log.warning("[%s]: Environment error. %s", webpath, matched_error)
+        raise SystemExit(28)
+
+    matched_error = strings.combine([line for line in ydl_errors if yt_recoverable_errors.match(line)])
+    if matched_error:
+        log.info("[%s]: Recoverable error matched (will try again later). %s", webpath, matched_error)
+        return DLStatus.RECOVERABLE_ERROR, matched_error
+
+    matched_error = strings.combine([line for line in ydl_errors if yt_unrecoverable_errors.match(line)])
+    if matched_error:
+        log.info("[%s]: Unrecoverable error matched. %s", webpath, matched_error)
+        return DLStatus.UNRECOVERABLE_ERROR, matched_error
+
+    log.error("[%s]: Unknown error. %s", webpath, ydl_errors_txt)
+    pprint(ydl_log)
+    return DLStatus.UNKNOWN_ERROR, ydl_errors_txt
+
+
 def download(args, m) -> None:
     yt_dlp = load_module_level_yt_dlp()
 
     ydl_log = {"error": [], "warning": [], "info": []}
 
     class DictLogger:
         def debug(self, msg):
@@ -405,21 +429,22 @@
         ydl_opts["format_sort"] = ["res:576"]
         ydl_opts["format"] = "bestvideo[filesize<2G]+bestaudio/best[filesize<2G]/bestvideo*+bestaudio/best"
 
     if args.profile == DBType.audio:
         ydl_opts[
             "format"
         ] = "bestaudio[ext=opus]/bestaudio[ext=mka]/bestaudio[ext=webm]/bestaudio[ext=ogg]/bestaudio[ext=oga]/bestaudio/best"
-        ydl_opts["postprocessors"].append({"key": "FFmpegExtractAudio", "preferredcodec": "opus"})
+        ydl_opts["postprocessors"].append({"key": "FFmpegExtractAudio", "preferredcodec": args.extract_audio_ext})
 
     def blocklist_check(info, *pargs, incomplete):
         if getattr(args, "blocklist_rules", False):
             media_entry = db_media.consolidate(deepcopy(info))
             if sql_utils.is_blocked_dict_like_sql(media_entry or {}, args.blocklist_rules):
                 raise yt_dlp.utils.RejectedVideoReached("Video matched library blocklist")
+
         ytdlp_match_filter = yt_dlp.utils.match_filter_func(" & ".join(match_filters).split(" | "))
         return ytdlp_match_filter(info, *pargs, incomplete)
 
     ydl_opts["match_filter"] = blocklist_check
 
     download_archive = Path(args.download_archive or "~/.local/share/yt_archive.txt").expanduser().resolve()
     if download_archive.exists() and not consts.PYTEST_RUNNING:
@@ -477,47 +502,39 @@
         if info is None:
             log.debug("[%s]: yt-dlp returned no info", webpath)
             info = m
         else:
             info = {**m, **info}
             local_path = info.get("local_path", None)
             if args.profile == DBType.audio:
-                local_path = ydl.prepare_filename({**info, "ext": args.ext})
+                local_path = ydl.prepare_filename({**info, "ext": args.extract_audio_ext})
             else:
                 local_path = ydl.prepare_filename(info)
 
-    ydl_full_log = ydl_log["error"] + ydl_log["warning"] + ydl_log["info"]
-    ydl_errors = [
-        line for log_entry in ydl_full_log for line in log_entry.splitlines() if not yt_meaningless_errors.match(line)
-    ]
-    ydl_errors_txt = "\n".join(ydl_errors)
-
-    if args.verbose >= consts.LOG_DEBUG_SQL:
-        log.debug("\n".join(ydl_full_log))
-
+    download_status = DLStatus.SUCCESS
+    media_check_failed = False
     if not ydl_log["error"] and info and local_path and Path(local_path).exists():
+        log.info("[%s]: Downloaded to %s", webpath, local_path)
         try:
             info["corruption"] = int(
                 media_check.calculate_corruption(local_path, threads=1, full_scan_if_corrupt=True) * 100
             )
         except (RuntimeError, CalledProcessError):
             info["corruption"] = 50
         if info["corruption"] > 7:
-            log.info("[%s]: Media check failed (will try again later)", webpath)
-            db_media.download_add(args, webpath, info, local_path, error="Media check failed")
-        else:
-            log.info("[%s]: Downloaded to %s", webpath, local_path)
-            db_media.download_add(args, webpath, info, local_path)
-    elif any(yt_recoverable_errors.match(line) for line in ydl_errors):
-        log.info("[%s]: Recoverable error matched (will try again later). %s", webpath, ydl_errors_txt)
-        db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt)
-    elif any(yt_unrecoverable_errors.match(line) for line in ydl_errors):
-        matched_error = iterables.conform([line for line in ydl_errors if yt_unrecoverable_errors.match(line)])
-        log.info("[%s]: Unrecoverable error matched. %s", webpath, ydl_errors_txt or strings.combine(matched_error))
-        db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt, unrecoverable_error=True)
-    elif any(prefix_unrecoverable_errors.match(line) for line in ydl_errors):
-        log.warning("[%s]: Prefix error. %s", webpath, ydl_errors_txt)
-        raise SystemExit(28)
+            media_check_failed = True
     else:
-        log.error("[%s]: Unknown error. %s", webpath, ydl_errors_txt)
-        pprint(ydl_full_log)
-        db_media.download_add(args, webpath, info, local_path, error=ydl_errors_txt)
+        download_status, ydl_errors_txt = log_error(ydl_log, webpath)
+
+    if media_check_failed:
+        log.info("[%s]: Media check failed", local_path)
+        download_status = DLStatus.RECOVERABLE_ERROR
+        ydl_errors_txt = "Media check failed\n" + ydl_errors_txt
+
+    db_media.download_add(
+        args,
+        webpath,
+        info,
+        local_path,
+        error=None if download_status == DLStatus.SUCCESS else ydl_errors_txt,
+        unrecoverable_error=download_status == DLStatus.UNRECOVERABLE_ERROR,
+    )
```

### Comparing `xklb-2.7.9/xklb/createdb/web_add.py` & `xklb-2.8.1/xklb/createdb/web_add.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,128 @@
-import argparse, json, random, sys, time
-from pathlib import Path
+import concurrent.futures, json, random, sys, time
 from urllib.parse import urlparse
 
 from xklb import usage
 from xklb.createdb import av, fs_add
 from xklb.files import sample_hash
 from xklb.mediadb import db_media, db_playlists
 from xklb.text import extract_links
-from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, iterables, objects, printing, strings, web
-from xklb.utils.consts import SC, DBType
+from xklb.utils import (
+    arg_utils,
+    arggroups,
+    argparse_utils,
+    consts,
+    db_utils,
+    file_utils,
+    iterables,
+    nums,
+    printing,
+    sql_utils,
+    strings,
+    web,
+)
+from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
-def parse_args(**kwargs):
-    parser = argparse.ArgumentParser(**kwargs)
+def parse_args(action, **kwargs):
+    parser = argparse_utils.ArgumentParser(**kwargs)
     arggroups.db_profiles(parser)
     arggroups.requests(parser)
     arggroups.selenium(parser)
     arggroups.filter_links(parser)
     arggroups.extractor(parser)
 
     parser.add_argument("--hash", action="store_true")
-    parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
+    parser.add_argument("--local-html", "--local-file", action="store_true", help="Treat paths as Local HTML files")
+    parser.add_argument(
+        "--sizes",
+        action="append",
+        help="Only grab extended metadata for files of specific sizes (uses the same syntax as fd-find)",
+    )
 
     arggroups.debug(parser)
     arggroups.database(parser)
-    if "add" in kwargs["prog"]:
+    if "add" in action:
         arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
+    args.action = action
 
     if not args.profiles:
         args.profiles = [DBType.filesystem]
 
-    if args.scroll:
-        args.selenium = True
-
-    if not args.case_sensitive:
-        args.before_include = [s.lower() for s in args.before_include]
-        args.path_include = [s.lower() for s in args.path_include]
-        args.text_include = [s.lower() for s in args.text_include]
-        args.after_include = [s.lower() for s in args.after_include]
-        args.before_exclude = [s.lower() for s in args.before_exclude]
-        args.path_exclude = [s.lower() for s in args.path_exclude]
-        args.text_exclude = [s.lower() for s in args.text_exclude]
-        args.after_exclude = [s.lower() for s in args.after_exclude]
-
-    if not args.no_url_decode:
-        args.path_include = [web.url_decode(s) for s in args.path_include]
-        args.path_exclude = [web.url_decode(s) for s in args.path_exclude]
+    if args.sizes:
+        args.sizes = sql_utils.parse_human_to_lambda(nums.human_to_bytes, args.sizes)
 
     if hasattr(args, "paths"):
         args.paths = [strings.strip_enclosing_quotes(s) for s in iterables.conform(args.paths)]
-    log.info(objects.dict_filter_bool(args.__dict__))
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
+    arggroups.extractor_post(args)
+    arggroups.filter_links_post(args)
+    arggroups.selenium_post(args)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
-    return args, parser
+    arggroups.args_post(args, parser, create_db=action == consts.SC.web_add)
+    return args
 
 
 def consolidate_media(args, path: str) -> dict:
     return {
-        "path": path,
+        "playlists_id": args.playlists_id,
         "time_created": consts.APPLICATION_START,
         "time_deleted": 0,
+        "path": path,
     }
 
 
 def add_media(args, media):
-    if isinstance(media[0], str):
-        media = [consolidate_media(args, s) for s in media]
-
     media = iterables.list_dict_filter_bool(media)
     args.db["media"].insert_all(media, pk="id", alter=True, replace=True)
 
 
+def add_extra_metadata(args, m):
+    extension = m["path"].rsplit(".", 1)[-1].lower()
+
+    remote_path = m["path"]  # for temp file extraction
+    if DBType.video in args.profiles and (extension in consts.VIDEO_EXTENSIONS or args.scan_all_files):
+        m |= av.munge_av_tags(args, m["path"])
+    if DBType.audio in args.profiles and (extension in consts.AUDIO_ONLY_EXTENSIONS or args.scan_all_files):
+        m |= av.munge_av_tags(args, m["path"])
+    if DBType.text in args.profiles and (extension in consts.TEXTRACT_EXTENSIONS or args.scan_all_files):
+        with web.PartialContent(m["path"]) as temp_file_path:
+            m |= fs_add.munge_book_tags_fast(temp_file_path)
+    if DBType.image in args.profiles and (extension in consts.IMAGE_EXTENSIONS or args.scan_all_files):
+        with web.PartialContent(m["path"], max_size=32 * 1024) as temp_file_path:
+            m |= fs_add.extract_image_metadata_chunk([{"path": temp_file_path}])[0]
+    m["path"] = remote_path  # restore from temp file extraction
+
+    return m
+
+
+def add_basic_metadata(args, m):
+    if DBType.filesystem in args.profiles:
+        m |= web.stat(m["path"])
+        m["type"] = file_utils.mimetype(m["path"])
+    else:
+        extension = m["path"].rsplit(".", 1)[-1].lower()
+        if (
+            args.scan_all_files
+            or (DBType.video in args.profiles and extension in consts.VIDEO_EXTENSIONS)
+            or (DBType.audio in args.profiles and extension in consts.AUDIO_ONLY_EXTENSIONS)
+            or (DBType.text in args.profiles and extension in consts.TEXTRACT_EXTENSIONS)
+            or (DBType.image in args.profiles and extension in consts.IMAGE_EXTENSIONS)
+        ):
+            m |= web.stat(m["path"])
+
+    if getattr(args, "hash", False):
+        # TODO: use head_foot_stream
+        m["hash"] = sample_hash.sample_hash_file(m["path"])
+
+    return m
+
+
 def spider(args, paths: set):
     original_paths = paths.copy()
     get_urls = iterables.return_unique(extract_links.get_inner_urls)
 
     new_media_count = 0
     known_paths = set()
     traversed_paths = set()
@@ -117,66 +160,42 @@
         else:
             if path not in (paths | traversed_paths):
                 if db_media.exists(args, path):
                     known_paths.add(path)
                 else:
                     new_paths[path] = None  # add key to map; title: None
 
-        media = [
-            {
-                "path": k,
-                "title": v,
-                "time_created": consts.APPLICATION_START,
-                "time_deleted": 0,
-            }
-            for k, v in new_paths.items()
-        ]
+        media = [consolidate_media(args, k) | {"title": v} for k, v in new_paths.items()]
         new_media_count += len(media)
-        for i, m in enumerate(media, start=1):
-            printing.print_overwrite(
-                f"Pages to scan {len(paths)} link scan: {new_media_count} new [{len(known_paths)} known]; basic metadata {i} of {len(media)}"
-            )
-
-            if DBType.filesystem in args.profiles:
-                m |= web.stat(m["path"])
-                m["type"] = file_utils.mimetype(m["path"])
-            else:
-                extension = m["path"].rsplit(".", 1)[-1].lower()
-                if (
-                    args.scan_all_files
-                    or (DBType.video in args.profiles and extension in consts.VIDEO_EXTENSIONS)
-                    or (DBType.audio in args.profiles and extension in consts.AUDIO_ONLY_EXTENSIONS)
-                    or (DBType.text in args.profiles and extension in consts.TEXTRACT_EXTENSIONS)
-                    or (DBType.image in args.profiles and extension in consts.IMAGE_EXTENSIONS)
-                ):
-                    m |= web.stat(m["path"])
-
-            if getattr(args, "hash", False):
-                # TODO: use head_foot_stream
-                m["hash"] = sample_hash.sample_hash_file(path)
-
-        for i, m in enumerate(media, start=1):
-            printing.print_overwrite(
-                f"Pages to scan {len(paths)} link scan: {new_media_count} new [{len(known_paths)} known]; extra metadata {i} of {len(media)}"
-            )
-
-            extension = m["path"].rsplit(".", 1)[-1].lower()
-
-            remote_path = m["path"]  # for temp file extraction
-            if DBType.video in args.profiles and (extension in consts.VIDEO_EXTENSIONS or args.scan_all_files):
-                m |= av.munge_av_tags(args, m["path"])
-            if DBType.audio in args.profiles and (extension in consts.AUDIO_ONLY_EXTENSIONS or args.scan_all_files):
-                m |= av.munge_av_tags(args, m["path"])
-            if DBType.text in args.profiles and (extension in consts.TEXTRACT_EXTENSIONS or args.scan_all_files):
-                with web.PartialContent(m["path"]) as temp_file_path:
-                    m |= fs_add.munge_book_tags_fast(temp_file_path)
-            if DBType.image in args.profiles and (extension in consts.IMAGE_EXTENSIONS or args.scan_all_files):
-                with web.PartialContent(m["path"], max_size=32 * 1024) as temp_file_path:
-                    m |= fs_add.extract_image_metadata_chunk([{"path": temp_file_path}])[0]
-            m["path"] = remote_path  # restore from temp file extraction
+
+        with concurrent.futures.ThreadPoolExecutor(max_workers=args.threads) as executor:
+            gen_media = (f.result() for f in [executor.submit(add_basic_metadata, args, m) for m in media])
+            for i, m in enumerate(gen_media):
+                media[i] = m
+                printing.print_overwrite(
+                    f"Pages to scan {len(paths)} link scan: {new_media_count} new [{len(known_paths)} known]; basic metadata {i + 1} of {len(media)}"
+                )
+
+        if args.sizes:
+            basic_media, extra_media = [], []
+            for d in media:
+                if d.get("size") is None or args.sizes(d["size"]):
+                    extra_media.append(d)
+                else:
+                    basic_media.append(d)
+            if basic_media:
+                add_media(args, basic_media)
+
+        with concurrent.futures.ThreadPoolExecutor(max_workers=args.threads) as executor:
+            gen_media = (f.result() for f in [executor.submit(add_extra_metadata, args, m) for m in media])
+            for i, m in enumerate(gen_media):
+                media[i] = m
+                printing.print_overwrite(
+                    f"Pages to scan {len(paths)} link scan: {new_media_count} new [{len(known_paths)} known]; extra metadata {i + 1} of {len(media)}"
+                )
 
         if media:
             add_media(args, media)
 
         printing.print_overwrite(
             f"Pages to scan {len(paths)} link scan: {new_media_count} new [{len(known_paths)} known]"
         )
@@ -184,59 +203,58 @@
     return new_media_count
 
 
 def add_playlist(args, path):
     info = {
         "hostname": urlparse(path).hostname,
         "extractor_key": "WebFolder",
-        "extractor_config": {k: v for k, v in args.__dict__.items() if k not in ["db", "database", "verbose", "paths"]},
+        "extractor_config": args.extractor_config,
         "time_deleted": 0,
     }
-    db_playlists.add(args, str(path), info)
+    return db_playlists.add(args, str(path), info)
 
 
 def web_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args, _parser = parse_args(prog=f"library {SC.web_add}", usage=usage.web_add)
+    args = parse_args(consts.SC.web_add, usage=usage.web_add)
     web.requests_session(args)  # configure session
 
     if args.insert_only:
         media_new = set()
         media_known = set()
         for p in arg_utils.gen_paths(args):
             if db_media.exists(args, p):
                 media_known.add(p)
             else:
-                add_media(args, [p])
+                add_media(args, [consolidate_media(args, p)])
                 media_new.add(p)
             printing.print_overwrite(f"Link import: {len(media_new)} new [{len(media_known)} known]")
     else:
         if args.selenium:
             web.load_selenium(args)
         try:
             for playlist_path in arg_utils.gen_paths(args):
+                args.playlists_id = add_playlist(args, playlist_path)
                 spider(args, {playlist_path})
-                if web.is_index(playlist_path):
-                    add_playlist(args, playlist_path)
 
         finally:
             if args.selenium:
                 web.quit_selenium(args)
 
     if not args.db["media"].detect_fts():
         db_utils.optimize(args)
 
 
 def web_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args, parser = parse_args(prog=f"library {SC.web_update}", usage=usage.web_update)
+    args = parse_args(consts.SC.web_add, usage=usage.web_update)
     web.requests_session(args)  # configure session
 
     web_playlists = db_playlists.get_all(
         args,
         sql_filters="extractor_key = 'WebFolder'",
         order_by="""length(path)-length(REPLACE(path, '/', '')) desc
         , random()
@@ -247,15 +265,15 @@
     if selenium_needed:
         web.load_selenium(args)
 
     try:
         playlist_count = 0
         for playlist in web_playlists:
             extractor_config = json.loads(playlist.get("extractor_config") or "{}")
-            args_env = arg_utils.override_config(parser, extractor_config, args)
+            args_env = arg_utils.override_config(args, extractor_config)
 
             # TODO: use directory Last-Modified header to skip file trees which don't need to be updated
             new_media = spider(args_env, {playlist["path"]})
 
             if new_media > 0:
                 db_playlists.decrease_update_delay(args, playlist["path"])
             else:
```

### Comparing `xklb-2.7.9/xklb/data/imagemagick_errors.py` & `xklb-2.8.1/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/data/wordbank.py` & `xklb-2.8.1/xklb/data/wordbank.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     "versus",
     "via",
     "with",
     "within",
     "without",
 )
 
-stop_words = (
+stop_words = [
     '"',
     "-",
     "'ll",
     "'ve",
     "&",
     "#",
     "^",
@@ -241,16 +241,14 @@
     "bu",
     "built",
     "bus",
     "buses",
     "but",
     "bx",
     "by",
-    "c'mon",
-    "c's",
     "c",
     "C",
     "c1",
     "c2",
     "c3",
     "ca",
     "call",
@@ -939,15 +937,14 @@
     "refs",
     "regarding",
     "regardless",
     "regards",
     "region",
     "related",
     "relatively",
-    "research-articl",
     "research",
     "respectively",
     "resulted",
     "resulting",
     "results",
     "rf",
     "rh",
@@ -1367,8 +1364,8 @@
     "ys",
     "yt",
     "z",
     "Z",
     "zero",
     "zi",
     "zz",
-)
+]
```

### Comparing `xklb-2.7.9/xklb/data/yt_dlp_errors.py` & `xklb-2.8.1/xklb/data/yt_dlp_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,19 +63,15 @@
 .*copyright claim""".splitlines(),
     ),
 )
 
 
 yt_meaningless_errors = re.compile(
     "|".join(
-        r""".*hidden
-.*timed out
-.*Timeout
-.*Timed
-.*Connection reset
+        r""".*Connection reset
 .*ConnectionReset
 .*Unable to extract
 .*Traceback
 .*Invalid argument
 .*KeyboardInterrupt
 .*Fatal Python error
 .*list index out of range
@@ -123,15 +119,14 @@
 .*Compressed file ended before the end-of-stream marker was reached
 .*Falling back on generic
 .*Some formats are possibly damaged
 .*WARNING: unable to obtain file audio codec with ffprobe
 .*matching opening tag for closing p tag not found
 .*the JSON object must be str, bytes or bytearray, not dict
 .*list indices must be integers
-.*The read operation timed out
 .*Unable to download JSON metadata
 .*Unable to recognize playlist.
 .*Premieres in""".splitlines(),
     ),
 )
 
 yt_unrecoverable_errors = re.compile(
@@ -245,15 +240,15 @@
 .*HTTP Error 410
 .*HTTPError 410
 .*stopping due to --break-match-filter""".splitlines(),
     ),
 )
 
 
-prefix_unrecoverable_errors = re.compile(
+environment_errors = re.compile(
     "|".join(
         r""".*unable to write data:
 .*No space left on device
 .*File name too long
 .*Transport endpoint is not connected
 .*unable to create directory
 .*Permission denied""".splitlines(),
```

### Comparing `xklb-2.7.9/xklb/editdb/dedupe_db.py` & `xklb-2.8.1/xklb/editdb/dedupe_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import argparse
-from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, argparse_utils, db_utils, objects
+from xklb.utils import arggroups, argparse_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library dedupe-dbs", usage=usage.dedupe_db)
+    parser = argparse_utils.ArgumentParser(prog="library dedupe-dbs", usage=usage.dedupe_db)
     parser.add_argument("--skip-upsert", action="store_true")
     parser.add_argument("--skip-0", action="store_true")
     parser.add_argument(
         "--only-columns", action=argparse_utils.ArgparseList, help="Comma separated column names to upsert"
     )
     parser.add_argument(
         "--primary-keys", "--pk", action=argparse_utils.ArgparseList, help="Comma separated primary keys"
@@ -25,19 +24,15 @@
     )
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("table")
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
-
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def dedupe_rows(args, tablename, primary_keys, business_keys):
     with args.db.conn:
         args.db.conn.execute(
             f"""
```

### Comparing `xklb-2.7.9/xklb/editdb/dedupe_media.py` & `xklb-2.8.1/xklb/editdb/dedupe_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from pathlib import Path
 
 import humanize
 
 from xklb import media_printer, usage
 from xklb.files import sample_compare, sample_hash
 from xklb.mediadb import db_media
-from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, objects, processes, strings
+from xklb.utils import arggroups, argparse_utils, consts, db_utils, devices, file_utils, processes, sql_utils
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library dedupe-media", usage=usage.dedupe_media)
+    parser = argparse_utils.ArgumentParser(prog="library dedupe-media", usage=usage.dedupe_media)
     arggroups.sql_fs(parser)
 
     profile = parser.add_mutually_exclusive_group()
     profile.add_argument(
         "--audio",
         action="store_const",
         dest="profile",
@@ -38,28 +38,21 @@
         "--title",
         action="store_const",
         dest="profile",
         const="title",
         help="Dedupe database by title",
     )
     profile.add_argument(
-        "--duration",
+        "--same-duration",
         action="store_const",
         dest="profile",
         const="duration",
         help="Dedupe database by duration (caution obviously)",
     )
     profile.add_argument(
-        "--fts",
-        action="store_const",
-        dest="profile",
-        const="fts",
-        help=argparse.SUPPRESS,
-    )
-    profile.add_argument(
         "--filesystem",
         "--fs",
         "--hash",
         action="store_const",
         dest="profile",
         const=DBType.filesystem,
         help="Dedupe filesystem database",
@@ -97,30 +90,28 @@
     )
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("paths", nargs="*")
     args = parser.parse_intermixed_args()
-    args.db = db_utils.connect(args)
-
     args.action = consts.SC.dedupe_media
+    arggroups.args_post(args, parser)
 
-    args.sort = "\n        , ".join(filter(bool, args.sort))
-    args.sort = args.sort.replace(",,", ",")
+    arggroups.sql_fs_post(args)
 
     args.filter_sql = []
     args.filter_bindings = {}
 
     COMPARE_DIRS = False
     if len(args.include + args.paths) == 2:
         COMPARE_DIRS = True
         if len(args.include) == 2:
             include2 = args.include.pop()
-            args.table2, search_bindings = db_utils.fts_search_sql(
+            args.table2, search_bindings = sql_utils.fts_search_sql(
                 "media",
                 fts_table=args.db["media"].detect_fts(),  # type: ignore
                 include=include2,
                 exclude=args.exclude,
                 flexible=args.flexible_search,
             )
             args.filter_bindings = {**args.filter_bindings, **search_bindings}
@@ -128,15 +119,15 @@
             path2 = args.paths.pop()
             args.table2 = "(select * from media where path like :path2)"
             for _idx, _path in enumerate(args.paths):  # this does not seem right...
                 args.filter_bindings["path2"] = path2.replace(" ", "%").replace("%%", " ") + "%"
 
     args.table = "media"
     if args.db["media"].detect_fts() and args.include:  # type: ignore
-        args.table, search_bindings = db_utils.fts_search_sql(
+        args.table, search_bindings = sql_utils.fts_search_sql(
             "media",
             fts_table=args.db["media"].detect_fts(),  # type: ignore
             include=args.include,
             exclude=args.exclude,
             flexible=args.flexible_search,
         )
         args.filter_bindings = {**args.filter_bindings, **search_bindings}
@@ -148,22 +139,23 @@
         )
         for idx, path in enumerate(args.paths):
             args.filter_bindings[f"path{idx}"] = path.replace(" ", "%").replace("%%", " ") + "%"
 
     if not COMPARE_DIRS:
         args.table2 = args.table
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def get_rows(args) -> list[dict]:
+def get_rows(args, m_columns) -> list[dict]:
+    m_columns = sql_utils.search_filter(args, m_columns)
+
     query = f"""
     SELECT
-        {', '.join(db_utils.config["media"]["search_columns"])}
+        {', '.join(s for s in db_utils.config["media"]["search_columns"] if s in m_columns)}
     FROM
         {args.table}
     WHERE 1=1
         and time_deleted = 0
         and audio_count > 0
         and duration is not null
         and path not like 'http%'
@@ -180,14 +172,16 @@
     """
 
     return args.db.query(query, args.filter_bindings)
 
 
 def get_music_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
+    m_columns = sql_utils.search_filter(args, m_columns)
+
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
         , m2.path duplicate_path
@@ -226,14 +220,16 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_id_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
+    m_columns = sql_utils.search_filter(args, m_columns)
+
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
         , m2.path duplicate_path
@@ -268,14 +264,16 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_title_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
+    m_columns = sql_utils.search_filter(args, m_columns)
+
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
         , m2.path duplicate_path
@@ -310,14 +308,16 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_duration_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
+    m_columns = sql_utils.search_filter(args, m_columns)
+
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
         , m2.path duplicate_path
@@ -352,14 +352,16 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_fs_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
+    m_columns = sql_utils.search_filter(args, m_columns)
+
     query = f"""
     SELECT
         path
         , size
         {', hash' if 'hash' in m_columns else ''}
     FROM
         {args.table} m1
@@ -473,64 +475,14 @@
 
             $ cbird -i.algos 1 -update
             $ cbird -dups -select-result -sort-rev resolution -chop -nuke  # exact duplicates
             $ cbird -p.dht 1 -similar -select-result -sort-rev resolution -chop -nuke  # similar photos
         """,
         )
         return
-    elif args.profile == "fts":
-        m_columns = db_utils.columns(args, "media")
-        m_columns.update(rank=int)
-        fts_table = args.db["media"].detect_fts()
-
-        rows = get_rows(args)
-        for row in rows:
-            words = set(
-                iterables.conform(strings.extract_words(Path(v).stem if k == "path" else v) for k, v in row.items()),
-            )
-            table, search_bindings = db_utils.fts_search_sql(
-                "media",
-                fts_table=fts_table,
-                include=sorted(words, key=len, reverse=True)[:100],
-                exclude=args.exclude,
-                flexible=False,
-            )
-
-            query = f"""
-                SELECT path
-                FROM {table} m
-                WHERE path in (select path from {args.table})
-                ORDER BY
-                    video_count > 0 DESC
-                    {', subtitle_count > 0 DESC' if 'subtitle_count' in m_columns else ''}
-                    , audio_count DESC
-                    , length(path)-length(REPLACE(path, '{os.sep}', '')) DESC
-                    , length(path)-length(REPLACE(path, '.', ''))
-                    , length(path)
-                    , size DESC
-                    , time_modified DESC
-                    , time_created DESC
-                    , duration DESC
-                    , path DESC
-                    , path
-                {"LIMIT " + str(args.limit) if args.limit else ""}
-                """
-
-            related_media = set(
-                filter_split_files(
-                    d["path"] for d in args.db.query(query, {**args.filter_bindings, **search_bindings})
-                ),
-            )
-            if len(related_media) > 1:
-                print("Found", len(related_media) - 1, "duplicates")
-                print(related_media)
-
-                breakpoint()  # TODO: get this working...
-
-        return
     else:
         raise NotImplementedError
 
     deletion_candidates = []
     deletion_paths = []
     for d in duplicates:
         if args.dirname and (
```

### Comparing `xklb-2.7.9/xklb/editdb/merge_online_local.py` & `xklb-2.8.1/xklb/editdb/merge_online_local.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import argparse, os
 from copy import deepcopy
 
 from xklb import media_printer, usage
 from xklb.mediadb import db_media
-from xklb.utils import arggroups, consts, db_utils, devices, objects
+from xklb.utils import arggroups, argparse_utils, consts, devices, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library merge-online-local", usage=usage.merge_online_local)
+    parser = argparse_utils.ArgumentParser(prog="library merge-online-local", usage=usage.merge_online_local)
     parser.add_argument("--no-confirm", "--yes", "-y", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="100")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_args()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser)
+
     return args
 
 
 def get_duplicates(args) -> list[dict]:
     query = f"""
     WITH m1 as (
         SELECT
```

### Comparing `xklb-2.7.9/xklb/editdb/mpv_watchlater.py` & `xklb-2.8.1/xklb/editdb/mpv_watchlater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import argparse
 from pathlib import Path
 
 from xklb import usage
 from xklb.mediadb import db_history
-from xklb.utils import arggroups, consts, db_utils, mpv_utils, nums, objects
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, consts, mpv_utils, nums
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library mpv-watchlater", usage=usage.mpv_watchlater)
+    parser = argparse_utils.ArgumentParser(prog="library mpv-watchlater", usage=usage.mpv_watchlater)
     parser.add_argument("--watch-later-directory", default=consts.DEFAULT_MPV_WATCH_LATER, help=argparse.SUPPRESS)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def scan_and_import(args, media) -> None:
     md5s = {mpv_utils.path_to_mpv_watchlater_md5(m["path"]): m for m in media}
     paths = set(Path(args.watch_later_directory).glob("*"))
```

### Comparing `xklb-2.7.9/xklb/editdb/pushshift.py` & `xklb-2.8.1/xklb/editdb/pushshift.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import argparse, sys
-from pathlib import Path
 
 from xklb import usage
 from xklb.createdb.reddit_add import slim_post_data
-from xklb.utils import arggroups, db_utils, objects, printing
+from xklb.utils import arggroups, argparse_utils, objects, printing
 from xklb.utils.log_utils import log
 
 try:
     import orjson
 except ModuleNotFoundError:
     import json as orjson
 
 
 def parse_args(action, usage) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
+    parser = argparse_utils.ArgumentParser(prog="library " + action, usage=usage)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
-
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def save_data(args, reddit_posts, media) -> None:
     if len(reddit_posts) > 0:
         args.db["reddit_posts"].insert_all(reddit_posts, alter=True)
         reddit_posts.clear()
```

### Comparing `xklb-2.7.9/xklb/editdb/reddit_selftext.py` & `xklb-2.8.1/xklb/editdb/reddit_selftext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import argparse, html
 from urllib.parse import urlparse
 
 from xklb import usage
 from xklb.mediadb import db_media
-from xklb.utils import arggroups, db_utils, log_utils, objects
+from xklb.utils import arggroups, argparse_utils, db_utils, log_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library reddit-selftext", usage=usage.reddit_selftext)
+    parser = argparse_utils.ArgumentParser(prog="library reddit-selftext", usage=usage.reddit_selftext)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def get_page_links(path, text) -> tuple[set, set]:
     from bs4 import BeautifulSoup
 
     soup = BeautifulSoup(html.unescape(text), "lxml")
```

### Comparing `xklb-2.7.9/xklb/files/christen.py` & `xklb-2.8.1/xklb/files/christen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import argparse, shutil
 from os import fsdecode, fsencode
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, file_utils, objects, path_utils
+from xklb.utils import arggroups, argparse_utils, file_utils, path_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library christen", usage=usage.christen)
+    parser = argparse_utils.ArgumentParser(prog="library christen", usage=usage.christen)
     parser.add_argument("--dot-space", action="store_true")
     parser.add_argument("--case-insensitive", action="store_true")
     parser.add_argument("--lowercase-folders", action="store_true")
     parser.add_argument("--overwrite", "--force", action="store_true")
     parser.add_argument("--run", "-r", action="store_true")
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def rename_path(args, base, b) -> None:
     fixed = path_utils.clean_path(
         b,
         dot_space=args.dot_space,
```

### Comparing `xklb-2.7.9/xklb/files/sample_compare.py` & `xklb-2.8.1/xklb/files/sample_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-import argparse, hashlib
+import hashlib
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from xklb import usage
 from xklb.files import sample_hash
-from xklb.utils import arggroups, nums, objects
+from xklb.utils import arggroups, argparse_utils
 from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(prog="library sample-compare", usage=usage.sample_compare)
+    parser = argparse_utils.ArgumentParser(prog="library sample-compare", usage=usage.sample_compare)
     arggroups.sample_hash_bytes(parser)
     parser.add_argument("--ignore-holes", "--ignore-sparse", action="store_true")
     parser.add_argument("--skip-full-hash", action="store_true")
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    args.gap = nums.float_from_percent(args.gap)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.sample_hash_bytes_post(args)
     return args
 
 
 def full_hash_file(path):
     sha256_hash = hashlib.sha256()
 
     try:
@@ -92,17 +91,17 @@
 
     return is_equal
 
 
 def sample_compare() -> None:
     args = parse_args()
 
-    args.paths = list(gen_paths(args))
+    paths = list(gen_paths(args))
     is_equal = sample_cmp(
-        *args.paths,
+        *paths,
         threads=args.threads,
         gap=args.gap,
         chunk_size=args.chunk_size,
         ignore_holes=args.ignore_holes,
         skip_full_hash=args.skip_full_hash,
     )
```

### Comparing `xklb-2.7.9/xklb/files/sample_hash.py` & `xklb-2.8.1/xklb/files/sample_hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import argparse, hashlib, shlex
+import hashlib, shlex
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, nums, objects
+from xklb.utils import arggroups, argparse_utils, nums
 from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(prog="library sample-hash", usage=usage.sample_hash)
+    parser = argparse_utils.ArgumentParser(prog="library sample-hash", usage=usage.sample_hash)
     arggroups.sample_hash_bytes(parser)
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    args.gap = nums.float_from_percent(args.gap)
+    arggroups.sample_hash_bytes_post(args)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def single_thread_read(path, segments, chunk_size):
     with open(path, "rb") as f:
         for start in segments:
             f.seek(start)
```

### Comparing `xklb-2.7.9/xklb/files/similar_files.py` & `xklb-2.8.1/xklb/files/similar_files.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 import argparse
 
 import humanize
 from tabulate import tabulate
 
 from xklb import usage
 from xklb.folders.similar_folders import cluster_folders, map_and_name
-from xklb.utils import arg_utils, arggroups, consts, nums, objects, printing
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, nums, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(usage=usage.similar_files)
-    arggroups.operation_cluster(parser)
+    parser = argparse_utils.ArgumentParser(usage=usage.similar_files)
+    arggroups.cluster(parser)
 
-    parser.add_argument("--print", "-p", default="", const="p", nargs="?")
-    parser.add_argument("--small", "--reverse", "-r", action="store_true")
+    parser.add_argument("--small", "--reverse", action="store_true")
     parser.add_argument("--only-duplicates", action="store_true")
     parser.add_argument("--only-originals", action="store_true")
 
     parser.add_argument("--full-path", action="store_true", help="Cluster using full path instead of only file name")
     parser.add_argument("--estimated-duplicates", "--dupes", type=float)
 
+    parser.add_argument("--durations-delta", "--duration-delta", type=float, default=10.0)
     parser.add_argument("--sizes-delta", "--size-delta", type=float, default=10.0)
 
-    parser.add_argument("--no-filter-names", dest="filter_names", action="store_false")
-    parser.add_argument("--no-filter-sizes", dest="filter_sizes", action="store_false")
+    parser.add_argument("--filter-names", action=argparse.BooleanOptionalAction, default=True)
+    parser.add_argument("--filter-sizes", action=argparse.BooleanOptionalAction, default=True)
+    parser.add_argument("--filter-durations", action=argparse.BooleanOptionalAction, default=True)
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    args.action = consts.SC.similar_files
+    arggroups.args_post(args, parser)
 
     if not args.filter_sizes:
         args.sizes_delta = 200.0
+    if not args.filter_durations:
+        args.durations_delta = 200.0
 
-    if not args.filter_names and not args.filter_sizes:
+    if not args.filter_names and not args.filter_sizes and not args.filter_durations:
         print("Nothing to do")
         raise NotImplementedError
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def is_same_size_group(args, m0, m):
     size_diff = nums.percentage_difference(m0["size"], m["size"])
+
+    if "duration" in m:
+        duration_diff = nums.percentage_difference(m0["duration"], m["duration"])
+        return size_diff < args.sizes_delta and duration_diff < args.durations_delta
+
     return size_diff < args.sizes_delta
 
 
 def cluster_by_size(args, media):
     group_id = 0
     temp_groups = []
     media_groups = []
@@ -91,35 +100,36 @@
     return groups
 
 
 def similar_files():
     args = parse_args()
     media = list(arg_utils.gen_d(args))
 
-    if args.filter_sizes:
+    groups: list[dict] = []
+    if args.filter_sizes or args.filter_durations:
         clusters = cluster_by_size(args, media)
         groups = map_and_name(media, clusters)
-        log.info("file size/count clustering sorted %s files into %s groups", len(media), len(groups))
+        log.info("file size/duration clustering sorted %s files into %s groups", len(media), len(groups))
         single_file_groups = [d for d in groups if len(d["grouped_paths"]) == 1]
         groups = [d for d in groups if len(d["grouped_paths"]) > 1]
         log.info("Filtered out %s single-file groups", len(single_file_groups))
         log.debug(single_file_groups)
 
         if args.filter_names:
             media = [d for group in groups for d in group["grouped_paths"]]
 
     if args.filter_names:
         groups = cluster_folders(args, media)
         groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_path"])))
         log.info("Name clustering sorted %s files into %s groups", len(media), len(groups))
 
-        if args.filter_sizes:
+        if args.filter_sizes or args.filter_durations:
             prev_count = len(groups)
             groups = filter_groups_by_size(args, groups)  # effectively a second pass
-            log.info("(2nd pass) group size/count filtering removed %s groups", prev_count - len(groups))
+            log.info("(2nd pass) group size/duration filtering removed %s groups", prev_count - len(groups))
 
     if not args.only_originals and not args.only_duplicates:
         print("Duplicate groups:")
 
     for group in groups:
         media = group["grouped_paths"]
         media = sorted(media, key=lambda d: d["size"], reverse=not args.small)
@@ -135,14 +145,15 @@
         else:
             print(
                 tabulate(
                     [
                         {
                             f'group {group["common_path"]}': d["path"],
                             "size": humanize.naturalsize(d["size"], binary=True),
+                            "duration": printing.human_duration(d["duration"]),
                         }
                         for d in media
                     ],
                     tablefmt=consts.TABULATE_STYLE,
                     headers="keys",
                     showindex=False,
                 )
```

### Comparing `xklb-2.7.9/xklb/folders/merge_folders.py` & `xklb-2.8.1/xklb/folders/merge_folders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import argparse, json, os
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arg_utils, arggroups, devices, file_utils, objects, printing
+from xklb.utils import arg_utils, arggroups, argparse_utils, devices, file_utils, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library merge-folders", usage=usage.merge_folders)
-    arggroups.capability_clobber(parser)
-    arggroups.capability_simulate(parser)
+    parser = argparse_utils.ArgumentParser(prog="library merge-folders", usage=usage.merge_folders)
+    arggroups.clobber(parser)
+    arggroups.simulate(parser)
     arggroups.debug(parser)
 
     parser.add_argument("sources", nargs="+")
     parser.add_argument("destination")
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser)
 
     args.destination = arg_utils.split_folder_glob(args.destination)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def existing_stats(root_folder, root_glob):
     prefix = f"{root_folder}{os.sep}{root_glob}"
 
     files: set[Path] = set()
@@ -66,18 +66,16 @@
             log.debug("%s can be renamed cleanly to %s", source_file, renamed_file)
         source_rename_data.append((is_conflict, source_file, renamed_file))
     return source_rename_data
 
 
 def get_clobber(args):
     choice = None
-    if args.replace:
-        choice = "replace"
-    elif args.no_replace:
-        choice = "no-replace"
+    if args.replace is not None:
+        choice = "replace" if args.replace else "no-replace"
     else:
         choice = devices.prompt(choices=["replace", "no-replace", "simulate-replace", "quit"])
 
     if choice == "quit":
         raise SystemExit(130)
     if choice == "simulate-replace":
         args.simulate = True
```

### Comparing `xklb-2.7.9/xklb/folders/mount_stats.py` & `xklb-2.8.1/xklb/folders/mount_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import argparse
-
 from xklb import usage
-from xklb.utils import arggroups
+from xklb.utils import arggroups, argparse_utils
 from xklb.utils.devices import get_mount_stats
 
 # TODO: filter out mount points with different paths but are subpaths of the same mount point
 
 
 def mount_stats() -> None:
-    parser = argparse.ArgumentParser(usage=usage.mount_stats)
+    parser = argparse_utils.ArgumentParser(usage=usage.mount_stats)
     arggroups.debug(parser)
 
     parser.add_argument("mounts", nargs="+")
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
     space = get_mount_stats(args.mounts)
 
     print("Relative disk dependence:")
     for d in space:
         print(f"{d['mount']}: {'#' * int(d['used'] * 80)} {d['used']:.1%}")
```

### Comparing `xklb-2.7.9/xklb/folders/move_list.py` & `xklb-2.8.1/xklb/folders/move_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,37 @@
 from copy import deepcopy
 from pathlib import Path
 
 import humanize
 from tabulate import tabulate
 
 from xklb import usage
-from xklb.utils import arggroups, consts, db_utils, devices, iterables, objects, printing
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, consts, devices, iterables, printing, sqlgroups
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library mv-list",
         usage=usage.mv_list,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     arggroups.sql_fs(parser)
-    arggroups.operation_group_folders(parser)
+    arggroups.group_folders(parser)
     parser.set_defaults(limit="25", lower=4, upper=4000)
     arggroups.debug(parser)
 
-    parser.add_argument("mount_point")
+    parser.add_argument("target_mount_point")
     arggroups.database(parser)
+    parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser)
+
+    arggroups.sql_fs_post(args)
+    arggroups.group_folders_post(args)
+
     return args
 
 
 def group_by_folder(args, media) -> list[dict]:
     d = {}
     for m in media:
         if m["path"].startswith("http"):
@@ -45,36 +48,24 @@
                 d[parent]["count"] += 1
             else:
                 d[parent] = {
                     "size": m["size"],
                     "count": 1,
                 }
 
-    for path, pdict in list(d.items()):
-        if any([pdict["count"] < args.lower, pdict["count"] > args.upper]):
-            d.pop(path)
+    if args.folder_counts:
+        for path, pdict in list(d.items()):
+            if not args.folder_counts(pdict["count"]):
+                d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def get_table(args) -> list[dict]:
-    media = list(
-        args.db.query(
-            """
-        select
-            path
-            , size
-        from media
-        where 1=1
-            and coalesce(time_deleted, 0)=0
-            and size > 0
-        order by path
-        """,
-        ),
-    )
+    media = list(args.db.query(*sqlgroups.fs_sql(args)))
 
     folders = group_by_folder(args, media)
     return sorted(folders, key=lambda x: x["size"] / x["count"])
 
 
 def iterate_and_show_options(args, tbl) -> tuple[list[dict], list[dict]]:
     vew = tbl[-int(args.limit) :] if args.limit else tbl
@@ -107,17 +98,17 @@
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
 def move_list() -> None:
     args = parse_args()
-    _total, _used, free = shutil.disk_usage(args.mount_point)
+    _total, _used, free = shutil.disk_usage(args.target_mount_point)
 
-    print("Current free space:", humanize.naturalsize(free))
+    print("Current free space in target:", humanize.naturalsize(free))
 
     data = get_table(args)
 
     tbl = deepcopy(data)
     cur, rest = iterate_and_show_options(args, tbl)
 
     data = {d["path"]: d for d in data}
@@ -186,15 +177,15 @@
             "; future free space:",
             humanize.naturalsize(selected_paths_size + free, binary=True),
         )
 
     if selected_paths:
         temp_file = Path(tempfile.mktemp())
         with temp_file.open("w") as f:
-            f.writelines("\n".join(selected_paths))
+            f.writelines(l + "\n" for l in selected_paths)
 
         print(
             f"""
 
     Folder list saved to {temp_file}. You may want to use the following command to move files to an EMPTY folder target:
 
         rsync -aE --xattrs --info=progress2 --no-inc-recursive --remove-source-files --files-from={temp_file} -r -vv --dry-run / jim:/free/real/estate/
```

### Comparing `xklb-2.7.9/xklb/folders/rel_mv.py` & `xklb-2.8.1/xklb/folders/rel_mv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,53 @@
 import argparse, shlex
 from os.path import commonprefix
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, argparse_utils, file_utils, objects, path_utils, processes
+from xklb.utils import arggroups, argparse_utils, file_utils, path_utils, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library relmv", usage=usage.relmv)
-    arggroups.capability_simulate(parser)
-    parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
+    parser = argparse_utils.ArgumentParser(prog="library relmv", usage=usage.relmv)
+    arggroups.simulate(parser)
     arggroups.debug(parser)
 
     parser.add_argument("sources", nargs="+", help="one or more source files or directories to move")
     parser.add_argument("dest", help="destination directory")
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
+def gen_rel_path(source, dest: Path, relative_from=None):
+    if relative_from:
+        relative_from = Path(relative_from).expanduser().resolve()
+
+    abspath = Path(source).expanduser().resolve()
+
+    if relative_from:
+        relpath = str(abspath.relative_to(relative_from))
+    else:
+        rel_prefix = commonprefix([abspath, dest])
+        try:
+            relpath = str(abspath.relative_to(rel_prefix))
+        except ValueError:
+            try:
+                relpath = str(abspath.relative_to(Path(rel_prefix).parent))
+            except ValueError:
+                relpath = str(source)
+
+    target_dir = (dest / relpath).parent
+    target_dir = path_utils.dedupe_path_parts(target_dir)
+    new_path = target_dir / abspath.name
+    return new_path
+
+
 def rel_move(sources, dest, simulate=False, relative_from=None):
     if relative_from:
         relative_from = Path(relative_from).expanduser().resolve()
 
     new_paths = []
     for source in sources:
         abspath = Path(source).expanduser().resolve()
@@ -70,14 +93,15 @@
 
 
 def rel_mv() -> None:
     args = parse_args()
 
     dest = Path(args.dest).expanduser().resolve()
 
+    sources = args.sources
     if args.ext:
-        args.sources = [p for source in args.sources for p in file_utils.rglob(source, args.ext)[0]]
-    rel_move(args.sources, dest, simulate=args.simulate)
+        sources = [p for source in sources for p in file_utils.rglob(source, args.ext)[0]]
+    rel_move(sources, dest, simulate=args.simulate)
 
 
 if __name__ == "__main__":
     rel_mv()
```

### Comparing `xklb-2.7.9/xklb/folders/scatter.py` & `xklb-2.8.1/xklb/folders/scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 from collections import Counter
 from pathlib import Path
 
 from humanize import naturalsize
 from tabulate import tabulate
 
 from xklb import usage
-from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, nums, objects, printing
+from xklb.utils import arggroups, argparse_utils, consts, db_utils, devices, file_utils, iterables, nums, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library scatter",
         usage=usage.scatter,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue")
     parser.add_argument("--max-files-per-folder", "--max-files-per-directory", type=int)
-    parser.add_argument("--policy", "-p")
-    parser.add_argument("--group", "-g")
-    parser.add_argument("--sort", "-s", default="random()", help="Sort files before moving")
+    parser.add_argument("--policy")
+    parser.add_argument("--group")
+    parser.add_argument("--sort", default="random()", help="Sort files before moving")
     parser.add_argument("--targets", "--srcmounts", "-m", help="Colon separated destinations eg. /mnt/d1:/mnt/d2")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument(
         "relative_paths",
         nargs="+",
         help="Paths to scatter; if using -m any path substring is valid (relative to the root of your mergerfs mount)",
     )
     args = parser.parse_intermixed_args()
-    args.db = db_utils.connect(args)
+    arggroups.args_post(args, parser)
 
     if args.targets:
         args.targets = [m.rstrip("\\/") for m in args.targets.split(":")]
         if args.group is None:
             args.group = "size"
         if args.policy is None:
             args.policy = "pfrd"
@@ -54,15 +54,14 @@
     if args.targets is None and args.policy not in ("rand", "used"):
         msg = "Without targets defined the only meaningful policies are: `rand` or `used`"
         raise ValueError(msg)
 
     args.relative_paths = file_utils.resolve_absolute_paths(args.relative_paths)
     args.targets = file_utils.resolve_absolute_paths(args.targets)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def get_table(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     or_paths = [f"path like :path_{i}" for i, _path in enumerate(args.relative_paths)]
```

### Comparing `xklb-2.7.9/xklb/folders/similar_folders.py` & `xklb-2.8.1/xklb/folders/similar_folders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 import argparse
 from pathlib import Path
 
 import humanize
 from tabulate import tabulate
 
 from xklb import usage
-from xklb.fsdb import big_dirs
+from xklb.folders import big_dirs
 from xklb.text import cluster_sort
-from xklb.utils import arg_utils, arggroups, consts, nums, objects, path_utils, printing, sql_utils, strings
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, file_utils, nums, path_utils, printing, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(usage=usage.similar_folders)
-    arggroups.operation_group_folders(parser)
-    arggroups.operation_cluster(parser)
+    parser = argparse_utils.ArgumentParser(usage=usage.similar_folders)
+    arggroups.group_folders(parser)
+    arggroups.cluster(parser)
 
-    parser.add_argument("--print", "-p", default="", const="p", nargs="?")
-    parser.add_argument("--small", "--reverse", "-r", action="store_true")
+    parser.add_argument("--small", "--reverse", action="store_true")
     parser.add_argument("--only-duplicates", action="store_true")
     parser.add_argument("--only-originals", action="store_true")
 
     parser.add_argument(
         "--full-path", action="store_true", help="Cluster using full path instead of just the parent folder name"
     )
     parser.add_argument("--estimated-duplicates", "--dupes", type=float)
 
     parser.add_argument("--total-sizes", action="store_true", help="Compare total size instead of median size")
+    parser.add_argument(
+        "--total-durations", action="store_true", help="Compare total duration instead of median duration"
+    )
     parser.add_argument("--sizes-delta", "--size-delta", type=float, default=10.0)
     parser.add_argument("--counts-delta", "--count-delta", type=float, default=3.0)
+    parser.add_argument("--durations-delta", "--duration-delta", type=float, default=5.0)
+
+    parser.add_argument("--filter-names", action=argparse.BooleanOptionalAction, default=True)
+    parser.add_argument("--filter-sizes", action=argparse.BooleanOptionalAction, default=True)
+    parser.add_argument("--filter-durations", action=argparse.BooleanOptionalAction, default=True)
+    parser.add_argument("--filter-counts", action=argparse.BooleanOptionalAction, default=True)
 
-    parser.add_argument("--no-filter-names", dest="filter_names", action="store_false")
-    parser.add_argument("--no-filter-counts", dest="filter_counts", action="store_false")
-    parser.add_argument("--no-filter-sizes", dest="filter_sizes", action="store_false")
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    args.action = consts.SC.similar_folders
+    arggroups.args_post(args, parser)
+
+    arggroups.group_folders_post(args)
 
     if not args.filter_counts:
         args.counts_delta = 200.0
     if not args.filter_sizes:
         args.sizes_delta = 200.0
+    if not args.filter_durations:
+        args.duration_delta = 200.0
 
-    if not args.filter_names and not args.filter_counts and not args.filter_sizes:
+    if not args.filter_names and not args.filter_counts and not args.filter_sizes and not args.filter_durations:
         print("Nothing to do")
         raise NotImplementedError
 
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.sql_fs_post(args)
+    arggroups.group_folders_post(args)
+
     return args
 
 
 def map_and_name(media, clusters):
     bound_dicts = cluster_sort.map_cluster_to_paths(media, clusters)
 
     result = []
@@ -78,97 +91,103 @@
 
     clusters = cluster_sort.find_clusters(n_clusters, sentence_strings, stop_words=args.stop_words)
     groups = map_and_name(media, clusters)
 
     return groups
 
 
-def is_same_size_group(args, m0, m):
+def is_same_group(args, m0, m):
     count_diff = nums.percentage_difference(m0["exists"], m["exists"])
     if args.total_sizes:
         size_diff = nums.percentage_difference(m0["size"], m["size"])
     else:
         size_diff = nums.percentage_difference(m0["median_size"], m["median_size"])
-    return size_diff < args.sizes_delta and count_diff < args.counts_delta
 
+    if args.total_durations:
+        duration_diff = nums.percentage_difference(m0["duration"], m["duration"])
+    else:
+        duration_diff = nums.percentage_difference(m0["median_duration"], m["median_duration"])
+
+    return size_diff < args.sizes_delta and count_diff < args.counts_delta and duration_diff < args.durations_delta
 
-def cluster_by_size(args, media):
+
+def cluster_by_numbers(args, media):
     group_id = 0
     temp_groups = []
     media_groups = []
     for m in media:
         grouped = False
         for i, group in enumerate(temp_groups):
             m0 = group[0]
-            if is_same_size_group(args, m0, m):
+            if is_same_group(args, m0, m):
                 group.append(m)
                 media_groups.append(i)
                 grouped = True
                 break
 
         if not grouped:
             temp_groups.append([m])
             media_groups.append(group_id)
             group_id += 1
 
     assert len(media_groups) == len(media)
     return media_groups
 
 
-def filter_group_by_size(args, group):
+def filter_group_by_numbers(args, group):
     media = group["grouped_paths"]
 
     output = []
     m0 = media[0]
     for m in media[1:]:
-        if is_same_size_group(args, m0, m):
+        if is_same_group(args, m0, m):
             output.append(m)
 
     if output:
         group["grouped_paths"] = [m0] + output
         return group
     else:
         return None
 
 
-def filter_groups_by_size(args, groups):
-    groups = [filter_group_by_size(args, group) for group in groups]
+def filter_groups_by_numbers(args, groups):
+    groups = [filter_group_by_numbers(args, group) for group in groups]
     groups = [group for group in groups if group]
     return groups
 
 
 def similar_folders():
     args = parse_args()
-    media = list(arg_utils.gen_d(args))
+    media = arg_utils.gen_d(args)
+    media = [d if "size" in d else file_utils.get_filesize(d) for d in media]
     media = big_dirs.group_files_by_parent(args, media)
-    if args.folder_size:
-        args.folder_size = sql_utils.parse_human_to_lambda(nums.human_to_bytes, args.folder_size)
-        media = [d for d in media if args.folder_size(d["size"])]
+    if args.folder_sizes:
+        media = [d for d in media if args.folder_sizes(d["size"])]
 
-    if args.filter_sizes or args.filter_counts:
-        clusters = cluster_by_size(args, media)
+    if args.filter_sizes or args.filter_counts or args.filter_durations:
+        clusters = cluster_by_numbers(args, media)
         groups = map_and_name(media, clusters)
-        log.info("Folder size/count clustering sorted %s folders into %s groups", len(media), len(groups))
+        log.info("Folder size/duration/count clustering sorted %s folders into %s groups", len(media), len(groups))
         single_folder_groups = [d for d in groups if len(d["grouped_paths"]) == 1]
         groups = [d for d in groups if len(d["grouped_paths"]) > 1]
         log.info("Filtered out %s single-folder groups", len(single_folder_groups))
         log.debug(single_folder_groups)
 
         if args.filter_names:
             media = [d for group in groups for d in group["grouped_paths"]]
 
     if args.filter_names:
         groups = cluster_folders(args, media)
         groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_path"])))
         log.info("Name clustering sorted %s folders into %s groups", len(media), len(groups))
 
-        if args.filter_sizes or args.filter_counts:
+        if args.filter_sizes or args.filter_counts or args.filter_durations:
             prev_count = len(groups)
-            groups = filter_groups_by_size(args, groups)  # effectively a second pass
-            log.info("(2nd pass) group size/count filtering removed %s groups", prev_count - len(groups))
+            groups = filter_groups_by_numbers(args, groups)  # effectively a second pass
+            log.info("(2nd pass) group size/duration/count filtering removed %s groups", prev_count - len(groups))
 
     if not args.only_originals and not args.only_duplicates:
         print("Duplicate groups:")
 
     for group in groups:
         media = group["grouped_paths"]
         media = sorted(media, key=lambda d: d["size"], reverse=not args.small)
@@ -185,14 +204,17 @@
             print(
                 tabulate(
                     [
                         {
                             f'group {group["common_path"]}': d["path"],
                             "total_size": humanize.naturalsize(d["size"], binary=True),
                             "median_size": humanize.naturalsize(d["median_size"], binary=True),
+                            "total_duration": printing.human_duration(d["duration"]),
+                            "median_duration": printing.human_duration(d["median_duration"]),
+                            "median_size": humanize.naturalsize(d["median_size"], binary=True),
                             "files": d["exists"],
                         }
                         for d in media
                     ],
                     tablefmt=consts.TABULATE_STYLE,
                     headers="keys",
                     showindex=False,
```

### Comparing `xklb-2.7.9/xklb/fsdb/big_dirs.py` & `xklb-2.8.1/xklb/folders/big_dirs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 import argparse, os
 from collections import defaultdict
 from pathlib import Path
 
 from xklb import media_printer, usage
-from xklb.mediadb import db_history
 from xklb.tablefiles import mcda
-from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, nums, objects, sql_utils
-from xklb.utils.log_utils import log
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, file_utils, iterables, nums
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library big_dirs",
         usage=usage.big_dirs,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    arggroups.sql_fs(parser)
-    arggroups.operation_cluster(parser)
-    arggroups.operation_group_folders(parser)
+    arggroups.cluster(parser)
+    arggroups.group_folders(parser)
     parser.set_defaults(limit="4000", lower=4, depth=0)
     arggroups.debug(parser)
 
-    arggroups.database(parser)
+    arggroups.paths_or_stdin(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
-    args.db = db_utils.connect(args)
+    args.action = consts.SC.big_dirs
+    arggroups.args_post(args, parser)
 
-    args.include += args.search
-    if args.include == ["."]:
-        args.include = [str(Path().cwd().resolve())]
+    arggroups.group_folders_post(args)
 
-    if len(args.include) == 1 and os.sep in args.include[0]:
-        args.include = [file_utils.resolve_absolute_path(args.include[0])]
+    return args
 
-    if args.sort_groups_by:
-        args.sort_groups_by = arg_utils.parse_ambiguous_sort(args.sort_groups_by)
-        args.sort_groups_by = ",".join(args.sort_groups_by)
 
-    if args.size:
-        args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
+def filter_deleted(args, d):
+    for path, pdict in list(d.items()):
+        if pdict["exists"] == 0:
+            d.pop(path)
 
-    args.action = consts.SC.big_dirs
-    log.info(objects.dict_filter_bool(args.__dict__))
-    return args
+    if args.folder_counts and not args.depth:
+        for path, pdict in list(d.items()):
+            if not args.folder_counts(pdict["exists"]):
+                d.pop(path)
 
 
 def group_files_by_parents(args, media) -> list[dict]:
     p_media = {}
     min_parts = 10
     for m in media:
         p = m["path"].split(os.sep)
@@ -61,62 +56,58 @@
                 p_media[parent].append(m)
 
     d = {}
     for parent, media in list(p_media.items()):
         d[parent] = {
             "size": sum(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
             "median_size": nums.safe_median(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "duration": sum(m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "median_duration": nums.safe_median(
+                m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))
+            ),
             "total": len(media),
             "exists": sum(not bool(m.get("time_deleted")) for m in media),
             "deleted": sum(bool(m.get("time_deleted")) for m in media),
             "deleted_size": sum(m.get("size") or 0 for m in media if bool(m.get("time_deleted"))),
+            "deleted_duration": sum(m.get("duration") or 0 for m in media if bool(m.get("time_deleted"))),
             "played": sum(bool(m.get("time_last_played")) for m in media),
         }
 
     for parent, _ in list(d.items()):
         if len(parent.split(os.sep)) < min_parts:
             d.pop(parent)
 
-    for path, pdict in list(d.items()):
-        if pdict["exists"] == 0:
-            d.pop(path)
-        elif not args.depth:
-            if args.lower and pdict["exists"] < args.lower:
-                d.pop(path)
-            elif args.upper and pdict["exists"] > args.upper:
-                d.pop(path)
+    filter_deleted(args, d)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def group_files_by_parent(args, media) -> list[dict]:
     p_media = defaultdict(list)
     for m in media:
         p_media[str(Path(m["path"]).parent)].append(m)
 
     d = {}
     for parent, media in list(p_media.items()):
         d[parent] = {
             "size": sum(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
             "median_size": nums.safe_median(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "duration": sum(m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "median_duration": nums.safe_median(
+                m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))
+            ),
             "total": len(media),
             "exists": sum(not bool(m.get("time_deleted")) for m in media),
             "deleted": sum(bool(m.get("time_deleted")) for m in media),
             "deleted_size": sum(m.get("size") or 0 for m in media if bool(m.get("time_deleted"))),
+            "deleted_duration": sum(m.get("duration") or 0 for m in media if bool(m.get("time_deleted"))),
             "played": sum(bool(m.get("time_last_played")) for m in media),
         }
 
-    for path, pdict in list(d.items()):
-        if pdict["exists"] == 0:
-            d.pop(path)
-        elif not args.depth:
-            if args.lower and pdict["exists"] < args.lower:
-                d.pop(path)
-            elif args.upper and pdict["exists"] > args.upper:
-                d.pop(path)
+    filter_deleted(args, d)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def folder_depth(args, folders) -> list[dict]:
     d = {}
     for f in folders:
@@ -126,81 +117,46 @@
         depth = 1 + args.depth
         parent = os.sep.join(p[:depth]) + os.sep
         if len(p) < depth:
             continue
 
         if d.get(parent):
             d[parent]["size"] += f["size"]
+            d[parent]["duration"] += f["duration"]
             d[parent]["total"] += f["total"]
             d[parent]["exists"] += f["exists"]
             d[parent]["deleted"] += f["deleted"]
             d[parent]["played"] += f["played"]
         else:
             d[parent] = f
 
-    for path, pdict in list(d.items()):
-        if args.lower is not None and pdict["exists"] < args.lower:
-            d.pop(path)
-        elif args.upper is not None and pdict["exists"] > args.upper:
-            d.pop(path)
+    if args.folder_counts:
+        for path, pdict in list(d.items()):
+            if not args.folder_counts(pdict["exists"]):
+                d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
-def get_table(args) -> list[dict]:
-    m_columns = db_utils.columns(args, "media")
-    args.filter_sql = []
-    args.filter_bindings = {}
-
-    if args.size:
-        args.filter_sql.append(" and size IS NOT NULL " + args.size)
-    db_utils.construct_search_bindings(
-        args,
-        [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-    )
-
-    media = list(
-        args.db.query(
-            f"""
-            SELECT
-                path
-                , size
-                {', time_deleted' if 'time_deleted' in m_columns else ''}
-                , MAX(h.time_played) time_played
-            FROM media m
-            LEFT JOIN history h on h.media_id = m.id
-            WHERE 1=1
-                {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
-                {" ".join(args.filter_sql)}
-            GROUP BY m.id
-            ORDER BY path
-            """,
-            args.filter_bindings,
-        ),
-    )
-    return media
-
-
 def process_big_dirs(args, folders) -> list[dict]:
     folders = [d for d in folders if d["total"] != d["deleted"]]  # remove folders where all deleted
 
     if args.depth:
         folders = folder_depth(args, folders)
-    if args.folder_size:
-        args.folder_size = sql_utils.parse_human_to_lambda(nums.human_to_bytes, args.folder_size)
-        folders = [d for d in folders if args.folder_size(d["size"])]
+    if args.folder_sizes:
+        folders = [d for d in folders if args.folder_sizes(d["size"])]
 
     return folders
 
 
 def big_dirs() -> None:
     args = parse_args()
-    db_history.create(args)
 
-    media = get_table(args)
+    media = list(arg_utils.gen_d(args))
+    media = [d if "size" in d else file_utils.get_filesize(d) for d in media]
     if args.cluster_sort and len(media) > 2:
         from xklb.text.cluster_sort import cluster_paths
 
         groups = cluster_paths([d["path"] for d in media], n_clusters=getattr(args, "clusters", None))
         groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_path"])))
 
         media_keyed = {d["path"]: d for d in media}
@@ -222,25 +178,36 @@
                     if not bool(media_keyed[s].get("time_deleted"))
                 ),
                 "median_size": nums.safe_median(
                     media_keyed[s].get("size") or 0
                     for s in group["grouped_paths"]
                     if not bool(media_keyed[s].get("time_deleted"))
                 ),
+                "duration": sum(
+                    media_keyed[s].get("duration") or 0
+                    for s in group["grouped_paths"]
+                    if not bool(media_keyed[s].get("time_deleted"))
+                ),
+                "median_duration": nums.safe_median(
+                    media_keyed[s].get("duration") or 0
+                    for s in group["grouped_paths"]
+                    if not bool(media_keyed[s].get("time_deleted"))
+                ),
             }
             for group in groups
         ]
     elif args.parents:
         folders = group_files_by_parents(args, media)
     else:
         folders = group_files_by_parent(args, media)
 
     folders = mcda.group_sort_by(args, folders)
     media = process_big_dirs(args, folders)
 
     if args.limit:
         media = media[-int(args.limit) :]
+    media = iterables.list_dict_filter_bool(media, keep_0=False)
     media_printer.media_printer(args, media, units="folders")
 
 
 if __name__ == "__main__":
     big_dirs()
```

### Comparing `xklb-2.7.9/xklb/fsdb/disk_usage.py` & `xklb-2.8.1/xklb/fsdb/disk_usage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,43 @@
 import argparse, os
-from pathlib import Path
 
 from xklb import media_printer, usage
-from xklb.utils import arggroups, consts, db_utils, file_utils, nums, objects, processes, sql_utils
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, consts, processes, sqlgroups
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library disk_usage",
         usage=usage.disk_usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     arggroups.sql_fs(parser)
-    arggroups.operation_group_folders(parser)
+    arggroups.group_folders(parser)
     parser.set_defaults(limit="4000", depth=0)
 
     parser.add_argument("--folders-only", "-td", action="store_true", help="Only print folders")
     parser.add_argument("--files-only", "-tf", action="store_true", help="Only print files")
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    parser.add_argument("working_directory", nargs="*", default=os.sep)
+    parser.add_argument("search", nargs="*", default=os.sep)
     args = parser.parse_intermixed_args()
-    args.db = db_utils.connect(args)
-
-    args.include += args.working_directory
-    if args.include == ["."]:
-        args.include = [str(Path().cwd().resolve())]
-
-    if len(args.include) == 1 and os.sep in args.include[0]:
-        args.include = [file_utils.resolve_absolute_path(args.include[0])]
-
-    if args.sort_groups_by:
-        args.sort_groups_by = " ".join(args.sort_groups_by)
+    args.action = consts.SC.disk_usage
+    arggroups.args_post(args, parser)
 
-    if args.size:
-        args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
+    arggroups.sql_fs_post(args)
+    arggroups.group_folders_post(args)
 
-    args.action = consts.SC.disk_usage
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def sort_by(args):
     if args.sort_groups_by:
-        return lambda x: x.get(args.sort_groups_by) or 0
+        return lambda x: x.get(args.sort_groups_by.replace(" desc", "")) or 0
 
     return lambda x: (x["size"] / (x.get("count") or 1), x["size"], x.get("count") or 1)
 
 
 def get_subset(args, level=None, prefix=None) -> list[dict]:
     d = {}
     excluded_files = set()
@@ -75,15 +62,14 @@
             if parent not in d:
                 d[parent] = {"size": 0, "count": 0}
             d[parent]["size"] += m.get("size") or 0
             d[parent]["count"] += 1
 
     reverse = True
     if args.sort_groups_by and " desc" in args.sort_groups_by:
-        args.sort_groups_by = args.sort_groups_by.replace(" desc", "")
         reverse = False
 
     return sorted(
         [{"path": k, **v} for k, v in d.items() if k not in excluded_files],
         key=sort_by(args),
         reverse=reverse,
     )
@@ -102,42 +88,15 @@
         processes.no_media_found()
 
     args.cwd = os.sep.join(args.subset[0]["path"].split(os.sep)[: level - 1]) + os.sep
     return args.cwd, args.subset
 
 
 def get_data(args) -> list[dict]:
-    m_columns = db_utils.columns(args, "media")
-    args.filter_sql = []
-    args.filter_bindings = {}
-
-    if args.size:
-        args.filter_sql.append(" and size IS NOT NULL " + args.size)
-    db_utils.construct_search_bindings(
-        args,
-        [f"{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-    )
-
-    media = list(
-        args.db.query(
-            f"""
-        SELECT
-            path
-            , size
-        FROM media m
-        WHERE 1=1
-            and size > 0
-            {'and coalesce(time_deleted, 0) = 0' if 'time_deleted' in m_columns else ''}
-            {'and coalesce(is_dir, 0) = 0' if 'is_dir' in m_columns else ''}
-            {" ".join(args.filter_sql)}
-        ORDER BY path
-        """,
-            args.filter_bindings,
-        ),
-    )
+    media = list(args.db.query(*sqlgroups.fs_sql(args)))
 
     if not media:
         processes.no_media_found()
     return media
 
 
 def disk_usage():
```

### Comparing `xklb-2.7.9/xklb/mediadb/block.py` & `xklb-2.8.1/xklb/mediadb/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import argparse, sys
 
 import humanize
 
 from xklb import media_printer, usage
 from xklb.createdb import tube_backend
 from xklb.playback import post_actions
-from xklb.utils import arggroups, consts, db_utils, devices, iterables, objects
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, db_utils, devices, iterables
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library block",
         usage=usage.block,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    arggroups.sql_fs(parser)
+    arggroups.extractor(parser)
+    arggroups.cluster(parser)
 
     parser.add_argument("--match-column", "-c", default="path", help="Column to block media if text matches")
 
-    parser.add_argument("--cluster", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--min-tried", default=0, type=int, help=argparse.SUPPRESS)
     parser.add_argument("--no-confirm", "--yes", "-y", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--offline", "--no-tube", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    parser.add_argument("playlists", nargs="*")
-    args = parser.parse_intermixed_args()
-
-    args.db = db_utils.connect(args)
-
-    args.playlists = iterables.conform(args.playlists)
+    arggroups.paths_or_stdin(parser)
+    parser.set_defaults(path=None)
 
+    args = parser.parse_intermixed_args()
     args.action = SC.block
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser)
+
+    arggroups.extractor_post(args)
 
     return args
 
 
 def add_to_blocklist(args, p):
     p = p.pop()
     args.db["blocklist"].insert({"key": args.match_column, "value": p}, alter=True, replace=True, pk=["key", "value"])
@@ -61,17 +60,18 @@
     m_columns = db_utils.columns(args, "media")
     if args.match_column not in m_columns:
         raise ValueError(
             "Match column does not exist in the media table. You may need to run tubeadd first or check your spelling",
         )
 
     columns = {"path", "webpath", args.match_column, "size", "playlist_path", "time_deleted"}
-    select_sql = ", ".join(s for s in columns if s in m_columns)
 
-    if not args.playlists:
+    paths = list(arg_utils.gen_paths(args))
+
+    if not paths:
         if "blocklist" in args.db.table_names():
             deleted_count = 0
             blocklist = [(d["key"], d["value"]) for d in args.db["blocklist"].rows if d["key"] in m_columns]
             # TODO: add support for playlists table block rules
             if blocklist:
                 # prevent Expression tree is too large (max depth 1000)
                 blocklist_chunked = iterables.chunks(blocklist, consts.SQLITE_PARAM_LIMIT // 100)
@@ -139,15 +139,15 @@
             ),
         )
 
         media_printer.media_printer(args, candidates, units="subdomains")
         return
 
     if args.match_column == "playlist_path":
-        playlist_paths = list(args.playlists)
+        playlist_paths = list(paths)
         for p in playlist_paths:
             add_to_blocklist(args, [p])
 
         with args.db.conn:
             args.db.conn.execute(
                 f"""UPDATE playlists
                 SET time_deleted={consts.APPLICATION_START}
@@ -188,16 +188,18 @@
             print(paths_to_delete)
             if devices.confirm(
                 f"Would you like to delete these {len(paths_to_delete)} local files ({humanize.naturalsize(total_size, binary=True)})?",
             ):
                 post_actions.delete_media(args, paths_to_delete)
         return
 
+    select_sql = ", ".join(s for s in columns if s in m_columns)
+
     unmatched_playlists = []
-    for p in args.playlists:
+    for p in paths:
         p = [p]
         if consts.PYTEST_RUNNING or args.force:
             if args.delete_rows:
                 remove_from_blocklist(args, p)
             else:
                 add_to_blocklist(args, p)
             continue
@@ -241,15 +243,15 @@
                             ),
                         )
 
         if not matching_media:
             unmatched_playlists.append(p)
             continue
 
-        if args.cluster:
+        if args.cluster_sort:
             from xklb.text.cluster_sort import cluster_dicts
 
             matching_media = list(reversed(cluster_dicts(args, matching_media)))
 
         media_printer.media_printer(args, matching_media)
         if args.no_confirm or devices.confirm("Add to blocklist?"):
             add_to_blocklist(args, p)
```

### Comparing `xklb-2.7.9/xklb/mediadb/db_history.py` & `xklb-2.8.1/xklb/mediadb/db_history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/mediadb/db_media.py` & `xklb-2.8.1/xklb/mediadb/db_media.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections.abc import Collection
 from datetime import datetime
 from pathlib import Path
 
 from dateutil import parser
 
 from xklb.createdb import fs_add
-from xklb.utils import consts, db_utils, iterables, nums, objects, processes, strings
+from xklb.utils import consts, db_utils, iterables, nums, objects, processes, sql_utils, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
 def exists(args, path) -> bool:
     m_columns = db_utils.columns(args, "media")
     try:
@@ -289,46 +289,34 @@
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
-def filter_args_sql(args, m_columns):
-    return f"""
-        {'and path like "http%"' if getattr(args, 'safe', False) else ''}
-        {f'and path not like "{args.keep_dir}%"' if getattr(args, 'keep_dir', False) and Path(args.keep_dir).exists() else ''}
-        {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and "deleted" not in (getattr(args, 'sort_groups_by',None) or '') and "time_deleted" not in " ".join(args.where) else ''}
-        {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
-        {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
-        {'AND path not like "http%"' if args.local_media_only and 'time_downloaded' not in m_columns else ''}
-        {'AND path like "http%"' if args.online_media_only and 'time_downloaded' not in m_columns else ''}
-        {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only and 'time_downloaded' in m_columns else ''}
-        {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only and 'time_downloaded' in m_columns else ''}
-    """
-
-
 def natsort_media(args, media):
     from natsort import natsorted, ns, os_sorted
 
+    config = args.play_in_order
+
     reverse = False
-    if args.play_in_order.startswith("reverse_"):
-        args.play_in_order = args.play_in_order.replace("reverse_", "", 1)
+    if config.startswith("reverse_"):
+        config = config.replace("reverse_", "", 1)
         reverse = True
 
     compat = False
     for opt in ("compat_", "nfkd_"):
-        if args.play_in_order.startswith(opt):
-            args.play_in_order = args.play_in_order.replace(opt, "", 1)
+        if config.startswith(opt):
+            config = config.replace(opt, "", 1)
             compat = True
 
-    if "_" in args.play_in_order:
-        alg, sort_key = args.play_in_order.split("_", 1)
+    if "_" in config:
+        alg, sort_key = config.split("_", 1)
     else:
-        alg, sort_key = args.play_in_order, "ps"
+        alg, sort_key = config, "ps"
 
     def func_sort_key(sort_key):
         def fn_key(d):
             if sort_key in ("parent", "stem", "ps", "pts"):
                 path = Path(d["path"])
 
                 if sort_key == "parent":
@@ -373,16 +361,14 @@
     return media
 
 
 def get_dir_media(args, dirs: Collection, include_subdirs=False, limit=2_000) -> list[dict]:
     if len(dirs) == 0:
         return processes.no_media_found()
 
-    m_columns = db_utils.columns(args, "media")
-
     if include_subdirs:
         filter_paths = "AND (" + " OR ".join([f"path LIKE :subpath{i}" for i in range(len(dirs))]) + ")"
     else:
         filter_paths = (
             "AND ("
             + " OR ".join(
                 [f"(path LIKE :subpath{i} and path not like :subpath{i} || '%{os.sep}%')" for i in range(len(dirs))]
@@ -395,20 +381,18 @@
     query = f"""WITH m as (
             SELECT
                 SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , MIN(h.time_played) time_first_played
                 , MAX(h.time_played) time_last_played
                 , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
                 , {select_sql}
-                , m.*
             FROM media m
             LEFT JOIN history h on h.media_id = m.id
             WHERE 1=1
                 and m.id in (select id from {args.table})
-                {filter_args_sql(args, m_columns)}
                 {filter_paths}
             GROUP BY m.id, m.path
         )
         SELECT *
         FROM m
         ORDER BY play_count
             , m.path LIKE "http%"
@@ -428,14 +412,58 @@
         log.debug("dir_media dirs %s", dirs)
     else:
         log.debug("get_dir_media[0] %s", media[0:1])
 
     return media
 
 
+def get_playlist_media(args, playlist_paths) -> list[dict]:
+    select_sql = "\n        , ".join(s for s in args.select if s not in ["rank"])
+
+    playlists_subquery = (
+        """AND playlists_id in (
+        SELECT id from playlists
+        WHERE path IN ("""
+        + ",".join(f":playlist{i}" for i, _ in enumerate(playlist_paths))
+        + "))"
+    )
+    playlists_params = {f"playlist{i}": value for i, value in enumerate(playlist_paths)}
+
+    query = f"""WITH m as (
+            SELECT
+                SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , MIN(h.time_played) time_first_played
+                , MAX(h.time_played) time_last_played
+                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                , {select_sql}
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
+            WHERE 1=1
+                and m.id in (select id from {args.table})
+                {playlists_subquery}
+                {" ".join(args.filter_sql)}
+            GROUP BY m.id, m.path
+        )
+        SELECT *
+        FROM m
+        ORDER BY play_count
+            , path
+            {'' if 'sort' in args.defaults else ', ' + args.sort}
+        {sql_utils.limit_sql(args)}
+    """
+
+    bindings = {**playlists_params}
+    bindings = {**bindings, **{k: v for k, v in args.filter_bindings.items() if k.startswith("FTS")}}
+
+    media = list(args.db.query(query, bindings))
+    log.debug("len(playlist_media) = %s", len(media))
+
+    return media
+
+
 def get_next_dir_media(args, folder):
     if args.play_in_order:
         media = get_dir_media(args, [folder], limit=100)
         media = natsort_media(args, media)
         m = media[0:1]
     else:
         m = get_dir_media(args, [folder], limit=1)[0:1]
@@ -477,50 +505,48 @@
     words = set(
         iterables.conform(
             strings.extract_words(m.get(k)) for k in m if k in db_utils.config["media"]["search_columns"]
         ),
     )
     args.include = sorted(words, key=len, reverse=True)[:100]
     log.info("related_words: %s", args.include)
-    args.table, search_bindings = db_utils.fts_search_sql(
+    args.table, search_bindings = sql_utils.fts_search_sql(
         "media",
         fts_table=args.db["media"].detect_fts(),
         include=args.include,
         exclude=args.exclude,
         flexible=True,
     )
     args.filter_bindings = {**args.filter_bindings, **search_bindings}
 
-    select_sql = "\n        , ".join(args.select)
-    limit_sql = "LIMIT " + str(args.limit - 1) if args.limit else ""
-    offset_sql = f"OFFSET {args.offset}" if args.offset and limit_sql else ""
+    select_sql = "\n        , ".join(s for s in args.select if s not in ["rank"])
+
     query = f"""WITH m as (
             SELECT
                 SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , MIN(h.time_played) time_first_played
                 , MAX(h.time_played) time_last_played
                 , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
                 , {select_sql}
                 , rank
             FROM {args.table} m
             LEFT JOIN history h on h.media_id = m.id
             WHERE 1=1
                 and path != :path
-                {filter_args_sql(args, m_columns)}
             GROUP BY m.id, m.path
         )
         SELECT *
         FROM m
         WHERE 1=1
             {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
         ORDER BY play_count
             , m.path like "http%"
             , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank)' + (f', {args.sort}' if args.sort else '')}
             , path
-        {limit_sql} {offset_sql}
+        {sql_utils.limit_sql(args, limit_adj=-1)}
     """
 
     bindings = {"path": m["path"]}
     if args.related >= consts.RELATED_NO_FILTER:
         bindings = {**bindings, **{k: v for k, v in args.filter_bindings.items() if k.startswith("FTS")}}
     else:
         bindings = {**bindings, **args.filter_bindings}
```

### Comparing `xklb-2.7.9/xklb/mediadb/db_playlists.py` & `xklb-2.8.1/xklb/mediadb/db_playlists.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         else:
             delete_subpath_playlists(args, playlist_path)
 
     pl = consolidate(args, objects.dumbcopy(info))
     playlist = {**pl, "path": playlist_path}
     if extractor_key:
         playlist["extractor_key"] = extractor_key
-    return _add(args, objects.dict_filter_bool(playlist))
+    return _add(args, objects.dict_filter_bool(playlist) or {})
 
 
 def media_exists(args, playlist_path, path) -> bool:
     m_columns = db_utils.columns(args, "media")
     try:
         known = args.db.execute(
             f"select 1 from media where playlists_id in (select id from playlists where path = ?) and (path=? or {'webpath' if 'webpath' in m_columns else 'path'}=?)",
@@ -232,12 +232,9 @@
     if exists(args, playlist_path):
         log.warning("Start of known playlist reached %s", playlist_path)
     else:
         log.warning("Could not add playlist %s", playlist_path)
 
 
 def save_undownloadable(args, playlist_path) -> None:
-    entry = {
-        "path": playlist_path,
-        "extractor_config": args.extractor_config,
-    }
-    _add(args, objects.dict_filter_bool(entry))
+    entry = {"path": playlist_path, "extractor_config": args.extractor_config}
+    _add(args, objects.dict_filter_bool(entry) or {})
```

### Comparing `xklb-2.7.9/xklb/mediadb/download_status.py` & `xklb-2.8.1/xklb/mediadb/download_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 import argparse
 
 from xklb import media_printer, usage
 from xklb.createdb import tube_backend
-from xklb.mediadb import download
-from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, sql_utils
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, consts, db_utils, sql_utils, sqlgroups
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         "library download-status",
         usage=usage.download_status,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     arggroups.sql_fs(parser)
-    arggroups.sql_media(parser)
 
     parser.set_defaults(print="p")
 
     arggroups.download(parser)
 
     arggroups.debug(parser)
     arggroups.database(parser)
     args = parser.parse_args()
-    args.defaults = []
-
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
-
     args.action = consts.SC.download_status
+    arggroups.args_post(args, parser)
+
+    arggroups.sql_fs_post(args)
     return args
 
 
 def download_status() -> None:
     args = parse_args()
-    arg_utils.parse_args_sort(args)
 
-    query, bindings = download.construct_query(args)
+    query, bindings = sqlgroups.construct_download_query(args)
 
     count_paths = ""
     if "time_modified" in query:
         if args.safe:
             args.db.register_function(tube_backend.is_supported, deterministic=True)
             count_paths += f", count(*) FILTER(WHERE cast(STRFTIME('%s', datetime( time_modified, 'unixepoch', '+{args.retry_delay}')) as int) >= STRFTIME('%s', datetime()) and is_supported(path)) failed_recently"
             count_paths += f", count(*) FILTER(WHERE time_modified>0 and cast(STRFTIME('%s', datetime( time_modified, 'unixepoch', '+{args.retry_delay}')) as int) < STRFTIME('%s', datetime()) and is_supported(path)) retry_queued"
```

### Comparing `xklb-2.7.9/xklb/mediadb/history_add.py` & `xklb-2.8.1/xklb/mediadb/history_add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-import argparse
-from pathlib import Path
-
 from xklb import usage
 from xklb.mediadb import db_history
-from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, printing
-from xklb.utils.log_utils import log
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, printing
 
 
 def parse_args(**kwargs):
-    parser = argparse.ArgumentParser(**kwargs)
+    parser = argparse_utils.ArgumentParser(**kwargs)
     arggroups.extractor(parser)
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
+    arggroups.extractor_post(args)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def history_add() -> None:
     args = parse_args(prog="library history-add", usage=usage.history_add)
 
     history_exists = set()
```

### Comparing `xklb-2.7.9/xklb/mediadb/redownload.py` & `xklb-2.8.1/xklb/mediadb/redownload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import argparse, json, tempfile
 from copy import deepcopy
 from pathlib import Path
 
 from xklb import media_printer, usage
-from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, objects
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, consts, db_utils, devices, file_utils, iterables
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library redownload",
         usage=usage.redownload,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--download-archive", default=str(Path("~/.local/share/yt_archive.txt").expanduser().resolve()))
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="100")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("deleted_at", nargs="?")
     parser.add_argument("deleted_to", nargs="?")
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def list_deletions(args) -> list[dict]:
     query = """
         SELECT
             strftime('%Y-%m-%dT%H:%M:%S', time_deleted, 'unixepoch', 'localtime') as time_deleted
```

### Comparing `xklb-2.7.9/xklb/mediadb/search.py` & `xklb-2.8.1/xklb/mediadb/download.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,182 +1,220 @@
-import argparse, textwrap
-from copy import deepcopy
-from itertools import groupby
+import argparse, os, sys
 
 from xklb import media_printer, usage
+from xklb.createdb import gallery_backend, tube_backend
 from xklb.mediadb import db_media
-from xklb.playback import media_player
-from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, printing, processes
+from xklb.utils import (
+    arg_utils,
+    arggroups,
+    argparse_utils,
+    consts,
+    db_utils,
+    iterables,
+    printing,
+    processes,
+    sql_utils,
+    web,
+)
+from xklb.utils.consts import SC, DBType
 from xklb.utils.log_utils import log
+from xklb.utils.sqlgroups import construct_download_query
 
 
-def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library search", usage=usage.search)
-
+def parse_args():
+    parser = argparse_utils.ArgumentParser(
+        prog="library download",
+        usage=usage.download,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     arggroups.sql_fs(parser)
-    arggroups.sql_media(parser)
-    arggroups.playback(parser)
-    arggroups.post_actions(parser)
-
-    parser.set_defaults(sort=["path", "time"])
 
-    parser.add_argument("--open", "--play", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--overlap", type=int, default=8, help=argparse.SUPPRESS)
-    parser.add_argument("--table", action="store_true")
+    arggroups.download(parser)
+    arggroups.download_subtitle(parser)
+    arggroups.requests(parser)
+
+    profile = parser.add_mutually_exclusive_group()
+    profile.add_argument(
+        "--audio",
+        action="store_const",
+        dest="profile",
+        const=DBType.audio,
+        help="Use audio downloader",
+    )
+    profile.add_argument(
+        "--video",
+        action="store_const",
+        dest="profile",
+        const=DBType.video,
+        help="Use video downloader",
+    )
+    profile.add_argument(
+        "--image",
+        "--photo",
+        action="store_const",
+        dest="profile",
+        const=DBType.image,
+        help="Use image downloader",
+    )
+    profile.add_argument(
+        "--filesystem",
+        "--fs",
+        "--web",
+        action="store_const",
+        dest="profile",
+        const=DBType.filesystem,
+        help="Use filesystem downloader",
+    )
 
-    parser.set_defaults(print="p")
+    parser.add_argument("--same-domain", action="store_true", help="Choose a random domain to focus on")
 
-    arggroups.debug(parser)
-    arggroups.database(parser)
-    parser.add_argument("search", nargs="*")
-    args = parser.parse_intermixed_args()
-    args.action = "search"
+    parser.add_argument("--prefix", default=os.getcwd(), help=argparse.SUPPRESS)
 
-    args.include += args.search
+    parser.add_argument("--small", action="store_true", help="Video: Prefer 480p-like")
 
-    if args.cols:
-        args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
+    parser.add_argument("--photos", action="store_true", help="Image: Download JPG and WEBP")
+    parser.add_argument("--drawings", action="store_true", help="Image: Download PNG")
+    parser.add_argument("--gifs", action="store_true", help="Image: Download MP4 and GIFs")
+    arggroups.debug(parser)
 
-    sort = [arg_utils.override_sort(s) for s in args.sort]
-    sort = "\n        , ".join(sort)
-    args.sort = sort.replace(",,", ",")
+    arggroups.database(parser)
+    arggroups.paths_or_stdin(parser)
+    parser.set_defaults(paths=None)
 
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    args, unk = parser.parse_known_intermixed_args()
+    args.action = SC.download
+    arggroups.args_post(args, parser)
+
+    if unk and not args.profile in (DBType.video, DBType.audio):
+        parser.error(f"unrecognized arguments: {' '.join(unk)}")
+    args.unk = unk
+
+    if not args.profile and not args.print:
+        log.error("Download profile must be specified. Use one of: --video OR --audio OR --image OR --filesystem")
+        raise SystemExit(1)
 
+    arggroups.sql_fs_post(args)
     return args
 
 
-def printer(args, captions) -> None:
-    captions = iterables.list_dict_filter_bool(captions)
-    if not captions:
+def process_downloadqueue(args) -> list[dict]:
+    query, bindings = construct_download_query(args)
+    if args.print:
+        media_printer.printer(args, query, bindings)
+        return []
+
+    media = list(args.db.query(query, bindings))
+    if not media:
         processes.no_media_found()
+    return media
 
-    tbl = deepcopy(captions)
-    printing.col_hhmmss(tbl, "time")
 
-    if args.print == "p":
-        print(f"{len(captions)} captions")
-        for path, path_group in groupby(tbl, key=lambda x: x["path"]):
-            path_group = list(path_group)
-            title = path_group[0].get("title")
-            print(" - ".join(iterables.concat(title, path)))
-            for caption in path_group:
-                for line in textwrap.wrap(caption["text"], subsequent_indent=" " * 9, initial_indent=f"{caption['time']} ", width=consts.TERMINAL_SIZE.columns - 2):  # type: ignore
-                    print(line)
-            print()
-    else:
-        media_printer.media_printer(args, captions, units="captions")
+def mark_download_attempt(args, paths) -> int:
+    paths = iterables.conform(paths)
 
+    modified_row_count = 0
+    if paths:
+        df_chunked = iterables.chunks(paths, consts.SQLITE_PARAM_LIMIT)
+        for chunk_paths in df_chunked:
+            with args.db.conn:
+                cursor = args.db.conn.execute(
+                    f"""update media
+                    set time_modified={consts.now()}
+                    where path in ("""
+                    + ",".join(["?"] * len(chunk_paths))
+                    + ")",
+                    (*chunk_paths,),
+                )
+                modified_row_count += cursor.rowcount
+
+    return modified_row_count
+
+
+def dl_download(args=None) -> None:
+    if args:
+        sys.argv = ["lb", *args]
 
-def construct_query(args) -> tuple[str, dict]:
+    args = parse_args()
     m_columns = db_utils.columns(args, "media")
-    c_columns = db_utils.columns(args, "captions")
-    args.filter_sql = []
-    args.filter_bindings = {}
-
-    args.filter_sql.extend([" and " + w for w in args.where])
-
-    table = "captions"
-    cols = args.cols or ["path", "text", "time", "title"]
-
-    is_fts = args.db["captions"].detect_fts()
-    if is_fts and args.include:
-        table, search_bindings = db_utils.fts_search_sql(
-            "captions",
-            fts_table=is_fts,
-            include=args.include,
-            exclude=args.exclude,
-            flexible=args.flexible_search,
-        )
-        args.filter_bindings = {**args.filter_bindings, **search_bindings}
-        c_columns = {**c_columns, "rank": int}
-        cols.append("id")
-        cols.append("rank")
-    else:
-        db_utils.construct_search_bindings(args, ["text"])
-
-    args.select = [c for c in cols if c in {**c_columns, **m_columns, **{"*": "Any"}}]
-
-    select_sql = "\n        , ".join(args.select)
-    limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
-    query = f"""WITH c as (
-        SELECT * FROM {table}
-        WHERE 1=1
-            {db_media.filter_args_sql(args, c_columns)}
-    )
-    SELECT
-        {select_sql}
-    FROM c
-    JOIN media m on m.id = c.media_id
-    WHERE 1=1
-        {" ".join(args.filter_sql)}
-    ORDER BY 1=1
-        , {args.sort}
-    {limit_sql}
-    """
-
-    return query, args.filter_bindings
-
-
-def merge_captions(args, captions):
-    def get_end(caption):
-        return caption["time"] + (len(caption["text"]) / 4.2 / 220 * 60)
-
-    merged_captions = []
-    for path, group in groupby(
-        captions,
-        key=lambda x: x["path"],
-    ):  # group by only does contiguous items with the same key
-        group = list(group)
-        merged_group = {"path": path, "title": group[0]["title"], "time": group[0]["time"], "end": get_end(group[0]), "text": group[0]["text"]}  # type: ignore
-        for i in range(1, len(group)):
-            end = get_end(group[i])
-
-            if (
-                abs(group[i]["time"] - merged_group["end"]) <= args.overlap  # type: ignore
-                or abs(group[i]["time"] - merged_group["time"]) <= args.overlap  # type: ignore
-            ):
-                merged_group["end"] = end
-                if group[i]["text"] not in merged_group["text"]:  # type: ignore
-                    merged_group["text"] += ". " + group[i]["text"]  # type: ignore
-            else:
-                merged_captions.append(merged_group)
-                merged_group = {
-                    "path": path,
-                    "time": group[i]["time"],  # type: ignore
-                    "end": end,
-                    "text": group[i]["text"],  # type: ignore
-                }
-        merged_captions.append(merged_group)
-
-    return merged_captions
-
 
-def search() -> None:
-    args = parse_args()
-    query, bindings = construct_query(args)
-    captions = list(args.db.query(query, bindings))
-    merged_captions = merge_captions(args, captions)
-
-    if args.open:
-        pl = media_player.MediaPrefetcher(args, merged_captions)
-        pl.fetch()
-        while pl.remaining:
-            d = pl.get_m()
+    if "limit" in args.defaults and "media" in args.db.table_names() and "webpath" in m_columns:
+        if args.db.pop("SELECT 1 from media WHERE webpath is NULL and path in (select webpath from media) LIMIT 1"):
+            with args.db.conn:
+                args.db.conn.execute(
+                    """
+                    DELETE from media WHERE webpath is NULL
+                    AND path in (
+                        select webpath from media
+                        WHERE error IS NULL OR error != 'Media check failed'
+                    )
+                    """
+                )
+
+    args.blocklist_rules = []
+    if "blocklist" in args.db.table_names():
+        args.blocklist_rules = [{d["key"]: d["value"]} for d in args.db["blocklist"].rows]
+
+    if args.profile == DBType.filesystem:
+        web.requests_session(args)  # prepare requests session
+
+    media = list(arg_utils.gen_d(args))
+    if not media:
+        media = process_downloadqueue(args)
+
+    for m in media:
+        if args.blocklist_rules and sql_utils.is_blocked_dict_like_sql(m, args.blocklist_rules):
+            mark_download_attempt(args, [m["path"]])
+            continue
+
+        if args.safe:
+            if (args.profile in (DBType.audio, DBType.video) and not tube_backend.is_supported(m["path"])) or (
+                args.profile in (DBType.image) and not gallery_backend.is_supported(args, m["path"])
+            ):
+                log.info("[%s]: Skipping unsupported URL (safe_mode)", m["path"])
+                mark_download_attempt(args, [m["path"]])
+                continue
+
+        # check if download already attempted recently by another process
+        previous_time_attempted = m.get("time_modified") or consts.APPLICATION_START  # 0 is nullified
+        if not args.force and "time_modified" in m_columns:
+            d = args.db.pop_dict(
+                f"""
+                SELECT time_modified, time_deleted from media m
+                WHERE 1=1
+                AND path=?
+                AND (time_modified > {str(previous_time_attempted)} OR time_deleted > 0)
+                """,
+                [m["path"]],
+            )
+            log.debug(d)
             if d:
-                print(d["text"])
-                m = args.db.pop_dict("select * from media where path = ?", [d["path"]])
-                m["player"].extend([f'--start={d["time"] - 2}', f'--end={int(d["end"] + 1.5)}'])
-                r = media_player.single_player(args, m)
-                if r.returncode != 0:
-                    log.warning("Player exited with code %s", r.returncode)
-                    if args.ignore_errors:
-                        return
-                    else:
-                        raise SystemExit(r.returncode)
-    else:
-        printer(args, merged_captions)
-
-
-if __name__ == "__main__":
-    search()
+                if d["time_deleted"]:
+                    log.info(
+                        "[%s]: Download marked deleted (%s ago). Skipping!",
+                        m["path"],
+                        printing.human_duration(consts.now() - d["time_deleted"]),
+                    )
+                    mark_download_attempt(args, [m["path"]])
+                    continue
+                elif d["time_modified"]:
+                    log.info(
+                        "[%s]: Download already attempted recently (%s ago). Skipping!",
+                        m["path"],
+                        printing.human_duration(consts.now() - d["time_modified"]),
+                    )
+                    continue
+
+        try:
+            log.debug(m)
+
+            if args.profile in (DBType.audio, DBType.video):
+                tube_backend.download(args, m)
+            elif args.profile == DBType.image:
+                gallery_backend.download(args, m)
+            elif args.profile == DBType.filesystem:
+                local_path = web.download_url(m["path"], output_prefix=args.prefix)
+                db_media.download_add(args, m["path"], m, local_path)
+            else:
+                raise NotImplementedError
+        except Exception:
+            print("db:", args.database)
+            raise
```

### Comparing `xklb-2.7.9/xklb/mediadb/stats.py` & `xklb-2.8.1/xklb/mediadb/stats.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,58 @@
 import argparse
 
 from xklb import media_printer, usage
-from xklb.utils import arggroups, consts, db_utils, objects, sql_utils, strings
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils, consts, db_utils, sql_utils
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         "library stats",
         usage=usage.stats,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     arggroups.sql_fs(parser)
-    arggroups.sql_media(parser)
 
     arggroups.frequency(parser)
     parser.add_argument("--hide-deleted", action="store_true")
+    parser.add_argument("--only-deleted", "--deleted", action="store_true")
     arggroups.history(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument(
         "facet",
         metavar="facet",
         type=str.lower,
         default="watched",
         const="watched",
         nargs="?",
         help=f"One of: {', '.join(consts.time_facets)}",
     )
     args = parser.parse_intermixed_args()
-
-    args.db = db_utils.connect(args)
+    args.action = consts.SC.stats
+    arggroups.args_post(args, parser)
 
     m_columns = db_utils.columns(args, "media")
     if args.facet not in m_columns:
         args.facet = "time_played"
-    args.frequency = strings.partial_startswith(args.frequency, consts.frequency)
-
-    args.action = consts.SC.stats
-    log.info(objects.dict_filter_bool(args.__dict__))
 
-    args.filter_bindings = {}
+    arggroups.sql_fs_post(args)
+    arggroups.frequency_post(args)
 
     return args
 
 
-def process_search(args, m_columns):
-    args.table = "media"
-    if args.db["media"].detect_fts():
-        if args.include:
-            args.table, search_bindings = db_utils.fts_search_sql(
-                "media",
-                fts_table=args.db["media"].detect_fts(),
-                include=args.include,
-                exclude=args.exclude,
-            )
-            args.filter_bindings = search_bindings
-        elif args.exclude:
-            db_utils.construct_search_bindings(
-                args,
-                [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-            )
-    else:
-        db_utils.construct_search_bindings(
-            args,
-            [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-        )
-
-
 def stats() -> None:
     args = parse_args()
 
     print(f"{args.facet.title()} media:")
     if args.facet == "time_played" or args.completed:
-        tbl = sql_utils.historical_usage(args, args.frequency, args.facet, args.hide_deleted)
+        tbl = sql_utils.historical_usage(args, args.frequency, args.facet, args.hide_deleted, args.only_deleted)
     else:
-        tbl = sql_utils.historical_usage_items(args, args.frequency, args.facet, args.hide_deleted)
+        tbl = sql_utils.historical_usage_items(args, args.frequency, args.facet, args.hide_deleted, args.only_deleted)
     media_printer.media_printer(args, tbl, units=args.frequency)
 
 
 if __name__ == "__main__":
     stats()
```

### Comparing `xklb-2.7.9/xklb/mediafiles/media_check.py` & `xklb-2.8.1/xklb/mediafiles/media_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-import argparse, fractions, json, os, shlex, subprocess, tempfile
+import fractions, json, os, shlex, subprocess, tempfile
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 from shutil import which
 
 from xklb import usage
-from xklb.utils import arggroups, consts, file_utils, nums, objects, printing, processes, strings
+from xklb.utils import arggroups, argparse_utils, consts, file_utils, nums, printing, processes, strings
 from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(prog="library media-check", usage=usage.media_check)
+    parser = argparse_utils.ArgumentParser(prog="library media-check", usage=usage.media_check)
     arggroups.capability_delete(parser)
     arggroups.media_check(parser)
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    args.gap = nums.float_from_percent(args.gap)
-    if args.delete_corrupt:
-        args.delete_corrupt = nums.float_from_percent(args.delete_corrupt)
-    if args.full_scan_if_corrupt:
-        args.full_scan_if_corrupt = nums.float_from_percent(args.full_scan_if_corrupt)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.media_check_post(args)
     return args
 
 
 def decode_quick_scan(path, scans, scan_duration=3):
     assert which("ffmpeg")
 
     def decode(scan):
@@ -123,15 +118,15 @@
     try:
         corruption = difference / metadata_duration
     except ZeroDivisionError:
         corruption = 0.5
 
     if difference > 0.1:
         log.info(
-            f"Metadata {printing.seconds_to_hhmmss(metadata_duration).strip()} does not match actual duration {printing.seconds_to_hhmmss(actual_duration).strip()} (diff {difference:.2f}s)\t{path}",
+            f"Metadata {printing.seconds_to_hhmmss(metadata_duration).strip()} does not match actual duration {printing.seconds_to_hhmmss(actual_duration).strip()} (diff {difference:.2f}s): {path}",
         )
 
     return corruption
 
 
 def corruption_threshold_exceeded(threshold, corruption, duration):
     if threshold:
@@ -159,28 +154,28 @@
         if corruption_threshold_exceeded(full_scan_if_corrupt, corruption, duration):
             corruption = decode_full_scan(path, audio_scan=audio_scan, threads=threads)
     return corruption
 
 
 def media_check() -> None:
     args = parse_args()
-    args.paths = list(gen_paths(args))
+    paths = list(gen_paths(args))
 
     with ThreadPoolExecutor(max_workers=1 if args.verbose >= consts.LOG_DEBUG else 4) as pool:
         future_to_path = {
             pool.submit(
                 calculate_corruption,
                 path,
                 chunk_size=args.chunk_size,
                 gap=args.gap,
                 full_scan=args.full_scan,
                 audio_scan=args.audio_scan,
                 threads=args.threads,
             ): path
-            for path in args.paths
+            for path in paths
             if Path(path).suffix.lower() not in consts.SKIP_MEDIA_CHECK
         }
         for future in as_completed(future_to_path):
             path = future_to_path[future]
             try:
                 corruption = future.result()
                 print(strings.safe_percent(corruption), shlex.quote(path), sep="\t")
```

### Comparing `xklb-2.7.9/xklb/mediafiles/process_ffmpeg.py` & `xklb-2.8.1/xklb/mediafiles/process_ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import argparse, os, shlex, subprocess
 from pathlib import Path
 
 from xklb import usage
 from xklb.mediafiles import process_image
-from xklb.utils import arggroups, nums, objects, path_utils, processes, web
+from xklb.utils import arggroups, argparse_utils, nums, path_utils, processes, web
 from xklb.utils.arg_utils import gen_paths, kwargs_overwrite
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library process-ffmpeg", usage=usage.process_ffmpeg)
-    arggroups.capability_simulate(parser)
+    parser = argparse_utils.ArgumentParser(prog="library process-ffmpeg", usage=usage.process_ffmpeg)
+    arggroups.simulate(parser)
     arggroups.process_ffmpeg(parser)
-    parser.add_argument("--delete-unplayable", action="store_true")
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    args.split_longer_than = nums.human_to_seconds(args.split_longer_than)
-    args.min_split_segment = nums.human_to_seconds(args.min_split_segment)
+    arggroups.process_ffmpeg_post(args)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def is_animation_from_probe(probe) -> bool:
     if probe.audio_streams:
         return True
     for stream in probe.video_streams:
@@ -105,18 +103,17 @@
     if video_stream:
         ff_opts.extend(["-c:v", "libsvtav1", "-preset", "8", "-crf", "44"])
 
         width = int(video_stream.get("width"))
         height = int(video_stream.get("height"))
 
         if width > (args.max_width * (1 + args.max_width_buffer)):
-            ff_opts.extend(["-vf", "scale=-2:min(iw\\,{args.max_width})"])
+            ff_opts.extend(["-vf", f"scale={args.max_width}:-2"])
         elif height > (args.max_height * (1 + args.max_height_buffer)):
-            ff_opts.extend(["-vf", "scale=-2:min(ih\\,{args.max_height})"])
-        # TODO: Source Width,Height must be even for YUV_420 colorspace
+            ff_opts.extend(["-vf", f"scale=-2:{args.max_height}"])
 
     is_split = bool(audio_stream)
     if audio_stream:
         channels = audio_stream.get("channels") or 2
         bitrate = int(audio_stream.get("bit_rate") or probe.format.get("bit_rate") or 256000)
         source_rate = int(audio_stream.get("sample_rate") or 44100)
```

### Comparing `xklb-2.7.9/xklb/mediafiles/process_image.py` & `xklb-2.8.1/xklb/mediafiles/process_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import argparse, os, shlex, subprocess
 from pathlib import Path
 
 from xklb import usage
 from xklb.data import imagemagick_errors
-from xklb.utils import arggroups, objects, path_utils, processes, web
+from xklb.utils import arggroups, argparse_utils, path_utils, processes, web
 from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library process-image", usage=usage.process_image)
-    arggroups.capability_simulate(parser)
+    parser = argparse_utils.ArgumentParser(prog="library process-image", usage=usage.process_image)
+    arggroups.simulate(parser)
     parser.add_argument("--delete-unplayable", action="store_true")
 
     parser.add_argument("--max-image-height", type=int, default=2400)
     parser.add_argument("--max-image-width", type=int, default=2400)
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def process_path(args, path):
     if str(path).startswith("http"):
         output_path = Path(web.url_to_local_path(path))
     else:
```

### Comparing `xklb-2.7.9/xklb/misc/dedupe_czkawka.py` & `xklb-2.8.1/xklb/misc/dedupe_czkawka.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import argparse, difflib, os, re, shlex, shutil, subprocess, sys, time
+import difflib, os, re, shlex, shutil, subprocess, sys, time
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 import humanize
 from screeninfo import get_monitors
 
 from xklb import usage
 from xklb.playback import media_player, post_actions
-from xklb.utils import arggroups, consts, devices, file_utils, iterables, mpv_utils, processes
+from xklb.utils import arggroups, argparse_utils, consts, devices, file_utils, iterables, mpv_utils, processes
 from xklb.utils.log_utils import log
 
 left_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
 right_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(usage.dedupe_czkawka)
+    parser = argparse_utils.ArgumentParser(usage.dedupe_czkawka)
     arggroups.playback(parser)
-    arggroups.capability_clobber(parser)
+    arggroups.clobber(parser)
     arggroups.capability_delete(parser)
     arggroups.post_actions(parser)
     parser.set_defaults(start="15%", volume="70")
 
     parser.add_argument(
         "--auto-select-min-ratio",
         type=float,
@@ -32,14 +32,19 @@
     parser.add_argument("--all-left", action="store_true")
     parser.add_argument("--all-right", action="store_true")
     parser.add_argument("--all-delete", action="store_true")
     arggroups.debug(parser)
 
     parser.add_argument("file_path", help="Path to the text file containing the file list.")
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
+
+    arggroups.playback_post(args)
+    arggroups.post_actions_post(args)
+
     return args
 
 
 def backup_and_read_file(file_path):
     backup_filename = file_path + ".bak"
     if not os.path.exists(backup_filename):
         try:
```

### Comparing `xklb-2.7.9/xklb/misc/export_text.py` & `xklb-2.8.1/xklb/misc/export_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import argparse
-from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, db_utils, objects
-from xklb.utils.log_utils import log
+from xklb.utils import arggroups, argparse_utils
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library export-text", usage=usage.export_text)
+    parser = argparse_utils.ArgumentParser(prog="library export-text", usage=usage.export_text)
     parser.add_argument("--format", default="html")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def media_to_files(args):
     if args.format != "html":
         raise NotImplementedError
```

### Comparing `xklb-2.7.9/xklb/multidb/copy_play_counts.py` & `xklb-2.8.1/xklb/multidb/copy_play_counts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import argparse
-from pathlib import Path
 
 from xklb import usage
 from xklb.editdb import dedupe_db
 from xklb.mediadb import db_history
-from xklb.utils import arggroups, db_utils, objects
+from xklb.utils import arggroups, argparse_utils, db_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
+    parser = argparse_utils.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
     parser.add_argument("--source-prefix", default="")
     parser.add_argument("--target-prefix", default="")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
-
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def copy_play_count(args, source_db) -> None:
     s_db = db_utils.connect(argparse.Namespace(database=source_db, verbose=args.verbose))
     m_columns = s_db["media"].columns_dict
```

### Comparing `xklb-2.7.9/xklb/multidb/merge_dbs.py` & `xklb-2.8.1/xklb/multidb/merge_dbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse, sqlite3
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, argparse_utils, db_utils, objects
+from xklb.utils import arggroups, argparse_utils, db_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library merge-dbs", usage=usage.merge_dbs)
+    parser = argparse_utils.ArgumentParser(prog="library merge-dbs", usage=usage.merge_dbs)
 
     parser.add_argument(
         "--only-tables", "-t", action=argparse_utils.ArgparseList, help="Comma separated specific table(s)"
     )
 
     parser.add_argument(
         "--primary-keys", "--pk", action=argparse_utils.ArgparseList, help="Comma separated primary keys"
@@ -30,50 +30,48 @@
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
-
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def merge_db(args, source_db) -> None:
     source_db = str(Path(source_db).resolve())
 
     s_db = db_utils.connect(args, conn=sqlite3.connect(args.database))
     for table in [s for s in s_db.table_names() if "_fts" not in s and not s.startswith("sqlite_")]:
         if args.only_tables and table not in args.only_tables:
             log.info("[%s]: Skipping %s", source_db, table)
             continue
         else:
             log.info("[%s]: %s", source_db, table)
 
+        skip_columns = args.skip_columns
+        primary_keys = args.primary_keys
         if args.business_keys:
-            if not args.primary_keys:
-                args.primary_keys = list(o.name for o in args.db[table].columns if o.is_pk)
+            if not primary_keys:
+                primary_keys = list(o.name for o in args.db[table].columns if o.is_pk)
 
-            args.skip_columns = [*(args.skip_columns or []), *args.primary_keys]
+            skip_columns = [*(args.skip_columns or []), *primary_keys]
 
         selected_columns = s_db[table].columns_dict
         if args.only_target_columns:
             target_columns = args.db[table].columns_dict
             selected_columns = [s for s in selected_columns if s in target_columns]
-        if args.skip_columns:
-            selected_columns = [s for s in selected_columns if s not in args.skip_columns]
+        if skip_columns:
+            selected_columns = [s for s in selected_columns if s not in skip_columns]
 
         log.info("[%s]: %s", table, selected_columns)
         kwargs = {}
-        if args.business_keys or args.primary_keys:
-            source_table_pks = [s for s in (args.business_keys or args.primary_keys) if s in selected_columns]
+        if args.business_keys or primary_keys:
+            source_table_pks = [s for s in (args.business_keys or primary_keys) if s in selected_columns]
             if source_table_pks:
                 log.info("[%s]: Using %s as primary key(s)", table, ", ".join(source_table_pks))
                 kwargs["pk"] = source_table_pks
 
         data = s_db[table].rows_where(where=" and ".join(args.where) if args.where else None)
         data = ({k: v for k, v in d.items() if k in selected_columns} for d in data)
         with args.db.conn:
```

### Comparing `xklb-2.7.9/xklb/playback/media_player.py` & `xklb-2.8.1/xklb/playback/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/playback/play_actions.py` & `xklb-2.8.1/xklb/utils/web.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,538 +1,716 @@
-import argparse, os, shlex, sys
+import argparse, datetime, functools, os, re, tempfile, time, urllib.error, urllib.parse, urllib.request
+from email.message import Message
 from pathlib import Path
+from shutil import which
+from urllib.parse import parse_qs, parse_qsl, quote, unquote, urlencode, urljoin, urlparse, urlunparse
 
-from xklb import media_printer, usage
-from xklb.createdb import tube_backend
-from xklb.fsdb import big_dirs
-from xklb.mediadb import db_history, db_media
-from xklb.playback import media_player
-from xklb.tablefiles import mcda
-from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, nums, objects, processes, sql_utils
-from xklb.utils.arg_utils import parse_args_limit, parse_args_sort
-from xklb.utils.consts import SC
-from xklb.utils.log_utils import Timer, log
-
-
-def parse_args(action, default_chromecast=None) -> argparse.Namespace:
-    DEFAULT_PLAYER_ARGS_SUB = ["--speed=1"]
-    DEFAULT_PLAYER_ARGS_NO_SUB = ["--speed=1.46"]
-
-    parser = argparse.ArgumentParser(prog="library " + action, usage=usage.play(action))
-    arggroups.sql_fs(parser)
-    arggroups.sql_media(parser)
-    arggroups.playback(parser)
-    arggroups.multiple_playback(parser)
-    arggroups.capability_clobber(parser)
-    arggroups.post_actions(parser)
-
-    parser.add_argument("--big-dirs", "--bigdirs", "-B", action="count", default=0, help=argparse.SUPPRESS)
-    arggroups.operation_group_folders(parser)
-    arggroups.operation_cluster(parser)
-    arggroups.operation_related(parser)
-    parser.add_argument("--play-in-order", "-O", nargs="?", const="natural_ps", help=argparse.SUPPRESS)
-
-    parser.add_argument(
-        "--chromecast-device",
-        "--cast-to",
-        "-t",
-        default=default_chromecast or "",
-        help=argparse.SUPPRESS,
+import requests
+from idna import decode as puny_decode
+
+from xklb.utils import consts, db_utils, iterables, nums, path_utils, pd_utils, strings
+from xklb.utils.log_utils import clamp_index, log
+
+headers = {"User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:121.0) Gecko/20100101 Firefox/121.0"}
+session = None
+
+
+def _get_retry_adapter(max_retries):
+    import requests.adapters
+
+    retry = requests.adapters.Retry(
+        total=max_retries,
+        connect=max_retries,
+        read=max_retries,
+        status=max_retries // 2,
+        other=1,
+        redirect=4,
+        raise_on_redirect=False,
+        backoff_factor=3,
+        backoff_jitter=2,
+        backoff_max=22 * 60,
+        status_forcelist=[
+            104,
+            413,
+            429,
+            500,
+            502,
+            503,
+            504,
+            522,
+        ],
     )
-    parser.add_argument("--chromecast", "--cast", "-c", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--cast-with-local", "-wl", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--interdimensional-cable", "-4dtv", type=int, help=argparse.SUPPRESS)
-
-    parser.add_argument(
-        "--partial",
-        "-P",
-        "--previous",
-        "--recent",
-        default=False,
-        const="n",
-        nargs="?",
-        help=argparse.SUPPRESS,
+
+    return requests.adapters.HTTPAdapter(max_retries=retry)
+
+
+def parse_cookies_from_browser(input_str):
+    from yt_dlp.cookies import SUPPORTED_BROWSERS, SUPPORTED_KEYRINGS
+
+    # lifted from yt_dlp to have a compatible interface
+    container = None
+    mobj = re.fullmatch(
+        r"""(?x)
+        (?P<name>[^+:]+)
+        (?:\s*\+\s*(?P<keyring>[^:]+))?
+        (?:\s*:\s*(?!:)(?P<profile>.+?))?
+        (?:\s*::\s*(?P<container>.+))?
+    """,
+        input_str,
     )
+    if mobj is None:
+        raise ValueError(f"invalid cookies from browser arguments: {input_str}")
+    browser_name, keyring, profile, container = mobj.group("name", "keyring", "profile", "container")
+    browser_name = browser_name.lower()
+    if browser_name not in SUPPORTED_BROWSERS:
+        raise ValueError(
+            f'unsupported browser specified for cookies: "{browser_name}". '
+            f'Supported browsers are: {", ".join(sorted(SUPPORTED_BROWSERS))}'
+        )
+    if keyring is not None:
+        keyring = keyring.upper()
+        if keyring not in SUPPORTED_KEYRINGS:
+            raise ValueError(
+                f'unsupported keyring specified for cookies: "{keyring}". '
+                f'Supported keyrings are: {", ".join(sorted(SUPPORTED_KEYRINGS))}'
+            )
+    return (browser_name, profile, keyring, container)
+
+
+def requests_session(args=argparse.Namespace()):
+    global session  # TODO: maybe run_once similar to log_utils.log
+
+    if session is None:
+        import requests
+
+        http_max_retries = getattr(args, "http_max_retries", None) or 8
+        cookie_file = getattr(args, "cookies", None)
+        cookies_from_browser = getattr(args, "cookies_from_browser", None)
+
+        session = requests.Session()
+        session.mount("http://", _get_retry_adapter(http_max_retries))
+        session.mount("https://", _get_retry_adapter(http_max_retries))
+        session.request = functools.partial(session.request, headers=headers, timeout=(5, 45))  # type: ignore
+
+        if getattr(args, "allow_insecure", False):
+            from urllib3.exceptions import InsecureRequestWarning
+
+            requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)  # type: ignore
+            session.verify = False
 
-    parser.add_argument("--watch-later-directory", default=consts.DEFAULT_MPV_WATCH_LATER, help=argparse.SUPPRESS)
-    parser.add_argument("--subtitle-mix", default=consts.DEFAULT_SUBTITLE_MIX, help=argparse.SUPPRESS)
+        if cookie_file or cookies_from_browser:
+            from yt_dlp.cookies import load_cookies
 
-    parser.add_argument("--player-args-sub", "-player-sub", nargs="*", default=DEFAULT_PLAYER_ARGS_SUB)
-    parser.add_argument("--player-args-no-sub", "-player-no-sub", nargs="*", default=DEFAULT_PLAYER_ARGS_NO_SUB)
-    parser.add_argument("--transcode", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--transcode-audio", action="store_true", help=argparse.SUPPRESS)
-
-    for i in range(0, 255):
-        parser.add_argument(f"--cmd{i}", help=argparse.SUPPRESS)
-    parser.add_argument("--shallow-organize", default="/mnt/d/", help=argparse.SUPPRESS)
-
-    parser.add_argument("--safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--refresh", "--rescan", action="store_true")
-
-    parser.add_argument("--fetch-siblings")
-    parser.add_argument("--sibling", "--episode", "--episodes", "--episodic", action="store_true")
-    parser.add_argument("--solo", action="store_true")
-
-    parser.add_argument("--prefetch", type=int, default=3)
-    parser.add_argument("--prefix", default="", help=argparse.SUPPRESS)
-
-    parser.add_argument("--timeout", "-T", help="Quit after x minutes")
-    parser.add_argument("--delete-unplayable", action="store_true")
-    arggroups.debug(parser)
-
-    arggroups.database(parser)
-    parser.add_argument("search", nargs="*")
-    args = parser.parse_intermixed_args()
-    args.action = action
-    args.defaults = []
-
-    args.include += args.search
-    if len(args.include) == 1:
-        if args.include == ["."]:
-            args.include = [str(Path().cwd().resolve())]
-        elif os.sep in args.include[0]:
-            args.include = [file_utils.resolve_absolute_path(args.include[0])]
-
-    args.db = db_utils.connect(args)
-
-    if args.mpv_socket is None:
-        if args.action in (SC.listen,):
-            args.mpv_socket = consts.DEFAULT_MPV_LISTEN_SOCKET
+            if cookies_from_browser:
+                cookies_from_browser = parse_cookies_from_browser(cookies_from_browser)
+            cookie_jar = load_cookies(cookie_file, cookies_from_browser, ydl=None)
+            session.cookies = cookie_jar  # type: ignore
+
+    return session
+
+
+def stat(path):
+    try:
+        r = requests_session().head(path)
+        info = {}
+
+        if 200 <= r.status_code < 400:
+            if "content-length" in r.headers:
+                info["size"] = int(r.headers["content-length"])
+
+            if "last-modified" in r.headers:
+                last_modified = r.headers["last-modified"]
+                info["time_modified"] = int(
+                    datetime.datetime.strptime(last_modified, "%a, %d %b %Y %H:%M:%S GMT").timestamp()
+                )
+
+        elif r.status_code == 404:
+            info["time_deleted"] = consts.now()
         else:
-            args.mpv_socket = consts.DEFAULT_MPV_WATCH_SOCKET
+            r.raise_for_status()
 
-    if args.big_dirs:
-        args.local_media_only = True
+        return info
+    except requests.RequestException as e:
+        log.exception("%s could not get metadata", path)
+        return {}
+
+
+def get(args, url, skip_404=True, ignore_errors=False, ignore_429=False, **kwargs):
+    s = requests_session(args)
+    try:
+        response = s.get(url, **kwargs)
+    except (
+        requests.exceptions.ConnectionError,
+        requests.exceptions.Timeout,
+        requests.exceptions.ChunkedEncodingError,
+        requests.exceptions.ContentDecodingError,
+        requests.exceptions.RequestException,
+    ):
+        raise
+    else:
+        code = response.status_code
 
-    parse_args_limit(args)
-    parse_args_sort(args)
+        if 200 <= code < 400:
+            return response
+        elif code == 404:
+            if skip_404:
+                log.warning("HTTP404 Not Found: %s", url)
+                return None
+            else:
+                raise FileNotFoundError
+        elif ignore_errors and (400 <= code < 429 or 431 <= code < 500):
+            return response
+        elif ignore_429 and (400 <= code < 500):
+            return response
+        else:
+            response.raise_for_status()
 
-    if args.cols:
-        args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
+    log.info("Something weird is happening probably: %s", url)
+    return response
 
-    if args.duration:
-        args.duration = sql_utils.parse_human_to_sql(nums.human_to_seconds, "duration", args.duration)
 
-    if args.size:
-        args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
+class PartialContent:
+    def __init__(self, url, max_size=1048576):
+        self.url = url
+        self.max_size = max_size
+        self.temp_file = None
 
-    if args.duration_from_size:
-        args.duration_from_size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.duration_from_size)
+    def __enter__(self):
+        response = requests_session().get(self.url, stream=True)
 
-    if args.chromecast:
-        from catt.api import CattDevice
+        code = response.status_code
+        if code == 404:
+            log.warning("HTTP404 Not Found: %s", self.url)
+            return None
+        else:
+            response.raise_for_status()
 
-        args.cc = CattDevice(args.chromecast_device, lazy=True)
-        args.cc_ip = devices.get_ip_of_chromecast(args.chromecast_device)
+        self.temp_file = tempfile.NamedTemporaryFile(delete=False)
 
-    if args.override_player:
-        args.override_player = shlex.split(args.override_player)
+        for chunk in response.iter_content(chunk_size=65536):
+            if self.temp_file.tell() < self.max_size:
+                self.temp_file.write(chunk)
+            else:
+                break
 
-    if args.multiple_playback > 1:
-        args.gui = True
+        self.temp_file.close()
+        return self.temp_file.name
 
-    if args.keep_dir:
-        args.keep_dir = Path(args.keep_dir).expanduser().resolve()
+    def __exit__(self, exc_type, exc_value, traceback):
+        if self.temp_file:
+            os.remove(self.temp_file.name)
 
-    if args.solo:
-        args.upper = 1
-    if args.sibling:
-        args.lower = 2
 
-    if args.post_action:
-        args.post_action = args.post_action.replace("-", "_")
+def download_embeds(args, soup):
+    for img in soup.find_all("img"):
+        local_path = Path.cwd() / "images"
+        local_path.mkdir(exist_ok=True)
+        local_path = local_path / Path(urllib.parse.unquote(img["src"])).name
 
-    log.info(objects.dict_filter_bool(args.__dict__))
+        response = get(args, img["src"])
+        if response:
+            with open(local_path, "wb") as f:
+                f.write(response.content)
 
-    processes.timeout(args.timeout)
+            img["src"] = local_path.relative_to(Path.cwd())  # Update image source to point to local file
 
-    args.sock = None
-    return args
 
+def find_date(soup):
+    import dateutil.parser
 
-def construct_query(args) -> tuple[str, dict]:
-    m_columns = db_utils.columns(args, "media")
+    for text in soup.find_all(text=True):
+        try:
+            date = dateutil.parser.parse(text)
+            return date
+        except ValueError:
+            pass
+    return None
 
-    args.filter_sql = []
-    args.aggregate_filter_sql = []
-    args.filter_bindings = {}
 
-    if args.duration:
-        args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
-    if args.size:
-        args.filter_sql.append(" and size IS NOT NULL " + args.size)
-    if args.duration_from_size:
-        args.filter_sql.append(
-            " and size IS NOT NULL and duration in (select distinct duration from media where 1=1 "
-            + args.duration_from_size
-            + ")",
-        )
+def set_timestamp(headers, path):
+    if "Last-Modified" in headers:
+        modified_time = datetime.datetime.strptime(headers["Last-Modified"], "%a, %d %b %Y %H:%M:%S GMT")
+        mtime = time.mktime(modified_time.timetuple())
+        atime = time.time()
+        os.utime(path, (atime, mtime))
 
-    if args.no_video:
-        args.filter_sql.append(" and video_count=0 ")
-    if args.no_audio:
-        args.filter_sql.append(" and audio_count=0 ")
-    if args.subtitles:
-        args.filter_sql.append(" and subtitle_count>0 ")
-    if args.no_subtitles:
-        args.filter_sql.append(" and subtitle_count=0 ")
-
-    if args.created_within:
-        args.aggregate_filter_sql.append(
-            f"and time_created >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.created_within)}')) as int)",
-        )
-    if args.created_before:
-        args.aggregate_filter_sql.append(
-            f"and time_created < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.created_before)}')) as int)",
-        )
-    if args.changed_within:
-        args.aggregate_filter_sql.append(
-            f"and time_modified >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.changed_within)}')) as int)",
-        )
-    if args.changed_before:
-        args.aggregate_filter_sql.append(
-            f"and time_modified < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.changed_before)}')) as int)",
-        )
-    if args.played_within:
-        args.aggregate_filter_sql.append(
-            f"and time_last_played >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.played_within)}')) as int)",
-        )
-    if args.played_before:
-        args.aggregate_filter_sql.append(
-            f"and time_last_played < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.played_before)}')) as int)",
-        )
-    if args.deleted_within:
-        args.aggregate_filter_sql.append(
-            f"and time_deleted >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.deleted_within)}')) as int)",
-        )
-    if args.deleted_before:
-        args.aggregate_filter_sql.append(
-            f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.deleted_before)}')) as int)",
-        )
-    if args.downloaded_within:
-        args.aggregate_filter_sql.append(
-            f"and time_downloaded >= cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.downloaded_within)}')) as int)",
-        )
-    if args.downloaded_before:
-        args.aggregate_filter_sql.append(
-            f"and time_downloaded < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.downloaded_before)}')) as int)",
-        )
 
-    args.table = "media"
-    if args.db["media"].detect_fts() and not args.no_fts:
-        if args.include:
-            args.table, search_bindings = db_utils.fts_search_sql(
-                "media",
-                fts_table=args.db["media"].detect_fts(),
-                include=args.include,
-                exclude=args.exclude,
-                flexible=args.flexible_search,
-            )
-            args.filter_bindings = {**args.filter_bindings, **search_bindings}
-            m_columns = {**m_columns, "rank": int}
-        elif args.exclude:
-            db_utils.construct_search_bindings(
-                args,
-                [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-            )
+def load_selenium(args, wire=False):
+    if wire:
+        import logging
+
+        from seleniumwire import webdriver
+
+        log_levels = [logging.ERROR, logging.ERROR, logging.WARNING, logging.INFO, logging.DEBUG]
+        for logger_name, logger in logging.root.manager.loggerDict.items():
+            if logger_name.startswith("selenium"):
+                logging.getLogger(logger_name).setLevel(clamp_index(log_levels, args.verbose - 1))
+
     else:
-        db_utils.construct_search_bindings(
-            args,
-            [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"]],
-        )
+        from selenium import webdriver
 
-    if args.table == "media" and args.random and not any([args.print, args.limit not in args.defaults]):
-        limit = 16 * (args.limit or consts.DEFAULT_PLAY_QUEUE)
-        where_not_deleted = (
-            "where COALESCE(time_deleted,0) = 0"
-            if "time_deleted" in m_columns
-            and "deleted" not in args.sort_groups_by
-            and "time_deleted" not in " ".join(args.where)
-            else ""
-        )
-        args.filter_sql.append(
-            f"and m.id in (select id from media {where_not_deleted} order by random() limit {limit})",
-        )
+    xvfb = None  # three states
+    if args.verbose < consts.LOG_DEBUG and not getattr(args, "manual", False):
+        xvfb = False
+        try:
+            from pyvirtualdisplay.display import Display
+
+            args.driver_display = Display(visible=False, size=(1280, 720))
+            args.driver_display.start()
+            xvfb = True
+        except Exception:
+            pass
 
-    aggregate_filter_columns = ["time_first_played", "time_last_played", "play_count", "playhead"]
+    if (which("firefox") or which("firefox.exe") or getattr(args, "firefox", False)) and not getattr(
+        args, "chrome", False
+    ):
+        from selenium.webdriver.firefox.options import Options
+        from selenium.webdriver.firefox.service import Service
 
-    cols = args.cols or ["path", "title", "duration", "size", "subtitle_count", "is_dir", "rank"]
-    if "deleted" in " ".join(sys.argv):
-        cols.append("time_deleted")
-    if "played" in " ".join(sys.argv):
-        cols.append("time_last_played")
-    args.select = [c for c in cols if c in m_columns or c in ["*"]] + getattr(args, "select", [])
-    if args.action == SC.read and "tags" in m_columns:
-        args.select += ["cast(length(tags) / 4.2 / 220 * 60 as INT) + 10 duration"]
-
-    select_sql = "\n        , ".join(args.select)
-    limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
-    offset_sql = f"OFFSET {args.offset}" if args.offset and args.limit else ""
-    query = f"""WITH m as (
-            SELECT
-                m.id
-                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-                , MIN(h.time_played) time_first_played
-                , MAX(h.time_played) time_last_played
-                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                , *
-            FROM {args.table} m
-            LEFT JOIN history h on h.media_id = m.id
-            WHERE 1=1
-                {db_media.filter_args_sql(args, m_columns)}
-                {" ".join(args.filter_sql)}
-                {" ".join([f" and path like '%.{ext}'" for ext in args.ext])}
-                {" ".join([" and " + w for w in args.where if not any(a in w for a in aggregate_filter_columns)])}
-            GROUP BY m.id, m.path
-        )
-        SELECT
-            {select_sql}
-            , play_count
-            , time_first_played
-            , time_last_played
-            , playhead
-        FROM m
-        WHERE 1=1
-            {" ".join(args.aggregate_filter_sql)}
-            {" ".join([" and " + w for w in args.where if any(a in w for a in aggregate_filter_columns)])}
-        ORDER BY 1=1
-            , {args.sort}
-        {limit_sql} {offset_sql}
-    """
-
-    args.filter_sql = [s for s in args.filter_sql if "id" not in s]  # only use random id constraint in first query
-
-    return query, args.filter_bindings
-
-
-def filter_episodic(args, media: list[dict]) -> list[dict]:
-    parent_dict = {}
-    for m in media:
-        path = Path(m["path"])
-        parent_path = path.parent
-        parent_dict.setdefault(parent_path, 0)
-        parent_dict[parent_path] += 1
-
-    filtered_media = []
-    for m in media:
-        path = Path(m["path"])
-        parent_path = path.parent
-
-        siblings = parent_dict[parent_path]
-
-        if args.lower is not None and siblings < args.lower:
-            continue
-        elif args.upper is not None and siblings > args.upper:
-            continue
-        else:
-            filtered_media.append(m)
+        service = Service(log_path=tempfile.mktemp(".geckodriver.log"))
+        options = Options()
+        if Path("selenium").exists():
+            options.profile = "selenium"
+
+        options.set_preference("media.volume_scale", "0.0")
+        if xvfb is False:
+            options.add_argument("--headless")
+
+        args.driver = webdriver.Firefox(service=service, options=options)
+
+        addons = [Path("~/.local/lib/ublock_origin.xpi").expanduser().resolve()]
+        if getattr(args, "auto_pager", False):
+            addons.append(Path("~/.local/lib/weautopagerize.xpi").expanduser().resolve())
+
+        for addon_path in addons:
+            try:
+                args.driver.install_addon(str(addon_path))
+            except Exception:
+                if args.verbose > 0:
+                    log.warning("Could not install firefox addon. Missing file %s", addon_path)
+                else:
+                    log.exception("Could not install firefox addon. Missing file %s", addon_path)
+
+        if getattr(args, "auto_pager", False):
+            time.sleep(60)  # let auto-pager initialize
 
-    return filtered_media
+    else:
+        from selenium.webdriver.chrome.options import Options
+
+        options = Options()
+        if Path("selenium").exists():
+            options.add_argument("user-data-dir=selenium")
+
+        options.add_argument("--mute-audio")
+        if xvfb is False:
+            options.add_argument("--headless=new")
+
+        addons = [Path("~/.local/lib/ublock_origin.crx").expanduser().resolve()]
+        if getattr(args, "auto_pager", False):
+            addons.append(Path("~/.local/lib/autopager.crx").expanduser().resolve())
+        for addon_path in addons:
+            try:
+                options.add_extension(str(addon_path))
+            except Exception:
+                if args.verbose > 0:
+                    log.warning("Could not install chrome extension. Missing file %s", addon_path)
+                else:
+                    log.exception("Could not install chrome extension. Missing file %s", addon_path)
 
+        args.driver = webdriver.Chrome(options=options)
 
-def history_sort(args, media) -> list[dict]:
-    if "s" in args.partial:  # skip; only play unseen
-        previously_watched_paths = [m["path"] for m in media if m["time_first_played"]]
-        return [m for m in media if m["path"] not in previously_watched_paths]
-
-    def mpv_progress(m):
-        playhead = m.get("playhead")
-        duration = m.get("duration")
-        if not playhead:
-            return float("-inf")
-        if not duration:
-            return float("-inf")
-
-        if "p" in args.partial and "t" in args.partial:
-            return (duration / playhead) * -(duration - playhead)  # weighted remaining
-        elif "t" in args.partial:
-            return -(duration - playhead)  # time remaining
-        else:
-            return playhead / duration  # percent remaining
 
-    def sorting_hat():
-        if "f" in args.partial:  # first-viewed
-            return lambda m: m.get("time_first_played") or 0
-        elif "p" in args.partial or "t" in args.partial:  # sort by remaining duration
-            return mpv_progress
-
-        return lambda m: m.get("time_last_played") or m.get("time_first_played") or 0
-
-    reverse_chronology = True
-    if "o" in args.partial:  # oldest first
-        reverse_chronology = False
-
-    key = sorting_hat()
-    if args.print:
-        reverse_chronology = not reverse_chronology
-
-    media = sorted(
-        media,
-        key=key,
-        reverse=reverse_chronology,
+def quit_selenium(args):
+    args.driver.quit()
+    if consts.LOG_DEBUG > args.verbose and not getattr(args, "manual", False):
+        try:
+            args.driver_display.stop()
+        except Exception:
+            pass
+
+
+def safe_unquote(url):
+    # https://en.wikipedia.org/wiki/Internationalized_Resource_Identifier
+    # we aren't writing HTML so we can unquote
+
+    try:
+        parsed_url = urlparse(url)
+    except UnicodeDecodeError:
+        return url
+
+    def selective_unquote(component, restricted_chars):
+        try:
+            unquoted = unquote(component, errors="strict")
+        except UnicodeDecodeError:
+            return component
+        # re-quote restricted chars
+        return "".join(quote(char, safe="") if char in restricted_chars else char for char in unquoted)
+
+    def unquote_query_params(query):
+        query_pairs = parse_qsl(query, keep_blank_values=True)
+        return "&".join(
+            selective_unquote(key, "=&#") + "=" + selective_unquote(value, "=&#") for key, value in query_pairs
+        )
+
+    unquoted_path = selective_unquote(parsed_url.path, ";?#")
+    unquoted_params = selective_unquote(parsed_url.params, "?#")
+    unquoted_query = unquote_query_params(parsed_url.query)
+    unquoted_fragment = selective_unquote(parsed_url.fragment, "")
+
+    new_url = urlunparse(
+        (parsed_url.scheme, parsed_url.netloc, unquoted_path, unquoted_params, unquoted_query, unquoted_fragment)
     )
 
-    if args.offset:
-        media = media[int(args.offset) :]
+    return new_url
 
-    return media
 
+def url_decode(href):
+    href = safe_unquote(href)
+    up = urlparse(href)
+    if up.netloc:
+        try:
+            href = href.replace(up.netloc, puny_decode(up.netloc), 1)
+        except Exception:
+            pass
+    return href
 
-def process_playqueue(args) -> None:
-    db_history.create(args)
 
-    query, bindings = construct_query(args)
-
-    if args.print and not any(
-        [
-            args.partial,
-            args.lower,
-            args.upper,
-            args.safe,
-            args.play_in_order,
-            args.big_dirs,
-            args.fetch_siblings,
-            args.related,
-            args.cluster_sort,
-            args.folders,
-            args.folder_glob,
-        ],
-    ):
-        media_printer.printer(args, query, bindings)
+def path_tuple_from_url(url):
+    url = url_decode(url)
+    parsed_url = urlparse(url)
+    relative_path = os.path.join(parsed_url.netloc, parsed_url.path.lstrip("/"))
+    base_path = os.path.dirname(relative_path)
+    filename = os.path.basename(parsed_url.path)
+    return base_path, filename
+
+
+def filename_from_content_disposition(response):
+    content_disposition = response.headers.get("Content-Disposition", "")
+    if "filename=" in content_disposition:
+        msg = Message()
+        msg["content-disposition"] = content_disposition
+        filename = msg.get_filename()
+        if filename:
+            return filename
+    return None
+
+
+def url_to_local_path(url, response=None, output_path=None, output_prefix=None):
+    base_path, filename = path_tuple_from_url(url)
+
+    if response:
+        filename_from_site = filename_from_content_disposition(response)
+        if filename_from_site:
+            filename = filename_from_site
+
+    if not output_path:
+        output_path = filename
+        if base_path:
+            output_path = os.path.join(base_path, filename)
+
+    output_path = path_utils.clean_path(output_path.encode())
+
+    if output_prefix:
+        output_path = os.path.join(output_prefix, output_path)
+
+    return output_path
+
+
+def download_url(url, output_path=None, output_prefix=None, chunk_size=8 * 1024 * 1024, retry_num=0, max_retries=10):
+    if retry_num > max_retries:
+        raise RuntimeError(f"Max retries exceeded for {url}")
+
+    session = requests_session()
+    r = session.get(url, stream=True)
+
+    if not 200 <= r.status_code < 400:
+        log.error(f"Error {r.status_code} {url}")
+
+    remote_size = nums.safe_int(r.headers.get("Content-Length"))
+
+    output_path = url_to_local_path(url, response=r, output_path=output_path, output_prefix=output_prefix)
+    if output_path == ".":
+        log.warning("Skipping directory %s", url)
         return
+    else:
+        log.info("Saving %s to %s", url, output_path)
 
-    t = Timer()
-    media = list(args.db.query(query, bindings))
-    log.debug("query: %s", t.elapsed())
-
-    if args.fetch_siblings:
-        media = db_media.get_sibling_media(args, media)
-
-    if args.partial:
-        media = history_sort(args, media)
-        log.debug("utils.history_sort: %s", t.elapsed())
-
-    if args.lower is not None or args.upper is not None:
-        media = filter_episodic(args, media)
-        log.debug("utils.filter_episodic: %s", t.elapsed())
-
-    if not media:
-        if args.include:
-            p = Path(" ".join(args.include)).resolve()
-            if p.is_file():
-                media = [{"path": str(p)}]
-            elif p.is_dir():
-                if args.folder_glob:
-                    media = [{"path": s} for s in file_utils.fast_glob(p)]
-                elif args.action in SC.watch:
-                    media = [{"path": s} for s in file_utils.rglob(str(p), consts.VIDEO_EXTENSIONS)[0]]
-                elif args.action == SC.listen:
-                    media = [{"path": s} for s in file_utils.rglob(str(p), consts.AUDIO_ONLY_EXTENSIONS)[0]]
-                elif args.action in SC.view:
-                    media = [{"path": s} for s in file_utils.rglob(str(p), consts.IMAGE_EXTENSIONS)[0]]
-                elif args.action in SC.read:
-                    media = [{"path": s} for s in file_utils.rglob(str(p), consts.TEXTRACT_EXTENSIONS)[0]]
-                else:
-                    media = [{"path": s} for s in file_utils.rglob(str(p))[0]]
+    p = Path(output_path)
+    p.parent.mkdir(parents=True, exist_ok=True)
+    if p.exists():
+        if remote_size:
+            local_size = p.stat().st_size
+            if local_size == remote_size:
+                log.warning(f"Download skipped. File with same size already exists: {output_path}")
+                return
+            elif local_size < 5242880:  # TODO: check if first few kilobytes match what already exists locally...
+                p.unlink()
             else:
-                processes.no_media_found()
+                headers = {"Range": f"bytes={local_size}-"}
+                r = session.get(url, headers=headers, stream=True)
+                if r.status_code != 206:  # HTTP Partial Content
+                    p.unlink()
+                    r = session.get(url, stream=True)
         else:
-            processes.no_media_found()
+            p.unlink()
 
-    if args.safe:
-        media = [d for d in media if tube_backend.is_supported(d["path"]) or Path(d["path"]).exists()]
-        log.debug("tube_backend.is_supported: %s", t.elapsed())
-
-    if args.related >= consts.RELATED:
-        media = db_media.get_related_media(args, media[0])
-        log.debug("player.get_related_media: %s", t.elapsed())
-
-    if args.big_dirs:
-        media_keyed = {d["path"]: d for d in media}
-        folders = big_dirs.group_files_by_parents(args, media)
-        dirs = big_dirs.process_big_dirs(args, folders)
-        dirs = mcda.group_sort_by(args, dirs)
-        log.debug("process_bigdirs: %s", t.elapsed())
-        dirs = list(reversed([d["path"] for d in dirs]))
-        if "limit" in args.defaults:
-            media = db_media.get_dir_media(args, dirs)
-            log.debug("get_dir_media: %s", t.elapsed())
-        else:
-            media = []
-            media_set = set()
-            for dir in dirs:
-                if len(dir) == 1:
-                    continue
-
-                for key in media_keyed:
-                    if key in media_set:
-                        continue
-
-                    if os.sep not in key.replace(dir, "") and key.startswith(dir):
-                        media_set.add(key)
-                        media.append(media_keyed[key])
-            log.debug("double for loop compare_block_strings: %s", t.elapsed())
-
-    if args.play_in_order:
-        media = db_media.natsort_media(args, media)
-
-    if args.cluster_sort:
-        from xklb.text.cluster_sort import cluster_dicts
-
-        media = cluster_dicts(args, media)
-        log.debug("cluster-sort: %s", t.elapsed())
-
-    if getattr(args, "refresh", False):
-        marked = db_media.mark_media_deleted(args, [d["path"] for d in media if not Path(d["path"]).exists()])
-        log.warning(f"Marked {marked} metadata records as deleted")
-        args.refresh = False
-        return process_playqueue(args)
-
-    if args.folders:
-        unique_folders = set()
-        media_unique_folders = []
-        for m in media:
-            folder_path = str(Path(m["path"]).parent)
-            if folder_path not in unique_folders:
-                unique_folders.add(folder_path)
-                media_unique_folders.append({**m, "path": folder_path})
-        media = media_unique_folders
-    elif args.folder_glob:
-        media = ({"path": s} for m in media for s in file_utils.fast_glob(Path(m["path"]).parent, args.folder_glob))
-
-    if any(
-        [
-            args.print,
-            args.delete_files,
-            args.delete_rows,
-            args.mark_deleted,
-            args.mark_watched,
-        ]
-    ):
-        media_printer.media_printer(args, media)
+    try:
+        with open(output_path, "ab") as f:
+            for chunk in r.iter_content(chunk_size=chunk_size):
+                if chunk:
+                    f.write(chunk)
+
+        if remote_size:
+            downloaded_size = os.path.getsize(output_path)
+            if downloaded_size < remote_size:
+                msg = f"Incomplete download ({strings.safe_percent(downloaded_size/remote_size)}) {output_path}"
+                raise RuntimeError(msg)
+    except OSError:
+        raise
+    except Exception:
+        retry_num += 1
+        log.info("Retry #%s %s", retry_num, url)
+        time.sleep(retry_num)
+        return download_url(url, output_path, output_prefix, chunk_size, retry_num)
+
+    set_timestamp(r.headers, output_path)
+    return output_path
+
+
+def get_elements_forward(start, end):
+    elements = []
+    current = start.next_sibling
+    while current and current != end:
+        elements.append(current)
+        current = current.next_sibling
+    return elements
+
+
+def extract_nearby_text(a_element):
+    prev_a = a_element.find_previous("a")
+    next_a = a_element.find_next("a")
+
+    before = ""
+    if prev_a:
+        before = " ".join(s.get_text(strip=True) for s in get_elements_forward(prev_a, a_element))
+
+    after = ""
+    if next_a:
+        after = " ".join(s.get_text(strip=True) for s in get_elements_forward(a_element, next_a))
+
+    return before, after
+
+
+def save_html_table(args, html_file):
+    import pandas as pd
+
+    dfs = pd.read_html(html_file, extract_links="body", flavor="bs4")
+    tables = []
+    for df in dfs:
+        df = pd_utils.columns_snake_case(df)
+
+        # extract URLs into their own columns
+        for col in df.columns:
+            if df[col].dtype == "object":
+                df[[col, f"{col}_url"]] = pd.DataFrame(df[col].tolist(), index=df.index)
+        df.columns = df.columns.astype(str)
+        df = df.dropna(axis=1, how="all")  # drop empty columns
+
+        df = pd_utils.convert_dtypes(df)
+
+        tables.append({"table_name": None, "data": df.to_dict(orient="records")})
+
+    tables = db_utils.add_missing_table_names(args, tables)
+    for d in tables:
+        args.db[d["table_name"]].insert_all(iterables.list_dict_filter_bool(d["data"]), alter=True)
+
+
+def re_trigger_input(driver):
+    from selenium.common.exceptions import NoSuchElementException
+    from selenium.webdriver.common.by import By
+    from selenium.webdriver.common.keys import Keys
+
+    input_field = None
+    for by, name in [
+        (By.NAME, "q"),
+        (By.NAME, "query"),
+        (By.CSS_SELECTOR, "input[type='search']"),
+        (By.NAME, "search"),
+        (By.NAME, "search-input"),
+        (By.NAME, "search-query"),
+        (By.NAME, "search-box"),
+        (By.ID, "q"),
+        (By.ID, "query"),
+        (By.ID, "search"),
+        (By.ID, "search-input"),
+        (By.ID, "search-query"),
+        (By.ID, "search-input"),
+        (By.ID, "search-box"),
+        (By.CLASS_NAME, "q"),
+        (By.CLASS_NAME, "query"),
+        (By.CLASS_NAME, "search"),
+        (By.CLASS_NAME, "search-input"),
+        (By.CLASS_NAME, "search-query"),
+        (By.CLASS_NAME, "search-input"),
+        (By.CLASS_NAME, "search-box"),
+        (By.TAG_NAME, "input"),
+    ]:
+        try:
+            input_field = driver.find_element(by, name)
+            break
+        except NoSuchElementException:
+            pass
+
+    if input_field is None:
+        return
     else:
-        media_player.play_list(args, media)
+        input_field.send_keys(Keys.RETURN)
+        driver.implicitly_wait(8)
+
 
+def selenium_get_page(args, url):
+    args.driver.get(url)
+    args.driver.implicitly_wait(5)
 
-def watch() -> None:
-    args = parse_args(SC.watch, default_chromecast="Living Room TV")
-    process_playqueue(args)
+    if getattr(args, "poke", False):
+        re_trigger_input(args.driver)
 
 
-def listen() -> None:
-    args = parse_args(SC.listen, default_chromecast="Xylo and Orchestra")
-    process_playqueue(args)
+def scroll_down(driver):
+    driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
+    time.sleep(2)
+    new_height = driver.execute_script("return document.body.scrollHeight")
+    return new_height
+
+
+def extract_html(url) -> str:
+    session = requests_session()
+    r = session.get(url, timeout=120, headers=headers)
+    r.raise_for_status()
+    markup = r.text
+    return markup
+
+
+def selenium_extract_html(driver) -> str:
+    # trigger rollover events
+    driver.execute_script(
+        "(function(){function k(x) { if (x.onmouseover) { x.onmouseover(); x.backupmouseover = x.onmouseover; x.backupmouseout = x.onmouseout; x.onmouseover = null; x.onmouseout = null; } else if (x.backupmouseover) { x.onmouseover = x.backupmouseover; x.onmouseout = x.backupmouseout; x.onmouseover(); x.onmouseout(); } } var i,x; for(i=0; x=document.links[i]; ++i) k(x); for (i=0; x=document.images[i]; ++i) k(x); })()"
+    )
+
+    # include Shadow DOM
+    html_text = driver.execute_script(
+        'function s(n=document.body){if(!n)return"";if(n.nodeType===Node.TEXT_NODE)return n.textContent.trim();if(n.nodeType!==Node.ELEMENT_NODE)return"";let t="";let r=n.cloneNode();n=n.shadowRoot||n;if(n.children.length)for(let o of n.childNodes)if(o.assignedNodes){if(o.assignedNodes()[0])t+=s(o.assignedNodes()[0]);else t+=o.innerHTML}else t+=s(o);else t=n.innerHTML;return r.innerHTML=t,r.outerHTML}; return s()'
+    )
 
+    return html_text
 
-def filesystem() -> None:
-    args = parse_args(SC.filesystem)
-    process_playqueue(args)
 
+def infinite_scroll(driver):
+    last_height = driver.execute_script("return document.body.scrollHeight")
+    while True:
+        new_height = scroll_down(driver)
+        yield selenium_extract_html(driver)
 
-def read() -> None:
-    args = parse_args(SC.read)
-    process_playqueue(args)
+        if new_height == last_height:  # last page
+            time.sleep(5)  # try once more in case slow page
+            new_height = scroll_down(driver)
+            if new_height == last_height:
+                break
+        last_height = new_height
+
+    yield selenium_extract_html(driver)
+
+
+def construct_search(engine, s):
+    s = urllib.parse.quote(s, safe="")
+    return engine.replace("%", s, 1)
+
+
+def construct_absolute_url(base_url, href):
+    href = safe_unquote(href)
+
+    up = urlparse(href)
+    if up.scheme and up.scheme not in ("https", "http", "ftp"):
+        return href
+
+    if not up.netloc:
+        href = urljoin(base_url, href)
+
+    up = urlparse(href)
+    if up.netloc:
+        try:
+            href = href.replace(up.netloc, puny_decode(up.netloc), 1)
+        except Exception:
+            pass
+    return href
+
+
+def is_index(url):
+    if url.endswith("/"):
+        return True
+
+    patterns = [
+        r"/index\.php\?dir=",
+        r"/index\.php$",
+        r"/index\.html?$",
+    ]
+    for pattern in patterns:
+        if re.search(pattern, url, re.IGNORECASE):
+            return True
+
+    return False
+
+
+def is_subpath(parent_url, child_url):
+    child = urlparse(child_url)
+    parent = urlparse(parent_url)
+
+    if child.scheme != parent.scheme or child.netloc != parent.netloc:
+        return False
+
+    return child_url.startswith(parent_url)
+
+
+def remove_apache_sorting_params(url):
+    parsed_url = urlparse(url)
+    query_params = parse_qs(parsed_url.query)
+
+    apache_sorting_keys = ["C", "O"]
+    for key in apache_sorting_keys:
+        query_params.pop(key, None)
+    new_query_string = urlencode(query_params, doseq=True)
+
+    new_url = urlunparse(
+        (
+            parsed_url.scheme,
+            parsed_url.netloc,
+            parsed_url.path,
+            parsed_url.params,
+            new_query_string,
+            parsed_url.fragment,
+        )
+    )
+
+    return new_url
+
+
+def is_html(url, max_size=15 * 1024 * 1024):
+    r = requests_session().get(url, stream=True)
+
+    content_length = r.headers.get("Content-Length")
+    if content_length and int(content_length) > max_size:
+        return False
+
+    content_type = r.headers.get("Content-Type")
+    if content_type and not any(
+        s in content_type for s in ("text/html", "text/xhtml", "text/xml", "application/xml", "application/xhtml+xml")
+    ):
+        return False
 
+    try:
+        chunk = next(r.iter_content(max_size + 1))  # one more byte than max_size
+        if len(chunk) > max_size:
+            return False
+    except (requests.RequestException, StopIteration):
+        return False
 
-def view() -> None:
-    args = parse_args(SC.view)
-    process_playqueue(args)
+    return True  # if ambiguous, return True
```

### Comparing `xklb-2.7.9/xklb/playback/playback_control.py` & `xklb-2.8.1/xklb/playback/playback_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import argparse, platform, textwrap
 from copy import deepcopy
 from pathlib import Path
 
-from xklb.utils import arggroups, consts, file_utils, iterables, mpv_utils, nums, objects, printing, processes
+from xklb.utils import (
+    arggroups,
+    argparse_utils,
+    consts,
+    file_utils,
+    iterables,
+    mpv_utils,
+    nums,
+    objects,
+    printing,
+    processes,
+)
 from xklb.utils.log_utils import log
 
 
 def parse_args(action) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog=f"library {action}",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     if action == "next":
         arggroups.capability_delete(parser)
 
     parser.add_argument("--mpv-socket", default=consts.DEFAULT_MPV_LISTEN_SOCKET)
     parser.add_argument("--chromecast-device", "--cast-to", "-t")
 
     arggroups.debug(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
     args.mpv = mpv_utils.connect_mpv(args.mpv_socket)
 
-    log.info(objects.dict_filter_bool(args.__dict__))
-
     return args
 
 
 def _now_playing(args) -> dict:
     media = {
         "catt": Path(consts.CAST_NOW_PLAYING).read_text() if Path(consts.CAST_NOW_PLAYING).exists() else None,
         "mpv": args.mpv.command("get_property", "path") if Path(args.mpv_socket).exists() else None,
```

### Comparing `xklb-2.7.9/xklb/playback/post_actions.py` & `xklb-2.8.1/xklb/playback/post_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import re, shlex, shutil
+import shlex, shutil
 from pathlib import Path
 
 import humanize
 
 from xklb.mediadb import db_history, db_media
 from xklb.utils import devices, file_utils, iterables, processes
 from xklb.utils.log_utils import log
@@ -15,18 +15,15 @@
 except ModuleNotFoundError:
     gui = None
 
 
 def mv_to_keep_folder(args, media_file: str):
     keep_path = Path(args.keep_dir)
     if not keep_path.is_absolute():
-        kp = re.match(args.shallow_organize + "(.*?)/", media_file)
-        if kp:
-            keep_path = Path(kp[0], f"{args.keep_dir}/")
-        elif Path(media_file).parent.match(f"*/{args.keep_dir}/*"):
+        if Path(media_file).parent.match(f"*/{args.keep_dir}/*"):
             return media_file
         else:
             keep_path = Path(media_file).parent / f"{args.keep_dir}/"
 
     keep_path.mkdir(exist_ok=True)
 
     try:
```

### Comparing `xklb-2.7.9/xklb/playback/surf.py` & `xklb-2.8.1/xklb/playback/surf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import argparse, logging, sys
 from time import sleep
 
 from xklb import usage
 from xklb.playback import media_player
-from xklb.utils import arggroups, db_utils, objects, processes
+from xklb.utils import arggroups, argparse_utils, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library surf",
         usage=usage.surf,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--count", "-n", default=2, type=int)
     parser.add_argument("--target-hosts", "--target", default=None, help="Target hosts IP:Port")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
     if args.database:
-        args.db = db_utils.connect(args)
         log.error("Currently only stdin is supported")
         raise NotImplementedError
 
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def list_tabs(args) -> list:
     return args.bt_api.list_tabs([])
```

### Comparing `xklb-2.7.9/xklb/scratch/javguru.py` & `xklb-2.8.1/xklb/scratch/javguru.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import argparse, time
+import time
 from pathlib import Path
 from urllib.parse import urljoin
 
 from xklb.mediafiles import media_check
-from xklb.utils import arggroups, file_utils, path_utils, processes, web
+from xklb.utils import arggroups, argparse_utils, file_utils, path_utils, processes, web
 
 
 def jav_guru() -> None:
-    parser = argparse.ArgumentParser()
+    parser = argparse_utils.ArgumentParser()
     parser.add_argument("--chrome", action="store_true")
     parser.add_argument("--small", action="store_true")
     arggroups.debug(parser)
 
     parser.add_argument("path", help="JAV.GURU URL")
     args = parser.parse_args()
```

### Comparing `xklb-2.7.9/xklb/scratch/javtiful.py` & `xklb-2.8.1/xklb/scratch/javtiful.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import argparse, time
+import time
 from pathlib import Path
 
 from xklb.mediafiles import media_check
-from xklb.utils import arggroups, file_utils, path_utils, processes, web
+from xklb.utils import arggroups, argparse_utils, file_utils, path_utils, processes, web
 
 
 def javtiful() -> None:
-    parser = argparse.ArgumentParser()
+    parser = argparse_utils.ArgumentParser()
     parser.add_argument("--chrome", action="store_true")
     arggroups.debug(parser)
 
     parser.add_argument("path")
     args = parser.parse_args()
 
     from selenium.webdriver.common.by import By
```

### Comparing `xklb-2.7.9/xklb/scratch/mam_search.py` & `xklb-2.8.1/xklb/scratch/mam_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import argparse, json, time
-from pathlib import Path
 from sqlite3 import IntegrityError
 
-from xklb.utils import arggroups, db_utils, nums, objects, web
+from xklb.utils import arggroups, argparse_utils, nums, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser()
+    parser = argparse_utils.ArgumentParser()
     parser.add_argument("--base-url", default="https://www.myanonamouse.net")
-    parser.add_argument("--no-title", action="store_false")
-    parser.add_argument("--no-author", action="store_false")
-    parser.add_argument("--narrator", action="store_true")
-    parser.add_argument("--series", action="store_true")
-    parser.add_argument("--description", action="store_true")
-
-    parser.add_argument("--books", action="store_true")
-    parser.add_argument("--audiobooks", action="store_true")
-    parser.add_argument("--comics", action="store_true")
-    parser.add_argument("--cookbooks", action="store_true")
-    parser.add_argument("--musicology", action="store_true")
-    parser.add_argument("--radio", action="store_true")
+    parser.add_argument("--title", action=argparse.BooleanOptionalAction, default=True)
+    parser.add_argument("--author", action=argparse.BooleanOptionalAction, default=True)
+    parser.add_argument("--narrator", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--series", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--description", action=argparse.BooleanOptionalAction, default=False)
+
+    parser.add_argument("--books", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--audiobooks", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--comics", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--cookbooks", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--musicology", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--radio", action=argparse.BooleanOptionalAction, default=False)
 
     parser.add_argument("--search-in", default="torrents")
 
+    parser.add_argument("--force", action="store_true")
     parser.add_argument("--cookie", required=True)
     arggroups.requests(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search_text", nargs="+")
     args = parser.parse_intermixed_args()
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def get_page(args, query_data):
     import pandas as pd
 
     response = web.requests_session(args).post(
@@ -79,27 +77,28 @@
 
 def save_to_db(args, data):
     for d in data:
         try:
             args.db["media"].insert(objects.dict_filter_bool(d), pk="id", alter=True)
         except IntegrityError:
             log.error("Reached existing id")
-            raise SystemExit(0)
+            if not args.force:
+                raise SystemExit(0)
 
 
 def mam_search():
     args = parse_args()
 
     query_data = {
         "tor": {
             "text": " ".join(args.search_text),
             "browse_lang": [1, 44],
             "srchIn": {
-                "title": args.no_title,
-                "author": args.no_author,
+                "title": args.title,
+                "author": args.author,
                 "narrator": args.narrator,
                 "series": args.series,
                 "description": args.description,
             },
             "searchType": "all",  # fl-VIP, fl, VIP, all
             "searchIn": args.search_in,
             "browseFlagsHideVsShow": 0,
```

### Comparing `xklb-2.7.9/xklb/tablefiles/eda.py` & `xklb-2.8.1/xklb/tablefiles/eda.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-import argparse
-
 from xklb import usage
-from xklb.utils import arggroups, file_utils, nums, web
+from xklb.utils import arggroups, argparse_utils, file_utils, nums, web
 from xklb.utils.consts import DEFAULT_FILE_ROWS_READ_LIMIT
 from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df, print_series
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="Perform EDA on one or more files", usage=usage.eda)
-    parser.add_argument("--print", "-p", default="p", const="p", nargs="?", help=argparse.SUPPRESS)
+    parser = argparse_utils.ArgumentParser(description="Perform EDA on one or more files", usage=usage.eda)
 
     parser.add_argument("--groupby", "--group-by", "-g", action="store_true")
     arggroups.table_like(parser)
 
     parser.add_argument("--sort", "-u", default="random()")
     parser.add_argument("--repl", "-r", action="store_true")
     arggroups.debug(parser)
@@ -21,19 +18,17 @@
     parser.add_argument(
         "paths",
         metavar="path",
         nargs="+",
         help="path to one or more files",
     )
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    if args.end_row.lower() in ("inf", "none", "all"):
-        args.end_row = None
-    else:
-        args.end_row = int(args.end_row)
+    arggroups.table_like_post(args)
 
     return args
 
 
 def df_column_values(df, column_name) -> dict:
     total = len(df)
```

### Comparing `xklb-2.7.9/xklb/tablefiles/incremental_diff.py` & `xklb-2.8.1/xklb/tablefiles/incremental_diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-import argparse
-
 from xklb import usage
-from xklb.utils import arggroups, consts, file_utils, web
+from xklb.utils import arggroups, argparse_utils, consts, file_utils, web
 from xklb.utils.argparse_utils import ArgparseList
 from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="Diff two table-like files", usage=usage.incremental_diff)
-    parser.add_argument("--print", "-p", default="p", const="p", nargs="?", help=argparse.SUPPRESS)
+    parser = argparse_utils.ArgumentParser(description="Diff two table-like files", usage=usage.incremental_diff)
     parser.add_argument("--mimetype1", "--filetype1")
     parser.add_argument("--encoding1")
     parser.add_argument("--mimetype2", "--filetype2")
     parser.add_argument("--encoding2")
     parser.add_argument("--table1-name", "--table1", "-t1")
     parser.add_argument("--table2-name", "--table2", "-t2")
     parser.add_argument("--table1-index", type=int)
@@ -23,14 +20,15 @@
     parser.add_argument("--join-keys", action=ArgparseList, help="Comma separated join keys")
     parser.add_argument("--sort", "-u")
     arggroups.debug(parser)
 
     parser.add_argument("path1", help="path to dataset 1")
     parser.add_argument("path2", help="path to dataset 2")
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser)
 
     # TODO: add an option to load from df2 where ids (select ids from df1)
 
     if args.batch_size.lower() in ("inf", "none", "all"):
         args.batch_size = None
     else:
         args.batch_size = int(args.batch_size)
```

### Comparing `xklb-2.7.9/xklb/tablefiles/mcda.py` & `xklb-2.8.1/xklb/tablefiles/mcda.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import argparse
 from pathlib import Path
 
 from xklb import usage
 from xklb.utils import arggroups, argparse_utils, file_utils, iterables, objects, pd_utils, sql_utils, web
 from xklb.utils.consts import DEFAULT_FILE_ROWS_READ_LIMIT
-from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df, print_series
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="Perform MCDA on one or more files", usage=usage.mcda)
+    parser = argparse_utils.ArgumentParser(description="Perform MCDA on one or more files", usage=usage.mcda)
     arggroups.table_like(parser)
     parser.add_argument(
         "--minimize-columns",
         "--minimize-cols",
         "--minimize",
         "--min",
         nargs="*",
@@ -27,16 +25,14 @@
         nargs="*",
         action=argparse_utils.ArgparseList,
         default=[],
     )
     parser.add_argument(
         "--columns-include",
         "--include-columns",
-        "--columns",
-        "--cols",
         nargs="*",
         action=argparse_utils.ArgparseList,
         default=[],
     )
     parser.add_argument("--words-nums-map")
     parser.add_argument("--mcda-method")
     parser.add_argument("--nodata", type=int, default=0)
@@ -47,24 +43,21 @@
     parser.add_argument(
         "paths",
         metavar="path",
         nargs="+",
         help="path to one or more files",
     )
     args = parser.parse_args()
-
-    if args.end_row.lower() in ("inf", "none", "all"):
-        args.end_row = None
-    else:
-        args.end_row = int(args.end_row)
+    arggroups.args_post(args, parser)
 
     if args.words_nums_map:
         Path(args.words_nums_map).touch()
 
-    log.info(objects.dict_filter_bool(args.__dict__))
+    arggroups.table_like_post(args)
+
     return args
 
 
 def words_to_numbers(args, words):
     default = {
         "high": 5,
         "above average": 4,
@@ -145,28 +138,28 @@
 
     df = auto_mcda(args, df, alternatives, minimize_cols={s.lstrip("-") for s in columns if s.startswith("-")})
     return df
 
 
 def group_sort_by(args, folders):
     if args.sort_groups_by is None:
-        sort_func = lambda x: x["size"] / x["exists"]
+        sort_func = lambda x: (0, x["size"] / x["exists"]) if x["exists"] else (1, x["size"] / x["total"])
     elif args.sort_groups_by.startswith("mcda "):
         import pandas as pd
 
         if not isinstance(folders, pd.DataFrame):
             folders = pd.DataFrame(folders)
         values = args.sort_groups_by.replace("mcda ", "", 1)
         df = sort(args, folders, values)
         return df.drop(columns=["TOPSIS", "MABAC", "SPOTIS", "BORDA"]).to_dict(orient="records")
     else:
         if args.sort_groups_by == "played_ratio":
-            sort_func = lambda x: x["played"] / x["deleted"] if x["deleted"] else 0
+            sort_func = lambda x: (0, x["played"] / x["deleted"]) if x["deleted"] else (1, x["played"] / x["total"])
         elif args.sort_groups_by == "deleted_ratio":
-            sort_func = lambda x: x["deleted"] / x["played"] if x["played"] else 0
+            sort_func = lambda x: (0, x["deleted"] / x["played"]) if x["played"] else (1, x["deleted"] / x["total"])
         else:
             sort_func = sql_utils.sort_like_sql(args.sort_groups_by)
 
     return sorted(folders, key=sort_func)
 
 
 def print_info(args, df):
```

### Comparing `xklb-2.7.9/xklb/text/cluster_sort.py` & `xklb-2.8.1/xklb/text/cluster_sort.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,77 +1,79 @@
-import argparse, difflib, json, os.path, sys
+import argparse, difflib, json, sys
 from pathlib import Path
 
 from xklb import usage
-from xklb.data import wordbank
 from xklb.tablefiles import eda, mcda
-from xklb.utils import arggroups, consts, db_utils, file_utils, iterables, nums, objects, path_utils, printing, strings
+from xklb.utils import (
+    arggroups,
+    argparse_utils,
+    consts,
+    db_utils,
+    file_utils,
+    iterables,
+    nums,
+    objects,
+    path_utils,
+    printing,
+    strings,
+)
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import Timer, log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
+    parser = argparse_utils.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
 
     profile = parser.add_mutually_exclusive_group()
     profile.add_argument(
         "--lines",
         action="store_const",
         dest="profile",
         const="lines",
         help="Cluster lines AS-IS",
     )
     profile.add_argument(
         "--image",
-        "-I",
         action="store_const",
         dest="profile",
         const=DBType.image,
         help="Read image data",
     )
     profile.add_argument(
         "--audio",
-        "-A",
         action="store_const",
         dest="profile",
         const=DBType.audio,
         help="Read audio data",
     )
     profile.add_argument(
         "--video",
-        "-V",
         action="store_const",
         dest="profile",
         const=DBType.video,
         help="Read video data",
     )
     profile.add_argument(
         "--text",
-        "-T",
         action="store_const",
         dest="profile",
         const=DBType.text,
         help="Read text data",
     )
     parser.set_defaults(profile="lines")
 
-    arggroups.operation_cluster(parser)
+    arggroups.cluster(parser)
     parser.set_defaults(cluster_sort=True)
     arggroups.debug(parser)
 
     parser.add_argument("input_path", nargs="?", type=argparse.FileType("r"), default=sys.stdin)
     parser.add_argument("output_path", nargs="?")
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    if args.stop_words is None:
-        args.stop_words = wordbank.stop_words
-    else:
-        args.stop_words = frozenset(*args.stop_words)
-
-    log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def map_cluster_to_paths(paths, clusters):
     grouped_strings = {}
     for i, group_string in enumerate(paths):
         cluster_id = clusters[i]
@@ -94,14 +96,19 @@
     return result
 
 
 def find_clusters(n_clusters, sentence_strings, stop_words=None):
     from sklearn.cluster import KMeans
     from sklearn.feature_extraction.text import TfidfVectorizer
 
+    if stop_words is None:
+        from xklb.data import wordbank
+
+        stop_words = wordbank.stop_words
+
     try:
         vectorizer = TfidfVectorizer(min_df=2, strip_accents="unicode", stop_words=stop_words)
         X = vectorizer.fit_transform(sentence_strings)
     except ValueError:
         try:
             vectorizer = TfidfVectorizer(strip_accents="unicode", stop_words=stop_words)
             X = vectorizer.fit_transform(sentence_strings)
@@ -115,15 +122,15 @@
 
     clusterizer = KMeans(n_clusters=n_clusters or int(X.shape[0] ** 0.5), random_state=0, n_init=10).fit(X)
     clusters = clusterizer.labels_
     return clusters
 
 
 def cluster_paths(paths, n_clusters=None, stop_words=None):
-    if len(paths) < 2:
+    if len(paths) < 3:
         return paths
 
     sentence_strings = (strings.path_to_sentence(s) for s in paths)
     clusters = find_clusters(n_clusters, sentence_strings, stop_words=stop_words)
     result = map_and_name(paths, clusters)
 
     return result
@@ -134,15 +141,15 @@
         group["grouped_paths"] = [s.rstrip("\n") for s in group["grouped_paths"]]
 
     print(json.dumps(groups, indent=4))
     raise SystemExit(0)
 
 
 def cluster_dicts(args, media):
-    if len(media) < 2:
+    if len(media) < 3:
         return media
 
     n_clusters = getattr(args, "clusters", None)
     search_columns = {
         col
         for _table, table_config in db_utils.config.items()
         if "search_columns" in table_config
@@ -161,15 +168,15 @@
         from pandas import DataFrame
 
         eda.print_info(objects.NoneSpace(end_row="inf"), DataFrame(clusters))
 
     groups = map_and_name(paths, clusters)
     groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_path"])))
 
-    if getattr(args, "sort_groups_by", None) is not None:
+    if getattr(args, "sort_groups_by", None):
         if args.sort_groups_by in ("duration", "duration desc"):
             sorted_paths = iterables.flatten(
                 sorted(d["grouped_paths"], key=lambda p: media_keyed[p]["duration"], reverse=" desc" in args.sort)
                 for d in groups
             )
         else:
             groups = [
```

### Comparing `xklb-2.7.9/xklb/text/extract_links.py` & `xklb-2.8.1/xklb/text/extract_links.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import argparse
-
 from xklb import usage
-from xklb.utils import arg_utils, arggroups, consts, devices, iterables, printing, strings, web
+from xklb.utils import arg_utils, arggroups, argparse_utils, consts, devices, iterables, printing, strings, web
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(
+    parser = argparse_utils.ArgumentParser(
         prog="library extract-links",
         usage=usage.extract_links,
     )
     arggroups.extractor(parser)
     arggroups.requests(parser)
     arggroups.selenium(parser)
     arggroups.filter_links(parser)
@@ -18,31 +16,19 @@
     parser.add_argument("--print-link-text", "--print-title", action="store_true")
     parser.add_argument("--download", action="store_true", help="Download filtered links")
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
 
     arggroups.debug(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    if args.scroll:
-        args.selenium = True
-
-    if not args.case_sensitive:
-        args.before_include = [s.lower() for s in args.before_include]
-        args.path_include = [s.lower() for s in args.path_include]
-        args.text_include = [s.lower() for s in args.text_include]
-        args.after_include = [s.lower() for s in args.after_include]
-        args.before_exclude = [s.lower() for s in args.before_exclude]
-        args.path_exclude = [s.lower() for s in args.path_exclude]
-        args.text_exclude = [s.lower() for s in args.text_exclude]
-        args.after_exclude = [s.lower() for s in args.after_exclude]
-
-    if not args.no_url_decode:
-        args.path_include = [web.url_decode(s) for s in args.path_include]
-        args.path_exclude = [web.url_decode(s) for s in args.path_exclude]
+    arggroups.extractor_post(args)
+    arggroups.filter_links_post(args)
+    arggroups.selenium_post(args)
 
     return args
 
 
 def is_desired_url(args, a_element, link, link_text) -> bool:
     include_cond = all if args.strict_include else any
     exclude_cond = all if args.strict_exclude else any
@@ -122,15 +108,15 @@
             while devices.confirm("Extract HTML from browser?"):
                 markup = web.selenium_extract_html(args.driver)
                 yield from parse_inner_urls(args, url, markup)
         else:
             for markup in web.infinite_scroll(args.driver):
                 yield from parse_inner_urls(args, url, markup)
     else:
-        if args.local_file:
+        if args.local_html:
             with open(url) as f:
                 markup = f.read()
             url = "file://" + url
         else:
             r = web.requests_session(args).get(url, timeout=120)
             if r.status_code == 404:
                 log.warning("404 Not Found Error: %s", url)
```

### Comparing `xklb-2.7.9/xklb/text/extract_text.py` & `xklb-2.8.1/xklb/text/extract_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import argparse, re
+import re
 from pathlib import Path
 
 from bs4 import BeautifulSoup, NavigableString
 
 from xklb import usage
-from xklb.utils import arg_utils, arggroups, devices, iterables, printing, strings, web
+from xklb.utils import arg_utils, arggroups, argparse_utils, devices, iterables, printing, strings, web
 from xklb.utils.log_utils import log
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(prog="library extract-text", usage=usage.extract_text)
+    parser = argparse_utils.ArgumentParser(prog="library extract-text", usage=usage.extract_text)
     arggroups.requests(parser)
     arggroups.selenium(parser)
 
     parser.add_argument("--skip-links", action="store_true")
     parser.add_argument("--download", "--save", "--write", action="store_true")
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
 
     arggroups.debug(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
-    if args.scroll:
-        args.selenium = True
+    arggroups.selenium_post(args)
 
     return args
 
 
 def un_paragraph(item):
     s = strings.remove_consecutive_whitespace(item.get_text(strip=True))
     s = re.sub(r"[“”‘’]", "'", s)
@@ -62,15 +62,15 @@
             while devices.confirm("Extract HTML from browser?"):
                 markup = web.selenium_extract_html(args.driver)
                 yield from parse_text(args, markup)
         else:
             for markup in web.infinite_scroll(args.driver):
                 yield from parse_text(args, markup)
     else:
-        if args.local_file:
+        if args.local_html:
             with open(url) as f:
                 markup = f.read()
             url = "file://" + url
         else:
             r = web.requests_session(args).get(url, timeout=120)
             if r.status_code == 404:
                 log.warning("404 Not Found Error: %s", url)
```

### Comparing `xklb-2.7.9/xklb/text/markdown_links.py` & `xklb-2.8.1/xklb/text/markdown_links.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,33 @@
-import argparse, urllib.parse
+import urllib.parse
 
 from xklb import usage
-from xklb.utils import arg_utils, arggroups, web
+from xklb.utils import arg_utils, arggroups, argparse_utils, web
 
 COMMON_SITE_TITLE_SUFFIXES = [
     " | Listen online for free on SoundCloud",
     " - YouTube",
 ]
 
 
+def parse_args():
+    parser = argparse_utils.ArgumentParser(usage=usage.markdown_links)
+    arggroups.requests(parser)
+    arggroups.selenium(parser)
+    arggroups.debug(parser)
+
+    arggroups.paths_or_stdin(parser)
+    args = parser.parse_args()
+    arggroups.args_post(args, parser)
+
+    arggroups.selenium_post(args)
+
+    return args
+
+
 def fake_title(url):
     p = urllib.parse.urlparse(url)
     title = f"{p.netloc} {p.path} {p.params} {p.query}: {p.fragment}"
 
     if title.startswith("www."):
         title = title[4:]
 
@@ -20,21 +35,15 @@
     title = title.replace("?", " ")
     title = title.replace("#", ": ")
 
     return title.strip()
 
 
 def markdown_links():
-    parser = argparse.ArgumentParser(usage=usage.markdown_links)
-    arggroups.requests(parser)
-    arggroups.selenium(parser)
-    arggroups.debug(parser)
-
-    arggroups.paths_or_stdin(parser)
-    args = parser.parse_args()
+    args = parse_args()
 
     import requests
     from bs4 import BeautifulSoup
 
     if args.selenium:
         web.load_selenium(args)
     try:
```

### Comparing `xklb-2.7.9/xklb/text/nouns.py` & `xklb-2.8.1/xklb/text/nouns.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import argparse, sys
+import sys
 from html.parser import HTMLParser
 from io import StringIO
 
 from xklb import usage
 from xklb.data import wordbank
-from xklb.utils import arggroups, printing
+from xklb.utils import arggroups, argparse_utils, printing
 
 
 class MLStripper(HTMLParser):
     def __init__(self) -> None:
         super().__init__()
         self.reset()
         self.strict = False
@@ -56,14 +56,15 @@
         )
 
     parts = line_processor.RE_NOUNS_SPLIT.split(txt)
     printer(parts)
 
 
 def nouns() -> None:
-    parser = argparse.ArgumentParser(usage.nouns)
+    parser = argparse_utils.ArgumentParser(usage.nouns)
     arggroups.debug(parser)
     args = parser.parse_args()
+    arggroups.args_post(args, parser)
 
     print("library nouns: Reading from stdin...", file=sys.stderr)
     for line in sys.stdin:
         line_processor(line)
```

### Comparing `xklb-2.7.9/xklb/utils/arg_utils.py` & `xklb-2.8.1/xklb/utils/arg_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,120 +1,89 @@
-import argparse, operator, random, sqlite3
+import argparse, json, operator, random
 from pathlib import Path
 
-from xklb.utils import arggroups, consts, db_utils, file_utils, iterables
+from xklb.utils import consts, file_utils, iterables
 from xklb.utils.consts import SC
 
 
-def is_sqlite(path):
-    try:
-        with open(path, "rb") as f:
-            header = f.read(16)
-        return header == b"SQLite format 3\000"
-    except OSError:
-        return False
-
-
 def gen_paths(args):
-    if args.paths_from_text:
+    if args.from_file:
         for path in args.paths:
-            with open(path) as f:
+            with open(path, "r") as f:
                 for line in f:
                     line = line.rstrip("\n")
                     if line.strip():
-                        yield line
-    elif args.paths_from_dbs or args.titles_from_dbs:
-        for path in args.paths:
-            if is_sqlite(path):
-                s_db = db_utils.connect(args, conn=sqlite3.connect(path))
-                m_columns = s_db["media"].columns_dict
-                yield from (
-                    d["path"]
-                    for d in s_db.query(
-                        f"""
-                    SELECT
-                        {'title AS path' if args.titles_from_dbs else 'path'}
-                    FROM media
-                    WHERE 1=1
-                    {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
-                    """
-                    )
-                )
+                        if args.from_json:
+                            json_data = json.loads(line)
+                            if isinstance(json_data, list):
+                                yield from (d["path"] for d in json_data)
+                            elif isinstance(json_data, dict):
+                                yield json_data["path"]
+                            else:
+                                raise TypeError
+                        else:
+                            yield line
+    elif args.from_json:
+        for path in args.paths:
+            json_data = json.loads(path)
+            if isinstance(json_data, list):
+                yield from (d["path"] for d in json_data)
+            elif isinstance(json_data, dict):
+                yield json_data["path"]
             else:
-                print("Skipping non-SQLite file:", path)
+                raise TypeError
     else:
         is_large = len(args.paths) > 1000
         for path in args.paths:
             if path.strip():
                 if is_large:
                     yield path
                 else:
                     p = Path(path)
                     if p.is_dir():
                         yield from file_utils.rglob(str(p), args.ext or None)[0]
                     else:
                         yield path
 
 
-def d_from_path(path):
-    try:
-        stat = Path(path).stat()
-        return {"path": str(path), "size": stat.st_size}
-    except FileNotFoundError:
-        print("Skipping non-existent file:", path)
-
-
 def gen_d(args):
-    if args.paths_from_text:
+    if args.from_file:
         for path in args.paths:
             with open(path) as f:
                 for line in f:
                     line = line.rstrip("\n")
                     if line.strip():
-                        d = d_from_path(line)
-                        if d:
-                            yield d
-    elif args.paths_from_dbs or args.titles_from_dbs:
-        for path in args.paths:
-            if is_sqlite(path):
-                s_db = db_utils.connect(args, conn=sqlite3.connect(path))
-                m_columns = s_db["media"].columns_dict
-                yield from s_db.query(
-                    f"""
-                    SELECT
-                        path
-                        {', size' if 'size' in m_columns else ''}
-                        {', title' if 'title' in m_columns else ''}
-                    FROM media
-                    WHERE 1=1
-                    {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
-                    """
-                )
+                        if args.from_json:
+                            json_data = json.loads(line)
+                            if isinstance(json_data, list):
+                                yield from json_data
+                            elif isinstance(json_data, dict):
+                                yield json_data
+                            else:
+                                raise TypeError
+                        else:
+                            yield {"path": line}
+    elif args.from_json:
+        for path in args.paths:
+            json_data = json.loads(path)
+            if isinstance(json_data, list):
+                yield from json_data
+            elif isinstance(json_data, dict):
+                yield json_data
             else:
-                print("Skipping non-SQLite file:", path)
+                raise TypeError
     else:
         for path in args.paths:
             if path.strip():
                 p = Path(path)
                 if p.is_dir():
                     for sp in file_utils.rglob(str(p), args.ext or None)[0]:
-                        d = d_from_path(sp)
-                        if d:
-                            yield d
+                        yield {"path": sp}
                 else:
-                    d = d_from_path(p)
-                    if d:
-                        yield d
-
-
-def stdarg():
-    parser = argparse.ArgumentParser()
-    arggroups.paths_or_stdin(parser)
-    args = parser.parse_args()
-    return gen_paths(args)
+                    yield {"path": path}
 
 
 def override_sort(sort_expression: str) -> str:
     def year_month_sql(var):
         return f"cast(strftime('%Y%m', datetime({var}, 'unixepoch')) as int)"
 
     def year_month_day_sql(var):
@@ -138,86 +107,77 @@
         if s.strip() in ["asc", "desc"] and combined_sort:
             combined_sort[-1] += " " + s.strip()
         else:
             combined_sort.append(s.strip())
     return combined_sort
 
 
-def parse_args_sort(args) -> None:
+def parse_args_sort(args, columns, table_prefix="m.") -> tuple[str, list[str]]:
+    sort_list = []
+    select_list = []
     if args.sort:
         combined_sort = parse_ambiguous_sort(args.sort)
 
-        sort_list = []
-        select_list = []
         for s in combined_sort:
             if s.startswith("same-"):
                 var = s[len("same-") :]
                 direction = "DESC"
                 if var.lower().endswith((" asc", " desc")):
                     var, direction = var.split(" ")
 
                 select_list.append(
                     f"CASE WHEN {var} IS NULL THEN NULL ELSE COUNT(*) OVER (PARTITION BY {var}) END AS same_{var}_count",
                 )
                 sort_list.append(f"same_{var}_count {direction}")
             else:
                 sort_list.append(s)
 
-        args.sort = sort_list
-        args.select = select_list
-    elif not args.sort and hasattr(args, "defaults"):
-        args.defaults.append("sort")
-
-    m_columns = db_utils.columns(args, "media")
-
     # switching between videos with and without subs is annoying
     subtitle_count = "=0"
     if random.random() < getattr(args, "subtitle_mix", consts.DEFAULT_SUBTITLE_MIX):
         # bias slightly toward videos without subtitles
         subtitle_count = ">0"
 
     sorts = [
         "random" if getattr(args, "random", False) else None,
-        "rank" if args.sort and "rank" in args.sort else None,
-        "video_count > 0 desc" if "video_count" in m_columns and args.action == SC.watch else None,
-        "audio_count > 0 desc" if "audio_count" in m_columns else None,
-        'm.path like "http%"',
-        "width < height desc" if "width" in m_columns and getattr(args, "portrait", False) else None,
+        "rank" if sort_list and "rank" in sort_list else None,
+        "video_count > 0 desc" if "video_count" in columns and args.action == SC.watch else None,
+        "audio_count > 0 desc" if "audio_count" in columns else None,
+        table_prefix + 'path like "http%"',
+        "width < height desc" if "width" in columns and getattr(args, "portrait", False) else None,
         (
             f"subtitle_count {subtitle_count} desc"
-            if "subtitle_count" in m_columns
+            if "subtitle_count" in columns
             and args.action == SC.watch
             and not any(
                 [
                     args.print,
                     consts.PYTEST_RUNNING,
                     "subtitle_count" in " ".join(args.where),
                     args.limit != consts.DEFAULT_PLAY_QUEUE,
                 ],
             )
             else None
         ),
-        *(args.sort or []),
+        *(sort_list or []),
         "duration desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "size desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "play_count" if args.action in (SC.listen, SC.watch) else None,
-        "m.title IS NOT NULL desc" if "title" in m_columns else None,
-        "m.path",
-        "random",
+        table_prefix + "title IS NOT NULL desc" if "title" in columns else None,
+        table_prefix + "path",
     ]
 
     sort = list(filter(bool, sorts))
     sort = [override_sort(s) for s in sort]
-    sort = "\n        , ".join(sort)
-    args.sort = sort.replace(",,", ",")
+    sort = ",".join(sort)
+    return sort.replace(",,", ","), select_list
 
 
 def parse_args_limit(args):
     if not args.limit:
-        args.defaults.append("limit")
         if not any(
             [
                 args.print and len(args.print.replace("p", "")) > 0,
                 getattr(args, "partial", False),
                 getattr(args, "lower", False),
                 getattr(args, "upper", False),
             ],
@@ -228,31 +188,35 @@
                 args.limit = consts.DEFAULT_PLAY_QUEUE * 4
             elif args.action in (SC.links_open):
                 args.limit = consts.MANY_LINKS - 1
             elif args.action in (SC.download):
                 args.limit = consts.DEFAULT_PLAY_QUEUE * 60
     elif args.limit.lower() in ("inf", "all"):
         args.limit = None
+    else:
+        args.limit = int(args.limit)
 
 
 def split_folder_glob(s):
     p = Path(s).resolve()
 
     if "*" not in s and not p.exists():
         p.mkdir(parents=True, exist_ok=True)
 
     if p.is_dir():
         return p, "*"
     return p.parent, p.name
 
 
-def override_config(parser, extractor_config, args):
-    default_args = {key: parser.get_default(key) for key in vars(args)}
-    overridden_args = {k: v for k, v in args.__dict__.items() if default_args.get(k) != v}
-    args_env = argparse.Namespace(**{**default_args, **extractor_config, **overridden_args})
+def override_config(args, extractor_config):
+    defaults = args.get("defaults")
+    overridden_args = {k: v for k, v in args.__dict__.items() if defaults.get(k) != v}
+    args_env = argparse.Namespace(
+        **{**defaults, **(extractor_config.get("extractor_config") or {}), **extractor_config, **overridden_args}
+    )
     return args_env
 
 
 def kwargs_overwrite(namespace, kwargs):
     namespace_dict = vars(namespace)
     namespace_dict.update(kwargs)
     return argparse.Namespace(**namespace_dict)
```

### Comparing `xklb-2.7.9/xklb/utils/consts.py` & `xklb-2.8.1/xklb/utils/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,30 +98,41 @@
     filesystem = "filesystem"
     tube_add = "tube-add"
     tube_update = "tube-update"
     gallery_add = "gallery-add"
     gallery_update = "gallery-update"
     tabs_open = "tabs-open"
     links_open = "links-open"
+    links_add = "links-add"
+    links_update = "links-update"
     read = "read"
     view = "view"
     download = "download"
     block = "block"
     stats = "stats"
     playlists = "playlists"
     download_status = "download-status"
     search = "search"
     history = "history"
     big_dirs = "big-dirs"
+    similar_folders = "similar-folders"
+    similar_files = "similar-files"
     disk_usage = "disk-usage"
     dedupe_media = "dedupe"
     web_add = "web-add"
     web_update = "web-update"
 
 
+class DLStatus:
+    SUCCESS = "SUCCESS"
+    RECOVERABLE_ERROR = "RECOVERABLE_ERROR"
+    UNRECOVERABLE_ERROR = "UNRECOVERABLE_ERROR"
+    UNKNOWN_ERROR = "UNKNOWN_ERROR"
+
+
 def reddit_frequency(frequency) -> str:
     mapper = {
         "daily": "day",
         "weekly": "week",
         "monthly": "month",
         "quarterly": "year",
         "yearly": "year",
```

### Comparing `xklb-2.7.9/xklb/utils/db_utils.py` & `xklb-2.8.1/xklb/utils/db_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -78,19 +78,20 @@
         return args.db[table_name].columns_dict
     except Exception:
         return {}
 
 
 config = {
     "playlists": {
+        "search_columns": ["path", "title"],
         "column_order": ["id", "path", "extractor_key"],
         "ignore_columns": ["extractor_playlist_id"],
     },
     "media": {
-        "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album"],
+        "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album", "category", "frequency"],
         "column_order": ["id", "path", "webpath", "extractor_id"],
         "ignore_columns": ["extractor_id"],
     },
     "history": {"column_order": ["id"]},
     "captions": {"search_columns": ["text"]},
     "reddit_posts": {
         "search_columns": ["title", "selftext"],
@@ -114,25 +115,22 @@
     "hn_story": {
         "search_columns": ["title", "text", "author", "path"],
     },
 }
 
 
 def optimize(args) -> None:
-    if not hasattr(args, "force"):
-        args.force = False
-
     log.info("\nOptimizing database")
 
     db: Database = args.db
 
     for table in config:
         if table not in db.table_names():
             continue
-        if args.force:
+        if getattr(args, "force", False):
             try:
                 db[table].disable_fts()  # type: ignore
             except Exception as e:
                 log.debug(e)
 
         log.info("Processing table: %s", table)
         table_columns = db[table].columns_dict
@@ -150,15 +148,15 @@
         compare_order = zip(table_columns, optimized_column_order)
         was_transformed = False
         if not all(x == y for x, y in compare_order):
             log.info("Transforming column order: %s", optimized_column_order)
             db[table].transform(column_order=optimized_column_order)  # type: ignore
             was_transformed = True
 
-        if args.force:
+        if getattr(args, "force", False):
             indexes = db[table].indexes  # type: ignore
             for index in indexes:
                 if index.unique == 1:
                     db.execute(f"REINDEX {index.name}")
                 else:
                     db.execute(f"DROP index {index.name}")
 
@@ -188,68 +186,14 @@
 
     log.info("Running VACUUM")
     db.vacuum()
     log.info("Running ANALYZE")
     db.analyze()
 
 
-def fts_quote(query: list[str]) -> list[str]:
-    fts_words = [" NOT ", " AND ", " OR ", "*", ":", "NEAR("]
-    return [s if any(r in s for r in fts_words) else '"' + s + '"' for s in query]
-
-
-def fts_search_sql(table, fts_table, include, exclude=None, flexible=False):
-    param_key = "FTS" + consts.random_string()
-    table = f"""(
-    with original as (select rowid, * from [{table}])
-    select
-        [original].*
-        , [{fts_table}].rank
-    from
-        [original]
-        join [{fts_table}] on [original].rowid = [{fts_table}].rowid
-    where
-        [{fts_table}] match :{param_key}
-    )
-    """
-    if flexible:
-        param_value = " OR ".join(fts_quote(include))
-    else:
-        param_value = " AND ".join(fts_quote(include))
-    if exclude:
-        param_value += " NOT " + " NOT ".join(fts_quote(exclude))
-
-    bound_parameters = {param_key: param_value}
-    return table, bound_parameters
-
-
-def construct_search_bindings(args, columns) -> None:
-    incl = ":include{0}"
-    includes = "(" + " OR ".join([f"{col} LIKE {incl}" for col in columns]) + ")"
-    includes_sql_parts = []
-    for idx, inc in enumerate(args.include):
-        includes_sql_parts.append(includes.format(idx))
-        if getattr(args, "exact", False):
-            args.filter_bindings[f"include{idx}"] = inc
-        else:
-            args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
-    join_op = " OR " if getattr(args, "flexible_search", False) else " AND "
-    if len(includes_sql_parts) > 0:
-        args.filter_sql.append("AND (" + join_op.join(includes_sql_parts) + ")")
-
-    excl = ":exclude{0}"
-    excludes = "AND (" + " AND ".join([f"COALESCE({col},'') NOT LIKE {excl}" for col in columns]) + ")"
-    for idx, exc in enumerate(args.exclude):
-        args.filter_sql.append(excludes.format(idx))
-        if getattr(args, "exact", False):
-            args.filter_bindings[f"exclude{idx}"] = exc
-        else:
-            args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
-
-
 def linear_interpolation(x, x1, y1, x2, y2):
     y = y1 + ((x - x1) / (x2 - x1)) * (y2 - y1)
     return y
 
 
 def has_similar_schema(set1, set2):
     len1 = len(set1)
```

### Comparing `xklb-2.7.9/xklb/utils/devices.py` & `xklb-2.8.1/xklb/utils/devices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os, platform, random, shutil, sys
 
+from xklb.utils import arggroups, argparse_utils
+from xklb.utils.arg_utils import gen_paths
 from xklb.utils.log_utils import log
 
 
 def get_ip_of_chromecast(device_name) -> str:
     from pychromecast import discovery
 
     cast_infos, browser = discovery.discover_listed_chromecasts(friendly_names=[device_name])
@@ -86,15 +88,15 @@
 
     readline.set_completer(create_completer(list_))
     readline.set_completer_delims("\t")
     readline.parse_and_bind("tab: complete")
     return
 
 
-def get_mount_stats(src_mounts) -> list[dict[str, str | int]]:
+def get_mount_stats(src_mounts) -> list[dict[str, int | float]]:
     mount_space = []
     total_used = 1
     total_free = 1
     grand_total = 1
     for src_mount in src_mounts:
         total, used, free = shutil.disk_usage(src_mount)
         total_used += used
@@ -102,7 +104,14 @@
         grand_total += total
         mount_space.append((src_mount, used, free, total))
 
     return [
         {"mount": mount, "used": used / total_used, "free": free / total_free, "total": total / grand_total}
         for mount, used, free, total in mount_space
     ]
+
+
+def stdarg():
+    parser = argparse_utils.ArgumentParser()
+    arggroups.paths_or_stdin(parser)
+    args = parser.parse_args()
+    return gen_paths(args)
```

### Comparing `xklb-2.7.9/xklb/utils/file_utils.py` & `xklb-2.8.1/xklb/utils/file_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import errno, mimetypes, os, shlex, shutil, tempfile, time
 from collections import Counter
-from collections.abc import Iterable
 from functools import wraps
 from io import StringIO
 from pathlib import Path
 from shutil import which
 
 import urllib3
 
@@ -15,15 +14,18 @@
 def scan_stats(files, filtered_files, folders):
     return (
         f"""Files: {len(files)}{f" [{len(filtered_files)} ignored]" if filtered_files else ''}"""
         f" Folders: {len(folders)}"
     )
 
 
-def rglob(base_dir: str, extensions: None | Iterable[str] = None) -> tuple[set[str], set[str], set[str]]:
+def rglob(
+    base_dir: str | Path,
+    extensions=None,  # None | Iterable[str]
+) -> tuple[set[str], set[str], set[str]]:
     files = set()
     filtered_files = set()
     folders = set()
     stack = [base_dir]
     while stack:
         current_dir = stack.pop()
         try:
@@ -56,15 +58,15 @@
 
     return files, filtered_files, folders
 
 
 def file_temp_copy(src) -> str:
     fo_dest = tempfile.NamedTemporaryFile(delete=False)
     with open(src, "r+b") as fo_src:
-        shutil.copyfileobj(fo_src, fo_dest)
+        shutil.copyfileobj(fo_src, fo_dest.file)
     fo_dest.seek(0)
     fname = fo_dest.name
     fo_dest.close()
     return fname
 
 
 def trash(args, path: Path | str, detach=True) -> None:
@@ -211,14 +213,23 @@
         temp.flush()
         os.fsync(temp.fileno())
 
         print(f"""### Move {len(file_list)} files to new folders: ###""")
         print(rf"PARALLEL_SHELL=sh parallel --colsep '\t' -a {temp.name} -j 20 {move_sh_path}")
 
 
+def is_sqlite(path):
+    try:
+        with open(path, "rb") as f:
+            header = f.read(16)
+        return header == b"SQLite format 3\000"
+    except OSError:
+        return False
+
+
 def get_file_encoding(path):
     import chardet
 
     if path.startswith("http"):
         detector = chardet.UniversalDetector()
         response = web.session.get(path, stream=True)
         response.raw.decode_content = True
@@ -477,7 +488,20 @@
         raise ValueError(msg)
 
     for table_index, df in enumerate(dfs):
         if not hasattr(df, "name"):
             df.name = str(table_index)
 
     return dfs
+
+
+def get_filesize(d):
+    try:
+        stat = Path(d["path"]).stat()
+        d["size"] = stat.st_size
+        d["time_deleted"] = 0
+    except FileNotFoundError:
+        d["size"] = None
+        if "time_deleted" not in d:
+            d["time_deleted"] = consts.APPLICATION_START
+
+    return d
```

### Comparing `xklb-2.7.9/xklb/utils/gui.py` & `xklb-2.8.1/xklb/utils/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 
 class MrSuperDialogue:
     def __init__(self, path, qty, geom_data=None, true_action="keep", false_action="delete") -> None:
         from tkinter import PhotoImage, Tk
         from tkinter.ttk import Button, Frame, Label, Style
 
+        self.action = None
+
         def raise_error(_self, *_args):
             raise  # pylint: disable=misplaced-bare-raise
 
         Tk.report_callback_exception = raise_error
 
         self.root = Tk()
         self.root.title("Library dialogue")
```

### Comparing `xklb-2.7.9/xklb/utils/iterables.py` & `xklb-2.8.1/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/utils/log_utils.py` & `xklb-2.8.1/xklb/utils/log_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import argparse, logging, os, sys
 from functools import wraps
 from timeit import default_timer
 
 from IPython.core import ultratb
 from IPython.terminal import debugger
 
-from xklb.utils import arggroups
-
 sys.breakpointhook = debugger.set_trace
 
 
 def clamp_index(arr, idx):
     return arr[min(max(idx, 0), len(arr) - 1)]
 
 
@@ -26,15 +24,15 @@
     f.has_run = False
     return wrapper
 
 
 @run_once
 def argparse_log() -> logging.Logger:
     parser = argparse.ArgumentParser(add_help=False)
-    arggroups.debug(parser)
+    parser.add_argument("--verbose", "-v", action="count", default=0)
     args, _unknown = parser.parse_known_args()
 
     try:
         if args.verbose > 0 and os.getpgrp() == os.tcgetpgrp(sys.stdout.fileno()):
             sys.excepthook = ultratb.FormattedTB(
                 mode="Verbose" if args.verbose > 1 else "Context",
                 color_scheme="Neutral",
```

### Comparing `xklb-2.7.9/xklb/utils/mpv_utils.py` & `xklb-2.8.1/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/utils/nums.py` & `xklb-2.8.1/xklb/utils/nums.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,17 @@
         v = float(s.rstrip("%")) / 100
     else:
         v = float(s)
     return v
 
 
 def percentage_difference(value1, value2):
+    value1 = value1 or 0
+    value2 = value2 or 0
+
     try:
         return abs((value1 - value2) / ((value1 + value2) / 2)) * 100
     except ZeroDivisionError:
         return 100.0
 
 
 def to_timestamp(dt_object):
```

### Comparing `xklb-2.7.9/xklb/utils/objects.py` & `xklb-2.8.1/xklb/utils/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,41 @@
 
 
 def take(gen, num=5):
     for value, _ in zip(gen, range(num)):
         yield value
 
 
+def gen_is_empty(generator):
+    try:
+        item = next(generator)
+
+        def g2():
+            yield item
+            yield from generator
+
+        return g2(), False
+    except StopIteration:
+        return (_ for _ in []), True
+
+
+def gen_len(gen, max_length=100):
+    items = []
+    for count, item in enumerate(gen, start=1):
+        items.append(item)
+        if count >= max_length:
+            break
+
+    def new_generator():
+        yield from items
+        yield from gen
+
+    return new_generator(), count
+
+
 def flatten_dict(nested_dict, parent_key="", sep="_", passthrough_keys=None):
     if passthrough_keys is None:
         passthrough_keys = []
     flattened_dict = {}
     for key, value in nested_dict.items():
         new_key = f"{parent_key}{sep}{key}" if parent_key else key
         if isinstance(value, dict) and key not in passthrough_keys:
```

### Comparing `xklb-2.7.9/xklb/utils/path_utils.py` & `xklb-2.8.1/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/utils/pd_utils.py` & `xklb-2.8.1/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/utils/printing.py` & `xklb-2.8.1/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/utils/processes.py` & `xklb-2.8.1/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/xklb/utils/strings.py` & `xklb-2.8.1/xklb/utils/strings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import html, re
+import html, re, textwrap
 from copy import deepcopy
+from itertools import zip_longest
 
 from xklb.data import wordbank
-from xklb.utils import iterables, nums
+from xklb.utils import consts, iterables, nums
 from xklb.utils.log_utils import log
 
 
 def repeat_until_same(fn):  # noqa: ANN201
     def wrapper(*args, **kwargs):
         p = args[0]
         while True:
@@ -225,7 +226,26 @@
 def safe_percent(v) -> str | None:
     if v in [None, ""]:
         return None
     try:
         return f"{v:.2%}"
     except Exception:
         return None
+
+
+def format_two_columns(text1, text2, width1=30, width2=70, left_gutter=2, middle_gutter=2, right_gutter=3):
+    terminal_width = min(consts.TERMINAL_SIZE.columns, 100) - (left_gutter + middle_gutter + right_gutter)
+    if text2:
+        width1 = int(terminal_width * (width1 / (width1 + width2)))
+        width2 = int(terminal_width * (width2 / (width1 + width2)))
+    else:
+        width1 = terminal_width
+
+    wrapped_text1 = textwrap.wrap(text1, width=width1)
+    wrapped_text2 = textwrap.wrap(text2, width=width2)
+
+    formatted_lines = [
+        f"{' ' * left_gutter}{line1:<{width1}}{' ' * middle_gutter}{line2:<{width2}}{' ' * right_gutter}".rstrip()
+        for line1, line2 in zip_longest(wrapped_text1, wrapped_text2, fillvalue="")
+    ]
+
+    return "\n".join(formatted_lines) + "\n"
```

### Comparing `xklb-2.7.9/xklb/assets/kotobago.png` & `xklb-2.8.1/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/.gitignore` & `xklb-2.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.7.9/pyproject.toml` & `xklb-2.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ]
 
 [tool.hatch.build.force-include]
 "xklb/assets/" = "xklb/assets/"
 
 [tool.black]
 line-length = 120
-target-version = ["py39", "py310", "py311"]
+target-version = ["py310", "py311", "py312"]
 
 [tool.isort]
 atomic = true
 combine_straight_imports = true
 float_to_top = true
 group_by_package = true
 line_length = 120
```

### Comparing `xklb-2.7.9/.github/README.md` & `xklb-2.8.1/.github/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    library (v2.7.009; 72 subcommands)
+    library (v2.8.001; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -365,15 +365,15 @@
     [Unit]
     Description=xklb daily browser tabs
 
     [Service]
     Type=simple
     RemainAfterExit=no
     Environment="DISPLAY=:0"
-    ExecStart="/usr/bin/fish" "-c" "lb tabs /home/xk/lb/tabs.db"
+    ExecStart=library tabs /home/my/tabs.db
 
     tee ~/.config/systemd/user/tabs.timer
     [Unit]
     Description=xklb daily browser tabs timer
 
     [Timer]
     Persistent=yes
@@ -644,16 +644,17 @@
         using the ask-keep action will mark a video as deleted when you 'quit 4' and it will mark a video as watched when you 'quit'.
 
         For example, here I bind "'" to "KEEP" and  "j" to "DELETE"
 
             ' quit
             j quit 4
 
-        This is pretty intuitive after you use it a few times but writing this out I realize this might seem a bit opaque.
-        Instead of using built-in post-actions (example above) you could also do something like
+        This is pretty intuitive after you use it a few times but another option is to
+        define your own post-actions:
+
             `--cmd5 'echo {} >> keep.txt' --cmd6 'echo {} >> rejected.txt'`
 
         But you will still bind keys in mpv input.conf:
 
             k quit 5  # goes to keep.txt
             r quit 6  # goes to rejected.txt
 
@@ -1314,15 +1315,15 @@
 
     Find similar folders based on ONLY total size
 
         $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
 
     Read paths from dbs
 
-        $ library similar-folders --dbs db1.db db2.db
+        $ lb fs audio.db --cols path,duration,size,time_deleted --to-json | lb similar-folders --from-json -v
 
     Print only paths
 
         $ library similar-folders ~/d/ -pf
         /home/xk/d/dump/datasets/vector/output/
         /home/xk/d/dump/datasets/vector/output2/
 
@@ -1400,15 +1401,15 @@
 
     Find similar files based on ONLY size
 
         $ library similar-files --no-filter-names ~/d/
 
     Read paths from dbs
 
-        $ library similar-files --dbs db1.db db2.db
+        $ lb fs audio.db --cols path,duration,size,time_deleted --to-json | lb similar-files --from-json -v
 
 
 
 </details>
 
 ### Tabular data subcommands
 
@@ -2297,14 +2298,17 @@
         as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
         library watch -RRCO
 
         You can even sort the items within each cluster by auto-MCDA ~LOL~
         library watch -B --sort-groups-by 'mcda median_size,-deleted'
         library watch -C --sort-groups-by 'mcda median_size,-deleted'
 
+    Filter media by playlist:
+        library watch --playlists URL1 URL2
+
     Filter media by file siblings of parent directory:
         library watch --sibling   # only include files which have more than or equal to one sibling
         library watch --solo      # only include files which are alone by themselves
 
         `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
         library watch --sibling --solo      # you will always get zero records here
         library watch --lower 2 --upper 1   # equivalent
```

### Comparing `xklb-2.7.9/PKG-INFO` & `xklb-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.7.9
+Version: 2.8.1
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -182,15 +182,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    library (v2.7.009; 72 subcommands)
+    library (v2.8.001; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -454,15 +454,15 @@
     [Unit]
     Description=xklb daily browser tabs
 
     [Service]
     Type=simple
     RemainAfterExit=no
     Environment="DISPLAY=:0"
-    ExecStart="/usr/bin/fish" "-c" "lb tabs /home/xk/lb/tabs.db"
+    ExecStart=library tabs /home/my/tabs.db
 
     tee ~/.config/systemd/user/tabs.timer
     [Unit]
     Description=xklb daily browser tabs timer
 
     [Timer]
     Persistent=yes
@@ -733,16 +733,17 @@
         using the ask-keep action will mark a video as deleted when you 'quit 4' and it will mark a video as watched when you 'quit'.
 
         For example, here I bind "'" to "KEEP" and  "j" to "DELETE"
 
             ' quit
             j quit 4
 
-        This is pretty intuitive after you use it a few times but writing this out I realize this might seem a bit opaque.
-        Instead of using built-in post-actions (example above) you could also do something like
+        This is pretty intuitive after you use it a few times but another option is to
+        define your own post-actions:
+
             `--cmd5 'echo {} >> keep.txt' --cmd6 'echo {} >> rejected.txt'`
 
         But you will still bind keys in mpv input.conf:
 
             k quit 5  # goes to keep.txt
             r quit 6  # goes to rejected.txt
 
@@ -1403,15 +1404,15 @@
 
     Find similar folders based on ONLY total size
 
         $ library similar-folders --no-filter-names --no-filter-counts --total-size ~/d/
 
     Read paths from dbs
 
-        $ library similar-folders --dbs db1.db db2.db
+        $ lb fs audio.db --cols path,duration,size,time_deleted --to-json | lb similar-folders --from-json -v
 
     Print only paths
 
         $ library similar-folders ~/d/ -pf
         /home/xk/d/dump/datasets/vector/output/
         /home/xk/d/dump/datasets/vector/output2/
 
@@ -1489,15 +1490,15 @@
 
     Find similar files based on ONLY size
 
         $ library similar-files --no-filter-names ~/d/
 
     Read paths from dbs
 
-        $ library similar-files --dbs db1.db db2.db
+        $ lb fs audio.db --cols path,duration,size,time_deleted --to-json | lb similar-files --from-json -v
 
 
 
 </details>
 
 ### Tabular data subcommands
 
@@ -2386,14 +2387,17 @@
         as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
         library watch -RRCO
 
         You can even sort the items within each cluster by auto-MCDA ~LOL~
         library watch -B --sort-groups-by 'mcda median_size,-deleted'
         library watch -C --sort-groups-by 'mcda median_size,-deleted'
 
+    Filter media by playlist:
+        library watch --playlists URL1 URL2
+
     Filter media by file siblings of parent directory:
         library watch --sibling   # only include files which have more than or equal to one sibling
         library watch --solo      # only include files which are alone by themselves
 
         `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
         library watch --sibling --solo      # you will always get zero records here
         library watch --lower 2 --upper 1   # equivalent
```


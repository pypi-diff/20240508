# Comparing `tmp/ocatari-1.0.6.tar.gz` & `tmp/ocatari-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocatari-1.0.6.tar", last modified: Tue May  7 15:33:03 2024, max compression
+gzip compressed data, was "ocatari-1.0.7.tar", last modified: Wed May  8 11:20:40 2024, max compression
```

## Comparing `ocatari-1.0.6.tar` & `ocatari-1.0.7.tar`

### file list

```diff
@@ -1,141 +1,140 @@
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:03.067300 ocatari-1.0.6/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1171 2023-06-14 17:01:45.000000 ocatari-1.0.6/LICENSE
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7744 2024-05-07 15:33:03.067300 ocatari-1.0.6/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6297 2024-03-13 13:04:01.000000 ocatari-1.0.6/README.md
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:02.967299 ocatari-1.0.6/ocatari/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       25 2024-02-13 13:58:13.000000 ocatari-1.0.6/ocatari/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    26172 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/core.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2891 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/environments.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:02.995299 ocatari-1.0.6/ocatari/ram/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:57:07.000000 ocatari-1.0.6/ocatari/ram/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3297 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/ram/_helper_methods.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14387 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7586 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4015 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15620 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5552 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9111 2023-08-23 09:50:18.000000 ocatari-1.0.6/ocatari/ram/asterix_old.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14794 2024-02-12 14:35:56.000000 ocatari-1.0.6/ocatari/ram/asterix_old2.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12738 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14088 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4552 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    19073 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5410 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10096 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5888 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5534 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7113 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11564 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11345 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    29685 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10183 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6241 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8247 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2102 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    17884 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/extract_ram_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2068 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/extract_ram_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4743 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3136 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12497 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6054 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/ram/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8640 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)   426388 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4005 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5966 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13579 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14946 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    38831 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6500 2024-03-20 15:36:32.000000 ocatari-1.0.6/ocatari/ram/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4625 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15588 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5915 2024-04-09 09:11:16.000000 ocatari-1.0.6/ocatari/ram/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16424 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14403 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10623 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13893 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14619 2024-04-09 09:11:51.000000 ocatari-1.0.6/ocatari/ram/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8491 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12411 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8869 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16258 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7136 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3036 2023-07-31 09:59:59.000000 ocatari-1.0.6/ocatari/ram/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9308 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5063 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5946 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/yarsrevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10518 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/utils.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:03.055300 ocatari-1.0.6/ocatari/vision/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:55:37.000000 ocatari-1.0.6/ocatari/vision/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5880 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2888 2023-09-07 09:07:40.000000 ocatari-1.0.6/ocatari/vision/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2003 2023-11-15 16:35:48.000000 ocatari-1.0.6/ocatari/vision/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6175 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8795 2023-03-14 16:04:08.000000 ocatari-1.0.6/ocatari/vision/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2588 2023-10-26 14:02:07.000000 ocatari-1.0.6/ocatari/vision/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7361 2023-04-12 13:10:52.000000 ocatari-1.0.6/ocatari/vision/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2106 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4570 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6024 2023-04-12 13:10:52.000000 ocatari-1.0.6/ocatari/vision/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2817 2023-05-29 14:25:14.000000 ocatari-1.0.6/ocatari/vision/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2486 2023-03-14 16:04:08.000000 ocatari-1.0.6/ocatari/vision/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1812 2023-10-18 14:47:32.000000 ocatari-1.0.6/ocatari/vision/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2992 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5182 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4292 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5801 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3765 2023-11-15 16:35:48.000000 ocatari-1.0.6/ocatari/vision/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3168 2023-11-23 15:00:40.000000 ocatari-1.0.6/ocatari/vision/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4350 2024-02-24 17:10:04.000000 ocatari-1.0.6/ocatari/vision/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2418 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7526 2024-02-13 14:20:55.000000 ocatari-1.0.6/ocatari/vision/extract_vision_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      597 2023-11-14 14:22:11.000000 ocatari-1.0.6/ocatari/vision/extract_vision_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5495 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1579 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5612 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3683 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3016 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11578 2023-10-10 09:58:35.000000 ocatari-1.0.6/ocatari/vision/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2639 2023-07-19 13:40:30.000000 ocatari-1.0.6/ocatari/vision/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4096 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5690 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8432 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6525 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2631 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2334 2024-02-14 13:21:26.000000 ocatari-1.0.6/ocatari/vision/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7216 2023-11-12 17:10:19.000000 ocatari-1.0.6/ocatari/vision/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2065 2023-06-16 08:15:13.000000 ocatari-1.0.6/ocatari/vision/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10116 2023-07-19 13:40:30.000000 ocatari-1.0.6/ocatari/vision/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3978 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3867 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8142 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4653 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2143 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2909 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2499 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6771 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3629 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    21751 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6659 2023-08-31 10:23:09.000000 ocatari-1.0.6/ocatari/vision/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4132 2023-08-31 10:23:09.000000 ocatari-1.0.6/ocatari/vision/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4128 2023-10-10 09:58:35.000000 ocatari-1.0.6/ocatari/vision/yarsrevenge.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:02.967299 ocatari-1.0.6/ocatari.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)     7744 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3413 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/SOURCES.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/dependency_links.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      122 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/requires.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       14 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/top_level.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       38 2024-05-07 15:33:03.067300 ocatari-1.0.6/setup.cfg
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1025 2024-05-07 15:32:52.000000 ocatari-1.0.6/setup.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:03.067300 ocatari-1.0.6/tests/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-14 17:01:46.000000 ocatari-1.0.6/tests/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2509 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/display_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4339 2023-08-23 08:04:55.000000 ocatari-1.0.6/tests/display_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10431 2024-02-24 17:17:25.000000 ocatari-1.0.6/tests/get_metrics.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10493 2023-08-23 09:50:18.000000 ocatari-1.0.6/tests/metrics_utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1673 2023-06-14 17:01:46.000000 ocatari-1.0.6/tests/plot_speed_results.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1604 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/pong_test.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1851 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/test_explanation.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2921 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/test_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4637 2024-02-24 17:08:28.000000 ocatari-1.0.6/tests/test_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5963 2023-10-26 14:02:07.000000 ocatari-1.0.6/tests/test_game_both_interactive.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1281 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/test_speed.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.980289 ocatari-1.0.7/
+-rw-r--r--   0 quentin    (501) staff       (20)     1171 2024-02-29 10:31:14.000000 ocatari-1.0.7/LICENSE
+-rw-r--r--   0 quentin    (501) staff       (20)     6883 2024-05-08 11:20:40.979505 ocatari-1.0.7/PKG-INFO
+-rw-r--r--   0 quentin    (501) staff       (20)     6297 2024-03-18 21:48:49.000000 ocatari-1.0.7/README.md
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.831988 ocatari-1.0.7/ocatari/
+-rw-r--r--   0 quentin    (501) staff       (20)       25 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)    26578 2024-05-08 11:15:35.000000 ocatari-1.0.7/ocatari/core.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2891 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/environments.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.890587 ocatari-1.0.7/ocatari/ram/
+-rw-r--r--   0 quentin    (501) staff       (20)      394 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3297 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/_helper_methods.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14387 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/adventure.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7586 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/alien.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4015 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/amidar.py
+-rw-r--r--   0 quentin    (501) staff       (20)    15620 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/assault.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5552 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/asterix.py
+-rw-r--r--   0 quentin    (501) staff       (20)     9111 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/asterix_old.py
+-rw-r--r--   0 quentin    (501) staff       (20)    12738 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/asteroids.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14088 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/atlantis.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4552 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/bankheist.py
+-rw-r--r--   0 quentin    (501) staff       (20)    19073 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/battlezone.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5410 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/beamrider.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10096 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/berzerk.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5888 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/bowling.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5534 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/boxing.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7113 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/breakout.py
+-rw-r--r--   0 quentin    (501) staff       (20)    11564 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/carnival.py
+-rw-r--r--   0 quentin    (501) staff       (20)    11345 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/centipede.py
+-rw-r--r--   0 quentin    (501) staff       (20)    29685 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/choppercommand.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10183 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/crazyclimber.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6241 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/demonattack.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8247 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/donkeykong.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2102 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/enduro.py
+-rw-r--r--   0 quentin    (501) staff       (20)    17884 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/extract_ram_info.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2068 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/extract_ram_info_short.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4743 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/fishingderby.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3136 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/freeway.py
+-rw-r--r--   0 quentin    (501) staff       (20)    12497 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/frostbite.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6054 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/game_objects.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8640 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/gopher.py
+-rw-r--r--   0 quentin    (501) staff       (20)   426388 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/hero.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4005 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/icehockey.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5966 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/jamesbond.py
+-rw-r--r--   0 quentin    (501) staff       (20)    13579 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/kangaroo.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14946 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/krull.py
+-rw-r--r--   0 quentin    (501) staff       (20)    38831 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/montezumarevenge.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6500 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/mspacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4625 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/pacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)    15588 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/pitfall.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5915 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/pong.py
+-rw-r--r--   0 quentin    (501) staff       (20)    16424 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/privateeye.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14403 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/qbert.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10623 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/riverraid.py
+-rw-r--r--   0 quentin    (501) staff       (20)    13893 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/roadrunner.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14619 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/seaquest.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8491 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/skiing.py
+-rw-r--r--   0 quentin    (501) staff       (20)    12411 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/spaceinvaders.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8869 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/tennis.py
+-rw-r--r--   0 quentin    (501) staff       (20)    16258 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/timepilot.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7136 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/upndown.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3036 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/utils.py
+-rw-r--r--   0 quentin    (501) staff       (20)     9308 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/venture.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5063 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/videopinball.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5946 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/yarsrevenge.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10518 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/utils.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.960806 ocatari-1.0.7/ocatari/vision/
+-rw-r--r--   0 quentin    (501) staff       (20)      394 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5880 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/adventure.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2888 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/alien.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2003 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/amidar.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6175 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/assault.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8795 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/asterix.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2588 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/asteroids.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7361 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/atlantis.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2106 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/bankheist.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4570 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/battlezone.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6024 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/beamrider.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2817 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/berzerk.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2486 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/bowling.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1812 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/boxing.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2992 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/breakout.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5182 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/carnival.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4292 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/centipede.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5801 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/choppercommand.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3765 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/crazyclimber.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3168 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/demonattack.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4350 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/donkeykong.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2418 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/enduro.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7526 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/extract_vision_info.py
+-rw-r--r--   0 quentin    (501) staff       (20)      597 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/extract_vision_info_short.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5495 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/fishingderby.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1579 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/freeway.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5612 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/frostbite.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3683 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/game_objects.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3016 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/gopher.py
+-rw-r--r--   0 quentin    (501) staff       (20)    11578 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/hero.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2639 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/icehockey.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4096 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/jamesbond.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5690 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/kangaroo.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8432 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/krull.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6525 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/montezumarevenge.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2631 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/mspacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2334 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/pacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7216 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/pitfall.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2065 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/pong.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10116 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/privateeye.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3978 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/qbert.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3867 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/riverraid.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8142 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/roadrunner.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4653 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/seaquest.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2143 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/skiing.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2909 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/spaceinvaders.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2499 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/tennis.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6771 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/timepilot.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3629 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/upndown.py
+-rw-r--r--   0 quentin    (501) staff       (20)    21751 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/utils.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6659 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/venture.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4132 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/videopinball.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4128 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/yarsrevenge.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.976378 ocatari-1.0.7/ocatari.egg-info/
+-rw-r--r--   0 quentin    (501) staff       (20)     6883 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/PKG-INFO
+-rw-r--r--   0 quentin    (501) staff       (20)     3385 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin    (501) staff       (20)        1 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin    (501) staff       (20)      122 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/requires.txt
+-rw-r--r--   0 quentin    (501) staff       (20)       14 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/top_level.txt
+-rw-r--r--   0 quentin    (501) staff       (20)       38 2024-05-08 11:20:40.980481 ocatari-1.0.7/setup.cfg
+-rw-r--r--   0 quentin    (501) staff       (20)     1025 2024-05-08 11:15:53.000000 ocatari-1.0.7/setup.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.973963 ocatari-1.0.7/tests/
+-rw-r--r--   0 quentin    (501) staff       (20)        0 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2509 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/display_game.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4339 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/display_game_both.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10431 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/get_metrics.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10493 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/metrics_utils.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1673 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/plot_speed_results.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1604 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/pong_test.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1851 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/test_explanation.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2921 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/test_game.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4637 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/test_game_both.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5963 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/test_game_both_interactive.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1281 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/test_speed.py
```

### Comparing `ocatari-1.0.6/LICENSE` & `ocatari-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/PKG-INFO` & `ocatari-1.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,155 +1,167 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.6
+Version: 1.0.7
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
-License: UNKNOWN
-Description: # Object-Centric Atari Environments
-        Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
-        
-        <img style="float: right;" width="400px" align="right" src="docs/_static/kangaroo.png">
-        
-        Inspired by thw work of [Anand et. al.](https://arxiv.org/abs/1906.08226), we present OCAtari, an improved, extended and object-centric version of their [ATARI ARI project](https://github.com/mila-iqia/atari-representation-learning). \
-        The [Arcade Learning Environment](https://github.com/mgbellemare/Arcade-Learning-Environment) allows us to read the RAM state at any time of a game. 
-        This repository provides a wrapper for the well known [Gynmasium project](https://github.com/Farama-Foundation/Gymnasium), that uses the state of the ram and reverse engineering to provide object centric representation of the screen. It provides code for benchmarking, testing and generating object-centric representations of states.
-        
-        * [Install](#install) -- Install all relevant dependencies and start using OCAtari yourself
-        * [Usage](#usage) -- Learn about the different environments OCAtari supports and enables
-        * [Producing your own dataset](#producing-your-own-dataset) -- OCAtari also support the generation of object-centric datasets for supported Atari games
-        * [Models and additional Information](#models-and-additional-information) -- Everything you need to know to reproduce our results
-        
-        
-        :heavy_exclamation_mark: [HERE IS A LINK TO THE DOCUMENTATION  :bookmark_tabs:](https://oc-atari.readthedocs.io/en/latest/)
-        
-        --- 
-        
-        ### Structure of this repository
-        This repository is structured into multiple folder:
-        * [dataset_generation](dataset_generation/) -- includes all scripts needed to generate object-centric datasets for Atari game
-        * [models](models/) -- includes all models needed to reproduce our results as well as to test out the environments
-        * [ocatari](ocatari/) -- the actual wrapper
-        * [scripts](scripts/) -- A huge amount of scripts to help and test while implementing, extending or using OCAtari. 
-        Most are used to reverse engineer the RAM state, like searching for correlations within the RAM state.
-        
-        
-        ## Install
-        You can install OCAtari in multiple ways, the recommended is to use the provided Dockerfile to install all requirements, like the Atari ROMs and gymnasium.
-        You can also simply:
-        `pip install ocatari`
-        `pip install "gymnasium[atari, accept-rom-license]"`
-        If you want to modify the code, you can clone this repo and run:
-        `python setup.py install` or if you want to modify the code `python setup.py develop`
-        
-        
-        ## Usage
-        To use the OCAtari environments:
-        ``` python
-        from ocatari.core import OCAtari
-        import random
-        
-        env = OCAtari("Pong", mode="ram", hud=True, render_mode="rgb_array")
-        observation, info = env.reset()
-        action = random.randint(0, env.nb_actions-1)
-        obs, reward, terminated, truncated, info = env.step(action)
-        ```
-        
-        ### Cite OCAtari:
-        If you are using OCAtari for your scientific pubplease use 'ram' mode insteadlications, please cite us:
-        ```bibtex
-        @inproceedings{Delfosse2023OCAtariOA,
-        title={OCAtari: Object-Centric Atari 2600 Reinforcement Learning Environments},
-        author={Quentin Delfosse and Jannis Blüml and Bjarne Gregori and Sebastian Sztwiertnia and Kristian Kersting},
-        year={2023}
-        }
-        ```
-        
-        ###  List of covered games
-        - [X] Alien
-        - [X] Amidar
-        - [X] Assault
-        - [X] Asterix
-        - [X] Asteroids  (only vision)
-        - [X] Atlantis
-        - [ ] BattleZone (in progress)
-        - [ ] Bankheist (in progress)
-        - [ ] BeamRider  (only vision)
-        - [X] Berzerk
-        - [X] Bowling
-        - [X] Boxing
-        - [X] Breakout
-        - [X] Carnival
-        - [X] Centipede
-        - [X] Chopper Command
-        - [X] Crazy Climbers
-        - [X] DemonAttack
-        - [X] DonkeyKong
-        - [X] Fishing Derby  
-        - [X] Freeway
-        - [X] Frostbite
-        - [X] Gopher
-        - [X] Hero
-        - [X] IceHockey
-        - [X] Kangaroo
-        - [X] Krull
-        - [X] MontezumaRevenge
-        - [X] MsPacman
-        - [X] Pacman
-        - [X] Pitfall
-        - [X] Pong
-        - [X] PrivateEye
-        - [X] Q\*Bert  
-        - [X] RiverRaid  
-        - [X] RoadRunner  
-        - [X] Seaquest
-        - [X] Skiing
-        - [X] Space Invaders
-        - [X] Tennis
-        - [X] Time Pilot
-        - [X] Up n Down (in progress)
-        - [X] Venture
-        - [X] VideoPinball
-        - [ ] YarsRevenge (in progress)
-        
-        A list of all gymnasium games can be found in the [Gymnasium Documentation](https://gymnasium.farama.org/environments/atari/)
-        
-        ### The two modes of OCAtari
-        OCAtari supports two different modes to extract objects from the current state:
-        
-        **Vision Extraction Mode (VEM):** Return a list of objects currently on the screen with their X, Y, Width, Height, R, G, B Values, based on handwritten rules used on the visual representation. 
-        
-        **Ram Extraction Mode (REM):** Uses the object values stored in the RAM to detect the objects currently on the screen.
-        
-        ### Use these trained agents and the demo script:
-        
-        A better example how to run OCAtari is given with our demo files showing you how to run each game with a provided agent. 
-        
-        Use the demo files in the scripts/demo folder to test it yourself. You can set the mode to 'raw', 'vision' or 'revised' in line 10 of the demo script.
-        You can also run the demo file with an already trained agent or your own developed agent. You can use the -p flag in the command to run the demo file by an agent and let the agent play the game.
-        Here is an example: 
-        
-        `python demo_pong.py -p models/Pong/model_50000000.gz`
-        
-        More information can be found in this [ReadMe](scripts/demo/README%20Demos.md)
-        
-        ### Extract the objects from a state 
-        
-        With `env.objects` one can access the list of objects found in the current state. Note that these lists can differ depending on the mode you used initiating the environment
-        
-        ### Producing your own dataset
-        
-        OCAtari can be used to generate datasets consisting of a represenation of the current state in form of an RGB array and a list of all objects within the state. 
-        More information can be found in the dataset_generation folder. 
-        
-        ## Models and additional Information
-        
-        As trained agents as well as to reproduce our results, we recomment to use the agents of [this repo](https://github.com/floringogianu/atari-agents).  
-        
-        ### Reproducing our results
-        In most of our scripts we added the following line to make the deterministic and easier to reproduce `make_deterministic(env, 42)`. This line can and should be removed if this is not the desired behavior. 
-        As seeds we used 0 for evaluating the metrics and 42 for generating the dataset. 
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: gymnasium
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: opencv_python
+Requires-Dist: scikit_image
+Requires-Dist: termcolor
+Requires-Dist: seaborn
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: keyboard
+Requires-Dist: tqdm
+Requires-Dist: pygame
+Requires-Dist: pyfiglet
+
+# Object-Centric Atari Environments
+Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
+
+<img style="float: right;" width="400px" align="right" src="docs/_static/kangaroo.png">
+
+Inspired by thw work of [Anand et. al.](https://arxiv.org/abs/1906.08226), we present OCAtari, an improved, extended and object-centric version of their [ATARI ARI project](https://github.com/mila-iqia/atari-representation-learning). \
+The [Arcade Learning Environment](https://github.com/mgbellemare/Arcade-Learning-Environment) allows us to read the RAM state at any time of a game. 
+This repository provides a wrapper for the well known [Gynmasium project](https://github.com/Farama-Foundation/Gymnasium), that uses the state of the ram and reverse engineering to provide object centric representation of the screen. It provides code for benchmarking, testing and generating object-centric representations of states.
+
+* [Install](#install) -- Install all relevant dependencies and start using OCAtari yourself
+* [Usage](#usage) -- Learn about the different environments OCAtari supports and enables
+* [Producing your own dataset](#producing-your-own-dataset) -- OCAtari also support the generation of object-centric datasets for supported Atari games
+* [Models and additional Information](#models-and-additional-information) -- Everything you need to know to reproduce our results
+
+
+:heavy_exclamation_mark: [HERE IS A LINK TO THE DOCUMENTATION  :bookmark_tabs:](https://oc-atari.readthedocs.io/en/latest/)
+
+--- 
+
+### Structure of this repository
+This repository is structured into multiple folder:
+* [dataset_generation](dataset_generation/) -- includes all scripts needed to generate object-centric datasets for Atari game
+* [models](models/) -- includes all models needed to reproduce our results as well as to test out the environments
+* [ocatari](ocatari/) -- the actual wrapper
+* [scripts](scripts/) -- A huge amount of scripts to help and test while implementing, extending or using OCAtari. 
+Most are used to reverse engineer the RAM state, like searching for correlations within the RAM state.
+
+
+## Install
+You can install OCAtari in multiple ways, the recommended is to use the provided Dockerfile to install all requirements, like the Atari ROMs and gymnasium.
+You can also simply:
+`pip install ocatari`
+`pip install "gymnasium[atari, accept-rom-license]"`
+If you want to modify the code, you can clone this repo and run:
+`python setup.py install` or if you want to modify the code `python setup.py develop`
+
+
+## Usage
+To use the OCAtari environments:
+``` python
+from ocatari.core import OCAtari
+import random
+
+env = OCAtari("Pong", mode="ram", hud=True, render_mode="rgb_array")
+observation, info = env.reset()
+action = random.randint(0, env.nb_actions-1)
+obs, reward, terminated, truncated, info = env.step(action)
+```
+
+### Cite OCAtari:
+If you are using OCAtari for your scientific pubplease use 'ram' mode insteadlications, please cite us:
+```bibtex
+@inproceedings{Delfosse2023OCAtariOA,
+title={OCAtari: Object-Centric Atari 2600 Reinforcement Learning Environments},
+author={Quentin Delfosse and Jannis Blüml and Bjarne Gregori and Sebastian Sztwiertnia and Kristian Kersting},
+year={2023}
+}
+```
+
+###  List of covered games
+- [X] Alien
+- [X] Amidar
+- [X] Assault
+- [X] Asterix
+- [X] Asteroids  (only vision)
+- [X] Atlantis
+- [ ] BattleZone (in progress)
+- [ ] Bankheist (in progress)
+- [ ] BeamRider  (only vision)
+- [X] Berzerk
+- [X] Bowling
+- [X] Boxing
+- [X] Breakout
+- [X] Carnival
+- [X] Centipede
+- [X] Chopper Command
+- [X] Crazy Climbers
+- [X] DemonAttack
+- [X] DonkeyKong
+- [X] Fishing Derby  
+- [X] Freeway
+- [X] Frostbite
+- [X] Gopher
+- [X] Hero
+- [X] IceHockey
+- [X] Kangaroo
+- [X] Krull
+- [X] MontezumaRevenge
+- [X] MsPacman
+- [X] Pacman
+- [X] Pitfall
+- [X] Pong
+- [X] PrivateEye
+- [X] Q\*Bert  
+- [X] RiverRaid  
+- [X] RoadRunner  
+- [X] Seaquest
+- [X] Skiing
+- [X] Space Invaders
+- [X] Tennis
+- [X] Time Pilot
+- [X] Up n Down (in progress)
+- [X] Venture
+- [X] VideoPinball
+- [ ] YarsRevenge (in progress)
+
+A list of all gymnasium games can be found in the [Gymnasium Documentation](https://gymnasium.farama.org/environments/atari/)
+
+### The two modes of OCAtari
+OCAtari supports two different modes to extract objects from the current state:
+
+**Vision Extraction Mode (VEM):** Return a list of objects currently on the screen with their X, Y, Width, Height, R, G, B Values, based on handwritten rules used on the visual representation. 
+
+**Ram Extraction Mode (REM):** Uses the object values stored in the RAM to detect the objects currently on the screen.
+
+### Use these trained agents and the demo script:
+
+A better example how to run OCAtari is given with our demo files showing you how to run each game with a provided agent. 
+
+Use the demo files in the scripts/demo folder to test it yourself. You can set the mode to 'raw', 'vision' or 'revised' in line 10 of the demo script.
+You can also run the demo file with an already trained agent or your own developed agent. You can use the -p flag in the command to run the demo file by an agent and let the agent play the game.
+Here is an example: 
+
+`python demo_pong.py -p models/Pong/model_50000000.gz`
+
+More information can be found in this [ReadMe](scripts/demo/README%20Demos.md)
+
+### Extract the objects from a state 
+
+With `env.objects` one can access the list of objects found in the current state. Note that these lists can differ depending on the mode you used initiating the environment
+
+### Producing your own dataset
+
+OCAtari can be used to generate datasets consisting of a represenation of the current state in form of an RGB array and a list of all objects within the state. 
+More information can be found in the dataset_generation folder. 
+
+## Models and additional Information
+
+As trained agents as well as to reproduce our results, we recomment to use the agents of [this repo](https://github.com/floringogianu/atari-agents).  
+
+### Reproducing our results
+In most of our scripts we added the following line to make the deterministic and easier to reproduce `make_deterministic(env, 42)`. This line can and should be removed if this is not the desired behavior. 
+As seeds we used 0 for evaluating the metrics and 42 for generating the dataset. 
+
```

### Comparing `ocatari-1.0.6/README.md` & `ocatari-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/core.py` & `ocatari-1.0.7/ocatari/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 from ocatari.ram.extract_ram_info import detect_objects_raw, detect_objects_ram, init_objects, get_max_objects
 from ocatari.vision.extract_vision_info import detect_objects_vision
 from ocatari.vision.utils import mark_bb, to_rgba
 from ocatari.ram.game_objects import GameObject, ValueObject
 from ocatari.utils import draw_label, draw_arrow, draw_orientation_indicator
 from gymnasium.error import NameNotFound
 
-from ale_py import ALEInterface
+try:
+    import ale_py
+except ModuleNotFoundError:
+    print(
+        '\nALE is required when using the ALE env wrapper. ',
+        'Try `pip install "gymnasium[atari, accept-rom-license]"`.\n',
+    )
 
 import warnings
 
 UPSCALE_FACTOR = 4
 
 try:
     import cv2
@@ -22,30 +28,38 @@
     print(
         "\nOpenCV is required when using the ALE env wrapper. ",
         "Try `pip install opencv-python`.\n",
     )
 try:
     import torch
     torch_imported = True
+    _tensor = torch.tensor
+    _uint8 = torch.uint8
+    _zeros = torch.zeros
+    _zeros_like = torch.zeros_like
+    _stack = torch.stack
+    DEVICE = "cpu" if torch.cuda.is_available() else "cpu"
 except ModuleNotFoundError:
     torch_imported = False
+    _tensor = np.array
+    _uint8 = np.uint8
+    _zeros = np.zeros
+    _zeros_like = np.zeros_like
+    _stack = np.stack
+    DEVICE = "cpu"
+    warnings.warn("pytorch installation not found, using numpy instead of torch")
 
 try:
     import pygame
 except ModuleNotFoundError:
     print(
         "\npygame is required for human rendering. ",
         "Try `pip install pygame`.\n",
     )
 
-if torch_imported:
-    DEVICE = "gpu" if torch.cuda.is_available() else "cpu"
-else:
-    DEVICE = "cpu" 
-    
 AVAILABLE_GAMES = ["Adventure", "Alien", "Amidar", "Assault", "Asterix", "Asteroids", "Atlantis", "Bankheist", "BattleZone","BeamRider", "Berzerk", "Bowling", "Boxing",
                    "Breakout", "Carnival", "Centipede", "ChoppperCommand", "CrazyClimber", "DemonAttack", "DonkeyKong", "Enduro", "FishingDerby", "Freeway",                   
                    "Frostbite", "Gopher", "Hero", "IceHockey", "Jamesbond", "Kangaroo", "Krull", "MontezumaRevenge", "MsPacman", "Pacman", "Pitfall", "Pong", "PrivateEye",
                    "Qbert", "Riverraid", "RoadRunner", "Seaquest", "Skiing", "SpaceInvaders", "Tennis", "TimePilot", "UpNDown", "Videocube", "VideoPinball", "Venture",
                    "Yarsrevenge", "Zaxxon"]
 
 
@@ -200,21 +214,21 @@
         # if self.obs_mode in ["dqn", "ori"]:
         #     obs = self._get_buffer_as_stack()
         return obs, reward, truncated, terminated, info
 
     def _reset_buffer_dqn(self):
         for _ in range(self.buffer_window_size):
             self._state_buffer.append(
-                torch.zeros(84, 84, device=DEVICE, dtype=torch.uint8)
+                _zeros(84, 84, device=DEVICE, dtype=_uint8)
             )
 
     def _reset_buffer_ori(self):
         for _ in range(self.buffer_window_size):
             self._state_buffer.append(
-                torch.zeros(210, 160, 3, device=DEVICE, dtype=torch.uint8)
+                _zeros(210, 160, 3, device=DEVICE, dtype=uint8)
             )
 
     def _reset_buffer_obj(self):
         for _ in range(self.buffer_window_size):
             self._state_buffer.append(
                 torch.zeros(len(self._objects), 4, device=DEVICE, dtype=torch.uint8)
             )
@@ -228,42 +242,41 @@
         self._objects = init_objects(self.game_name, self.hud)
         return self._env.reset(*args, **kwargs)
 
     def _fill_buffer_dqn(self):
         state = cv2.resize(
             self._ale.getScreenGrayscale(), (84, 84), interpolation=cv2.INTER_AREA,
         )
+        self._state_buffer.append(_tensor(state, dtype=_uint8, device=DEVICE))
         if self.game_name == "Skiing":
-            #import ipdb;ipdb.set_trace()
             tmp = self._state_buffer[1]
             tmp[tmp >= 0] = self.objects[0].orientation
             self._state_buffer[1] = tmp
         elif self.game_name == "Seaquest":
-            #import ipdb;ipdb.set_trace()
             tmp = self._state_buffer[1]
             tmp[tmp >= 0] = self.objects[0].orientation.value
             self._state_buffer[1] = tmp
-        self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
+        self._state_buffer.append(_tensor(state, dtype=_uint8,
                                                device=DEVICE))
 
     def _fill_buffer_ori(self):
         state = self._ale.getScreenRGB()
-        self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
+        self._state_buffer.append(_tensor(state, dtype=_uint8,
                                                device=DEVICE))
 
     def _fill_buffer_obj(self):
         tensor = []
         for obj in self._objects:
             tensor.append(np.asarray(obj.xywh))
         state = np.asarray(tensor)
         self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
                                                device=DEVICE))
 
     def _get_buffer_as_stack(self):
-        return torch.stack(list(self._state_buffer), 0).unsqueeze(0).byte()
+        return _stack(list(self._state_buffer), 0).unsqueeze(0).byte()
 
     window : pygame.Surface = None
     clock : pygame.time.Clock = None
 
     def _initialize_rendering(self, sample_image):
         assert sample_image is not None
         pygame.init()
@@ -456,15 +469,15 @@
 
         :type: list of GameObjects
         """
         return [obj for obj in self._objects if obj] # filtering out None objects
 
     def render_explanations(self):
         coefs = [0.05, 0.1, 0.25, 0.6]
-        rendered = torch.zeros_like(self._state_buffer[0]).float()
+        rendered = _zeros_like(self._state_buffer[0]).float()
         for coef, state_i in zip(coefs, self._state_buffer):
             rendered += coef * state_i
         rendered = rendered.cpu().detach().to(int).numpy()
         for obj in self.objects:
             mark_bb(rendered, obj.xywh, color=obj.rgb)
         import matplotlib.pyplot as plt
         plt.imshow(rendered)
@@ -485,15 +498,15 @@
                           loc='top')
         table.set_fontsize(14)
         plt.subplots_adjust(top=0.8)
         plt.show()
 
 
     def aggregated_render(self, coefs=[0.05, 0.1, 0.25, 0.6]):
-        rendered = torch.zeros_like(self._state_buffer[0]).float()
+        rendered = zeros_like(self._state_buffer[0]).float()
         for coef, state_i in zip(coefs, self._state_buffer):
             rendered += coef * state_i
         rendered = rendered.cpu().detach().to(int).numpy()
         return rendered
 
 
 class HideEnemyPong(OCAtari):
@@ -541,15 +554,15 @@
     
     def _fill_buffer_dqn(self):
         image = self._ale.getScreenGrayscale()
         image[34:194, 8:24] = 87
         state = cv2.resize(
             image, (84, 84), interpolation=cv2.INTER_AREA,
         )
-        self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
+        self._state_buffer.append(_tensor(state, dtype=_uint8,
                                                device=DEVICE))
 
 
 class EasyDonkey(OCAtari):
     def __init__(self, env_name="ALE/DonkeyKong", mode="ram", hud=False, obs_mode="dqn", render_mode=None, render_oc_overlay=False, *args, **kwargs):
         self.lasty = 154
         self.nb_lives = 2
```

### Comparing `ocatari-1.0.6/ocatari/environments.py` & `ocatari-1.0.7/ocatari/environments.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/_helper_methods.py` & `ocatari-1.0.7/ocatari/ram/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/adventure.py` & `ocatari-1.0.7/ocatari/ram/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/alien.py` & `ocatari-1.0.7/ocatari/ram/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/amidar.py` & `ocatari-1.0.7/ocatari/ram/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/assault.py` & `ocatari-1.0.7/ocatari/ram/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/asterix.py` & `ocatari-1.0.7/ocatari/ram/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/asterix_old.py` & `ocatari-1.0.7/ocatari/ram/asterix_old.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/asteroids.py` & `ocatari-1.0.7/ocatari/ram/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/atlantis.py` & `ocatari-1.0.7/ocatari/ram/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/bankheist.py` & `ocatari-1.0.7/ocatari/ram/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/battlezone.py` & `ocatari-1.0.7/ocatari/ram/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/beamrider.py` & `ocatari-1.0.7/ocatari/ram/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/berzerk.py` & `ocatari-1.0.7/ocatari/ram/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/bowling.py` & `ocatari-1.0.7/ocatari/ram/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/boxing.py` & `ocatari-1.0.7/ocatari/ram/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/breakout.py` & `ocatari-1.0.7/ocatari/ram/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/carnival.py` & `ocatari-1.0.7/ocatari/ram/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/centipede.py` & `ocatari-1.0.7/ocatari/ram/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/choppercommand.py` & `ocatari-1.0.7/ocatari/ram/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/crazyclimber.py` & `ocatari-1.0.7/ocatari/ram/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/demonattack.py` & `ocatari-1.0.7/ocatari/ram/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/donkeykong.py` & `ocatari-1.0.7/ocatari/ram/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/enduro.py` & `ocatari-1.0.7/ocatari/ram/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/extract_ram_info.py` & `ocatari-1.0.7/ocatari/ram/extract_ram_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/extract_ram_info_short.py` & `ocatari-1.0.7/ocatari/ram/extract_ram_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/fishingderby.py` & `ocatari-1.0.7/ocatari/ram/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/freeway.py` & `ocatari-1.0.7/ocatari/ram/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/frostbite.py` & `ocatari-1.0.7/ocatari/ram/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/game_objects.py` & `ocatari-1.0.7/ocatari/ram/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/gopher.py` & `ocatari-1.0.7/ocatari/ram/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/hero.py` & `ocatari-1.0.7/ocatari/ram/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/icehockey.py` & `ocatari-1.0.7/ocatari/ram/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/jamesbond.py` & `ocatari-1.0.7/ocatari/ram/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/kangaroo.py` & `ocatari-1.0.7/ocatari/ram/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/krull.py` & `ocatari-1.0.7/ocatari/ram/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/montezumarevenge.py` & `ocatari-1.0.7/ocatari/ram/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/mspacman.py` & `ocatari-1.0.7/ocatari/ram/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/pacman.py` & `ocatari-1.0.7/ocatari/ram/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/pitfall.py` & `ocatari-1.0.7/ocatari/ram/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/pong.py` & `ocatari-1.0.7/ocatari/ram/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/privateeye.py` & `ocatari-1.0.7/ocatari/ram/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/qbert.py` & `ocatari-1.0.7/ocatari/ram/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/riverraid.py` & `ocatari-1.0.7/ocatari/ram/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/roadrunner.py` & `ocatari-1.0.7/ocatari/ram/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/seaquest.py` & `ocatari-1.0.7/ocatari/ram/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/skiing.py` & `ocatari-1.0.7/ocatari/ram/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/spaceinvaders.py` & `ocatari-1.0.7/ocatari/ram/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/tennis.py` & `ocatari-1.0.7/ocatari/ram/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/timepilot.py` & `ocatari-1.0.7/ocatari/ram/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/upndown.py` & `ocatari-1.0.7/ocatari/ram/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/utils.py` & `ocatari-1.0.7/ocatari/ram/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/venture.py` & `ocatari-1.0.7/ocatari/ram/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/videopinball.py` & `ocatari-1.0.7/ocatari/ram/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/ram/yarsrevenge.py` & `ocatari-1.0.7/ocatari/ram/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/utils.py` & `ocatari-1.0.7/ocatari/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/adventure.py` & `ocatari-1.0.7/ocatari/vision/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/alien.py` & `ocatari-1.0.7/ocatari/vision/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/amidar.py` & `ocatari-1.0.7/ocatari/vision/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/assault.py` & `ocatari-1.0.7/ocatari/vision/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/asterix.py` & `ocatari-1.0.7/ocatari/vision/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/asteroids.py` & `ocatari-1.0.7/ocatari/vision/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/atlantis.py` & `ocatari-1.0.7/ocatari/vision/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/bankheist.py` & `ocatari-1.0.7/ocatari/vision/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/battlezone.py` & `ocatari-1.0.7/ocatari/vision/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/beamrider.py` & `ocatari-1.0.7/ocatari/vision/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/berzerk.py` & `ocatari-1.0.7/ocatari/vision/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/bowling.py` & `ocatari-1.0.7/ocatari/vision/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/boxing.py` & `ocatari-1.0.7/ocatari/vision/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/breakout.py` & `ocatari-1.0.7/ocatari/vision/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/carnival.py` & `ocatari-1.0.7/ocatari/vision/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/centipede.py` & `ocatari-1.0.7/ocatari/vision/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/choppercommand.py` & `ocatari-1.0.7/ocatari/vision/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/crazyclimber.py` & `ocatari-1.0.7/ocatari/vision/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/demonattack.py` & `ocatari-1.0.7/ocatari/vision/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/donkeykong.py` & `ocatari-1.0.7/ocatari/vision/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/enduro.py` & `ocatari-1.0.7/ocatari/vision/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/extract_vision_info.py` & `ocatari-1.0.7/ocatari/vision/extract_vision_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/extract_vision_info_short.py` & `ocatari-1.0.7/ocatari/vision/extract_vision_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/fishingderby.py` & `ocatari-1.0.7/ocatari/vision/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/freeway.py` & `ocatari-1.0.7/ocatari/vision/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/frostbite.py` & `ocatari-1.0.7/ocatari/vision/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/game_objects.py` & `ocatari-1.0.7/ocatari/vision/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/gopher.py` & `ocatari-1.0.7/ocatari/vision/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/hero.py` & `ocatari-1.0.7/ocatari/vision/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/icehockey.py` & `ocatari-1.0.7/ocatari/vision/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/jamesbond.py` & `ocatari-1.0.7/ocatari/vision/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/kangaroo.py` & `ocatari-1.0.7/ocatari/vision/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/krull.py` & `ocatari-1.0.7/ocatari/vision/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/montezumarevenge.py` & `ocatari-1.0.7/ocatari/vision/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/mspacman.py` & `ocatari-1.0.7/ocatari/vision/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/pacman.py` & `ocatari-1.0.7/ocatari/vision/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/pitfall.py` & `ocatari-1.0.7/ocatari/vision/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/pong.py` & `ocatari-1.0.7/ocatari/vision/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/privateeye.py` & `ocatari-1.0.7/ocatari/vision/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/qbert.py` & `ocatari-1.0.7/ocatari/vision/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/riverraid.py` & `ocatari-1.0.7/ocatari/vision/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/roadrunner.py` & `ocatari-1.0.7/ocatari/vision/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/seaquest.py` & `ocatari-1.0.7/ocatari/vision/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/skiing.py` & `ocatari-1.0.7/ocatari/vision/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/spaceinvaders.py` & `ocatari-1.0.7/ocatari/vision/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/tennis.py` & `ocatari-1.0.7/ocatari/vision/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/timepilot.py` & `ocatari-1.0.7/ocatari/vision/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/upndown.py` & `ocatari-1.0.7/ocatari/vision/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/utils.py` & `ocatari-1.0.7/ocatari/vision/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/venture.py` & `ocatari-1.0.7/ocatari/vision/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/videopinball.py` & `ocatari-1.0.7/ocatari/vision/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari/vision/yarsrevenge.py` & `ocatari-1.0.7/ocatari/vision/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/ocatari.egg-info/PKG-INFO` & `ocatari-1.0.7/ocatari.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,155 +1,167 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.6
+Version: 1.0.7
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
-License: UNKNOWN
-Description: # Object-Centric Atari Environments
-        Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
-        
-        <img style="float: right;" width="400px" align="right" src="docs/_static/kangaroo.png">
-        
-        Inspired by thw work of [Anand et. al.](https://arxiv.org/abs/1906.08226), we present OCAtari, an improved, extended and object-centric version of their [ATARI ARI project](https://github.com/mila-iqia/atari-representation-learning). \
-        The [Arcade Learning Environment](https://github.com/mgbellemare/Arcade-Learning-Environment) allows us to read the RAM state at any time of a game. 
-        This repository provides a wrapper for the well known [Gynmasium project](https://github.com/Farama-Foundation/Gymnasium), that uses the state of the ram and reverse engineering to provide object centric representation of the screen. It provides code for benchmarking, testing and generating object-centric representations of states.
-        
-        * [Install](#install) -- Install all relevant dependencies and start using OCAtari yourself
-        * [Usage](#usage) -- Learn about the different environments OCAtari supports and enables
-        * [Producing your own dataset](#producing-your-own-dataset) -- OCAtari also support the generation of object-centric datasets for supported Atari games
-        * [Models and additional Information](#models-and-additional-information) -- Everything you need to know to reproduce our results
-        
-        
-        :heavy_exclamation_mark: [HERE IS A LINK TO THE DOCUMENTATION  :bookmark_tabs:](https://oc-atari.readthedocs.io/en/latest/)
-        
-        --- 
-        
-        ### Structure of this repository
-        This repository is structured into multiple folder:
-        * [dataset_generation](dataset_generation/) -- includes all scripts needed to generate object-centric datasets for Atari game
-        * [models](models/) -- includes all models needed to reproduce our results as well as to test out the environments
-        * [ocatari](ocatari/) -- the actual wrapper
-        * [scripts](scripts/) -- A huge amount of scripts to help and test while implementing, extending or using OCAtari. 
-        Most are used to reverse engineer the RAM state, like searching for correlations within the RAM state.
-        
-        
-        ## Install
-        You can install OCAtari in multiple ways, the recommended is to use the provided Dockerfile to install all requirements, like the Atari ROMs and gymnasium.
-        You can also simply:
-        `pip install ocatari`
-        `pip install "gymnasium[atari, accept-rom-license]"`
-        If you want to modify the code, you can clone this repo and run:
-        `python setup.py install` or if you want to modify the code `python setup.py develop`
-        
-        
-        ## Usage
-        To use the OCAtari environments:
-        ``` python
-        from ocatari.core import OCAtari
-        import random
-        
-        env = OCAtari("Pong", mode="ram", hud=True, render_mode="rgb_array")
-        observation, info = env.reset()
-        action = random.randint(0, env.nb_actions-1)
-        obs, reward, terminated, truncated, info = env.step(action)
-        ```
-        
-        ### Cite OCAtari:
-        If you are using OCAtari for your scientific pubplease use 'ram' mode insteadlications, please cite us:
-        ```bibtex
-        @inproceedings{Delfosse2023OCAtariOA,
-        title={OCAtari: Object-Centric Atari 2600 Reinforcement Learning Environments},
-        author={Quentin Delfosse and Jannis Blüml and Bjarne Gregori and Sebastian Sztwiertnia and Kristian Kersting},
-        year={2023}
-        }
-        ```
-        
-        ###  List of covered games
-        - [X] Alien
-        - [X] Amidar
-        - [X] Assault
-        - [X] Asterix
-        - [X] Asteroids  (only vision)
-        - [X] Atlantis
-        - [ ] BattleZone (in progress)
-        - [ ] Bankheist (in progress)
-        - [ ] BeamRider  (only vision)
-        - [X] Berzerk
-        - [X] Bowling
-        - [X] Boxing
-        - [X] Breakout
-        - [X] Carnival
-        - [X] Centipede
-        - [X] Chopper Command
-        - [X] Crazy Climbers
-        - [X] DemonAttack
-        - [X] DonkeyKong
-        - [X] Fishing Derby  
-        - [X] Freeway
-        - [X] Frostbite
-        - [X] Gopher
-        - [X] Hero
-        - [X] IceHockey
-        - [X] Kangaroo
-        - [X] Krull
-        - [X] MontezumaRevenge
-        - [X] MsPacman
-        - [X] Pacman
-        - [X] Pitfall
-        - [X] Pong
-        - [X] PrivateEye
-        - [X] Q\*Bert  
-        - [X] RiverRaid  
-        - [X] RoadRunner  
-        - [X] Seaquest
-        - [X] Skiing
-        - [X] Space Invaders
-        - [X] Tennis
-        - [X] Time Pilot
-        - [X] Up n Down (in progress)
-        - [X] Venture
-        - [X] VideoPinball
-        - [ ] YarsRevenge (in progress)
-        
-        A list of all gymnasium games can be found in the [Gymnasium Documentation](https://gymnasium.farama.org/environments/atari/)
-        
-        ### The two modes of OCAtari
-        OCAtari supports two different modes to extract objects from the current state:
-        
-        **Vision Extraction Mode (VEM):** Return a list of objects currently on the screen with their X, Y, Width, Height, R, G, B Values, based on handwritten rules used on the visual representation. 
-        
-        **Ram Extraction Mode (REM):** Uses the object values stored in the RAM to detect the objects currently on the screen.
-        
-        ### Use these trained agents and the demo script:
-        
-        A better example how to run OCAtari is given with our demo files showing you how to run each game with a provided agent. 
-        
-        Use the demo files in the scripts/demo folder to test it yourself. You can set the mode to 'raw', 'vision' or 'revised' in line 10 of the demo script.
-        You can also run the demo file with an already trained agent or your own developed agent. You can use the -p flag in the command to run the demo file by an agent and let the agent play the game.
-        Here is an example: 
-        
-        `python demo_pong.py -p models/Pong/model_50000000.gz`
-        
-        More information can be found in this [ReadMe](scripts/demo/README%20Demos.md)
-        
-        ### Extract the objects from a state 
-        
-        With `env.objects` one can access the list of objects found in the current state. Note that these lists can differ depending on the mode you used initiating the environment
-        
-        ### Producing your own dataset
-        
-        OCAtari can be used to generate datasets consisting of a represenation of the current state in form of an RGB array and a list of all objects within the state. 
-        More information can be found in the dataset_generation folder. 
-        
-        ## Models and additional Information
-        
-        As trained agents as well as to reproduce our results, we recomment to use the agents of [this repo](https://github.com/floringogianu/atari-agents).  
-        
-        ### Reproducing our results
-        In most of our scripts we added the following line to make the deterministic and easier to reproduce `make_deterministic(env, 42)`. This line can and should be removed if this is not the desired behavior. 
-        As seeds we used 0 for evaluating the metrics and 42 for generating the dataset. 
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: gymnasium
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: opencv_python
+Requires-Dist: scikit_image
+Requires-Dist: termcolor
+Requires-Dist: seaborn
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: keyboard
+Requires-Dist: tqdm
+Requires-Dist: pygame
+Requires-Dist: pyfiglet
+
+# Object-Centric Atari Environments
+Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
+
+<img style="float: right;" width="400px" align="right" src="docs/_static/kangaroo.png">
+
+Inspired by thw work of [Anand et. al.](https://arxiv.org/abs/1906.08226), we present OCAtari, an improved, extended and object-centric version of their [ATARI ARI project](https://github.com/mila-iqia/atari-representation-learning). \
+The [Arcade Learning Environment](https://github.com/mgbellemare/Arcade-Learning-Environment) allows us to read the RAM state at any time of a game. 
+This repository provides a wrapper for the well known [Gynmasium project](https://github.com/Farama-Foundation/Gymnasium), that uses the state of the ram and reverse engineering to provide object centric representation of the screen. It provides code for benchmarking, testing and generating object-centric representations of states.
+
+* [Install](#install) -- Install all relevant dependencies and start using OCAtari yourself
+* [Usage](#usage) -- Learn about the different environments OCAtari supports and enables
+* [Producing your own dataset](#producing-your-own-dataset) -- OCAtari also support the generation of object-centric datasets for supported Atari games
+* [Models and additional Information](#models-and-additional-information) -- Everything you need to know to reproduce our results
+
+
+:heavy_exclamation_mark: [HERE IS A LINK TO THE DOCUMENTATION  :bookmark_tabs:](https://oc-atari.readthedocs.io/en/latest/)
+
+--- 
+
+### Structure of this repository
+This repository is structured into multiple folder:
+* [dataset_generation](dataset_generation/) -- includes all scripts needed to generate object-centric datasets for Atari game
+* [models](models/) -- includes all models needed to reproduce our results as well as to test out the environments
+* [ocatari](ocatari/) -- the actual wrapper
+* [scripts](scripts/) -- A huge amount of scripts to help and test while implementing, extending or using OCAtari. 
+Most are used to reverse engineer the RAM state, like searching for correlations within the RAM state.
+
+
+## Install
+You can install OCAtari in multiple ways, the recommended is to use the provided Dockerfile to install all requirements, like the Atari ROMs and gymnasium.
+You can also simply:
+`pip install ocatari`
+`pip install "gymnasium[atari, accept-rom-license]"`
+If you want to modify the code, you can clone this repo and run:
+`python setup.py install` or if you want to modify the code `python setup.py develop`
+
+
+## Usage
+To use the OCAtari environments:
+``` python
+from ocatari.core import OCAtari
+import random
+
+env = OCAtari("Pong", mode="ram", hud=True, render_mode="rgb_array")
+observation, info = env.reset()
+action = random.randint(0, env.nb_actions-1)
+obs, reward, terminated, truncated, info = env.step(action)
+```
+
+### Cite OCAtari:
+If you are using OCAtari for your scientific pubplease use 'ram' mode insteadlications, please cite us:
+```bibtex
+@inproceedings{Delfosse2023OCAtariOA,
+title={OCAtari: Object-Centric Atari 2600 Reinforcement Learning Environments},
+author={Quentin Delfosse and Jannis Blüml and Bjarne Gregori and Sebastian Sztwiertnia and Kristian Kersting},
+year={2023}
+}
+```
+
+###  List of covered games
+- [X] Alien
+- [X] Amidar
+- [X] Assault
+- [X] Asterix
+- [X] Asteroids  (only vision)
+- [X] Atlantis
+- [ ] BattleZone (in progress)
+- [ ] Bankheist (in progress)
+- [ ] BeamRider  (only vision)
+- [X] Berzerk
+- [X] Bowling
+- [X] Boxing
+- [X] Breakout
+- [X] Carnival
+- [X] Centipede
+- [X] Chopper Command
+- [X] Crazy Climbers
+- [X] DemonAttack
+- [X] DonkeyKong
+- [X] Fishing Derby  
+- [X] Freeway
+- [X] Frostbite
+- [X] Gopher
+- [X] Hero
+- [X] IceHockey
+- [X] Kangaroo
+- [X] Krull
+- [X] MontezumaRevenge
+- [X] MsPacman
+- [X] Pacman
+- [X] Pitfall
+- [X] Pong
+- [X] PrivateEye
+- [X] Q\*Bert  
+- [X] RiverRaid  
+- [X] RoadRunner  
+- [X] Seaquest
+- [X] Skiing
+- [X] Space Invaders
+- [X] Tennis
+- [X] Time Pilot
+- [X] Up n Down (in progress)
+- [X] Venture
+- [X] VideoPinball
+- [ ] YarsRevenge (in progress)
+
+A list of all gymnasium games can be found in the [Gymnasium Documentation](https://gymnasium.farama.org/environments/atari/)
+
+### The two modes of OCAtari
+OCAtari supports two different modes to extract objects from the current state:
+
+**Vision Extraction Mode (VEM):** Return a list of objects currently on the screen with their X, Y, Width, Height, R, G, B Values, based on handwritten rules used on the visual representation. 
+
+**Ram Extraction Mode (REM):** Uses the object values stored in the RAM to detect the objects currently on the screen.
+
+### Use these trained agents and the demo script:
+
+A better example how to run OCAtari is given with our demo files showing you how to run each game with a provided agent. 
+
+Use the demo files in the scripts/demo folder to test it yourself. You can set the mode to 'raw', 'vision' or 'revised' in line 10 of the demo script.
+You can also run the demo file with an already trained agent or your own developed agent. You can use the -p flag in the command to run the demo file by an agent and let the agent play the game.
+Here is an example: 
+
+`python demo_pong.py -p models/Pong/model_50000000.gz`
+
+More information can be found in this [ReadMe](scripts/demo/README%20Demos.md)
+
+### Extract the objects from a state 
+
+With `env.objects` one can access the list of objects found in the current state. Note that these lists can differ depending on the mode you used initiating the environment
+
+### Producing your own dataset
+
+OCAtari can be used to generate datasets consisting of a represenation of the current state in form of an RGB array and a list of all objects within the state. 
+More information can be found in the dataset_generation folder. 
+
+## Models and additional Information
+
+As trained agents as well as to reproduce our results, we recomment to use the agents of [this repo](https://github.com/floringogianu/atari-agents).  
+
+### Reproducing our results
+In most of our scripts we added the following line to make the deterministic and easier to reproduce `make_deterministic(env, 42)`. This line can and should be removed if this is not the desired behavior. 
+As seeds we used 0 for evaluating the metrics and 42 for generating the dataset. 
+
```

### Comparing `ocatari-1.0.6/ocatari.egg-info/SOURCES.txt` & `ocatari-1.0.7/ocatari.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 ocatari/ram/_helper_methods.py
 ocatari/ram/adventure.py
 ocatari/ram/alien.py
 ocatari/ram/amidar.py
 ocatari/ram/assault.py
 ocatari/ram/asterix.py
 ocatari/ram/asterix_old.py
-ocatari/ram/asterix_old2.py
 ocatari/ram/asteroids.py
 ocatari/ram/atlantis.py
 ocatari/ram/bankheist.py
 ocatari/ram/battlezone.py
 ocatari/ram/beamrider.py
 ocatari/ram/berzerk.py
 ocatari/ram/bowling.py
```

### Comparing `ocatari-1.0.6/setup.py` & `ocatari-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
```

### Comparing `ocatari-1.0.6/tests/display_game.py` & `ocatari-1.0.7/tests/display_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/display_game_both.py` & `ocatari-1.0.7/tests/display_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/get_metrics.py` & `ocatari-1.0.7/tests/get_metrics.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/metrics_utils.py` & `ocatari-1.0.7/tests/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/plot_speed_results.py` & `ocatari-1.0.7/tests/plot_speed_results.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/pong_test.py` & `ocatari-1.0.7/tests/pong_test.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/test_explanation.py` & `ocatari-1.0.7/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/test_game.py` & `ocatari-1.0.7/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/test_game_both.py` & `ocatari-1.0.7/tests/test_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/test_game_both_interactive.py` & `ocatari-1.0.7/tests/test_game_both_interactive.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.6/tests/test_speed.py` & `ocatari-1.0.7/tests/test_speed.py`

 * *Files identical despite different names*


# Comparing `tmp/ocatari-1.0.7.tar.gz` & `tmp/ocatari-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocatari-1.0.7.tar", last modified: Wed May  8 11:20:40 2024, max compression
+gzip compressed data, was "ocatari-1.0.8.tar", last modified: Wed May  8 11:37:31 2024, max compression
```

## Comparing `ocatari-1.0.7.tar` & `ocatari-1.0.8.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.980289 ocatari-1.0.7/
--rw-r--r--   0 quentin    (501) staff       (20)     1171 2024-02-29 10:31:14.000000 ocatari-1.0.7/LICENSE
--rw-r--r--   0 quentin    (501) staff       (20)     6883 2024-05-08 11:20:40.979505 ocatari-1.0.7/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)     6297 2024-03-18 21:48:49.000000 ocatari-1.0.7/README.md
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.831988 ocatari-1.0.7/ocatari/
--rw-r--r--   0 quentin    (501) staff       (20)       25 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)    26578 2024-05-08 11:15:35.000000 ocatari-1.0.7/ocatari/core.py
--rw-r--r--   0 quentin    (501) staff       (20)     2891 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/environments.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.890587 ocatari-1.0.7/ocatari/ram/
--rw-r--r--   0 quentin    (501) staff       (20)      394 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)     3297 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/_helper_methods.py
--rw-r--r--   0 quentin    (501) staff       (20)    14387 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/adventure.py
--rw-r--r--   0 quentin    (501) staff       (20)     7586 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/alien.py
--rw-r--r--   0 quentin    (501) staff       (20)     4015 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/amidar.py
--rw-r--r--   0 quentin    (501) staff       (20)    15620 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/assault.py
--rw-r--r--   0 quentin    (501) staff       (20)     5552 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/asterix.py
--rw-r--r--   0 quentin    (501) staff       (20)     9111 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/asterix_old.py
--rw-r--r--   0 quentin    (501) staff       (20)    12738 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/asteroids.py
--rw-r--r--   0 quentin    (501) staff       (20)    14088 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/atlantis.py
--rw-r--r--   0 quentin    (501) staff       (20)     4552 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/bankheist.py
--rw-r--r--   0 quentin    (501) staff       (20)    19073 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/battlezone.py
--rw-r--r--   0 quentin    (501) staff       (20)     5410 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/beamrider.py
--rw-r--r--   0 quentin    (501) staff       (20)    10096 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/berzerk.py
--rw-r--r--   0 quentin    (501) staff       (20)     5888 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/bowling.py
--rw-r--r--   0 quentin    (501) staff       (20)     5534 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/boxing.py
--rw-r--r--   0 quentin    (501) staff       (20)     7113 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/breakout.py
--rw-r--r--   0 quentin    (501) staff       (20)    11564 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/carnival.py
--rw-r--r--   0 quentin    (501) staff       (20)    11345 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/centipede.py
--rw-r--r--   0 quentin    (501) staff       (20)    29685 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/choppercommand.py
--rw-r--r--   0 quentin    (501) staff       (20)    10183 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/crazyclimber.py
--rw-r--r--   0 quentin    (501) staff       (20)     6241 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/demonattack.py
--rw-r--r--   0 quentin    (501) staff       (20)     8247 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/donkeykong.py
--rw-r--r--   0 quentin    (501) staff       (20)     2102 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/enduro.py
--rw-r--r--   0 quentin    (501) staff       (20)    17884 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/extract_ram_info.py
--rw-r--r--   0 quentin    (501) staff       (20)     2068 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/extract_ram_info_short.py
--rw-r--r--   0 quentin    (501) staff       (20)     4743 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/fishingderby.py
--rw-r--r--   0 quentin    (501) staff       (20)     3136 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/freeway.py
--rw-r--r--   0 quentin    (501) staff       (20)    12497 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/frostbite.py
--rw-r--r--   0 quentin    (501) staff       (20)     6054 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/game_objects.py
--rw-r--r--   0 quentin    (501) staff       (20)     8640 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/gopher.py
--rw-r--r--   0 quentin    (501) staff       (20)   426388 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/hero.py
--rw-r--r--   0 quentin    (501) staff       (20)     4005 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/icehockey.py
--rw-r--r--   0 quentin    (501) staff       (20)     5966 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/jamesbond.py
--rw-r--r--   0 quentin    (501) staff       (20)    13579 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/kangaroo.py
--rw-r--r--   0 quentin    (501) staff       (20)    14946 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/krull.py
--rw-r--r--   0 quentin    (501) staff       (20)    38831 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/montezumarevenge.py
--rw-r--r--   0 quentin    (501) staff       (20)     6500 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/mspacman.py
--rw-r--r--   0 quentin    (501) staff       (20)     4625 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/pacman.py
--rw-r--r--   0 quentin    (501) staff       (20)    15588 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/pitfall.py
--rw-r--r--   0 quentin    (501) staff       (20)     5915 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/pong.py
--rw-r--r--   0 quentin    (501) staff       (20)    16424 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/privateeye.py
--rw-r--r--   0 quentin    (501) staff       (20)    14403 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/qbert.py
--rw-r--r--   0 quentin    (501) staff       (20)    10623 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/riverraid.py
--rw-r--r--   0 quentin    (501) staff       (20)    13893 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/roadrunner.py
--rw-r--r--   0 quentin    (501) staff       (20)    14619 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/seaquest.py
--rw-r--r--   0 quentin    (501) staff       (20)     8491 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/skiing.py
--rw-r--r--   0 quentin    (501) staff       (20)    12411 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/ram/spaceinvaders.py
--rw-r--r--   0 quentin    (501) staff       (20)     8869 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/tennis.py
--rw-r--r--   0 quentin    (501) staff       (20)    16258 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/timepilot.py
--rw-r--r--   0 quentin    (501) staff       (20)     7136 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/upndown.py
--rw-r--r--   0 quentin    (501) staff       (20)     3036 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/ram/utils.py
--rw-r--r--   0 quentin    (501) staff       (20)     9308 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/venture.py
--rw-r--r--   0 quentin    (501) staff       (20)     5063 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/videopinball.py
--rw-r--r--   0 quentin    (501) staff       (20)     5946 2024-03-18 21:48:49.000000 ocatari-1.0.7/ocatari/ram/yarsrevenge.py
--rw-r--r--   0 quentin    (501) staff       (20)    10518 2024-05-08 11:13:31.000000 ocatari-1.0.7/ocatari/utils.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.960806 ocatari-1.0.7/ocatari/vision/
--rw-r--r--   0 quentin    (501) staff       (20)      394 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)     5880 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/adventure.py
--rw-r--r--   0 quentin    (501) staff       (20)     2888 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/alien.py
--rw-r--r--   0 quentin    (501) staff       (20)     2003 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/amidar.py
--rw-r--r--   0 quentin    (501) staff       (20)     6175 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/assault.py
--rw-r--r--   0 quentin    (501) staff       (20)     8795 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/asterix.py
--rw-r--r--   0 quentin    (501) staff       (20)     2588 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/asteroids.py
--rw-r--r--   0 quentin    (501) staff       (20)     7361 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/atlantis.py
--rw-r--r--   0 quentin    (501) staff       (20)     2106 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/bankheist.py
--rw-r--r--   0 quentin    (501) staff       (20)     4570 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/battlezone.py
--rw-r--r--   0 quentin    (501) staff       (20)     6024 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/beamrider.py
--rw-r--r--   0 quentin    (501) staff       (20)     2817 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/berzerk.py
--rw-r--r--   0 quentin    (501) staff       (20)     2486 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/bowling.py
--rw-r--r--   0 quentin    (501) staff       (20)     1812 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/boxing.py
--rw-r--r--   0 quentin    (501) staff       (20)     2992 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/breakout.py
--rw-r--r--   0 quentin    (501) staff       (20)     5182 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/carnival.py
--rw-r--r--   0 quentin    (501) staff       (20)     4292 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/centipede.py
--rw-r--r--   0 quentin    (501) staff       (20)     5801 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/choppercommand.py
--rw-r--r--   0 quentin    (501) staff       (20)     3765 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/crazyclimber.py
--rw-r--r--   0 quentin    (501) staff       (20)     3168 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/demonattack.py
--rw-r--r--   0 quentin    (501) staff       (20)     4350 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/donkeykong.py
--rw-r--r--   0 quentin    (501) staff       (20)     2418 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/enduro.py
--rw-r--r--   0 quentin    (501) staff       (20)     7526 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/extract_vision_info.py
--rw-r--r--   0 quentin    (501) staff       (20)      597 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/extract_vision_info_short.py
--rw-r--r--   0 quentin    (501) staff       (20)     5495 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/fishingderby.py
--rw-r--r--   0 quentin    (501) staff       (20)     1579 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/freeway.py
--rw-r--r--   0 quentin    (501) staff       (20)     5612 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/frostbite.py
--rw-r--r--   0 quentin    (501) staff       (20)     3683 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/game_objects.py
--rw-r--r--   0 quentin    (501) staff       (20)     3016 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/gopher.py
--rw-r--r--   0 quentin    (501) staff       (20)    11578 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/hero.py
--rw-r--r--   0 quentin    (501) staff       (20)     2639 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/icehockey.py
--rw-r--r--   0 quentin    (501) staff       (20)     4096 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/jamesbond.py
--rw-r--r--   0 quentin    (501) staff       (20)     5690 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/kangaroo.py
--rw-r--r--   0 quentin    (501) staff       (20)     8432 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/krull.py
--rw-r--r--   0 quentin    (501) staff       (20)     6525 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/montezumarevenge.py
--rw-r--r--   0 quentin    (501) staff       (20)     2631 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/mspacman.py
--rw-r--r--   0 quentin    (501) staff       (20)     2334 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/pacman.py
--rw-r--r--   0 quentin    (501) staff       (20)     7216 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/pitfall.py
--rw-r--r--   0 quentin    (501) staff       (20)     2065 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/pong.py
--rw-r--r--   0 quentin    (501) staff       (20)    10116 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/privateeye.py
--rw-r--r--   0 quentin    (501) staff       (20)     3978 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/qbert.py
--rw-r--r--   0 quentin    (501) staff       (20)     3867 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/riverraid.py
--rw-r--r--   0 quentin    (501) staff       (20)     8142 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/roadrunner.py
--rw-r--r--   0 quentin    (501) staff       (20)     4653 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/seaquest.py
--rw-r--r--   0 quentin    (501) staff       (20)     2143 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/skiing.py
--rw-r--r--   0 quentin    (501) staff       (20)     2909 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/spaceinvaders.py
--rw-r--r--   0 quentin    (501) staff       (20)     2499 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/tennis.py
--rw-r--r--   0 quentin    (501) staff       (20)     6771 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/timepilot.py
--rw-r--r--   0 quentin    (501) staff       (20)     3629 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/upndown.py
--rw-r--r--   0 quentin    (501) staff       (20)    21751 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/utils.py
--rw-r--r--   0 quentin    (501) staff       (20)     6659 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/venture.py
--rw-r--r--   0 quentin    (501) staff       (20)     4132 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/videopinball.py
--rw-r--r--   0 quentin    (501) staff       (20)     4128 2024-02-29 10:31:19.000000 ocatari-1.0.7/ocatari/vision/yarsrevenge.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.976378 ocatari-1.0.7/ocatari.egg-info/
--rw-r--r--   0 quentin    (501) staff       (20)     6883 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)     3385 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/SOURCES.txt
--rw-r--r--   0 quentin    (501) staff       (20)        1 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/dependency_links.txt
--rw-r--r--   0 quentin    (501) staff       (20)      122 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/requires.txt
--rw-r--r--   0 quentin    (501) staff       (20)       14 2024-05-08 11:20:40.000000 ocatari-1.0.7/ocatari.egg-info/top_level.txt
--rw-r--r--   0 quentin    (501) staff       (20)       38 2024-05-08 11:20:40.980481 ocatari-1.0.7/setup.cfg
--rw-r--r--   0 quentin    (501) staff       (20)     1025 2024-05-08 11:15:53.000000 ocatari-1.0.7/setup.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:20:40.973963 ocatari-1.0.7/tests/
--rw-r--r--   0 quentin    (501) staff       (20)        0 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)     2509 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/display_game.py
--rw-r--r--   0 quentin    (501) staff       (20)     4339 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/display_game_both.py
--rw-r--r--   0 quentin    (501) staff       (20)    10431 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/get_metrics.py
--rw-r--r--   0 quentin    (501) staff       (20)    10493 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/metrics_utils.py
--rw-r--r--   0 quentin    (501) staff       (20)     1673 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/plot_speed_results.py
--rw-r--r--   0 quentin    (501) staff       (20)     1604 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/pong_test.py
--rw-r--r--   0 quentin    (501) staff       (20)     1851 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/test_explanation.py
--rw-r--r--   0 quentin    (501) staff       (20)     2921 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/test_game.py
--rw-r--r--   0 quentin    (501) staff       (20)     4637 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/test_game_both.py
--rw-r--r--   0 quentin    (501) staff       (20)     5963 2024-02-29 10:31:20.000000 ocatari-1.0.7/tests/test_game_both_interactive.py
--rw-r--r--   0 quentin    (501) staff       (20)     1281 2024-03-18 21:48:50.000000 ocatari-1.0.7/tests/test_speed.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:37:31.092375 ocatari-1.0.8/
+-rw-r--r--   0 quentin    (501) staff       (20)     1171 2024-02-29 10:31:14.000000 ocatari-1.0.8/LICENSE
+-rw-r--r--   0 quentin    (501) staff       (20)     6883 2024-05-08 11:37:31.089491 ocatari-1.0.8/PKG-INFO
+-rw-r--r--   0 quentin    (501) staff       (20)     6297 2024-03-18 21:48:49.000000 ocatari-1.0.8/README.md
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:37:30.946552 ocatari-1.0.8/ocatari/
+-rw-r--r--   0 quentin    (501) staff       (20)       25 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)    26559 2024-05-08 11:36:59.000000 ocatari-1.0.8/ocatari/core.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2891 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/environments.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:37:31.005597 ocatari-1.0.8/ocatari/ram/
+-rw-r--r--   0 quentin    (501) staff       (20)      394 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/ram/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3297 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/ram/_helper_methods.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14387 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/adventure.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7586 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/alien.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4015 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/amidar.py
+-rw-r--r--   0 quentin    (501) staff       (20)    15620 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/assault.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5552 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/asterix.py
+-rw-r--r--   0 quentin    (501) staff       (20)     9111 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/ram/asterix_old.py
+-rw-r--r--   0 quentin    (501) staff       (20)    12738 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/asteroids.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14088 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/atlantis.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4552 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/bankheist.py
+-rw-r--r--   0 quentin    (501) staff       (20)    19073 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/battlezone.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5410 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/beamrider.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10096 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/berzerk.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5888 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/bowling.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5534 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/boxing.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7113 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/breakout.py
+-rw-r--r--   0 quentin    (501) staff       (20)    11564 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/carnival.py
+-rw-r--r--   0 quentin    (501) staff       (20)    11345 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/centipede.py
+-rw-r--r--   0 quentin    (501) staff       (20)    29685 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/choppercommand.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10183 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/crazyclimber.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6241 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/demonattack.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8247 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/donkeykong.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2102 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/enduro.py
+-rw-r--r--   0 quentin    (501) staff       (20)    17884 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/extract_ram_info.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2068 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/extract_ram_info_short.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4743 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/fishingderby.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3136 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/freeway.py
+-rw-r--r--   0 quentin    (501) staff       (20)    12497 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/frostbite.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6054 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/ram/game_objects.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8640 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/gopher.py
+-rw-r--r--   0 quentin    (501) staff       (20)   426388 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/hero.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4005 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/icehockey.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5966 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/jamesbond.py
+-rw-r--r--   0 quentin    (501) staff       (20)    13579 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/kangaroo.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14946 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/krull.py
+-rw-r--r--   0 quentin    (501) staff       (20)    38831 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/montezumarevenge.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6500 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/mspacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4625 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/pacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)    15588 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/pitfall.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5915 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/pong.py
+-rw-r--r--   0 quentin    (501) staff       (20)    16424 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/privateeye.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14403 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/qbert.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10623 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/riverraid.py
+-rw-r--r--   0 quentin    (501) staff       (20)    13893 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/roadrunner.py
+-rw-r--r--   0 quentin    (501) staff       (20)    14619 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/seaquest.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8491 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/skiing.py
+-rw-r--r--   0 quentin    (501) staff       (20)    12411 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/ram/spaceinvaders.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8869 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/tennis.py
+-rw-r--r--   0 quentin    (501) staff       (20)    16258 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/timepilot.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7136 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/upndown.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3036 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/ram/utils.py
+-rw-r--r--   0 quentin    (501) staff       (20)     9308 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/venture.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5063 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/videopinball.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5946 2024-03-18 21:48:49.000000 ocatari-1.0.8/ocatari/ram/yarsrevenge.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10518 2024-05-08 11:13:31.000000 ocatari-1.0.8/ocatari/utils.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:37:31.071923 ocatari-1.0.8/ocatari/vision/
+-rw-r--r--   0 quentin    (501) staff       (20)      394 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5880 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/adventure.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2888 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/alien.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2003 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/amidar.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6175 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/assault.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8795 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/asterix.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2588 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/asteroids.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7361 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/atlantis.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2106 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/bankheist.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4570 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/battlezone.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6024 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/beamrider.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2817 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/berzerk.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2486 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/bowling.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1812 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/boxing.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2992 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/breakout.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5182 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/carnival.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4292 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/centipede.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5801 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/choppercommand.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3765 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/crazyclimber.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3168 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/demonattack.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4350 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/donkeykong.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2418 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/enduro.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7526 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/extract_vision_info.py
+-rw-r--r--   0 quentin    (501) staff       (20)      597 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/extract_vision_info_short.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5495 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/fishingderby.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1579 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/freeway.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5612 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/frostbite.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3683 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/game_objects.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3016 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/gopher.py
+-rw-r--r--   0 quentin    (501) staff       (20)    11578 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/hero.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2639 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/icehockey.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4096 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/jamesbond.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5690 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/kangaroo.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8432 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/krull.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6525 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/montezumarevenge.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2631 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/mspacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2334 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/pacman.py
+-rw-r--r--   0 quentin    (501) staff       (20)     7216 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/pitfall.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2065 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/pong.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10116 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/privateeye.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3978 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/qbert.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3867 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/riverraid.py
+-rw-r--r--   0 quentin    (501) staff       (20)     8142 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/roadrunner.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4653 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/seaquest.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2143 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/skiing.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2909 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/spaceinvaders.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2499 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/tennis.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6771 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/timepilot.py
+-rw-r--r--   0 quentin    (501) staff       (20)     3629 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/upndown.py
+-rw-r--r--   0 quentin    (501) staff       (20)    21751 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/utils.py
+-rw-r--r--   0 quentin    (501) staff       (20)     6659 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/venture.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4132 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/videopinball.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4128 2024-02-29 10:31:19.000000 ocatari-1.0.8/ocatari/vision/yarsrevenge.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:37:31.088507 ocatari-1.0.8/ocatari.egg-info/
+-rw-r--r--   0 quentin    (501) staff       (20)     6883 2024-05-08 11:37:30.000000 ocatari-1.0.8/ocatari.egg-info/PKG-INFO
+-rw-r--r--   0 quentin    (501) staff       (20)     3385 2024-05-08 11:37:30.000000 ocatari-1.0.8/ocatari.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin    (501) staff       (20)        1 2024-05-08 11:37:30.000000 ocatari-1.0.8/ocatari.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin    (501) staff       (20)      122 2024-05-08 11:37:30.000000 ocatari-1.0.8/ocatari.egg-info/requires.txt
+-rw-r--r--   0 quentin    (501) staff       (20)       14 2024-05-08 11:37:30.000000 ocatari-1.0.8/ocatari.egg-info/top_level.txt
+-rw-r--r--   0 quentin    (501) staff       (20)       38 2024-05-08 11:37:31.092741 ocatari-1.0.8/setup.cfg
+-rw-r--r--   0 quentin    (501) staff       (20)     1025 2024-05-08 11:37:14.000000 ocatari-1.0.8/setup.py
+drwxr-xr-x   0 quentin    (501) staff       (20)        0 2024-05-08 11:37:31.086612 ocatari-1.0.8/tests/
+-rw-r--r--   0 quentin    (501) staff       (20)        0 2024-02-29 10:31:20.000000 ocatari-1.0.8/tests/__init__.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2509 2024-03-18 21:48:50.000000 ocatari-1.0.8/tests/display_game.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4339 2024-02-29 10:31:20.000000 ocatari-1.0.8/tests/display_game_both.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10431 2024-02-29 10:31:20.000000 ocatari-1.0.8/tests/get_metrics.py
+-rw-r--r--   0 quentin    (501) staff       (20)    10493 2024-02-29 10:31:20.000000 ocatari-1.0.8/tests/metrics_utils.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1673 2024-02-29 10:31:20.000000 ocatari-1.0.8/tests/plot_speed_results.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1604 2024-03-18 21:48:50.000000 ocatari-1.0.8/tests/pong_test.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1851 2024-03-18 21:48:50.000000 ocatari-1.0.8/tests/test_explanation.py
+-rw-r--r--   0 quentin    (501) staff       (20)     2921 2024-03-18 21:48:50.000000 ocatari-1.0.8/tests/test_game.py
+-rw-r--r--   0 quentin    (501) staff       (20)     4637 2024-02-29 10:31:20.000000 ocatari-1.0.8/tests/test_game_both.py
+-rw-r--r--   0 quentin    (501) staff       (20)     5963 2024-02-29 10:31:20.000000 ocatari-1.0.8/tests/test_game_both_interactive.py
+-rw-r--r--   0 quentin    (501) staff       (20)     1281 2024-03-18 21:48:50.000000 ocatari-1.0.8/tests/test_speed.py
```

### Comparing `ocatari-1.0.7/LICENSE` & `ocatari-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/PKG-INFO` & `ocatari-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.7
+Version: 1.0.8
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium
```

### Comparing `ocatari-1.0.7/README.md` & `ocatari-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/core.py` & `ocatari-1.0.8/ocatari/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,21 +220,21 @@
             self._state_buffer.append(
                 _zeros(84, 84, device=DEVICE, dtype=_uint8)
             )
 
     def _reset_buffer_ori(self):
         for _ in range(self.buffer_window_size):
             self._state_buffer.append(
-                _zeros(210, 160, 3, device=DEVICE, dtype=uint8)
+                _zeros(210, 160, 3, device=DEVICE, dtype=_uint8)
             )
 
     def _reset_buffer_obj(self):
         for _ in range(self.buffer_window_size):
             self._state_buffer.append(
-                torch.zeros(len(self._objects), 4, device=DEVICE, dtype=torch.uint8)
+                _zeros(len(self._objects), 4, device=DEVICE, dtype=_uint8)
             )
 
     def reset(self, *args, **kwargs):
         """
         Resets the buffer and environment to an initial internal state, returning an initial observation and info.
         See `env.reset() <https://gymnasium.farama.org/api/env/#gymnasium.Env.reset>`_ for gymnasium details.
         """
@@ -264,15 +264,15 @@
                                                device=DEVICE))
 
     def _fill_buffer_obj(self):
         tensor = []
         for obj in self._objects:
             tensor.append(np.asarray(obj.xywh))
         state = np.asarray(tensor)
-        self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
+        self._state_buffer.append(_tensor(state, dtype=_uint8,
                                                device=DEVICE))
 
     def _get_buffer_as_stack(self):
         return _stack(list(self._state_buffer), 0).unsqueeze(0).byte()
 
     window : pygame.Surface = None
     clock : pygame.time.Clock = None
```

### Comparing `ocatari-1.0.7/ocatari/environments.py` & `ocatari-1.0.8/ocatari/environments.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/_helper_methods.py` & `ocatari-1.0.8/ocatari/ram/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/adventure.py` & `ocatari-1.0.8/ocatari/ram/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/alien.py` & `ocatari-1.0.8/ocatari/ram/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/amidar.py` & `ocatari-1.0.8/ocatari/ram/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/assault.py` & `ocatari-1.0.8/ocatari/ram/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/asterix.py` & `ocatari-1.0.8/ocatari/ram/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/asterix_old.py` & `ocatari-1.0.8/ocatari/ram/asterix_old.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/asteroids.py` & `ocatari-1.0.8/ocatari/ram/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/atlantis.py` & `ocatari-1.0.8/ocatari/ram/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/bankheist.py` & `ocatari-1.0.8/ocatari/ram/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/battlezone.py` & `ocatari-1.0.8/ocatari/ram/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/beamrider.py` & `ocatari-1.0.8/ocatari/ram/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/berzerk.py` & `ocatari-1.0.8/ocatari/ram/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/bowling.py` & `ocatari-1.0.8/ocatari/ram/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/boxing.py` & `ocatari-1.0.8/ocatari/ram/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/breakout.py` & `ocatari-1.0.8/ocatari/ram/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/carnival.py` & `ocatari-1.0.8/ocatari/ram/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/centipede.py` & `ocatari-1.0.8/ocatari/ram/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/choppercommand.py` & `ocatari-1.0.8/ocatari/ram/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/crazyclimber.py` & `ocatari-1.0.8/ocatari/ram/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/demonattack.py` & `ocatari-1.0.8/ocatari/ram/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/donkeykong.py` & `ocatari-1.0.8/ocatari/ram/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/enduro.py` & `ocatari-1.0.8/ocatari/ram/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/extract_ram_info.py` & `ocatari-1.0.8/ocatari/ram/extract_ram_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/extract_ram_info_short.py` & `ocatari-1.0.8/ocatari/ram/extract_ram_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/fishingderby.py` & `ocatari-1.0.8/ocatari/ram/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/freeway.py` & `ocatari-1.0.8/ocatari/ram/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/frostbite.py` & `ocatari-1.0.8/ocatari/ram/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/game_objects.py` & `ocatari-1.0.8/ocatari/ram/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/gopher.py` & `ocatari-1.0.8/ocatari/ram/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/hero.py` & `ocatari-1.0.8/ocatari/ram/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/icehockey.py` & `ocatari-1.0.8/ocatari/ram/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/jamesbond.py` & `ocatari-1.0.8/ocatari/ram/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/kangaroo.py` & `ocatari-1.0.8/ocatari/ram/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/krull.py` & `ocatari-1.0.8/ocatari/ram/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/montezumarevenge.py` & `ocatari-1.0.8/ocatari/ram/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/mspacman.py` & `ocatari-1.0.8/ocatari/ram/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/pacman.py` & `ocatari-1.0.8/ocatari/ram/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/pitfall.py` & `ocatari-1.0.8/ocatari/ram/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/pong.py` & `ocatari-1.0.8/ocatari/ram/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/privateeye.py` & `ocatari-1.0.8/ocatari/ram/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/qbert.py` & `ocatari-1.0.8/ocatari/ram/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/riverraid.py` & `ocatari-1.0.8/ocatari/ram/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/roadrunner.py` & `ocatari-1.0.8/ocatari/ram/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/seaquest.py` & `ocatari-1.0.8/ocatari/ram/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/skiing.py` & `ocatari-1.0.8/ocatari/ram/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/spaceinvaders.py` & `ocatari-1.0.8/ocatari/ram/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/tennis.py` & `ocatari-1.0.8/ocatari/ram/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/timepilot.py` & `ocatari-1.0.8/ocatari/ram/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/upndown.py` & `ocatari-1.0.8/ocatari/ram/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/utils.py` & `ocatari-1.0.8/ocatari/ram/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/venture.py` & `ocatari-1.0.8/ocatari/ram/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/videopinball.py` & `ocatari-1.0.8/ocatari/ram/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/ram/yarsrevenge.py` & `ocatari-1.0.8/ocatari/ram/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/utils.py` & `ocatari-1.0.8/ocatari/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/adventure.py` & `ocatari-1.0.8/ocatari/vision/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/alien.py` & `ocatari-1.0.8/ocatari/vision/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/amidar.py` & `ocatari-1.0.8/ocatari/vision/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/assault.py` & `ocatari-1.0.8/ocatari/vision/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/asterix.py` & `ocatari-1.0.8/ocatari/vision/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/asteroids.py` & `ocatari-1.0.8/ocatari/vision/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/atlantis.py` & `ocatari-1.0.8/ocatari/vision/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/bankheist.py` & `ocatari-1.0.8/ocatari/vision/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/battlezone.py` & `ocatari-1.0.8/ocatari/vision/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/beamrider.py` & `ocatari-1.0.8/ocatari/vision/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/berzerk.py` & `ocatari-1.0.8/ocatari/vision/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/bowling.py` & `ocatari-1.0.8/ocatari/vision/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/boxing.py` & `ocatari-1.0.8/ocatari/vision/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/breakout.py` & `ocatari-1.0.8/ocatari/vision/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/carnival.py` & `ocatari-1.0.8/ocatari/vision/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/centipede.py` & `ocatari-1.0.8/ocatari/vision/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/choppercommand.py` & `ocatari-1.0.8/ocatari/vision/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/crazyclimber.py` & `ocatari-1.0.8/ocatari/vision/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/demonattack.py` & `ocatari-1.0.8/ocatari/vision/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/donkeykong.py` & `ocatari-1.0.8/ocatari/vision/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/enduro.py` & `ocatari-1.0.8/ocatari/vision/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/extract_vision_info.py` & `ocatari-1.0.8/ocatari/vision/extract_vision_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/extract_vision_info_short.py` & `ocatari-1.0.8/ocatari/vision/extract_vision_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/fishingderby.py` & `ocatari-1.0.8/ocatari/vision/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/freeway.py` & `ocatari-1.0.8/ocatari/vision/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/frostbite.py` & `ocatari-1.0.8/ocatari/vision/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/game_objects.py` & `ocatari-1.0.8/ocatari/vision/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/gopher.py` & `ocatari-1.0.8/ocatari/vision/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/hero.py` & `ocatari-1.0.8/ocatari/vision/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/icehockey.py` & `ocatari-1.0.8/ocatari/vision/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/jamesbond.py` & `ocatari-1.0.8/ocatari/vision/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/kangaroo.py` & `ocatari-1.0.8/ocatari/vision/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/krull.py` & `ocatari-1.0.8/ocatari/vision/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/montezumarevenge.py` & `ocatari-1.0.8/ocatari/vision/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/mspacman.py` & `ocatari-1.0.8/ocatari/vision/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/pacman.py` & `ocatari-1.0.8/ocatari/vision/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/pitfall.py` & `ocatari-1.0.8/ocatari/vision/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/pong.py` & `ocatari-1.0.8/ocatari/vision/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/privateeye.py` & `ocatari-1.0.8/ocatari/vision/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/qbert.py` & `ocatari-1.0.8/ocatari/vision/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/riverraid.py` & `ocatari-1.0.8/ocatari/vision/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/roadrunner.py` & `ocatari-1.0.8/ocatari/vision/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/seaquest.py` & `ocatari-1.0.8/ocatari/vision/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/skiing.py` & `ocatari-1.0.8/ocatari/vision/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/spaceinvaders.py` & `ocatari-1.0.8/ocatari/vision/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/tennis.py` & `ocatari-1.0.8/ocatari/vision/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/timepilot.py` & `ocatari-1.0.8/ocatari/vision/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/upndown.py` & `ocatari-1.0.8/ocatari/vision/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/utils.py` & `ocatari-1.0.8/ocatari/vision/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/venture.py` & `ocatari-1.0.8/ocatari/vision/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/videopinball.py` & `ocatari-1.0.8/ocatari/vision/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari/vision/yarsrevenge.py` & `ocatari-1.0.8/ocatari/vision/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/ocatari.egg-info/PKG-INFO` & `ocatari-1.0.8/ocatari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.7
+Version: 1.0.8
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium
```

### Comparing `ocatari-1.0.7/ocatari.egg-info/SOURCES.txt` & `ocatari-1.0.8/ocatari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/setup.py` & `ocatari-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
```

### Comparing `ocatari-1.0.7/tests/display_game.py` & `ocatari-1.0.8/tests/display_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/display_game_both.py` & `ocatari-1.0.8/tests/display_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/get_metrics.py` & `ocatari-1.0.8/tests/get_metrics.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/metrics_utils.py` & `ocatari-1.0.8/tests/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/plot_speed_results.py` & `ocatari-1.0.8/tests/plot_speed_results.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/pong_test.py` & `ocatari-1.0.8/tests/pong_test.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/test_explanation.py` & `ocatari-1.0.8/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/test_game.py` & `ocatari-1.0.8/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/test_game_both.py` & `ocatari-1.0.8/tests/test_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/test_game_both_interactive.py` & `ocatari-1.0.8/tests/test_game_both_interactive.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.7/tests/test_speed.py` & `ocatari-1.0.8/tests/test_speed.py`

 * *Files identical despite different names*


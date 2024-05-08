# Comparing `tmp/agt_server-1.5.1.tar.gz` & `tmp/agt_server-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agt_server-1.5.1.tar", last modified: Wed May  8 00:40:31 2024, max compression
+gzip compressed data, was "agt_server-1.5.2.tar", last modified: Wed May  8 02:03:14 2024, max compression
```

## Comparing `agt_server-1.5.1.tar` & `agt_server-1.5.2.tar`

### file list

```diff
@@ -1,445 +1,445 @@
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.822452 agt_server-1.5.1/
--rw-r--r--   0 johnwu     (501) staff       (20)     3537 2024-01-25 22:07:40.000000 agt_server-1.5.1/.gitignore
--rw-r--r--   0 johnwu     (501) staff       (20)     1063 2024-01-17 14:08:17.000000 agt_server-1.5.1/LICENSE
--rw-r--r--   0 johnwu     (501) staff       (20)       66 2024-01-25 21:21:35.000000 agt_server-1.5.1/MANIFEST.in
--rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-05-08 00:40:31.822182 agt_server-1.5.1/PKG-INFO
--rw-r--r--   0 johnwu     (501) staff       (20)     5853 2024-02-06 19:53:48.000000 agt_server-1.5.1/README.md
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.722945 agt_server-1.5.1/data/
--rw-r--r--   0 johnwu     (501) staff       (20)    80155 2024-01-23 17:19:42.000000 agt_server-1.5.1/data/profile.svg
--rw-r--r--   0 johnwu     (501) staff       (20)       63 2024-04-21 07:32:05.000000 agt_server-1.5.1/requirements.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       38 2024-05-08 00:40:31.822494 agt_server-1.5.1/setup.cfg
--rw-r--r--   0 johnwu     (501) staff       (20)     1176 2024-05-08 00:40:12.000000 agt_server-1.5.1/setup.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.724003 agt_server-1.5.1/src/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:10.000000 agt_server-1.5.1/src/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.724103 agt_server-1.5.1/src/agt_server/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:24.000000 agt_server-1.5.1/src/agt_server/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.724827 agt_server-1.5.1/src/agt_server/agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/agents/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.727710 agt_server-1.5.1/src/agt_server/agents/base_agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2328 2024-04-24 01:52:33.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1917 2024-02-26 02:01:22.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/bos_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     8115 2024-02-26 02:01:35.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/bosii_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1875 2024-02-26 02:01:43.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/chicken_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     6043 2024-02-10 11:47:44.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/cm_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)    12373 2024-04-27 03:33:03.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/game_report.py
--rw-r--r--   0 johnwu     (501) staff       (20)    10046 2024-03-31 16:34:04.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/lemonade_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)    20201 2024-05-02 22:54:31.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/lsvm_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1969 2024-02-26 02:02:18.000000 agt_server-1.5.1/src/agt_server/agents/base_agents/rps_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.728081 agt_server-1.5.1/src/agt_server/agents/test_agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.713422 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.728306 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/always_compromise/
--rw-r--r--   0 johnwu     (501) staff       (20)     1636 2024-01-25 21:04:23.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.728645 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/always_stubborn/
--rw-r--r--   0 johnwu     (501) staff       (20)     1600 2024-01-25 21:04:29.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.728852 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/anti_punitive/
--rw-r--r--   0 johnwu     (501) staff       (20)     1755 2024-01-25 21:04:34.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.729258 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/fishing_chip/
--rw-r--r--   0 johnwu     (501) staff       (20)     1996 2024-01-25 21:04:39.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.729616 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/punitive_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2211 2024-01-25 21:04:43.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.729832 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1618 2024-01-25 21:04:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.730049 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/reluctant_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1985 2024-01-25 21:04:54.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.730195 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1541 2024-01-25 21:05:00.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.730338 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:05:04.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.730480 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1586 2024-01-25 21:05:08.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.730624 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:05:13.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.730784 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1575 2024-01-25 21:05:17.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.731003 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1591 2024-01-25 21:05:22.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.714806 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.731146 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/always_compromise/
--rw-r--r--   0 johnwu     (501) staff       (20)     1679 2024-01-25 21:05:44.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.731477 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/always_stubborn/
--rw-r--r--   0 johnwu     (501) staff       (20)     1658 2024-01-25 21:05:47.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.732762 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/anti_punitive/
--rw-r--r--   0 johnwu     (501) staff       (20)     1813 2024-01-25 21:05:53.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.733069 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/chipping_fish/
--rw-r--r--   0 johnwu     (501) staff       (20)     3915 2024-01-25 21:05:57.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.733246 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     4518 2024-01-25 21:06:03.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.733563 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     4667 2024-01-25 21:06:09.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.733884 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/fishing_chip/
--rw-r--r--   0 johnwu     (501) staff       (20)     2054 2024-01-25 21:06:13.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.734131 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/mystery/
--rw-r--r--   0 johnwu     (501) staff       (20)     3403 2024-01-25 21:06:17.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.734459 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/punitive_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2263 2024-01-30 22:46:02.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.734697 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2993 2024-01-25 21:06:27.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.734939 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1676 2024-01-25 21:06:31.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.735185 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/reluctant_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2041 2024-01-25 21:06:36.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.735394 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2474 2024-01-25 21:06:40.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.735636 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1604 2024-01-25 21:06:44.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.735920 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1628 2024-01-25 21:06:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.736368 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1649 2024-01-25 21:06:53.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.736510 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1632 2024-01-25 21:06:57.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.736650 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1693 2024-01-25 21:07:01.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.736783 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1654 2024-01-25 21:07:07.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.736917 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.737013 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/always_continue/
--rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:09:10.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.737276 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/always_swerve/
--rw-r--r--   0 johnwu     (501) staff       (20)     1605 2024-01-25 21:09:14.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.737719 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/basic_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:09:07.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/basic_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1708 2024-01-25 21:09:18.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.737864 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     3331 2024-01-25 21:09:23.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.738117 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     3252 2024-01-25 21:09:28.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.739519 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-05 15:59:43.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2890 2024-01-25 21:09:36.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:52.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-05 15:59:58.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.740864 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:24:35.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3075 2024-01-25 21:09:42.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:45:02.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:24:35.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.741158 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/mystery_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:17:17.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/mystery_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1993 2024-01-25 21:09:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.742252 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:30:36.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3219 2024-01-25 21:09:54.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:25.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:30:36.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.742451 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1629 2024-01-25 21:09:59.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.742703 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:10:03.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.743083 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1587 2024-01-25 21:10:07.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.743219 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1612 2024-01-25 21:10:11.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.743353 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1648 2024-01-25 21:10:15.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.743597 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1521 2024-01-25 21:10:19.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.744052 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1613 2024-01-25 21:10:25.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.744888 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:41:39.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.749875 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/always_stay/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:09.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/always_stay/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-02-15 18:47:18.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.750837 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/best_respond_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-15 18:47:54.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.751301 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/circular_hotel/
--rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-15 18:48:36.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.751746 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:15.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-15 18:48:57.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.752119 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/del_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-15 18:49:07.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.752449 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/dumb_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)     1975 2024-02-15 18:49:21.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.752787 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     7288 2024-02-15 18:49:40.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.755020 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/etch_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     3073 2024-02-15 18:50:03.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.755764 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/eyes_out/
--rw-r--r--   0 johnwu     (501) staff       (20)     2418 2024-02-15 18:50:12.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.756100 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/good_bot/
--rw-r--r--   0 johnwu     (501) staff       (20)     2088 2024-02-15 18:50:23.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.756529 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/hi_bot/
--rw-r--r--   0 johnwu     (501) staff       (20)     2798 2024-02-15 18:50:37.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.757359 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/increment_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:22.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/increment_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1614 2024-02-15 18:50:57.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.757763 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/jimbus/
--rw-r--r--   0 johnwu     (501) staff       (20)     2284 2024-02-15 18:51:08.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.758239 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/kamen_rider/
--rw-r--r--   0 johnwu     (501) staff       (20)     2588 2024-02-15 18:51:19.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.758515 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/q_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     3798 2024-02-15 18:51:31.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.758796 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-02-15 18:51:42.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.759029 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/spinner/
--rw-r--r--   0 johnwu     (501) staff       (20)     2056 2024-02-15 18:51:51.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.759277 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1485 2024-02-15 18:52:13.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.759669 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1515 2024-02-15 18:52:23.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.759931 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:52:30.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.760157 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-15 18:52:44.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.760673 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1533 2024-02-15 18:52:57.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.760836 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1531 2024-02-15 18:53:11.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.761211 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/stick_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:20:02.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/stick_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:53:22.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.761374 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/sticky/
--rw-r--r--   0 johnwu     (501) staff       (20)     2441 2024-02-15 18:53:32.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.761520 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/team_player/
--rw-r--r--   0 johnwu     (501) staff       (20)     3659 2024-02-15 18:53:44.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.761709 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/zenly/
--rw-r--r--   0 johnwu     (501) staff       (20)     3045 2024-02-15 18:53:56.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.718808 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.762004 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:10:52.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-04-01 18:00:21.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.762227 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-18 02:11:06.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.762458 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/
--rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-18 02:11:20.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.762757 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:11:25.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-18 02:11:25.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.762949 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/del_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-22 06:12:46.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.763189 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-22 06:07:27.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.763564 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-22 06:12:45.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.763815 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:39:15.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.764394 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:54.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:01.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1304 2024-04-24 02:15:23.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.765133 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:59.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:42.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1259 2024-04-02 19:34:13.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.765789 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:05.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:45:45.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1277 2024-04-02 19:34:47.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.766332 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:10.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      187 2024-04-02 21:41:36.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1275 2024-04-02 18:08:23.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.766904 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:16.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      202 2024-04-02 21:46:00.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1292 2024-04-02 19:36:57.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.767646 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:22.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:46:05.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1293 2024-04-02 19:37:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.767909 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.768022 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     2954 2024-01-26 06:19:46.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.768288 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     3052 2024-01-26 05:13:48.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.768544 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1549 2024-01-25 21:15:25.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.768815 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/rock_lover/
--rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:32.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.769156 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1506 2024-01-25 21:15:38.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.769461 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:43.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.769834 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1543 2024-01-25 21:16:13.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.770220 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-01-25 21:16:18.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.770460 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1444 2024-01-25 22:02:30.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.770727 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1527 2024-01-25 21:16:28.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.771047 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/ta_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 22:14:36.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/ta_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1454 2024-01-25 21:16:33.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)      662 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/agents/test_agents/stress_test.txt
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.720228 agt_server-1.5.1/src/agt_server/configs/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.772787 agt_server-1.5.1/src/agt_server/configs/handin_configs/
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:28:03.000000 agt_server-1.5.1/src/agt_server/configs/handin_configs/bos_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      223 2024-02-22 04:27:55.000000 agt_server-1.5.1/src/agt_server/configs/handin_configs/bosii_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      231 2024-02-22 04:27:45.000000 agt_server-1.5.1/src/agt_server/configs/handin_configs/chicken_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      263 2024-03-02 19:44:48.000000 agt_server-1.5.1/src/agt_server/configs/handin_configs/lemonade_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      294 2024-04-02 18:15:54.000000 agt_server-1.5.1/src/agt_server/configs/handin_configs/lsvm_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:27:36.000000 agt_server-1.5.1/src/agt_server/configs/handin_configs/rps_config.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.774608 agt_server-1.5.1/src/agt_server/configs/server_configs/
--rw-r--r--   0 johnwu     (501) staff       (20)      603 2024-02-01 23:47:38.000000 agt_server-1.5.1/src/agt_server/configs/server_configs/bos_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      797 2024-02-06 00:46:41.000000 agt_server-1.5.1/src/agt_server/configs/server_configs/bosii_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      608 2024-02-15 16:14:51.000000 agt_server-1.5.1/src/agt_server/configs/server_configs/chicken_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      621 2024-01-30 21:38:03.000000 agt_server-1.5.1/src/agt_server/configs/server_configs/lemonade_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      623 2024-03-31 16:36:02.000000 agt_server-1.5.1/src/agt_server/configs/server_configs/lsvm_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      604 2024-01-30 21:37:55.000000 agt_server-1.5.1/src/agt_server/configs/server_configs/rps_config.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.774792 agt_server-1.5.1/src/agt_server/handin/
--rw-r--r--   0 johnwu     (501) staff       (20)     3656 2024-04-03 02:38:28.000000 agt_server-1.5.1/src/agt_server/handin/handin.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.774910 agt_server-1.5.1/src/agt_server/handin/results/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:56.000000 agt_server-1.5.1/src/agt_server/handin/results/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.775015 agt_server-1.5.1/src/agt_server/handin/results/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:49.000000 agt_server-1.5.1/src/agt_server/handin/results/bos/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.775112 agt_server-1.5.1/src/agt_server/handin/results/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:04.000000 agt_server-1.5.1/src/agt_server/handin/results/bosii/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.775217 agt_server-1.5.1/src/agt_server/handin/results/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:25.000000 agt_server-1.5.1/src/agt_server/handin/results/chicken/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.805144 agt_server-1.5.1/src/agt_server/handin/results/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)     2786 2024-02-22 23:10:32.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3094 2024-02-23 00:23:34.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3249 2024-02-26 03:46:11.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:12:09.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:13:49.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:14:53.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:21:10.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:23:39.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:25:31.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:26:34.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:27:17.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1737 2024-02-26 04:27:28.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1673 2024-02-26 04:27:55.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:28:23.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:31:07.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:32:45.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:33:29.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2631 2024-02-26 04:34:38.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2866 2024-02-26 04:55:11.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2759 2024-02-26 06:39:27.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-26 06:49:59.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2674 2024-02-26 06:59:09.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     9873 2024-02-26 23:17:30.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      526 2024-02-26 23:18:48.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2722 2024-02-26 23:36:33.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2784 2024-02-26 23:37:56.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2494 2024-02-26 23:38:30.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      219 2024-02-26 23:45:11.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:24.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:28.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-28_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:31.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:46:21.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-46-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3054 2024-02-26 23:47:10.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:47:41.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-47-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-26 23:50:39.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-50-38_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-26 23:58:51.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-58-51_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-27 00:09:44.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:09:46.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-09-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2416 2024-02-27 00:13:56.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2610 2024-02-27 00:14:32.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:19:21.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-19-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:21:53.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-21-53_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     4940 2024-02-27 20:26:21.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3215 2024-02-27 20:27:18.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     7406 2024-02-27 20:32:27.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3367 2024-02-27 20:33:47.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     7165 2024-02-27 20:36:53.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6897 2024-02-27 20:40:29.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5795 2024-02-27 20:40:37.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6689 2024-02-27 20:49:05.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    69971 2024-02-28 04:53:17.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    42190 2024-02-28 08:28:23.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    38084 2024-02-28 10:04:34.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    38027 2024-02-28 11:31:24.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5240 2024-02-28 11:34:41.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1921 2024-02-28 11:35:40.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     8899 2024-02-28 11:42:21.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    39034 2024-02-28 14:22:14.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    74776 2024-02-28 19:14:37.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5920 2024-02-28 21:11:22.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5102 2024-02-28 21:13:24.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     4669 2024-02-28 21:16:32.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5107 2024-02-28 21:19:34.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    16781 2024-02-28 21:40:00.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    15945 2024-02-28 21:51:18.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    17789 2024-02-28 22:18:47.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    15831 2024-02-28 22:55:20.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3939 2024-03-01 00:34:13.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    14259 2024-03-01 00:45:25.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3812 2024-03-01 00:46:34.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3998 2024-03-01 00:48:27.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6081 2024-03-01 01:51:10.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     9474 2024-03-01 01:52:08.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     8767 2024-03-01 01:52:36.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5900 2024-03-01 01:54:12.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    12641 2024-03-01 02:00:54.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    33503 2024-03-01 03:09:35.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    31050 2024-03-01 05:10:15.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    18142 2024-03-01 05:31:08.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    18785 2024-03-01 06:24:52.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    19642 2024-03-01 07:22:31.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3325 2024-03-01 07:22:31.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/LemonadeArena.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3900 2024-02-26 04:14:53.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/LemonadeTest.txt
--rw-r--r--   0 johnwu     (501) staff       (20)   785905 2024-03-01 23:54:21.000000 agt_server-1.5.1/src/agt_server/handin/results/lemonade/shortcut.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.807261 agt_server-1.5.1/src/agt_server/handin/results/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:14.000000 agt_server-1.5.1/src/agt_server/handin/results/rps/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.813794 agt_server-1.5.1/src/agt_server/local_games/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/local_games/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2334 2024-04-17 23:51:57.000000 agt_server-1.5.1/src/agt_server/local_games/base.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9604 2024-02-15 18:16:30.000000 agt_server-1.5.1/src/agt_server/local_games/bos_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    10213 2024-02-15 18:16:15.000000 agt_server-1.5.1/src/agt_server/local_games/bosii_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9731 2024-02-15 18:17:49.000000 agt_server-1.5.1/src/agt_server/local_games/chicken_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    17831 2024-04-02 02:32:20.000000 agt_server-1.5.1/src/agt_server/local_games/lemonade_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    26523 2024-05-08 00:39:44.000000 agt_server-1.5.1/src/agt_server/local_games/lsvm_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9703 2024-02-15 18:17:04.000000 agt_server-1.5.1/src/agt_server/local_games/rps_arena.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.814184 agt_server-1.5.1/src/agt_server/server/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/server/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.816636 agt_server-1.5.1/src/agt_server/server/games/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.1/src/agt_server/server/games/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      596 2024-01-31 02:48:39.000000 agt_server-1.5.1/src/agt_server/server/games/bos_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    18510 2024-01-30 21:30:44.000000 agt_server-1.5.1/src/agt_server/server/games/bosii_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      606 2024-01-25 21:17:28.000000 agt_server-1.5.1/src/agt_server/server/games/chicken_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    16908 2024-01-30 21:34:09.000000 agt_server-1.5.1/src/agt_server/server/games/complete_2x2_matrix_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      710 2024-01-23 13:08:08.000000 agt_server-1.5.1/src/agt_server/server/games/game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    19180 2024-01-30 21:32:26.000000 agt_server-1.5.1/src/agt_server/server/games/lemonade_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      671 2024-01-25 21:17:39.000000 agt_server-1.5.1/src/agt_server/server/games/rps_game.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.816892 agt_server-1.5.1/src/agt_server/server/results/
--rw-r--r--   0 johnwu     (501) staff       (20)       18 2024-01-25 18:51:20.000000 agt_server-1.5.1/src/agt_server/server/results/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.817907 agt_server-1.5.1/src/agt_server/server/results/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:35.000000 agt_server-1.5.1/src/agt_server/server/results/bos/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.818006 agt_server-1.5.1/src/agt_server/server/results/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:39.000000 agt_server-1.5.1/src/agt_server/server/results/bosii/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.818100 agt_server-1.5.1/src/agt_server/server/results/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:43.000000 agt_server-1.5.1/src/agt_server/server/results/chicken/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.818191 agt_server-1.5.1/src/agt_server/server/results/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:49.000000 agt_server-1.5.1/src/agt_server/server/results/lemonade/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.818281 agt_server-1.5.1/src/agt_server/server/results/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:54.000000 agt_server-1.5.1/src/agt_server/server/results/rps/.gitkeep
--rw-r--r--   0 johnwu     (501) staff       (20)    23118 2024-02-15 16:20:24.000000 agt_server-1.5.1/src/agt_server/server/server.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.724706 agt_server-1.5.1/src/agt_server.egg-info/
--rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-05-08 00:40:31.000000 agt_server-1.5.1/src/agt_server.egg-info/PKG-INFO
--rw-r--r--   0 johnwu     (501) staff       (20)    18184 2024-05-08 00:40:31.000000 agt_server-1.5.1/src/agt_server.egg-info/SOURCES.txt
--rw-r--r--   0 johnwu     (501) staff       (20)        1 2024-05-08 00:40:31.000000 agt_server-1.5.1/src/agt_server.egg-info/dependency_links.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       62 2024-05-08 00:40:31.000000 agt_server-1.5.1/src/agt_server.egg-info/requires.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       11 2024-05-08 00:40:31.000000 agt_server-1.5.1/src/agt_server.egg-info/top_level.txt
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.721583 agt_server-1.5.1/test/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.721874 agt_server-1.5.1/test/server_test/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.818810 agt_server-1.5.1/test/server_test/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)     7014 2024-01-25 21:24:06.000000 agt_server-1.5.1/test/server_test/bos/bos_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     8015 2024-01-25 21:22:03.000000 agt_server-1.5.1/test/server_test/bos/bos_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.819517 agt_server-1.5.1/test/server_test/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)    10139 2024-01-25 21:26:19.000000 agt_server-1.5.1/test/server_test/bosii/bosii_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    11361 2024-01-25 21:28:31.000000 agt_server-1.5.1/test/server_test/bosii/bosii_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.820115 agt_server-1.5.1/test/server_test/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)    10276 2024-01-25 21:35:28.000000 agt_server-1.5.1/test/server_test/chicken/chicken_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    11631 2024-01-25 21:50:35.000000 agt_server-1.5.1/test/server_test/chicken/chicken_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.821094 agt_server-1.5.1/test/server_test/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)    13981 2024-01-25 21:53:38.000000 agt_server-1.5.1/test/server_test/lemonade/lemonade_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     8108 2024-01-25 21:56:56.000000 agt_server-1.5.1/test/server_test/lemonade/lemonade_ql.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    16031 2024-01-25 21:58:30.000000 agt_server-1.5.1/test/server_test/lemonade/lemonade_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 00:40:31.821665 agt_server-1.5.1/test/server_test/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)     5940 2024-01-25 22:00:19.000000 agt_server-1.5.1/test/server_test/rps/rps_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     6884 2024-01-25 22:00:40.000000 agt_server-1.5.1/test/server_test/rps/rps_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.130596 agt_server-1.5.2/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3537 2024-01-25 22:07:40.000000 agt_server-1.5.2/.gitignore
+-rw-r--r--   0 johnwu     (501) staff       (20)     1063 2024-01-17 14:08:17.000000 agt_server-1.5.2/LICENSE
+-rw-r--r--   0 johnwu     (501) staff       (20)       66 2024-01-25 21:21:35.000000 agt_server-1.5.2/MANIFEST.in
+-rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-05-08 02:03:14.130389 agt_server-1.5.2/PKG-INFO
+-rw-r--r--   0 johnwu     (501) staff       (20)     5853 2024-02-06 19:53:48.000000 agt_server-1.5.2/README.md
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.048046 agt_server-1.5.2/data/
+-rw-r--r--   0 johnwu     (501) staff       (20)    80155 2024-01-23 17:19:42.000000 agt_server-1.5.2/data/profile.svg
+-rw-r--r--   0 johnwu     (501) staff       (20)       63 2024-04-21 07:32:05.000000 agt_server-1.5.2/requirements.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       38 2024-05-08 02:03:14.130641 agt_server-1.5.2/setup.cfg
+-rw-r--r--   0 johnwu     (501) staff       (20)     1176 2024-05-08 02:03:06.000000 agt_server-1.5.2/setup.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.048915 agt_server-1.5.2/src/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:10.000000 agt_server-1.5.2/src/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.049031 agt_server-1.5.2/src/agt_server/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:24.000000 agt_server-1.5.2/src/agt_server/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.049814 agt_server-1.5.2/src/agt_server/agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/agents/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.052263 agt_server-1.5.2/src/agt_server/agents/base_agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2328 2024-04-24 01:52:33.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1917 2024-02-26 02:01:22.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/bos_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     8115 2024-02-26 02:01:35.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/bosii_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1875 2024-02-26 02:01:43.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/chicken_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     6043 2024-02-10 11:47:44.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/cm_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    12373 2024-04-27 03:33:03.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/game_report.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    10046 2024-03-31 16:34:04.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/lemonade_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    20201 2024-05-02 22:54:31.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/lsvm_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1969 2024-02-26 02:02:18.000000 agt_server-1.5.2/src/agt_server/agents/base_agents/rps_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.052607 agt_server-1.5.2/src/agt_server/agents/test_agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.038171 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.052829 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/always_compromise/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1636 2024-01-25 21:04:23.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.053168 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/always_stubborn/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1600 2024-01-25 21:04:29.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.053402 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/anti_punitive/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1755 2024-01-25 21:04:34.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.053728 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/fishing_chip/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1996 2024-01-25 21:04:39.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.054022 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/punitive_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2211 2024-01-25 21:04:43.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.054232 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1618 2024-01-25 21:04:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.054443 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/reluctant_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1985 2024-01-25 21:04:54.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.054600 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1541 2024-01-25 21:05:00.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.054752 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:05:04.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.054903 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1586 2024-01-25 21:05:08.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.055056 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:05:13.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.055199 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1575 2024-01-25 21:05:17.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.055413 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1591 2024-01-25 21:05:22.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.039907 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.055558 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/always_compromise/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1679 2024-01-25 21:05:44.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.055885 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/always_stubborn/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1658 2024-01-25 21:05:47.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.056107 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/anti_punitive/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1813 2024-01-25 21:05:53.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.056332 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/chipping_fish/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3915 2024-01-25 21:05:57.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.056480 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     4518 2024-01-25 21:06:03.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.056770 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     4667 2024-01-25 21:06:09.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.057051 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/fishing_chip/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2054 2024-01-25 21:06:13.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.057307 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/mystery/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3403 2024-01-25 21:06:17.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.057625 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/punitive_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2263 2024-01-30 22:46:02.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.057868 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2993 2024-01-25 21:06:27.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.058119 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1676 2024-01-25 21:06:31.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.058359 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/reluctant_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2041 2024-01-25 21:06:36.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.058589 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2474 2024-01-25 21:06:40.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.058831 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1604 2024-01-25 21:06:44.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.059115 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1628 2024-01-25 21:06:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.059550 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1649 2024-01-25 21:06:53.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.059698 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1632 2024-01-25 21:06:57.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.059841 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1693 2024-01-25 21:07:01.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.059980 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1654 2024-01-25 21:07:07.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.060121 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.060212 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/always_continue/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:09:10.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.060359 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/always_swerve/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1605 2024-01-25 21:09:14.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.060790 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/basic_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:09:07.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/basic_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1708 2024-01-25 21:09:18.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.060941 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3331 2024-01-25 21:09:23.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.061186 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3252 2024-01-25 21:09:28.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.062385 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-05 15:59:43.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2890 2024-01-25 21:09:36.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:52.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-05 15:59:58.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.063821 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:24:35.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3075 2024-01-25 21:09:42.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:45:02.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:24:35.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.064214 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/mystery_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:17:17.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/mystery_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1993 2024-01-25 21:09:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.065555 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:30:36.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3219 2024-01-25 21:09:54.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:25.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:30:36.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.065796 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1629 2024-01-25 21:09:59.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.065971 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:10:03.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.066410 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1587 2024-01-25 21:10:07.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.066622 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1612 2024-01-25 21:10:11.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.066799 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1648 2024-01-25 21:10:15.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.066969 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1521 2024-01-25 21:10:19.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.067250 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1613 2024-01-25 21:10:25.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.067424 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:41:39.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.067640 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/always_stay/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:09.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/always_stay/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-02-15 18:47:18.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.067915 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/best_respond_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-15 18:47:54.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.068158 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/circular_hotel/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-15 18:48:36.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.068539 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:15.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-15 18:48:57.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.068821 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/del_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-15 18:49:07.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.069087 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/dumb_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1975 2024-02-15 18:49:21.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.069374 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     7288 2024-02-15 18:49:40.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.069690 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/etch_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3073 2024-02-15 18:50:03.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.069954 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/eyes_out/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2418 2024-02-15 18:50:12.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.070170 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/good_bot/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2088 2024-02-15 18:50:23.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.070468 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/hi_bot/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2798 2024-02-15 18:50:37.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.070789 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/increment_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:22.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/increment_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1614 2024-02-15 18:50:57.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.071078 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/jimbus/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2284 2024-02-15 18:51:08.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.071313 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/kamen_rider/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2588 2024-02-15 18:51:19.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.071608 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/q_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3798 2024-02-15 18:51:31.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.071853 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-02-15 18:51:42.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.073817 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/spinner/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2056 2024-02-15 18:51:51.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.074096 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1485 2024-02-15 18:52:13.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.074384 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1515 2024-02-15 18:52:23.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.074709 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:52:30.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.075111 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-15 18:52:44.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.075326 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1533 2024-02-15 18:52:57.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.075507 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1531 2024-02-15 18:53:11.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.075896 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/stick_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:20:02.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/stick_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:53:22.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.076115 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/sticky/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2441 2024-02-15 18:53:32.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.076292 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/team_player/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3659 2024-02-15 18:53:44.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.076466 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/zenly/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3045 2024-02-15 18:53:56.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.043787 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.076724 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:10:52.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-04-01 18:00:21.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.076963 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-18 02:11:06.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.077194 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-18 02:11:20.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.077500 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:11:25.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-18 02:11:25.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.077691 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/del_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-22 06:12:46.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.077944 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-22 06:07:27.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.078199 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-22 06:12:45.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.078460 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:39:15.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.079034 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:54.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:01.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1304 2024-04-24 02:15:23.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.080003 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:59.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:42.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1259 2024-04-02 19:34:13.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.080624 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:05.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:45:45.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1277 2024-04-02 19:34:47.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.081092 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:10.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      187 2024-04-02 21:41:36.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1275 2024-04-02 18:08:23.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.081596 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:16.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      202 2024-04-02 21:46:00.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1292 2024-04-02 19:36:57.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.082403 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:22.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:46:05.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1293 2024-04-02 19:37:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.082648 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.082799 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2954 2024-01-26 06:19:46.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.083122 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3052 2024-01-26 05:13:48.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.083372 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1549 2024-01-25 21:15:25.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.083640 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/rock_lover/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:32.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.083954 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1506 2024-01-25 21:15:38.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.084234 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:43.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.084522 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1543 2024-01-25 21:16:13.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.084790 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-01-25 21:16:18.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.085013 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1444 2024-01-25 22:02:30.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.085269 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1527 2024-01-25 21:16:28.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.085571 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/ta_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 22:14:36.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/ta_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1454 2024-01-25 21:16:33.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      662 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/agents/test_agents/stress_test.txt
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.045400 agt_server-1.5.2/src/agt_server/configs/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.086909 agt_server-1.5.2/src/agt_server/configs/handin_configs/
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:28:03.000000 agt_server-1.5.2/src/agt_server/configs/handin_configs/bos_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      223 2024-02-22 04:27:55.000000 agt_server-1.5.2/src/agt_server/configs/handin_configs/bosii_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      231 2024-02-22 04:27:45.000000 agt_server-1.5.2/src/agt_server/configs/handin_configs/chicken_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      263 2024-03-02 19:44:48.000000 agt_server-1.5.2/src/agt_server/configs/handin_configs/lemonade_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      294 2024-04-02 18:15:54.000000 agt_server-1.5.2/src/agt_server/configs/handin_configs/lsvm_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:27:36.000000 agt_server-1.5.2/src/agt_server/configs/handin_configs/rps_config.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.088547 agt_server-1.5.2/src/agt_server/configs/server_configs/
+-rw-r--r--   0 johnwu     (501) staff       (20)      603 2024-02-01 23:47:38.000000 agt_server-1.5.2/src/agt_server/configs/server_configs/bos_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      797 2024-02-06 00:46:41.000000 agt_server-1.5.2/src/agt_server/configs/server_configs/bosii_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      608 2024-02-15 16:14:51.000000 agt_server-1.5.2/src/agt_server/configs/server_configs/chicken_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      621 2024-01-30 21:38:03.000000 agt_server-1.5.2/src/agt_server/configs/server_configs/lemonade_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      623 2024-03-31 16:36:02.000000 agt_server-1.5.2/src/agt_server/configs/server_configs/lsvm_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      604 2024-01-30 21:37:55.000000 agt_server-1.5.2/src/agt_server/configs/server_configs/rps_config.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.088737 agt_server-1.5.2/src/agt_server/handin/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3656 2024-04-03 02:38:28.000000 agt_server-1.5.2/src/agt_server/handin/handin.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.088868 agt_server-1.5.2/src/agt_server/handin/results/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:56.000000 agt_server-1.5.2/src/agt_server/handin/results/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.088991 agt_server-1.5.2/src/agt_server/handin/results/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:49.000000 agt_server-1.5.2/src/agt_server/handin/results/bos/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.089085 agt_server-1.5.2/src/agt_server/handin/results/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:04.000000 agt_server-1.5.2/src/agt_server/handin/results/bosii/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.089196 agt_server-1.5.2/src/agt_server/handin/results/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:25.000000 agt_server-1.5.2/src/agt_server/handin/results/chicken/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.116331 agt_server-1.5.2/src/agt_server/handin/results/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2786 2024-02-22 23:10:32.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3094 2024-02-23 00:23:34.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3249 2024-02-26 03:46:11.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:12:09.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:13:49.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:14:53.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:21:10.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:23:39.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:25:31.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:26:34.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:27:17.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1737 2024-02-26 04:27:28.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1673 2024-02-26 04:27:55.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:28:23.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:31:07.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:32:45.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:33:29.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2631 2024-02-26 04:34:38.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2866 2024-02-26 04:55:11.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2759 2024-02-26 06:39:27.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-26 06:49:59.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2674 2024-02-26 06:59:09.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     9873 2024-02-26 23:17:30.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      526 2024-02-26 23:18:48.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2722 2024-02-26 23:36:33.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2784 2024-02-26 23:37:56.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2494 2024-02-26 23:38:30.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      219 2024-02-26 23:45:11.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:24.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:28.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-28_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:31.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:46:21.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-46-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3054 2024-02-26 23:47:10.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:47:41.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-47-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-26 23:50:39.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-50-38_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-26 23:58:51.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-58-51_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-27 00:09:44.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:09:46.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-09-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2416 2024-02-27 00:13:56.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2610 2024-02-27 00:14:32.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:19:21.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-19-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:21:53.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-21-53_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     4940 2024-02-27 20:26:21.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3215 2024-02-27 20:27:18.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     7406 2024-02-27 20:32:27.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3367 2024-02-27 20:33:47.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     7165 2024-02-27 20:36:53.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6897 2024-02-27 20:40:29.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5795 2024-02-27 20:40:37.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6689 2024-02-27 20:49:05.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    69971 2024-02-28 04:53:17.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    42190 2024-02-28 08:28:23.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    38084 2024-02-28 10:04:34.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    38027 2024-02-28 11:31:24.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5240 2024-02-28 11:34:41.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1921 2024-02-28 11:35:40.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     8899 2024-02-28 11:42:21.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    39034 2024-02-28 14:22:14.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    74776 2024-02-28 19:14:37.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5920 2024-02-28 21:11:22.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5102 2024-02-28 21:13:24.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     4669 2024-02-28 21:16:32.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5107 2024-02-28 21:19:34.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    16781 2024-02-28 21:40:00.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    15945 2024-02-28 21:51:18.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    17789 2024-02-28 22:18:47.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    15831 2024-02-28 22:55:20.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3939 2024-03-01 00:34:13.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    14259 2024-03-01 00:45:25.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3812 2024-03-01 00:46:34.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3998 2024-03-01 00:48:27.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6081 2024-03-01 01:51:10.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     9474 2024-03-01 01:52:08.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     8767 2024-03-01 01:52:36.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5900 2024-03-01 01:54:12.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    12641 2024-03-01 02:00:54.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    33503 2024-03-01 03:09:35.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    31050 2024-03-01 05:10:15.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    18142 2024-03-01 05:31:08.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    18785 2024-03-01 06:24:52.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    19642 2024-03-01 07:22:31.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3325 2024-03-01 07:22:31.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/LemonadeArena.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3900 2024-02-26 04:14:53.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/LemonadeTest.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)   785905 2024-03-01 23:54:21.000000 agt_server-1.5.2/src/agt_server/handin/results/lemonade/shortcut.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.117993 agt_server-1.5.2/src/agt_server/handin/results/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:14.000000 agt_server-1.5.2/src/agt_server/handin/results/rps/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.119884 agt_server-1.5.2/src/agt_server/local_games/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/local_games/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2334 2024-04-17 23:51:57.000000 agt_server-1.5.2/src/agt_server/local_games/base.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9604 2024-02-15 18:16:30.000000 agt_server-1.5.2/src/agt_server/local_games/bos_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    10213 2024-02-15 18:16:15.000000 agt_server-1.5.2/src/agt_server/local_games/bosii_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9731 2024-02-15 18:17:49.000000 agt_server-1.5.2/src/agt_server/local_games/chicken_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    17831 2024-04-02 02:32:20.000000 agt_server-1.5.2/src/agt_server/local_games/lemonade_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    26522 2024-05-08 02:03:02.000000 agt_server-1.5.2/src/agt_server/local_games/lsvm_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9703 2024-02-15 18:17:04.000000 agt_server-1.5.2/src/agt_server/local_games/rps_arena.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.120513 agt_server-1.5.2/src/agt_server/server/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/server/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.125838 agt_server-1.5.2/src/agt_server/server/games/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.5.2/src/agt_server/server/games/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      596 2024-01-31 02:48:39.000000 agt_server-1.5.2/src/agt_server/server/games/bos_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    18510 2024-01-30 21:30:44.000000 agt_server-1.5.2/src/agt_server/server/games/bosii_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      606 2024-01-25 21:17:28.000000 agt_server-1.5.2/src/agt_server/server/games/chicken_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    16908 2024-01-30 21:34:09.000000 agt_server-1.5.2/src/agt_server/server/games/complete_2x2_matrix_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      710 2024-01-23 13:08:08.000000 agt_server-1.5.2/src/agt_server/server/games/game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    19180 2024-01-30 21:32:26.000000 agt_server-1.5.2/src/agt_server/server/games/lemonade_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      671 2024-01-25 21:17:39.000000 agt_server-1.5.2/src/agt_server/server/games/rps_game.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.126091 agt_server-1.5.2/src/agt_server/server/results/
+-rw-r--r--   0 johnwu     (501) staff       (20)       18 2024-01-25 18:51:20.000000 agt_server-1.5.2/src/agt_server/server/results/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.126339 agt_server-1.5.2/src/agt_server/server/results/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:35.000000 agt_server-1.5.2/src/agt_server/server/results/bos/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.126441 agt_server-1.5.2/src/agt_server/server/results/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:39.000000 agt_server-1.5.2/src/agt_server/server/results/bosii/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.126534 agt_server-1.5.2/src/agt_server/server/results/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:43.000000 agt_server-1.5.2/src/agt_server/server/results/chicken/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.126629 agt_server-1.5.2/src/agt_server/server/results/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:49.000000 agt_server-1.5.2/src/agt_server/server/results/lemonade/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.126719 agt_server-1.5.2/src/agt_server/server/results/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:54.000000 agt_server-1.5.2/src/agt_server/server/results/rps/.gitkeep
+-rw-r--r--   0 johnwu     (501) staff       (20)    23118 2024-02-15 16:20:24.000000 agt_server-1.5.2/src/agt_server/server/server.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.049685 agt_server-1.5.2/src/agt_server.egg-info/
+-rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-05-08 02:03:14.000000 agt_server-1.5.2/src/agt_server.egg-info/PKG-INFO
+-rw-r--r--   0 johnwu     (501) staff       (20)    18184 2024-05-08 02:03:14.000000 agt_server-1.5.2/src/agt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)        1 2024-05-08 02:03:14.000000 agt_server-1.5.2/src/agt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       62 2024-05-08 02:03:14.000000 agt_server-1.5.2/src/agt_server.egg-info/requires.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       11 2024-05-08 02:03:14.000000 agt_server-1.5.2/src/agt_server.egg-info/top_level.txt
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.046612 agt_server-1.5.2/test/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.046968 agt_server-1.5.2/test/server_test/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.127224 agt_server-1.5.2/test/server_test/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)     7014 2024-01-25 21:24:06.000000 agt_server-1.5.2/test/server_test/bos/bos_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     8015 2024-01-25 21:22:03.000000 agt_server-1.5.2/test/server_test/bos/bos_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.127860 agt_server-1.5.2/test/server_test/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)    10139 2024-01-25 21:26:19.000000 agt_server-1.5.2/test/server_test/bosii/bosii_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    11361 2024-01-25 21:28:31.000000 agt_server-1.5.2/test/server_test/bosii/bosii_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.128372 agt_server-1.5.2/test/server_test/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)    10276 2024-01-25 21:35:28.000000 agt_server-1.5.2/test/server_test/chicken/chicken_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    11631 2024-01-25 21:50:35.000000 agt_server-1.5.2/test/server_test/chicken/chicken_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.129252 agt_server-1.5.2/test/server_test/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)    13981 2024-01-25 21:53:38.000000 agt_server-1.5.2/test/server_test/lemonade/lemonade_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     8108 2024-01-25 21:56:56.000000 agt_server-1.5.2/test/server_test/lemonade/lemonade_ql.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    16031 2024-01-25 21:58:30.000000 agt_server-1.5.2/test/server_test/lemonade/lemonade_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-05-08 02:03:14.129860 agt_server-1.5.2/test/server_test/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)     5940 2024-01-25 22:00:19.000000 agt_server-1.5.2/test/server_test/rps/rps_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     6884 2024-01-25 22:00:40.000000 agt_server-1.5.2/test/server_test/rps/rps_test.sh
```

### Comparing `agt_server-1.5.1/.gitignore` & `agt_server-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/LICENSE` & `agt_server-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/PKG-INFO` & `agt_server-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agt_server
-Version: 1.5.1
+Version: 1.5.2
 Summary: The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.
 Home-page: https://github.com/brown-agt/agt-server-remastered
 Author: John Wu
 Author-email: john_w_wu@brown.edu
 Project-URL: Bug Tracker, https://github.com/brown-agt/agt-server-remastered/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agt_server-1.5.1/README.md` & `agt_server-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/data/profile.svg` & `agt_server-1.5.2/data/profile.svg`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/setup.py` & `agt_server-1.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='agt_server', 
-    version='1.5.1',
+    version='1.5.2',
     author='John Wu', 
     author_email='john_w_wu@brown.edu', 
     description='The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.',  # Provide a short description
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/brown-agt/agt-server-remastered',  
     project_urls={
```

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/bos_agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/bos_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/bosii_agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/bosii_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/chicken_agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/chicken_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/cm_agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/cm_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/game_report.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/game_report.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/lemonade_agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/lemonade_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/lsvm_agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/lsvm_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/base_agents/rps_agent.py` & `agt_server-1.5.2/src/agt_server/agents/base_agents/rps_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/exponential/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py` & `agt_server-1.5.2/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/agents/test_agents/stress_test.txt` & `agt_server-1.5.2/src/agt_server/agents/test_agents/stress_test.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/configs/server_configs/bos_config.json` & `agt_server-1.5.2/src/agt_server/configs/server_configs/bos_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/configs/server_configs/bosii_config.json` & `agt_server-1.5.2/src/agt_server/configs/server_configs/bosii_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/configs/server_configs/chicken_config.json` & `agt_server-1.5.2/src/agt_server/configs/server_configs/chicken_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/configs/server_configs/lemonade_config.json` & `agt_server-1.5.2/src/agt_server/configs/server_configs/lemonade_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/configs/server_configs/lsvm_config.json` & `agt_server-1.5.2/src/agt_server/configs/server_configs/lsvm_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/configs/server_configs/rps_config.json` & `agt_server-1.5.2/src/agt_server/configs/server_configs/rps_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/handin.py` & `agt_server-1.5.2/src/agt_server/handin/handin.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/LemonadeArena.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/LemonadeArena.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/LemonadeTest.txt` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/LemonadeTest.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/handin/results/lemonade/shortcut.json` & `agt_server-1.5.2/src/agt_server/handin/results/lemonade/shortcut.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/local_games/base.py` & `agt_server-1.5.2/src/agt_server/local_games/base.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/local_games/bos_arena.py` & `agt_server-1.5.2/src/agt_server/local_games/bos_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/local_games/bosii_arena.py` & `agt_server-1.5.2/src/agt_server/local_games/bosii_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/local_games/chicken_arena.py` & `agt_server-1.5.2/src/agt_server/local_games/chicken_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/local_games/lemonade_arena.py` & `agt_server-1.5.2/src/agt_server/local_games/lemonade_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/local_games/lsvm_arena.py` & `agt_server-1.5.2/src/agt_server/local_games/lsvm_arena.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pandas as pd
 import os
 import math
 from tqdm import tqdm
 
 class LSVMArena(LocalArena):
     def __init__(self, num_cycles_per_player = 3, players=[], timeout=1, handin=False, logging_path = None, save_path = None, elo_path = "local_elo_ranking.json", local_save_path = None, num_rounds = 1000):
-        slack = 1000 
+        slack = 400 
         random_number = np.random.exponential(scale=slack / 2)
         random_number_clipped = min(max(0, random_number), slack)
         num_rounds += random_number_clipped
         num_rounds = math.ceil(num_rounds)
         super().__init__(num_rounds, players, timeout, handin, logging_path, save_path)
         self.game_name = "Spectrum Auction - Local Synergy Value Model (LSVM)"
         self.num_cycles_per_player = num_cycles_per_player
```

### Comparing `agt_server-1.5.1/src/agt_server/local_games/rps_arena.py` & `agt_server-1.5.2/src/agt_server/local_games/rps_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/games/bos_game.py` & `agt_server-1.5.2/src/agt_server/server/games/bos_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/games/bosii_game.py` & `agt_server-1.5.2/src/agt_server/server/games/bosii_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/games/chicken_game.py` & `agt_server-1.5.2/src/agt_server/server/games/chicken_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/games/complete_2x2_matrix_game.py` & `agt_server-1.5.2/src/agt_server/server/games/complete_2x2_matrix_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/games/game.py` & `agt_server-1.5.2/src/agt_server/server/games/game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/games/lemonade_game.py` & `agt_server-1.5.2/src/agt_server/server/games/lemonade_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/games/rps_game.py` & `agt_server-1.5.2/src/agt_server/server/games/rps_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server/server/server.py` & `agt_server-1.5.2/src/agt_server/server/server.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/src/agt_server.egg-info/PKG-INFO` & `agt_server-1.5.2/src/agt_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agt-server
-Version: 1.5.1
+Version: 1.5.2
 Summary: The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.
 Home-page: https://github.com/brown-agt/agt-server-remastered
 Author: John Wu
 Author-email: john_w_wu@brown.edu
 Project-URL: Bug Tracker, https://github.com/brown-agt/agt-server-remastered/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agt_server-1.5.1/src/agt_server.egg-info/SOURCES.txt` & `agt_server-1.5.2/src/agt_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/bos/bos_local_test.sh` & `agt_server-1.5.2/test/server_test/bos/bos_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/bos/bos_test.sh` & `agt_server-1.5.2/test/server_test/bos/bos_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/bosii/bosii_local_test.sh` & `agt_server-1.5.2/test/server_test/bosii/bosii_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/bosii/bosii_test.sh` & `agt_server-1.5.2/test/server_test/bosii/bosii_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/chicken/chicken_local_test.sh` & `agt_server-1.5.2/test/server_test/chicken/chicken_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/chicken/chicken_test.sh` & `agt_server-1.5.2/test/server_test/chicken/chicken_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/lemonade/lemonade_local_test.sh` & `agt_server-1.5.2/test/server_test/lemonade/lemonade_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/lemonade/lemonade_ql.sh` & `agt_server-1.5.2/test/server_test/lemonade/lemonade_ql.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/lemonade/lemonade_test.sh` & `agt_server-1.5.2/test/server_test/lemonade/lemonade_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/rps/rps_local_test.sh` & `agt_server-1.5.2/test/server_test/rps/rps_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.5.1/test/server_test/rps/rps_test.sh` & `agt_server-1.5.2/test/server_test/rps/rps_test.sh`

 * *Files identical despite different names*


# Comparing `tmp/skilleter_thingy-0.0.37.tar.gz` & `tmp/skilleter_thingy-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skilleter_thingy-0.0.37.tar", last modified: Wed May  8 12:36:33 2024, max compression
+gzip compressed data, was "skilleter_thingy-0.0.38.tar", last modified: Wed May  8 12:51:19 2024, max compression
```

## Comparing `skilleter_thingy-0.0.37.tar` & `skilleter_thingy-0.0.38.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:36:33.056764 skilleter_thingy-0.0.37/
--rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.37/LICENSE
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:36:33.056764 skilleter_thingy-0.0.37/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.37/README.md
--rw-rw-r--   0 jms       (1000) jms       (1000)     2855 2024-05-08 12:36:22.000000 skilleter_thingy-0.0.37/pyproject.toml
--rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-05-08 12:36:33.056764 skilleter_thingy-0.0.37/setup.cfg
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:36:33.048763 skilleter_thingy-0.0.37/skilleter_thingy/
--rw-rw-r--   0 jms       (1000) jms       (1000)      110 2024-05-08 12:30:06.000000 skilleter_thingy-0.0.37/skilleter_thingy/__init__.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/addpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/borger.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1781 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/console_colours.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/diskspacecheck.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3349 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/docker_purge.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    19345 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/ffind.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2480 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/ggit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5863 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/ggrep.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5799 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_br.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4963 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_ca.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    10201 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_cleanup.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8212 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_co.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1879 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_common.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4617 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_hold.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3087 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_mr.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2683 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_parent.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    51769 2024-05-08 12:34:45.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_review.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    13972 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_update.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-05-08 12:35:39.000000 skilleter_thingy-0.0.37/skilleter_thingy/git_wt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11245 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/gitcmp_helper.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8912 2024-05-08 12:09:08.000000 skilleter_thingy-0.0.37/skilleter_thingy/gitprompt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5954 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/gl.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    22035 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/gphotosync.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4310 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/linecount.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/moviemover.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4195 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/photodupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7818 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/phototidier.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/py_audit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     9474 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/readable.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4610 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/remdir.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/rmdupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2635 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/rpylint.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/splitpics.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/strreplace.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/sysmon.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    33703 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/tfm.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2988 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/tfparse.py
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:36:33.056764 skilleter_thingy-0.0.37/skilleter_thingy/thingy/
--rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-05-08 12:30:06.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/__init__.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/colour.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/dc_curses.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/dc_defaults.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/dc_util.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12264 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/dircolors.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2449 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/docker.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4257 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/files.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    38043 2024-05-08 12:10:59.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/git.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    35751 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/git2.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6079 2024-05-08 12:07:21.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/gitlab.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/logger.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4732 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/path.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/popup.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3560 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/process.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12607 2024-05-08 12:32:05.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/run.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    19814 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/tfm_pane.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/thingy/tidy.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2385 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.37/skilleter_thingy/trimpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/window_rename.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/xchmod.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.37/skilleter_thingy/yamlcheck.py
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:36:33.056764 skilleter_thingy-0.0.37/skilleter_thingy.egg-info/
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:36:33.000000 skilleter_thingy-0.0.37/skilleter_thingy.egg-info/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     2115 2024-05-08 12:36:33.000000 skilleter_thingy-0.0.37/skilleter_thingy.egg-info/SOURCES.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-05-08 12:36:33.000000 skilleter_thingy-0.0.37/skilleter_thingy.egg-info/dependency_links.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-05-08 12:36:33.000000 skilleter_thingy-0.0.37/skilleter_thingy.egg-info/entry_points.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-05-08 12:36:33.000000 skilleter_thingy-0.0.37/skilleter_thingy.egg-info/requires.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-05-08 12:36:33.000000 skilleter_thingy-0.0.37/skilleter_thingy.egg-info/top_level.txt
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:51:19.873672 skilleter_thingy-0.0.38/
+-rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.38/LICENSE
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:51:19.873672 skilleter_thingy-0.0.38/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.38/README.md
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2309 2024-05-08 12:51:11.000000 skilleter_thingy-0.0.38/pyproject.toml
+-rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-05-08 12:51:19.873672 skilleter_thingy-0.0.38/setup.cfg
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:51:19.865671 skilleter_thingy-0.0.38/src/
+-rw-rw-r--   0 jms       (1000) jms       (1000)      110 2024-05-08 12:30:06.000000 skilleter_thingy-0.0.38/src/__init__.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/addpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/borger.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1781 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/console_colours.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/diskspacecheck.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3349 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/docker_purge.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    19345 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/ffind.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2480 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/ggit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5863 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/ggrep.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5799 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_br.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4963 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_ca.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    10201 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_cleanup.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8212 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_co.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1879 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_common.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4617 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_hold.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3087 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_mr.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2683 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_parent.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    51769 2024-05-08 12:34:45.000000 skilleter_thingy-0.0.38/src/git_review.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    13972 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/git_update.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-05-08 12:35:39.000000 skilleter_thingy-0.0.38/src/git_wt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11245 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/gitcmp_helper.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8912 2024-05-08 12:09:08.000000 skilleter_thingy-0.0.38/src/gitprompt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5954 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/gl.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    22035 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/gphotosync.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4310 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/linecount.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/moviemover.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4195 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/photodupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7818 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/phototidier.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/py_audit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     9474 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/readable.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4610 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/remdir.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/rmdupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2635 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/rpylint.py
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:51:19.873672 skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:51:19.000000 skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1359 2024-05-08 12:51:19.000000 skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-05-08 12:51:19.000000 skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1425 2024-05-08 12:51:19.000000 skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/entry_points.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-05-08 12:51:19.000000 skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/requires.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)      393 2024-05-08 12:51:19.000000 skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/top_level.txt
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/splitpics.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/strreplace.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/sysmon.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    33703 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/tfm.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2988 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/tfparse.py
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:51:19.873672 skilleter_thingy-0.0.38/src/thingy/
+-rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-05-08 12:30:06.000000 skilleter_thingy-0.0.38/src/thingy/__init__.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/thingy/colour.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/thingy/dc_curses.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/thingy/dc_defaults.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/thingy/dc_util.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12264 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/thingy/dircolors.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2449 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.38/src/thingy/docker.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4257 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/thingy/files.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    38043 2024-05-08 12:10:59.000000 skilleter_thingy-0.0.38/src/thingy/git.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    35751 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/thingy/git2.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6079 2024-05-08 12:07:21.000000 skilleter_thingy-0.0.38/src/thingy/gitlab.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/thingy/logger.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4732 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/thingy/path.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/thingy/popup.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3560 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/thingy/process.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12607 2024-05-08 12:32:05.000000 skilleter_thingy-0.0.38/src/thingy/run.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    19814 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/thingy/tfm_pane.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/thingy/tidy.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2385 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.38/src/trimpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/window_rename.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/xchmod.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.38/src/yamlcheck.py
```

### Comparing `skilleter_thingy-0.0.37/LICENSE` & `skilleter_thingy-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/PKG-INFO` & `skilleter_thingy-0.0.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.37
+Version: 0.0.38
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.37/README.md` & `skilleter_thingy-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/addpath.py` & `skilleter_thingy-0.0.38/src/addpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/borger.py` & `skilleter_thingy-0.0.38/src/borger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/console_colours.py` & `skilleter_thingy-0.0.38/src/console_colours.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/diskspacecheck.py` & `skilleter_thingy-0.0.38/src/diskspacecheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/docker_purge.py` & `skilleter_thingy-0.0.38/src/docker_purge.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/ffind.py` & `skilleter_thingy-0.0.38/src/ffind.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/ggit.py` & `skilleter_thingy-0.0.38/src/ggit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/ggrep.py` & `skilleter_thingy-0.0.38/src/ggrep.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_br.py` & `skilleter_thingy-0.0.38/src/git_br.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_ca.py` & `skilleter_thingy-0.0.38/src/git_ca.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_cleanup.py` & `skilleter_thingy-0.0.38/src/git_cleanup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_co.py` & `skilleter_thingy-0.0.38/src/git_co.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_common.py` & `skilleter_thingy-0.0.38/src/git_common.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_hold.py` & `skilleter_thingy-0.0.38/src/git_hold.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_mr.py` & `skilleter_thingy-0.0.38/src/git_mr.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_parent.py` & `skilleter_thingy-0.0.38/src/git_parent.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_review.py` & `skilleter_thingy-0.0.38/src/git_review.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_update.py` & `skilleter_thingy-0.0.38/src/git_update.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/git_wt.py` & `skilleter_thingy-0.0.38/src/git_wt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/gitcmp_helper.py` & `skilleter_thingy-0.0.38/src/gitcmp_helper.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/gitprompt.py` & `skilleter_thingy-0.0.38/src/gitprompt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/gl.py` & `skilleter_thingy-0.0.38/src/gl.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/gphotosync.py` & `skilleter_thingy-0.0.38/src/gphotosync.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/linecount.py` & `skilleter_thingy-0.0.38/src/linecount.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/moviemover.py` & `skilleter_thingy-0.0.38/src/moviemover.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/photodupe.py` & `skilleter_thingy-0.0.38/src/photodupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/phototidier.py` & `skilleter_thingy-0.0.38/src/phototidier.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/py_audit.py` & `skilleter_thingy-0.0.38/src/py_audit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/readable.py` & `skilleter_thingy-0.0.38/src/readable.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/remdir.py` & `skilleter_thingy-0.0.38/src/remdir.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/rmdupe.py` & `skilleter_thingy-0.0.38/src/rmdupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/rpylint.py` & `skilleter_thingy-0.0.38/src/rpylint.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/splitpics.py` & `skilleter_thingy-0.0.38/src/splitpics.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/strreplace.py` & `skilleter_thingy-0.0.38/src/strreplace.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/sysmon.py` & `skilleter_thingy-0.0.38/src/sysmon.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/tfm.py` & `skilleter_thingy-0.0.38/src/tfm.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/tfparse.py` & `skilleter_thingy-0.0.38/src/tfparse.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/colour.py` & `skilleter_thingy-0.0.38/src/thingy/colour.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/dc_curses.py` & `skilleter_thingy-0.0.38/src/thingy/dc_curses.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/dc_defaults.py` & `skilleter_thingy-0.0.38/src/thingy/dc_defaults.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/dc_util.py` & `skilleter_thingy-0.0.38/src/thingy/dc_util.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/dircolors.py` & `skilleter_thingy-0.0.38/src/thingy/dircolors.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/docker.py` & `skilleter_thingy-0.0.38/src/thingy/docker.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/files.py` & `skilleter_thingy-0.0.38/src/thingy/files.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/git.py` & `skilleter_thingy-0.0.38/src/thingy/git.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/git2.py` & `skilleter_thingy-0.0.38/src/thingy/git2.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/gitlab.py` & `skilleter_thingy-0.0.38/src/thingy/gitlab.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/logger.py` & `skilleter_thingy-0.0.38/src/thingy/logger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/path.py` & `skilleter_thingy-0.0.38/src/thingy/path.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/popup.py` & `skilleter_thingy-0.0.38/src/thingy/popup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/process.py` & `skilleter_thingy-0.0.38/src/thingy/process.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/run.py` & `skilleter_thingy-0.0.38/src/thingy/run.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/tfm_pane.py` & `skilleter_thingy-0.0.38/src/thingy/tfm_pane.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/thingy/tidy.py` & `skilleter_thingy-0.0.38/src/thingy/tidy.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/trimpath.py` & `skilleter_thingy-0.0.38/src/trimpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/window_rename.py` & `skilleter_thingy-0.0.38/src/window_rename.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/xchmod.py` & `skilleter_thingy-0.0.38/src/xchmod.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy/yamlcheck.py` & `skilleter_thingy-0.0.38/src/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.37/skilleter_thingy.egg-info/PKG-INFO` & `skilleter_thingy-0.0.38/src/skilleter_thingy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.37
+Version: 0.0.38
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```


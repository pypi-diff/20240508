# Comparing `tmp/skilleter_thingy-0.0.28.tar.gz` & `tmp/skilleter_thingy-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skilleter_thingy-0.0.28.tar", last modified: Tue Apr 30 15:35:29 2024, max compression
+gzip compressed data, was "skilleter_thingy-0.0.29.tar", last modified: Wed May  8 12:13:41 2024, max compression
```

## Comparing `skilleter_thingy-0.0.28.tar` & `skilleter_thingy-0.0.29.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/
--rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/LICENSE
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/README.md
--rw-rw-r--   0 jms       (1000) jms       (1000)     2855 2024-04-30 15:33:43.000000 skilleter_thingy-0.0.28/pyproject.toml
--rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/setup.cfg
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/skilleter_thingy/
--rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/__init__.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/addpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/borger.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/colour.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1786 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/console_colours.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dc_curses.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dc_defaults.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dc_util.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12268 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/dircolors.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/diskspacecheck.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2453 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/docker.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3359 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/docker_purge.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    19373 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/ffind.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4261 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/files.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2493 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/ggit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5876 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/ggrep.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    38049 2024-04-30 15:33:22.000000 skilleter_thingy-0.0.28/skilleter_thingy/git.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    35764 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git2.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5812 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_br.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4981 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_ca.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    10214 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_cleanup.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8225 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_co.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1892 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_common.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4630 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_hold.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3100 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_mr.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2696 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_parent.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    51796 2024-04-30 15:35:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_review.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    13985 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_update.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3143 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/git_wt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11279 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gitcmp_helper.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6062 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gitlab.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8925 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gitprompt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5964 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gl.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    22040 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/gphotosync.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4316 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/linecount.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/logger.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/moviemover.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4737 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/path.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4195 2024-04-22 10:33:30.000000 skilleter_thingy-0.0.28/skilleter_thingy/photodupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7823 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/phototidier.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/popup.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3565 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/process.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/py_audit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     9487 2024-04-26 08:30:25.000000 skilleter_thingy-0.0.28/skilleter_thingy/readable.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4620 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/remdir.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/rmdupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2639 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/rpylint.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12619 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/run.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/splitpics.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/strreplace.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/sysmon.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    33712 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tfm.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    19829 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tfm_pane.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2993 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tfparse.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/tidy.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2397 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/trimpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/window_rename.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/xchmod.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.28/skilleter_thingy/yamlcheck.py
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-30 15:35:29.155484 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     1960 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/SOURCES.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/dependency_links.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/entry_points.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/requires.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-04-30 15:35:29.000000 skilleter_thingy-0.0.28/skilleter_thingy.egg-info/top_level.txt
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:13:41.654957 skilleter_thingy-0.0.29/
+-rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.29/LICENSE
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:13:41.650959 skilleter_thingy-0.0.29/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.29/README.md
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2855 2024-05-08 12:13:10.000000 skilleter_thingy-0.0.29/pyproject.toml
+-rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-05-08 12:13:41.654957 skilleter_thingy-0.0.29/setup.cfg
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:13:41.638964 skilleter_thingy-0.0.29/skilleter_thingy/
+-rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/__init__.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/addpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/borger.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1781 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/console_colours.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/diskspacecheck.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3349 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/docker_purge.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    19345 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/ffind.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2480 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/ggit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5863 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/ggrep.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5799 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_br.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4963 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_ca.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    10201 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_cleanup.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8212 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_co.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1879 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_common.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4617 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_hold.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3087 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_mr.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2683 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_parent.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    51769 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_review.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    13972 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_update.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3136 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/git_wt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11245 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/gitcmp_helper.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8912 2024-05-08 12:09:08.000000 skilleter_thingy-0.0.29/skilleter_thingy/gitprompt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5954 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/gl.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    22035 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/gphotosync.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4310 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/linecount.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/moviemover.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4195 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/photodupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7818 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/phototidier.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/py_audit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     9474 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/readable.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4610 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/remdir.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/rmdupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2635 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/rpylint.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/splitpics.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/strreplace.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/sysmon.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    33703 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/tfm.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2988 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/tfparse.py
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:13:41.646960 skilleter_thingy-0.0.29/skilleter_thingy/thingy/
+-rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/colour.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/dc_curses.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/dc_defaults.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/dc_util.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12264 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/dircolors.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2449 2024-05-08 12:12:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/docker.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4257 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/files.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    38043 2024-05-08 12:10:59.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/git.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    35751 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/git2.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6079 2024-05-08 12:07:21.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/gitlab.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/logger.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4732 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/path.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/popup.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3560 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/process.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12589 2024-05-08 12:07:07.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/run.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    19814 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/tfm_pane.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/thingy/tidy.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2385 2024-05-08 12:12:55.000000 skilleter_thingy-0.0.29/skilleter_thingy/trimpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/window_rename.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/xchmod.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-05-08 11:33:56.000000 skilleter_thingy-0.0.29/skilleter_thingy/yamlcheck.py
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:13:41.650959 skilleter_thingy-0.0.29/skilleter_thingy.egg-info/
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:13:41.000000 skilleter_thingy-0.0.29/skilleter_thingy.egg-info/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2079 2024-05-08 12:13:41.000000 skilleter_thingy-0.0.29/skilleter_thingy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-05-08 12:13:41.000000 skilleter_thingy-0.0.29/skilleter_thingy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-05-08 12:13:41.000000 skilleter_thingy-0.0.29/skilleter_thingy.egg-info/entry_points.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-05-08 12:13:41.000000 skilleter_thingy-0.0.29/skilleter_thingy.egg-info/requires.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-05-08 12:13:41.000000 skilleter_thingy-0.0.29/skilleter_thingy.egg-info/top_level.txt
```

### Comparing `skilleter_thingy-0.0.28/LICENSE` & `skilleter_thingy-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/PKG-INFO` & `skilleter_thingy-0.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.28
+Version: 0.0.29
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.28/README.md` & `skilleter_thingy-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/pyproject.toml` & `skilleter_thingy-0.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skilleter_thingy"
 
 # Version must be incremented to install updated Thingy
 
-version = "0.0.28"
+version = "0.0.29"
 
 authors = [
     {name="John Skilleter", email="john@skilleter.org.uk"},
 ]
 
 description = "A collection of useful utilities, mainly aimed at making Git more friendly"
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/addpath.py` & `skilleter_thingy-0.0.29/skilleter_thingy/addpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/borger.py` & `skilleter_thingy-0.0.29/skilleter_thingy/borger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/colour.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/colour.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/console_colours.py` & `skilleter_thingy-0.0.29/skilleter_thingy/console_colours.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Licence: GPL v3 or later
 """
 ################################################################################
 
 import sys
 
-from skilleter_thingy import colour
+import thingy.colour as colour
 
 ################################################################################
 
 def main():
     """ Main function - draw the colour grid """
 
     # Extended ANSI colour are slightly weird.
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/dc_curses.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/dc_curses.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/dc_defaults.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/dc_defaults.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/dc_util.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/dc_util.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/dircolors.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/dircolors.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 for terminal use, like GNU ls and dircolors. """
 
 from collections import OrderedDict
 from io import StringIO, TextIOBase
 import os
 import stat
 
-from skilleter_thingy import dc_defaults
-from skilleter_thingy import dc_util
+import thingy.dc_defaults as dc_defaults
+import thingy.dc_util as dc_util
 
 __all__ = ['Dircolors']
 
 _CODE_MAP = OrderedDict()
 def _init_code_map():
     """ mapping between the key name in the .dircolors file and the two letter
     code found in the LS_COLORS environment variable.
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/diskspacecheck.py` & `skilleter_thingy-0.0.29/skilleter_thingy/diskspacecheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/docker.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/docker.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         * Only implements functions required by docker-purge
         * Only has basic error checking, in that it raises DockerError
           for any error returned by the external docker command.
 """
 ################################################################################
 
 # TODO: Convert to use thingy.proc
-from skilleter_thingy import process
+import thingy.process as process
 
 ################################################################################
 
 class DockerError(Exception):
     """ Exception for dockery things """
 
     pass
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/docker_purge.py` & `skilleter_thingy-0.0.29/skilleter_thingy/docker_purge.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 """
 ################################################################################
 
 import sys
 import re
 import argparse
 
-from skilleter_thingy import logger
-from skilleter_thingy import docker
+import thingy.logger as logger
+import thingy.docker as docker
 
 ################################################################################
 
 def initialise():
     """ Parse the command line """
 
     parser = argparse.ArgumentParser(description='Purge docker instances and images')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/ffind.py` & `skilleter_thingy-0.0.29/skilleter_thingy/ffind.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 import grp
 import pwd
 import datetime
 import re
 import shlex
 import copy
 
-from skilleter_thingy import git
-from skilleter_thingy import logger
-from skilleter_thingy import run
-from skilleter_thingy import dircolors
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.logger as logger
+import thingy.run as run
+import thingy.dircolors as dircolors
+import thingy.colour as colour
 
 ################################################################################
 
 log = logger.init(__name__)
 
 ################################################################################
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/files.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 ################################################################################
 
 import os
 import shutil
 
 # TODO: Convert to use thingy.proc
-from skilleter_thingy import process
+import thingy.process as process
 
 ################################################################################
 
 def is_binary_file(filename):
     """ Return True if there is a strong likelihood that the specified file
         is binary. """
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/ggit.py` & `skilleter_thingy-0.0.29/skilleter_thingy/ggit.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """ Run a git command in all working trees in/under the specified subdirectory """
 
 import sys
 import os
 import subprocess
 import argparse
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 ################################################################################
 
 def run_git(args, directory, command):
     """ Run a git command in the specified directory """
 
     if not args.quiet:
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/ggrep.py` & `skilleter_thingy-0.0.29/skilleter_thingy/ggrep.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ################################################################################
 
 import os
 import re
 import sys
 import argparse
 
-from skilleter_thingy import colour
-from skilleter_thingy import git
+import thingy.colour as colour
+import thingy.git as git
 
 ################################################################################
 
 BINARY_RE = re.compile(r'(Binary file )(.*)( matches)')
 
 ################################################################################
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import shutil
 import sys
 import re
 import logging
 import fnmatch
 import subprocess
 
-from skilleter_thingy import run
-from skilleter_thingy import gitlab
+import thingy.run as run
+import thingy.gitlab as gitlab
 
 ################################################################################
 # Configuration files to access
 
 (LOCAL, GLOBAL, SYSTEM) = list(range(3))
 
 ################################################################################
@@ -43,15 +43,15 @@
 
     def __init__(self, msg, status=1):
         super().__init__(msg, status)
 
 ################################################################################
 
 def git(cmd, stdout=None, stderr=None):
-    """ Wrapper for run.run that raises a GitError instead of RunError
+    """ Wrapper for thingy.run.run that raises a GitError instead of RunError
         so that Git module users do not to include the run module just
         to get the exception.
         Optionally redirect stdout and stderr as specified. """
 
     logging.debug('Running git %s', ' '.join(cmd))
 
     try:
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git2.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/git2.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 import re
 import logging
 import fnmatch
 import subprocess
 
 import pygit2
 
-from skilleter_thingy import run
-from skilleter_thingy import gitlab
+import thingy.run as run
+import thingy.gitlab as gitlab
 
 ################################################################################
 # Configuration files to access
 
 (LOCAL, GLOBAL, SYSTEM) = list(range(3))
 
 ################################################################################
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_br.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_br.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import argparse
 import fnmatch
 import datetime
 
 from dateutil.parser import parse
 from dateutil.relativedelta import relativedelta
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 ################################################################################
 
 def parse_command_line():
     """ Parse the command line """
 
     parser = argparse.ArgumentParser(description='List or delete branches that have been merged')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_ca.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_ca.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 """
 ################################################################################
 
 import os
 import argparse
 import sys
 
-from skilleter_thingy import colour
-from skilleter_thingy import git
-from skilleter_thingy import logger
+import thingy.colour as colour
+import thingy.git as git
+import thingy.logger as logger
 
 ################################################################################
 
 def main():
     """ Amend a comment, updating modified files that are already committed and
         adding files that are listed on the command line """
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_cleanup.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_cleanup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 """
 ################################################################################
 
 import sys
 import argparse
 import logging
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 ################################################################################
 # Constants
 
 # Branches that we will never delete
 
 PROTECTED_BRANCHES = ['develop', 'master', 'main', 'release', 'hotfix']
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_co.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_co.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 """
 ################################################################################
 
 import logging
 import sys
 import argparse
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 assert sys.version_info.major >= 3 and sys.version_info.minor >= 6
 
 ################################################################################
 
 DESCRIPTION = \
 """
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_common.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 """
 
 ################################################################################
 
 import sys
 import argparse
 
-from skilleter_thingy import colour
-from skilleter_thingy import git
+import thingy.colour as colour
+import thingy.git as git
 
 ################################################################################
 
 def main():
     """ Main function """
 
     parser = argparse.ArgumentParser(description='Find the most recent common ancestor for two commits')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_hold.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_hold.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """Archive one or more branches by tagging the branch then deleting it
    The branch tag is 'archive/BRANCH_NAME'"""
 
 import sys
 import argparse
 import fnmatch
 
-from skilleter_thingy import colour
-from skilleter_thingy import git
+import thingy.colour as colour
+import thingy.git as git
 
 ################################################################################
 # Prefix for tags representing archived branches
 
 ARCHIVE_PREFIX = 'archive/'
 
 ################################################################################
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_mr.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_mr.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """ Push to Gitlab and create a merge request at the same time """
 ################################################################################
 
 import logging
 import sys
 import argparse
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 ################################################################################
 
 DESCRIPTION = 'Push a feature branch to GitLab and create a merge request'
 
 ################################################################################
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_parent.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_parent.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 the same commit. Can optionally ignore feature branches and/or report
 the distance to the potential parent.
 """
 
 import argparse
 import sys
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 ################################################################################
 
 def main():
     """ Main function """
 
     parser = argparse.ArgumentParser(description='Attempt to determine the parent branch for the specified branch (defaulting to the current one)')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_review.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 import curses.textpad
 import pickle
 import fnmatch
 import subprocess
 import time
 from enum import IntEnum
 
-from skilleter_thingy import git
-from skilleter_thingy import dc_curses
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.dc_curses as dc_curses
+import thingy.colour as colour
 
 ################################################################################
 # Colour pair codes
 
 COLOUR_NORMAL = 1
 COLOUR_STATUS = 2
 COLOUR_REVIEWED = 3
@@ -1281,17 +1281,17 @@
     args = parser.parse_args()
 
     args.paths = None
 
     if args.debug:
         from pudb.remote import set_trace
         set_trace()
-        
+
     # Move to a new directory, if required
-    
+
     if args.dir:
         os.chdir(args.dir)
 
     # Make sure that we're actually in a git working tree
 
     if not git.working_tree():
         colour.error(f'[RED:ERROR] Not a git repository')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_update.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 import os
 import sys
 import argparse
 import fnmatch
 import logging
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 ################################################################################
 
 def parse_command_line():
     """Parse the command line"""
 
     parser = argparse.ArgumentParser(description='Rebase branch(es) against their parent branch, updating both in the process')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/git_wt.py` & `skilleter_thingy-0.0.29/skilleter_thingy/git_wt.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 ################################################################################
 
 import sys
 import argparse
 import os
 
-from skilleter_thingy import git2 as git
+import thingy.git2 as git as git2
 
 ################################################################################
 
 def main():
     """ Main function """
 
     # Command line parameters
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/gitcmp_helper.py` & `skilleter_thingy-0.0.29/skilleter_thingy/gitcmp_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 
 import sys
 import os
 import argparse
 import filecmp
 import re
 
-from skilleter_thingy import logger
-from skilleter_thingy import colour
-from skilleter_thingy import run
-from skilleter_thingy import files
-from skilleter_thingy import git
-from skilleter_thingy import dircolors
+import thingy.logger as logger
+import thingy.colour as colour
+import thingy.run as run
+import thingy.files as files
+import thingy.git as git
+import thingy.dircolors as dircolors
 
 ################################################################################
 # Constants
 
 # A file must be at least this size to be considered binary - if it is smaller
 # we give it the benefit of the doubt.
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/gitlab.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/gitlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import sys
 import os
 
 try:
     import requests
 except ModuleNotFoundError:
-    sys.stderr.write('This code requires the Python "requests" module which should be installed via Pip\n')
+    sys.stderr.write('This code requires the Python "requests" module which should be installed via your package manager\n')
     sys.exit(1)
 
 ################################################################################
 
 class GitLabError(Exception):
     """ Gitlab exceptions """
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/gitprompt.py` & `skilleter_thingy-0.0.29/skilleter_thingy/gitprompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 
 signal.signal(signal.SIGINT, signal.SIG_IGN)
 
 import os
 import sys
 import argparse
 
-from skilleter_thingy import git
-from skilleter_thingy import colour
+import thingy.git as git
+import thingy.colour as colour
 
 ################################################################################
 # Constants
 
 # Prefix text used when showing git status in the prompt - first entry is the
 # abbreviated form and the second is the verbose.
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/gl.py` & `skilleter_thingy-0.0.29/skilleter_thingy/gl.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ################################################################################
 
 import argparse
 import os
 import sys
 from collections import defaultdict
 
-from skilleter_thingy import colour
-from skilleter_thingy import gitlab
+import thingy.colour as colour
+import thingy.gitlab as gitlab
 
 ################################################################################
 
 def mr_list(args):
     """ List merge requests """
 
     gl = gitlab.GitLab(args.server)
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/gphotosync.py` & `skilleter_thingy-0.0.29/skilleter_thingy/gphotosync.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import imagehash
 
 from collections import defaultdict
 
 from dateutil.relativedelta import relativedelta
 from PIL import Image, ExifTags
 
-from skilleter_thingy import colour
+import thingy.colour as colour
 
 ################################################################################
 
 # Default locations for local storage of photos and videos
 
 DEFAULT_PHOTO_DIR = os.path.expanduser('~/Pictures')
 DEFAULT_VIDEO_DIR = os.path.expanduser('~/Videos')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/linecount.py` & `skilleter_thingy-0.0.29/skilleter_thingy/linecount.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import os
 import sys
 import argparse
 
 import filetype
 
-from skilleter_thingy import files
+import thingy.files as files
 
 ################################################################################
 
 def guess_filetype(filepath):
     """ Guess the type of a file """
 
     binary = False
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/logger.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/logger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/moviemover.py` & `skilleter_thingy-0.0.29/skilleter_thingy/moviemover.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/path.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Licence: GPL v3 or later
 """
 ################################################################################
 
 import os
 
-from skilleter_thingy import logger
+import thingy.logger as logger
 
 ################################################################################
 
 class PathError(Exception):
     """ Exception raised by the module """
 
     def __init__(self, msg):
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/photodupe.py` & `skilleter_thingy-0.0.29/skilleter_thingy/photodupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/phototidier.py` & `skilleter_thingy-0.0.29/skilleter_thingy/phototidier.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import pathlib
 import re
 
 from PIL import UnidentifiedImageError
 from PIL import Image
 from PIL.ExifTags import TAGS
 
-from skilleter_thingy import colour
+import thingy.colour as colour
 
 ################################################################################
 
 FILE_TYPES = ('.jpg', '.jpeg')
 
 DATE_RE = re.compile(r'[0-9]{4}-[0-9]{2}-[0-9]{2}')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/popup.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/popup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/process.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Licence: GPL v3 or later
 """
 ################################################################################
 
 import subprocess
 import sys
 
-from skilleter_thingy import logger
+import thingy.logger as logger
 
 ################################################################################
 
 class RunError(Exception):
     """ Run exception """
 
     def __init__(self, msg, status=1):
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/py_audit.py` & `skilleter_thingy-0.0.29/skilleter_thingy/py_audit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/readable.py` & `skilleter_thingy-0.0.29/skilleter_thingy/readable.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import argparse
 import tempfile
 import os
 import re
 import filecmp
 import shutil
 
-from skilleter_thingy import tidy
-from skilleter_thingy import files
+import thingy.tidy as tidy
+import thingy.files as files
 
 ################################################################################
 
 TF_OBJECTS_CHANGED_END = 'Terraform detected the following changes made outside of Terraform since the last "terraform apply":'
 TF_IGNORE_MSG = 'Unless you have made equivalent changes to your configuration, or ignored the relevant attributes using ignore_changes, the following plan may include actions to undo or respond to these changes.'
 
 TF_REFRESHING_AND_READING = re.compile(r'.*: (?:Refreshing state\.\.\.|Reading\.\.\.|Read complete after |Preparing import\.\.\.).*')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/remdir.py` & `skilleter_thingy-0.0.29/skilleter_thingy/remdir.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 import sys
 import os
 import argparse
 import fnmatch
 import shutil
 
-from skilleter_thingy import colour
-from skilleter_thingy import logger
+import thingy.colour as colour
+import thingy.logger as logger
 
 log = logger.init('remdir')
 
 ################################################################################
 
 def main():
     """ Entry point """
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/rmdupe.py` & `skilleter_thingy-0.0.29/skilleter_thingy/rmdupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/rpylint.py` & `skilleter_thingy-0.0.29/skilleter_thingy/rpylint.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import os
 import sys
 import argparse
 import glob
 
 # TODO: Convert to use thingy.proc
-from skilleter_thingy import process
+import thingy.process as process
 
 ################################################################################
 
 def main():
     """ Main code. Exits directly on failure to locate source files, or returns
         the status code from Pylint otherwise. """
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/run.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 # Imports
 
 import sys
 import subprocess
 import threading
 import shlex
 
-from skilleter_thingy import colour
-from skilleter_thingy import tidy
+import thingy.colour
+import thingy.tidy
 
 ################################################################################
 
 class RunError(Exception):
     """ Run exception """
 
     def __init__(self, msg, status=1):
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/splitpics.py` & `skilleter_thingy-0.0.29/skilleter_thingy/splitpics.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/strreplace.py` & `skilleter_thingy-0.0.29/skilleter_thingy/strreplace.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/sysmon.py` & `skilleter_thingy-0.0.29/skilleter_thingy/sysmon.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/tfm.py` & `skilleter_thingy-0.0.29/skilleter_thingy/tfm.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 import curses.textpad
 import subprocess
 import shutil
 from collections import defaultdict
 import threading
 import queue
 
-from skilleter_thingy import popup
-from skilleter_thingy import tfm_pane
+import thingy.popup as popup
+import thingy.tfm_pane as tfm_pane
 
 ################################################################################
 # Colour pair codes
 
 COLOUR_NORMAL = 1
 COLOUR_STATUS = 2
 COLOUR_BACKGROUND = 3
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/tfm_pane.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/tfm_pane.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import threading
 
 from enum import IntEnum
 
 if sys.platform == 'linux':
     import inotify.adapters
 
-from skilleter_thingy import dc_curses
-from skilleter_thingy import path
-from skilleter_thingy import popup
+import thingy.dc_curses as dc_curses
+import thingy.path as path
+import thingy.popup as popup
 
 ################################################################################
 
 class SortOrder(IntEnum):
     """ Sort order for filename list """
 
     FILENAME = 0
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/tfparse.py` & `skilleter_thingy-0.0.29/skilleter_thingy/tfparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import os
 import sys
 import json
 import argparse
 from collections import defaultdict
 
-from skilleter_thingy import colour
+import thingy.colour as colour
 
 ################################################################################
 
 def error(msg, status=1):
     """Report an error and quit"""
 
     colour.write(f'[RED:ERROR]: {msg}')
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/tidy.py` & `skilleter_thingy-0.0.29/skilleter_thingy/thingy/tidy.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/trimpath.py` & `skilleter_thingy-0.0.29/skilleter_thingy/trimpath.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 ################################################################################
 
 import sys
 import os
 import argparse
 import shutil
 
-from skilleter_thingy import path
-from skilleter_thingy import logger
+import thingy.path as path
+import thingy.logger as logger
 
 ################################################################################
 
 def main():
     """ Trim a path to a specified width """
 
     # Set up the command line parser
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/window_rename.py` & `skilleter_thingy-0.0.29/skilleter_thingy/window_rename.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/xchmod.py` & `skilleter_thingy-0.0.29/skilleter_thingy/xchmod.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy/yamlcheck.py` & `skilleter_thingy-0.0.29/skilleter_thingy/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy.egg-info/PKG-INFO` & `skilleter_thingy-0.0.29/skilleter_thingy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.28
+Version: 0.0.29
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy.egg-info/SOURCES.txt` & `skilleter_thingy-0.0.29/skilleter_thingy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 LICENSE
 README.md
 pyproject.toml
 skilleter_thingy/__init__.py
 skilleter_thingy/addpath.py
 skilleter_thingy/borger.py
-skilleter_thingy/colour.py
 skilleter_thingy/console_colours.py
-skilleter_thingy/dc_curses.py
-skilleter_thingy/dc_defaults.py
-skilleter_thingy/dc_util.py
-skilleter_thingy/dircolors.py
 skilleter_thingy/diskspacecheck.py
-skilleter_thingy/docker.py
 skilleter_thingy/docker_purge.py
 skilleter_thingy/ffind.py
-skilleter_thingy/files.py
 skilleter_thingy/ggit.py
 skilleter_thingy/ggrep.py
-skilleter_thingy/git.py
-skilleter_thingy/git2.py
 skilleter_thingy/git_br.py
 skilleter_thingy/git_ca.py
 skilleter_thingy/git_cleanup.py
 skilleter_thingy/git_co.py
 skilleter_thingy/git_common.py
 skilleter_thingy/git_hold.py
 skilleter_thingy/git_mr.py
 skilleter_thingy/git_parent.py
 skilleter_thingy/git_review.py
 skilleter_thingy/git_update.py
 skilleter_thingy/git_wt.py
 skilleter_thingy/gitcmp_helper.py
-skilleter_thingy/gitlab.py
 skilleter_thingy/gitprompt.py
 skilleter_thingy/gl.py
 skilleter_thingy/gphotosync.py
 skilleter_thingy/linecount.py
-skilleter_thingy/logger.py
 skilleter_thingy/moviemover.py
-skilleter_thingy/path.py
 skilleter_thingy/photodupe.py
 skilleter_thingy/phototidier.py
-skilleter_thingy/popup.py
-skilleter_thingy/process.py
 skilleter_thingy/py_audit.py
 skilleter_thingy/readable.py
 skilleter_thingy/remdir.py
 skilleter_thingy/rmdupe.py
 skilleter_thingy/rpylint.py
-skilleter_thingy/run.py
 skilleter_thingy/splitpics.py
 skilleter_thingy/strreplace.py
 skilleter_thingy/sysmon.py
 skilleter_thingy/tfm.py
-skilleter_thingy/tfm_pane.py
 skilleter_thingy/tfparse.py
-skilleter_thingy/tidy.py
 skilleter_thingy/trimpath.py
 skilleter_thingy/window_rename.py
 skilleter_thingy/xchmod.py
 skilleter_thingy/yamlcheck.py
 skilleter_thingy.egg-info/PKG-INFO
 skilleter_thingy.egg-info/SOURCES.txt
 skilleter_thingy.egg-info/dependency_links.txt
 skilleter_thingy.egg-info/entry_points.txt
 skilleter_thingy.egg-info/requires.txt
-skilleter_thingy.egg-info/top_level.txt
+skilleter_thingy.egg-info/top_level.txt
+skilleter_thingy/thingy/colour.py
+skilleter_thingy/thingy/dc_curses.py
+skilleter_thingy/thingy/dc_defaults.py
+skilleter_thingy/thingy/dc_util.py
+skilleter_thingy/thingy/dircolors.py
+skilleter_thingy/thingy/docker.py
+skilleter_thingy/thingy/files.py
+skilleter_thingy/thingy/git.py
+skilleter_thingy/thingy/git2.py
+skilleter_thingy/thingy/gitlab.py
+skilleter_thingy/thingy/logger.py
+skilleter_thingy/thingy/path.py
+skilleter_thingy/thingy/popup.py
+skilleter_thingy/thingy/process.py
+skilleter_thingy/thingy/run.py
+skilleter_thingy/thingy/tfm_pane.py
+skilleter_thingy/thingy/tidy.py
```

### Comparing `skilleter_thingy-0.0.28/skilleter_thingy.egg-info/entry_points.txt` & `skilleter_thingy-0.0.29/skilleter_thingy.egg-info/entry_points.txt`

 * *Files identical despite different names*


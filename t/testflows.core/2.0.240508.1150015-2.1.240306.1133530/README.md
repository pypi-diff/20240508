# Comparing `tmp/testflows.core-2.0.240508.1150015.tar.gz` & `tmp/testflows.core-2.1.240306.1133530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.core-2.0.240508.1150015.tar", last modified: Wed May  8 15:00:15 2024, max compression
+gzip compressed data, was "testflows.core-2.1.240306.1133530.tar", last modified: Wed Mar  6 13:35:31 2024, max compression
```

## Comparing `testflows.core-2.0.240508.1150015.tar` & `testflows.core-2.1.240306.1133530.tar`

### file list

```diff
@@ -1,540 +1,632 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      783 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      212 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     3799 2024-05-08 15:00:15.000000 testflows.core-2.0.240508.1150015/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/
--rw-rw-r--   0 user      (1000) user      (1000)     1671 2024-05-08 15:00:15.000000 testflows.core-2.0.240508.1150015/testflows/_core/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4898 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/baseobject.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)     2403 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/bin/tfs
--rw-rw-r--   0 user      (1000) user      (1000)     5031 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/bin/tfs-worker
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4534 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/common.py
--rw-rw-r--   0 user      (1000) user      (1000)     1579 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/exit.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2449 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/convert.py
--rw-rw-r--   0 user      (1000) user      (1000)     1932 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/handler.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/new/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/new/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1487 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/new/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     2764 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/new/requirements.py
--rw-rw-r--   0 user      (1000) user      (1000)     2648 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/toc.py
--rw-rw-r--   0 user      (1000) user      (1000)      971 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     2116 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/log.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16566 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/command.py
--rw-rw-r--   0 user      (1000) user      (1000)     1662 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     5795 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/metrics.py
--rw-rw-r--   0 user      (1000) user      (1000)     1958 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/results.py
--rw-rw-r--   0 user      (1000) user      (1000)     1014 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/copyright.py
--rw-rw-r--   0 user      (1000) user      (1000)    18199 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/coverage.py
--rw-rw-r--   0 user      (1000) user      (1000)     2394 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     4345 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/metrics.py
--rw-rw-r--   0 user      (1000) user      (1000)    18714 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/results.py
--rw-rw-r--   0 user      (1000) user      (1000)    10802 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/specification.py
--rw-rw-r--   0 user      (1000) user      (1000)     9794 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/srs_coverage.py
--rw-rw-r--   0 user      (1000) user      (1000)     8758 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/tracebility.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/requirement/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/requirement/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1891 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/requirement/generate.py
--rw-rw-r--   0 user      (1000) user      (1000)     1513 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/requirement/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     5943 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/run.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3297 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/arguments.py
--rw-rw-r--   0 user      (1000) user      (1000)     3301 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/attributes.py
--rw-rw-r--   0 user      (1000) user      (1000)     1901 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/coverage.py
--rw-rw-r--   0 user      (1000) user      (1000)     3299 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/description.py
--rw-rw-r--   0 user      (1000) user      (1000)     3146 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/details.py
--rw-rw-r--   0 user      (1000) user      (1000)     3293 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/examples.py
--rw-rw-r--   0 user      (1000) user      (1000)     2095 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/fails.py
--rw-rw-r--   0 user      (1000) user      (1000)     4122 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     3618 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/messages.py
--rw-rw-r--   0 user      (1000) user      (1000)     3289 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/metrics.py
--rw-rw-r--   0 user      (1000) user      (1000)     1907 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/passing.py
--rw-rw-r--   0 user      (1000) user      (1000)     3207 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/procedure.py
--rw-rw-r--   0 user      (1000) user      (1000)     3309 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/requirements.py
--rw-rw-r--   0 user      (1000) user      (1000)     3286 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/result.py
--rw-rw-r--   0 user      (1000) user      (1000)     1901 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/results.py
--rw-rw-r--   0 user      (1000) user      (1000)     3317 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/specifications.py
--rw-rw-r--   0 user      (1000) user      (1000)     3277 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/tags.py
--rw-rw-r--   0 user      (1000) user      (1000)     3284 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/tests.py
--rw-rw-r--   0 user      (1000) user      (1000)     1897 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/totals.py
--rw-rw-r--   0 user      (1000) user      (1000)     1907 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/unstable.py
--rw-rw-r--   0 user      (1000) user      (1000)     1911 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/snapshot/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/snapshot/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1489 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/snapshot/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     1927 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/snapshot/rewrite.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1907 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/brisk.py
--rw-rw-r--   0 user      (1000) user      (1000)     1925 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/classic.py
--rw-rw-r--   0 user      (1000) user      (1000)     2411 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/compact.py
--rw-rw-r--   0 user      (1000) user      (1000)     1916 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/compress.py
--rw-rw-r--   0 user      (1000) user      (1000)     1889 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/decompress.py
--rw-rw-r--   0 user      (1000) user      (1000)     1902 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/dots.py
--rw-rw-r--   0 user      (1000) user      (1000)     2112 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/fails.py
--rw-rw-r--   0 user      (1000) user      (1000)     3486 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/handler.py
--rw-rw-r--   0 user      (1000) user      (1000)     1912 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/manual.py
--rw-rw-r--   0 user      (1000) user      (1000)     1902 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/nice.py
--rw-rw-r--   0 user      (1000) user      (1000)     1937 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/pnice.py
--rw-rw-r--   0 user      (1000) user      (1000)     1897 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/raw.py
--rw-rw-r--   0 user      (1000) user      (1000)     1907 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/short.py
--rw-rw-r--   0 user      (1000) user      (1000)     1907 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/slick.py
--rw-rw-r--   0 user      (1000) user      (1000)     3975 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/parser.py
--rw-rw-r--   0 user      (1000) user      (1000)     7940 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/type.py
--rw-rw-r--   0 user      (1000) user      (1000)     4694 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/colors.py
--rw-rw-r--   0 user      (1000) user      (1000)     1902 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/cli/text.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/combinatorics/
--rw-rw-r--   0 user      (1000) user      (1000)     1805 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/combinatorics/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    13614 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/combinatorics/covering_array.py
--rw-rw-r--   0 user      (1000) user      (1000)     8522 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/compress.py
--rw-rw-r--   0 user      (1000) user      (1000)      756 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/constants.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/
--rw-rw-r--   0 user      (1000) user      (1000)      653 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/aiomsg/
--rw-rw-r--   0 user      (1000) user      (1000)    46147 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/aiomsg/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1179 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/aiomsg/header.py
--rw-rw-r--   0 user      (1000) user      (1000)     1030 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/aiomsg/msgproto.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/
--rw-rw-r--   0 user      (1000) user      (1000)    62569 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2853 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/cleanpeg.py
--rw-rw-r--   0 user      (1000) user      (1000)     6682 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/export.py
--rw-rw-r--   0 user      (1000) user      (1000)    10645 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/peg.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/cloudpickle/
--rw-rw-r--   0 user      (1000) user      (1000)      333 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/cloudpickle/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    35841 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/cloudpickle/cloudpickle.py
--rw-rw-r--   0 user      (1000) user      (1000)    32278 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/cloudpickle/cloudpickle_fast.py
--rw-rw-r--   0 user      (1000) user      (1000)      354 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/cloudpickle/compat.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/markdown2/
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/markdown2/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)   111514 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/markdown2/markdown2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/
--rw-rw-r--   0 user      (1000) user      (1000)      175 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/
--rw-rw-r--   0 user      (1000) user      (1000)       59 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/
--rw-rw-r--   0 user      (1000) user      (1000)       59 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    59972 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/decoder.py
--rw-rw-r--   0 user      (1000) user      (1000)    27957 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/encoder.py
--rw-rw-r--   0 user      (1000) user      (1000)      674 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/eoo.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/cer/
--rw-rw-r--   0 user      (1000) user      (1000)       59 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/cer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3841 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/cer/decoder.py
--rw-rw-r--   0 user      (1000) user      (1000)     9529 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/cer/encoder.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/der/
--rw-rw-r--   0 user      (1000) user      (1000)       59 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/der/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2770 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/der/decoder.py
--rw-rw-r--   0 user      (1000) user      (1000)     3145 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/der/encoder.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/native/
--rw-rw-r--   0 user      (1000) user      (1000)       59 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/native/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     7839 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/native/decoder.py
--rw-rw-r--   0 user      (1000) user      (1000)     8170 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/native/encoder.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/
--rw-rw-r--   0 user      (1000) user      (1000)       59 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      698 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/binary.py
--rw-rw-r--   0 user      (1000) user      (1000)      379 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/calling.py
--rw-rw-r--   0 user      (1000) user      (1000)      482 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/dateandtime.py
--rw-rw-r--   0 user      (1000) user      (1000)     3012 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/integer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1359 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/octets.py
--rw-rw-r--   0 user      (1000) user      (1000)      505 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/string.py
--rw-rw-r--   0 user      (1000) user      (1000)     3798 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/debug.py
--rw-rw-r--   0 user      (1000) user      (1000)     2257 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/error.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/
--rw-rw-r--   0 user      (1000) user      (1000)       59 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    22506 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/base.py
--rw-rw-r--   0 user      (1000) user      (1000)    11469 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/char.py
--rw-rw-r--   0 user      (1000) user      (1000)    22156 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/constraint.py
--rw-rw-r--   0 user      (1000) user      (1000)      270 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/error.py
--rw-rw-r--   0 user      (1000) user      (1000)    16440 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/namedtype.py
--rw-rw-r--   0 user      (1000) user      (1000)     4910 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/namedval.py
--rw-rw-r--   0 user      (1000) user      (1000)     2848 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/opentype.py
--rw-rw-r--   0 user      (1000) user      (1000)     9510 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/tag.py
--rw-rw-r--   0 user      (1000) user      (1000)     3022 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/tagmap.py
--rw-rw-r--   0 user      (1000) user      (1000)   109185 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/univ.py
--rw-rw-r--   0 user      (1000) user      (1000)     5512 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/useful.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/
--rw-rw-r--   0 user      (1000) user      (1000)     3211 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    19789 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/cmdline.py
--rw-rw-r--   0 user      (1000) user      (1000)     1721 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/console.py
--rw-rw-r--   0 user      (1000) user      (1000)     2038 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/filter.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/filters/
--rw-rw-r--   0 user      (1000) user      (1000)    11669 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/filters/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2996 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatter.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.515014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/
--rw-rw-r--   0 user      (1000) user      (1000)     5229 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)     6238 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/_mapping.py
--rw-rw-r--   0 user      (1000) user      (1000)     3362 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/bbcode.py
--rw-rw-r--   0 user      (1000) user      (1000)    32759 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/html.py
--rw-rw-r--   0 user      (1000) user      (1000)    19886 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/img.py
--rw-rw-r--   0 user      (1000) user      (1000)     5941 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/irc.py
--rw-rw-r--   0 user      (1000) user      (1000)    17854 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/latex.py
--rw-rw-r--   0 user      (1000) user      (1000)     5236 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     5098 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/rtf.py
--rw-rw-r--   0 user      (1000) user      (1000)     5888 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/svg.py
--rw-rw-r--   0 user      (1000) user      (1000)     5093 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/terminal.py
--rw-rw-r--   0 user      (1000) user      (1000)    11140 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/terminal256.py
--rw-rw-r--   0 user      (1000) user      (1000)    31818 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexer.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/
--rw-rw-r--   0 user      (1000) user      (1000)    11505 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    27311 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_asy_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    14018 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_cl_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    40001 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_cocoa_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    17504 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_csound_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)   134534 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_lasso_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)     8340 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_lua_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    68999 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_mapping.py
--rw-rw-r--   0 user      (1000) user      (1000)    24737 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_mql_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    48362 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_openedge_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)   154429 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_php_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    11234 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_postgres_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    52429 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_scilab_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    27137 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_sourcemod_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    10481 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_stan_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    25228 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_stata_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    15484 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_tsql_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)     4249 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_vbscript_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    57090 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_vim_builtins.py
--rw-rw-r--   0 user      (1000) user      (1000)    11229 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/actionscript.py
--rw-rw-r--   0 user      (1000) user      (1000)     1140 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/agile.py
--rw-rw-r--   0 user      (1000) user      (1000)     7249 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/algebra.py
--rw-rw-r--   0 user      (1000) user      (1000)     2605 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ambient.py
--rw-rw-r--   0 user      (1000) user      (1000)     4171 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ampl.py
--rw-rw-r--   0 user      (1000) user      (1000)     3222 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/apl.py
--rw-rw-r--   0 user      (1000) user      (1000)    11184 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/archetype.py
--rw-rw-r--   0 user      (1000) user      (1000)    29951 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/asm.py
--rw-rw-r--   0 user      (1000) user      (1000)    19688 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/automation.py
--rw-rw-r--   0 user      (1000) user      (1000)    27648 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/basic.py
--rw-rw-r--   0 user      (1000) user      (1000)     4773 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/bibtex.py
--rw-rw-r--   0 user      (1000) user      (1000)     3990 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/boa.py
--rw-rw-r--   0 user      (1000) user      (1000)    27737 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/business.py
--rw-rw-r--   0 user      (1000) user      (1000)    10584 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/c_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)    25176 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/c_like.py
--rw-rw-r--   0 user      (1000) user      (1000)     2242 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/capnproto.py
--rw-rw-r--   0 user      (1000) user      (1000)     3872 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/chapel.py
--rw-rw-r--   0 user      (1000) user      (1000)     6410 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/clean.py
--rw-rw-r--   0 user      (1000) user      (1000)     1865 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/compiled.py
--rw-rw-r--   0 user      (1000) user      (1000)    32231 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/configs.py
--rw-rw-r--   0 user      (1000) user      (1000)     4168 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/console.py
--rw-rw-r--   0 user      (1000) user      (1000)    16893 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/crystal.py
--rw-rw-r--   0 user      (1000) user      (1000)    16883 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/csound.py
--rw-rw-r--   0 user      (1000) user      (1000)    31581 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/css.py
--rw-rw-r--   0 user      (1000) user      (1000)     9578 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/d.py
--rw-rw-r--   0 user      (1000) user      (1000)     4468 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dalvik.py
--rw-rw-r--   0 user      (1000) user      (1000)    19104 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/data.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/diff.py
--rw-rw-r--   0 user      (1000) user      (1000)    27719 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dotnet.py
--rw-rw-r--   0 user      (1000) user      (1000)    35884 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dsls.py
--rw-rw-r--   0 user      (1000) user      (1000)    10450 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dylan.py
--rw-rw-r--   0 user      (1000) user      (1000)     5923 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ecl.py
--rw-rw-r--   0 user      (1000) user      (1000)     2530 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/eiffel.py
--rw-rw-r--   0 user      (1000) user      (1000)     3045 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/elm.py
--rw-rw-r--   0 user      (1000) user      (1000)     5303 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/email.py
--rw-rw-r--   0 user      (1000) user      (1000)    19024 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/erlang.py
--rw-rw-r--   0 user      (1000) user      (1000)     9537 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/esoteric.py
--rw-rw-r--   0 user      (1000) user      (1000)     3092 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ezhil.py
--rw-rw-r--   0 user      (1000) user      (1000)    17912 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/factor.py
--rw-rw-r--   0 user      (1000) user      (1000)    10030 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/fantom.py
--rw-rw-r--   0 user      (1000) user      (1000)     9456 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/felix.py
--rw-rw-r--   0 user      (1000) user      (1000)     2715 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/floscript.py
--rw-rw-r--   0 user      (1000) user      (1000)     7227 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/forth.py
--rw-rw-r--   0 user      (1000) user      (1000)     9889 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/fortran.py
--rw-rw-r--   0 user      (1000) user      (1000)    26284 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/foxpro.py
--rw-rw-r--   0 user      (1000) user      (1000)    27182 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/freefem.py
--rw-rw-r--   0 user      (1000) user      (1000)      818 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/functional.py
--rw-rw-r--   0 user      (1000) user      (1000)     3749 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/go.py
--rw-rw-r--   0 user      (1000) user      (1000)     6377 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/grammar_notation.py
--rw-rw-r--   0 user      (1000) user      (1000)     2804 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/graph.py
--rw-rw-r--   0 user      (1000) user      (1000)    38331 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/graphics.py
--rw-rw-r--   0 user      (1000) user      (1000)    32168 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/haskell.py
--rw-rw-r--   0 user      (1000) user      (1000)    31007 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/haxe.py
--rw-rw-r--   0 user      (1000) user      (1000)    18227 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/hdl.py
--rw-rw-r--   0 user      (1000) user      (1000)     3555 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/hexdump.py
--rw-rw-r--   0 user      (1000) user      (1000)    19448 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/html.py
--rw-rw-r--   0 user      (1000) user      (1000)    15034 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/idl.py
--rw-rw-r--   0 user      (1000) user      (1000)    30965 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/igor.py
--rw-rw-r--   0 user      (1000) user      (1000)     3165 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/inferno.py
--rw-rw-r--   0 user      (1000) user      (1000)    12914 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/installers.py
--rw-rw-r--   0 user      (1000) user      (1000)    55827 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/int_fiction.py
--rw-rw-r--   0 user      (1000) user      (1000)     1953 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/iolang.py
--rw-rw-r--   0 user      (1000) user      (1000)     4575 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/j.py
--rw-rw-r--   0 user      (1000) user      (1000)    60360 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/javascript.py
--rw-rw-r--   0 user      (1000) user      (1000)    14251 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/julia.py
--rw-rw-r--   0 user      (1000) user      (1000)    70443 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/jvm.py
--rw-rw-r--   0 user      (1000) user      (1000)   143705 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/lisp.py
--rw-rw-r--   0 user      (1000) user      (1000)     7398 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/make.py
--rw-rw-r--   0 user      (1000) user      (1000)    20896 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/markup.py
--rw-rw-r--   0 user      (1000) user      (1000)      868 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/math.py
--rw-rw-r--   0 user      (1000) user      (1000)    30416 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/matlab.py
--rw-rw-r--   0 user      (1000) user      (1000)     8071 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/mime.py
--rw-rw-r--   0 user      (1000) user      (1000)    27925 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ml.py
--rw-rw-r--   0 user      (1000) user      (1000)    13505 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/modeling.py
--rw-rw-r--   0 user      (1000) user      (1000)    52633 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/modula2.py
--rw-rw-r--   0 user      (1000) user      (1000)     6355 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/monte.py
--rw-rw-r--   0 user      (1000) user      (1000)    64034 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ncl.py
--rw-rw-r--   0 user      (1000) user      (1000)     5222 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/nimrod.py
--rw-rw-r--   0 user      (1000) user      (1000)     2791 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/nit.py
--rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/nix.py
--rw-rw-r--   0 user      (1000) user      (1000)     3781 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/oberon.py
--rw-rw-r--   0 user      (1000) user      (1000)    22909 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/objective.py
--rw-rw-r--   0 user      (1000) user      (1000)     3047 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ooc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2320 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     2785 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/parasail.py
--rw-rw-r--   0 user      (1000) user      (1000)    27854 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/parsers.py
--rw-rw-r--   0 user      (1000) user      (1000)    32741 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/pascal.py
--rw-rw-r--   0 user      (1000) user      (1000)     8117 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/pawn.py
--rw-rw-r--   0 user      (1000) user      (1000)    32084 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/perl.py
--rw-rw-r--   0 user      (1000) user      (1000)    10941 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/php.py
--rw-rw-r--   0 user      (1000) user      (1000)     3317 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/pony.py
--rw-rw-r--   0 user      (1000) user      (1000)    12340 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/praat.py
--rw-rw-r--   0 user      (1000) user      (1000)    12453 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/prolog.py
--rw-rw-r--   0 user      (1000) user      (1000)    47495 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/python.py
--rw-rw-r--   0 user      (1000) user      (1000)     6145 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/qvt.py
--rw-rw-r--   0 user      (1000) user      (1000)     6327 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/r.py
--rw-rw-r--   0 user      (1000) user      (1000)    14656 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rdf.py
--rw-rw-r--   0 user      (1000) user      (1000)    18672 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rebol.py
--rw-rw-r--   0 user      (1000) user      (1000)     2974 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/resource.py
--rw-rw-r--   0 user      (1000) user      (1000)     2038 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rnc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2118 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/roboconf.py
--rw-rw-r--   0 user      (1000) user      (1000)    18808 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/robotframework.py
--rw-rw-r--   0 user      (1000) user      (1000)    22240 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ruby.py
--rw-rw-r--   0 user      (1000) user      (1000)     7786 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rust.py
--rw-rw-r--   0 user      (1000) user      (1000)     9497 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/sas.py
--rw-rw-r--   0 user      (1000) user      (1000)     2031 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/scdoc.py
--rw-rw-r--   0 user      (1000) user      (1000)    67884 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/scripting.py
--rw-rw-r--   0 user      (1000) user      (1000)     2072 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/sgf.py
--rw-rw-r--   0 user      (1000) user      (1000)    33942 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/shell.py
--rw-rw-r--   0 user      (1000) user      (1000)     8594 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/slash.py
--rw-rw-r--   0 user      (1000) user      (1000)     7263 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/smalltalk.py
--rw-rw-r--   0 user      (1000) user      (1000)     2850 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/smv.py
--rw-rw-r--   0 user      (1000) user      (1000)     2804 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/snobol.py
--rw-rw-r--   0 user      (1000) user      (1000)     3303 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/solidity.py
--rw-rw-r--   0 user      (1000) user      (1000)     3224 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/special.py
--rw-rw-r--   0 user      (1000) user      (1000)    31926 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/sql.py
--rw-rw-r--   0 user      (1000) user      (1000)     6529 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/stata.py
--rw-rw-r--   0 user      (1000) user      (1000)     3564 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/supercollider.py
--rw-rw-r--   0 user      (1000) user      (1000)     5470 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/tcl.py
--rw-rw-r--   0 user      (1000) user      (1000)    73849 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/templates.py
--rw-rw-r--   0 user      (1000) user      (1000)     6358 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/teraterm.py
--rw-rw-r--   0 user      (1000) user      (1000)     1565 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/testflows.py
--rw-rw-r--   0 user      (1000) user      (1000)    10800 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/testing.py
--rw-rw-r--   0 user      (1000) user      (1000)     1294 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/text.py
--rw-rw-r--   0 user      (1000) user      (1000)     6188 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/textedit.py
--rw-rw-r--   0 user      (1000) user      (1000)    13898 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/textfmts.py
--rw-rw-r--   0 user      (1000) user      (1000)    18950 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/theorem.py
--rw-rw-r--   0 user      (1000) user      (1000)     1594 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/trafficscript.py
--rw-rw-r--   0 user      (1000) user      (1000)     8272 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/typoscript.py
--rw-rw-r--   0 user      (1000) user      (1000)    18049 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/unicon.py
--rw-rw-r--   0 user      (1000) user      (1000)     5798 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/urbi.py
--rw-rw-r--   0 user      (1000) user      (1000)     7313 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/varnish.py
--rw-rw-r--   0 user      (1000) user      (1000)     3753 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/verification.py
--rw-rw-r--   0 user      (1000) user      (1000)     1086 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/web.py
--rw-rw-r--   0 user      (1000) user      (1000)    40077 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/webmisc.py
--rw-rw-r--   0 user      (1000) user      (1000)     4060 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/whiley.py
--rw-rw-r--   0 user      (1000) user      (1000)     2013 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/x10.py
--rw-rw-r--   0 user      (1000) user      (1000)      935 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/xorg.py
--rw-rw-r--   0 user      (1000) user      (1000)     4195 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/zig.py
--rw-rw-r--   0 user      (1000) user      (1000)     1010 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/modeline.py
--rw-rw-r--   0 user      (1000) user      (1000)     1734 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/plugin.py
--rw-rw-r--   0 user      (1000) user      (1000)     3094 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/regexopt.py
--rw-rw-r--   0 user      (1000) user      (1000)     3123 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/scanner.py
--rw-rw-r--   0 user      (1000) user      (1000)     4729 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/sphinxext.py
--rw-rw-r--   0 user      (1000) user      (1000)     5806 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/style.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/
--rw-rw-r--   0 user      (1000) user      (1000)     2966 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      799 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/abap.py
--rw-rw-r--   0 user      (1000) user      (1000)     2311 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/algol.py
--rw-rw-r--   0 user      (1000) user      (1000)     2326 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/algol_nu.py
--rw-rw-r--   0 user      (1000) user      (1000)     4540 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/arduino.py
--rw-rw-r--   0 user      (1000) user      (1000)     2192 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/autumn.py
--rw-rw-r--   0 user      (1000) user      (1000)     1610 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/borland.py
--rw-rw-r--   0 user      (1000) user      (1000)     1403 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/bw.py
--rw-rw-r--   0 user      (1000) user      (1000)     2826 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/colorful.py
--rw-rw-r--   0 user      (1000) user      (1000)     2580 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/default.py
--rw-rw-r--   0 user      (1000) user      (1000)     2534 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/emacs.py
--rw-rw-r--   0 user      (1000) user      (1000)     2563 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/friendly.py
--rw-rw-r--   0 user      (1000) user      (1000)     1346 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/fruity.py
--rw-rw-r--   0 user      (1000) user      (1000)      787 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/igor.py
--rw-rw-r--   0 user      (1000) user      (1000)     2395 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/inkpot.py
--rw-rw-r--   0 user      (1000) user      (1000)     3221 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/lovelace.py
--rw-rw-r--   0 user      (1000) user      (1000)     2422 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/manni.py
--rw-rw-r--   0 user      (1000) user      (1000)     5134 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/monokai.py
--rw-rw-r--   0 user      (1000) user      (1000)     2799 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/murphy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1986 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/native.py
--rw-rw-r--   0 user      (1000) user      (1000)     5689 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/paraiso_dark.py
--rw-rw-r--   0 user      (1000) user      (1000)     5693 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/paraiso_light.py
--rw-rw-r--   0 user      (1000) user      (1000)     2521 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/pastie.py
--rw-rw-r--   0 user      (1000) user      (1000)     2223 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/perldoc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2528 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/rainbow_dash.py
--rw-rw-r--   0 user      (1000) user      (1000)      900 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/rrt.py
--rw-rw-r--   0 user      (1000) user      (1000)     1489 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/sas.py
--rw-rw-r--   0 user      (1000) user      (1000)     3795 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/solarized.py
--rw-rw-r--   0 user      (1000) user      (1000)     1293 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/stata_dark.py
--rw-rw-r--   0 user      (1000) user      (1000)     1322 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/stata_light.py
--rw-rw-r--   0 user      (1000) user      (1000)     7144 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/tango.py
--rw-rw-r--   0 user      (1000) user      (1000)     1981 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/trac.py
--rw-rw-r--   0 user      (1000) user      (1000)     2024 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/vim.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/vs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1549 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/xcode.py
--rw-rw-r--   0 user      (1000) user      (1000)     6490 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/token.py
--rw-rw-r--   0 user      (1000) user      (1000)    64749 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/unistring.py
--rw-rw-r--   0 user      (1000) user      (1000)    11924 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/util.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/
--rw-rw-r--   0 user      (1000) user      (1000)     1536 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1486 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/_compat.py
--rw-rw-r--   0 user      (1000) user      (1000)     1779 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/asn1.py
--rw-rw-r--   0 user      (1000) user      (1000)     9947 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/cli.py
--rw-rw-r--   0 user      (1000) user      (1000)     4668 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/common.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/core.py
--rw-rw-r--   0 user      (1000) user      (1000)    26191 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/key.py
--rw-rw-r--   0 user      (1000) user      (1000)     2361 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/parallel.py
--rw-rw-r--   0 user      (1000) user      (1000)     3976 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/pem.py
--rw-rw-r--   0 user      (1000) user      (1000)    15539 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/pkcs1.py
--rw-rw-r--   0 user      (1000) user      (1000)     3448 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/pkcs1_v2.py
--rw-rw-r--   0 user      (1000) user      (1000)     5136 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/prime.py
--rw-rw-r--   0 user      (1000) user      (1000)     2695 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/randnum.py
--rw-rw-r--   0 user      (1000) user      (1000)     2200 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/transform.py
--rw-rw-r--   0 user      (1000) user      (1000)     2994 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/util.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/schema/
--rw-rw-r--   0 user      (1000) user      (1000)    28963 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/schema/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/snowflake/
--rw-rw-r--   0 user      (1000) user      (1000)      201 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/snowflake/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4096 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/snowflake/snowflake.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/x256/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/x256/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4519 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/x256/x256.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/
--rw-rw-r--   0 user      (1000) user      (1000)    13170 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4883 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/composer.py
--rw-rw-r--   0 user      (1000) user      (1000)    28639 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/constructor.py
--rw-rw-r--   0 user      (1000) user      (1000)     3851 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/cyaml.py
--rw-rw-r--   0 user      (1000) user      (1000)     2837 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/dumper.py
--rw-rw-r--   0 user      (1000) user      (1000)    43006 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/emitter.py
--rw-rw-r--   0 user      (1000) user      (1000)     2533 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/error.py
--rw-rw-r--   0 user      (1000) user      (1000)     2445 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/events.py
--rw-rw-r--   0 user      (1000) user      (1000)     2061 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/loader.py
--rw-rw-r--   0 user      (1000) user      (1000)     1440 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)    25495 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/parser.py
--rw-rw-r--   0 user      (1000) user      (1000)     6794 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/reader.py
--rw-rw-r--   0 user      (1000) user      (1000)    14184 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/representer.py
--rw-rw-r--   0 user      (1000) user      (1000)     8999 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/resolver.py
--rw-rw-r--   0 user      (1000) user      (1000)    51277 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/scanner.py
--rw-rw-r--   0 user      (1000) user      (1000)     4165 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/serializer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2573 2024-05-08 13:13:26.000000 testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/tokens.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/document/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/document/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2402 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/document/convert.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/document/new/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/document/new/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3667 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/document/new/requirements.md
--rw-rw-r--   0 user      (1000) user      (1000)    13924 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/document/srs.py
--rw-rw-r--   0 user      (1000) user      (1000)    40891 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/document/style.css
--rw-rw-r--   0 user      (1000) user      (1000)     5291 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/document/toc.py
--rw-rw-r--   0 user      (1000) user      (1000)      695 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1386 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/filters.py
--rw-rw-r--   0 user      (1000) user      (1000)     5464 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/flags.py
--rw-rw-r--   0 user      (1000) user      (1000)    16368 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/funcs.py
--rw-rw-r--   0 user      (1000) user      (1000)     4489 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/has.py
--rw-rw-r--   0 user      (1000) user      (1000)     7821 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/init.py
--rw-rw-r--   0 user      (1000) user      (1000)    18077 2024-05-08 13:13:02.000000 testflows.core-2.0.240508.1150015/testflows/_core/io.py
--rw-rw-r--   0 user      (1000) user      (1000)      876 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/jupyter_notebook.py
--rw-rw-r--   0 user      (1000) user      (1000)     1672 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/message.py
--rw-rw-r--   0 user      (1000) user      (1000)    10818 2024-05-08 13:13:02.000000 testflows.core-2.0.240508.1150015/testflows/_core/name.py
--rw-rw-r--   0 user      (1000) user      (1000)    33609 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/objects.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/parallel/
--rw-rw-r--   0 user      (1000) user      (1000)     8507 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2790 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/asyncio.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/
--rw-rw-r--   0 user      (1000) user      (1000)      673 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9857 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/asyncio.py
--rw-rw-r--   0 user      (1000) user      (1000)     1181 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/future.py
--rw-rw-r--   0 user      (1000) user      (1000)    16848 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/process.py
--rw-rw-r--   0 user      (1000) user      (1000)     6726 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/thread.py
--rw-rw-r--   0 user      (1000) user      (1000)    38297 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/parallel/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1914 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/serialize.py
--rw-rw-r--   0 user      (1000) user      (1000)     1258 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/temp.py
--rw-rw-r--   0 user      (1000) user      (1000)   139440 2024-05-08 14:39:04.000000 testflows.core-2.0.240508.1150015/testflows/_core/test.py
--rw-rw-r--   0 user      (1000) user      (1000)     1409 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/testtype.py
--rw-rw-r--   0 user      (1000) user      (1000)     8137 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/tracing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.519014 testflows.core-2.0.240508.1150015/testflows/_core/transform/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    19603 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/brisk.py
--rw-rw-r--   0 user      (1000) user      (1000)     5383 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/classic.py
--rw-rw-r--   0 user      (1000) user      (1000)      818 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/collect.py
--rw-rw-r--   0 user      (1000) user      (1000)     3242 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/dots.py
--rw-rw-r--   0 user      (1000) user      (1000)     4968 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/fails.py
--rw-rw-r--   0 user      (1000) user      (1000)    15087 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/flat.py
--rw-rw-r--   0 user      (1000) user      (1000)    19272 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/manual.py
--rw-rw-r--   0 user      (1000) user      (1000)    18153 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/nice.py
--rw-rw-r--   0 user      (1000) user      (1000)     1164 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/parse.py
--rw-rw-r--   0 user      (1000) user      (1000)    21957 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/pipeline.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/procedure.py
--rw-rw-r--   0 user      (1000) user      (1000)     4025 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/progress.py
--rw-rw-r--   0 user      (1000) user      (1000)     5088 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/quiet.py
--rw-rw-r--   0 user      (1000) user      (1000)      905 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/raw.py
--rw-rw-r--   0 user      (1000) user      (1000)     1686 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/read.py
--rw-rw-r--   0 user      (1000) user      (1000)     1731 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/read_and_filter.py
--rw-rw-r--   0 user      (1000) user      (1000)     1479 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/read_raw.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     8415 2024-05-08 13:13:02.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/coverage.py
--rw-rw-r--   0 user      (1000) user      (1000)     4072 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/fails.py
--rw-rw-r--   0 user      (1000) user      (1000)     1471 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/metrics.py
--rw-rw-r--   0 user      (1000) user      (1000)     3448 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/passing.py
--rw-rw-r--   0 user      (1000) user      (1000)     5391 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/results.py
--rw-rw-r--   0 user      (1000) user      (1000)    15059 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/totals.py
--rw-rw-r--   0 user      (1000) user      (1000)     4476 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/unstable.py
--rw-rw-r--   0 user      (1000) user      (1000)     1698 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/version.py
--rw-rw-r--   0 user      (1000) user      (1000)    16566 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/short.py
--rw-rw-r--   0 user      (1000) user      (1000)     7262 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/slick.py
--rw-rw-r--   0 user      (1000) user      (1000)      987 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/sort.py
--rw-rw-r--   0 user      (1000) user      (1000)      838 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/stop.py
--rw-rw-r--   0 user      (1000) user      (1000)      981 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/tests.py
--rw-rw-r--   0 user      (1000) user      (1000)      810 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/values.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/transform/log/write.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/testflows/_core/utils/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      772 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/enum.py
--rw-rw-r--   0 user      (1000) user      (1000)     1142 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/format.py
--rw-rw-r--   0 user      (1000) user      (1000)     1151 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/sort.py
--rw-rw-r--   0 user      (1000) user      (1000)      855 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/string.py
--rw-rw-r--   0 user      (1000) user      (1000)     1590 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/strip.py
--rw-rw-r--   0 user      (1000) user      (1000)     3597 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/timefuncs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1367 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/_core/utils/timer.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/testflows/combinatorics/
--rw-rw-r--   0 user      (1000) user      (1000)      887 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/combinatorics/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/testflows/core/
--rw-rw-r--   0 user      (1000) user      (1000)     4696 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/core/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      695 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/core/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)      955 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/core/name.py
--rw-rw-r--   0 user      (1000) user      (1000)      844 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/core/objects.py
--rw-rw-r--   0 user      (1000) user      (1000)     1317 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/core/parallel.py
--rw-rw-r--   0 user      (1000) user      (1000)      701 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/core/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/testflows/exceptions/
--rw-rw-r--   0 user      (1000) user      (1000)     2403 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/exceptions/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.523014 testflows.core-2.0.240508.1150015/testflows/settings/
--rw-rw-r--   0 user      (1000) user      (1000)     1531 2024-03-14 16:48:36.000000 testflows.core-2.0.240508.1150015/testflows/settings/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:00:15.511014 testflows.core-2.0.240508.1150015/testflows.core.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      783 2024-05-08 15:00:15.000000 testflows.core-2.0.240508.1150015/testflows.core.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    22405 2024-05-08 15:00:15.000000 testflows.core-2.0.240508.1150015/testflows.core.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-08 15:00:15.000000 testflows.core-2.0.240508.1150015/testflows.core.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-08 13:04:15.000000 testflows.core-2.0.240508.1150015/testflows.core.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)        7 2024-05-08 15:00:15.000000 testflows.core-2.0.240508.1150015/testflows.core.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2024-05-08 15:00:15.000000 testflows.core-2.0.240508.1150015/testflows.core.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.076213 testflows.core-2.1.240306.1133530/.github/
+-rw-rw-r--   0 user      (1000) user      (1000)      597 2023-03-13 22:24:42.000000 testflows.core-2.1.240306.1133530/.github/pull_request_template.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.076213 testflows.core-2.1.240306.1133530/.github/workflows/
+-rw-rw-r--   0 user      (1000) user      (1000)     1574 2023-03-13 22:24:42.000000 testflows.core-2.1.240306.1133530/.github/workflows/cla.yml
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      763 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      212 2023-10-17 22:46:06.000000 testflows.core-2.1.240306.1133530/README.md
+-rwxrwxr-x   0 user      (1000) user      (1000)      819 2022-12-23 06:55:24.000000 testflows.core-2.1.240306.1133530/install
+-rwxrwxr-x   0 user      (1000) user      (1000)     4527 2023-10-17 22:45:21.000000 testflows.core-2.1.240306.1133530/package
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     3799 2024-03-06 13:35:30.000000 testflows.core-2.1.240306.1133530/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.076213 testflows.core-2.1.240306.1133530/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/
+-rw-rw-r--   0 user      (1000) user      (1000)     1668 2024-03-06 13:35:30.000000 testflows.core-2.1.240306.1133530/testflows/_core/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4898 2023-06-23 21:23:00.000000 testflows.core-2.1.240306.1133530/testflows/_core/baseobject.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)     2403 2023-03-15 00:25:55.000000 testflows.core-2.1.240306.1133530/testflows/_core/bin/tfs
+-rw-rw-r--   0 user      (1000) user      (1000)     5031 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/bin/tfs-worker
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4534 2024-02-02 00:03:11.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/common.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1579 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/exit.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2449 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/convert.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1932 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/handler.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/new/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/new/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1487 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/new/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2764 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/new/requirements.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2648 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/toc.py
+-rw-rw-r--   0 user      (1000) user      (1000)      971 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2116 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/log.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16566 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/command.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1662 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5795 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/metrics.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1958 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/results.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1014 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/copyright.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18199 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/coverage.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2394 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4345 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/metrics.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18714 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/results.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10802 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/specification.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9794 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/srs_coverage.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8758 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/tracebility.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.080213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/requirement/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/requirement/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1891 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/requirement/generate.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1513 2023-10-17 22:20:53.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/requirement/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5943 2023-01-31 04:15:47.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/run.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3297 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/arguments.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3301 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/attributes.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1901 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/coverage.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3299 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/description.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3146 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/details.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3293 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/examples.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2095 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/fails.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4122 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3618 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/messages.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3289 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/metrics.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1907 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/passing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3207 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/procedure.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3309 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/requirements.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3286 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/result.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1901 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/results.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3317 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/specifications.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3277 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/tags.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3284 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/tests.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1897 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/totals.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1907 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/unstable.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1911 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/snapshot/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-10-17 22:22:19.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/snapshot/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1489 2023-10-17 22:23:46.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/snapshot/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1927 2023-10-17 23:28:55.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/snapshot/rewrite.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1907 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/brisk.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1925 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/classic.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2411 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/compact.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1916 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/compress.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1889 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/decompress.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1902 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/dots.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2112 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/fails.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3486 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/handler.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1912 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/manual.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1902 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/nice.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1937 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/pnice.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1897 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/raw.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1907 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/short.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1907 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/slick.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3975 2023-10-17 22:48:22.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/parser.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7940 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/type.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4694 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/colors.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1902 2023-06-23 21:21:32.000000 testflows.core-2.1.240306.1133530/testflows/_core/cli/text.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/combinatorics/
+-rw-rw-r--   0 user      (1000) user      (1000)     1805 2023-09-21 21:37:14.000000 testflows.core-2.1.240306.1133530/testflows/_core/combinatorics/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13614 2023-09-21 21:36:59.000000 testflows.core-2.1.240306.1133530/testflows/_core/combinatorics/covering_array.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-06-23 21:23:01.000000 testflows.core-2.1.240306.1133530/testflows/_core/compress.py
+-rw-rw-r--   0 user      (1000) user      (1000)      756 2023-06-23 21:23:00.000000 testflows.core-2.1.240306.1133530/testflows/_core/constants.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/
+-rw-rw-r--   0 user      (1000) user      (1000)      653 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    41001 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/VERSION
+-rw-rw-r--   0 user      (1000) user      (1000)    46147 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1179 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/header.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1030 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/msgproto.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/
+-rw-rw-r--   0 user      (1000) user      (1000)      381 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/AUTHORS.md
+-rw-rw-r--   0 user      (1000) user      (1000)     8232 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/CHANGELOG.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1218 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     1010 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)      978 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/THANKS.md
+-rw-rw-r--   0 user      (1000) user      (1000)    62569 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2853 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/cleanpeg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6682 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/export.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10645 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/peg.py
+-rw-rw-r--   0 user      (1000) user      (1000)      416 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/
+-rw-rw-r--   0 user      (1000) user      (1000)     1754 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      333 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    35841 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/cloudpickle.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32278 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/cloudpickle_fast.py
+-rw-rw-r--   0 user      (1000) user      (1000)      354 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/compat.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.084213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/markdown2/
+-rw-rw-r--   0 user      (1000) user      (1000)     2313 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/markdown2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/markdown2/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)   111514 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/markdown2/markdown2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/
+-rw-rw-r--   0 user      (1000) user      (1000)    32933 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/CHANGES.rst
+-rw-rw-r--   0 user      (1000) user      (1000)     1334 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/LICENSE.rst
+-rw-rw-r--   0 user      (1000) user      (1000)     6451 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      152 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/THANKS.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      175 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    59972 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/decoder.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27957 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/encoder.py
+-rw-rw-r--   0 user      (1000) user      (1000)      674 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/eoo.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/cer/
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/cer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3841 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/cer/decoder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9529 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/cer/encoder.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/der/
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/der/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2770 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/der/decoder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3145 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/der/encoder.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/native/
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/native/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7839 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/native/decoder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8170 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/native/encoder.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      698 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/binary.py
+-rw-rw-r--   0 user      (1000) user      (1000)      379 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/calling.py
+-rw-rw-r--   0 user      (1000) user      (1000)      482 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/dateandtime.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3012 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/integer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1359 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/octets.py
+-rw-rw-r--   0 user      (1000) user      (1000)      505 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/string.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3798 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/debug.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2257 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/error.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.088213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22506 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11469 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/char.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22156 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/constraint.py
+-rw-rw-r--   0 user      (1000) user      (1000)      270 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16440 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/namedtype.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4910 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/namedval.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2848 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/opentype.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9510 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/tag.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3022 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/tagmap.py
+-rw-rw-r--   0 user      (1000) user      (1000)   109185 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/univ.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5512 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/useful.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.092213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/
+-rw-rw-r--   0 user      (1000) user      (1000)       28 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/.coveragerc
+-rw-rw-r--   0 user      (1000) user      (1000)      188 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)     8343 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/AUTHORS
+-rw-rw-r--   0 user      (1000) user      (1000)    36753 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/CHANGES
+-rw-rw-r--   0 user      (1000) user      (1000)     1331 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     3211 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      416 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19789 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/cmdline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1721 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/console.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2038 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/filter.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.092213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/filters/
+-rw-rw-r--   0 user      (1000) user      (1000)    11669 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/filters/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2996 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatter.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.092213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/
+-rw-rw-r--   0 user      (1000) user      (1000)     5229 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     6238 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/_mapping.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3362 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/bbcode.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32759 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/html.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19886 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/img.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5941 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/irc.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17854 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/latex.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5236 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/other.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5098 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/rtf.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5888 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/svg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5093 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/terminal.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11140 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/terminal256.py
+-rw-rw-r--   0 user      (1000) user      (1000)    31818 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexer.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.108213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/
+-rw-rw-r--   0 user      (1000) user      (1000)    11505 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27311 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_asy_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14018 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_cl_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    40001 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_cocoa_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17504 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_csound_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)   134534 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_lasso_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8340 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_lua_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    68999 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_mapping.py
+-rw-rw-r--   0 user      (1000) user      (1000)    24737 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_mql_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    48362 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_openedge_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)   154429 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_php_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11234 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_postgres_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    52429 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_scilab_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27137 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_sourcemod_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10481 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_stan_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25228 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_stata_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15484 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_tsql_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4249 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_vbscript_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    57090 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_vim_builtins.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11229 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/actionscript.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1140 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/agile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7249 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/algebra.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2605 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ambient.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4171 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ampl.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3222 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/apl.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11184 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/archetype.py
+-rw-rw-r--   0 user      (1000) user      (1000)    29951 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/asm.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19688 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/automation.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27648 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/basic.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4773 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/bibtex.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3990 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/boa.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27737 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/business.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10584 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/c_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25176 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/c_like.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2242 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/capnproto.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3872 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/chapel.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6410 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/clean.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1865 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/compiled.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32231 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/configs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4168 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/console.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16893 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/crystal.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16883 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/csound.py
+-rw-rw-r--   0 user      (1000) user      (1000)    31581 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/css.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9578 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/d.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4468 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dalvik.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19104 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/data.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/diff.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27719 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dotnet.py
+-rw-rw-r--   0 user      (1000) user      (1000)    35884 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dsls.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10450 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dylan.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5923 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ecl.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2530 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/eiffel.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3045 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/elm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5303 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/email.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19024 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/erlang.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9537 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/esoteric.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3092 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ezhil.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17912 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/factor.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10030 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/fantom.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9456 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/felix.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2715 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/floscript.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7227 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/forth.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9889 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/fortran.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26284 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/foxpro.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27182 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/freefem.py
+-rw-rw-r--   0 user      (1000) user      (1000)      818 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/functional.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3749 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/go.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6377 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/grammar_notation.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2804 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/graph.py
+-rw-rw-r--   0 user      (1000) user      (1000)    38331 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/graphics.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32168 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/haskell.py
+-rw-rw-r--   0 user      (1000) user      (1000)    31007 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/haxe.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18227 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/hdl.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3555 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/hexdump.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19448 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/html.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15034 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/idl.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30965 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/igor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3165 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/inferno.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12914 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/installers.py
+-rw-rw-r--   0 user      (1000) user      (1000)    55827 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/int_fiction.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1953 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/iolang.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4575 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/j.py
+-rw-rw-r--   0 user      (1000) user      (1000)    60360 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/javascript.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14251 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/julia.py
+-rw-rw-r--   0 user      (1000) user      (1000)    70443 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/jvm.py
+-rw-rw-r--   0 user      (1000) user      (1000)   143705 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/lisp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7398 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/make.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20896 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/markup.py
+-rw-rw-r--   0 user      (1000) user      (1000)      868 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/math.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30416 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/matlab.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8071 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/mime.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27925 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13505 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/modeling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    52633 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/modula2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6355 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/monte.py
+-rw-rw-r--   0 user      (1000) user      (1000)    64034 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ncl.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5222 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/nimrod.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2791 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/nit.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/nix.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3781 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/oberon.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22909 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/objective.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3047 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ooc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2320 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/other.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2785 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/parasail.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27854 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/parsers.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32741 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/pascal.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8117 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/pawn.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32084 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/perl.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10941 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/php.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3317 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/pony.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12340 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/praat.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12453 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/prolog.py
+-rw-rw-r--   0 user      (1000) user      (1000)    47495 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/python.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6145 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/qvt.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6327 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/r.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14656 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rdf.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18672 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rebol.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2974 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/resource.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2038 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rnc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2118 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/roboconf.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18808 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/robotframework.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22240 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ruby.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7786 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rust.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9497 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/sas.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2031 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/scdoc.py
+-rw-rw-r--   0 user      (1000) user      (1000)    67884 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/scripting.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2072 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/sgf.py
+-rw-rw-r--   0 user      (1000) user      (1000)    33942 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/shell.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8594 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/slash.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7263 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/smalltalk.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2850 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/smv.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2804 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/snobol.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3303 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/solidity.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3224 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/special.py
+-rw-rw-r--   0 user      (1000) user      (1000)    31926 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/sql.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6529 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/stata.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3564 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/supercollider.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5470 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/tcl.py
+-rw-rw-r--   0 user      (1000) user      (1000)    73849 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/templates.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6358 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/teraterm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1565 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/testflows.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10800 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/testing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1294 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/text.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6188 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/textedit.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13898 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/textfmts.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18950 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/theorem.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1594 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/trafficscript.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8272 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/typoscript.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18049 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/unicon.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5798 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/urbi.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7313 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/varnish.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3753 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/verification.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1086 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/web.py
+-rw-rw-r--   0 user      (1000) user      (1000)    40077 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/webmisc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4060 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/whiley.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2013 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/x10.py
+-rw-rw-r--   0 user      (1000) user      (1000)      935 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/xorg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4195 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/zig.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1010 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/modeline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1734 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/plugin.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3094 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/regexopt.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3123 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/scanner.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4729 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/sphinxext.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5806 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/style.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.108213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/
+-rw-rw-r--   0 user      (1000) user      (1000)     2966 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      799 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/abap.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2311 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/algol.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2326 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/algol_nu.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4540 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/arduino.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2192 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/autumn.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1610 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/borland.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1403 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/bw.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2826 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/colorful.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2580 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/default.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2534 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/emacs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2563 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/friendly.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1346 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/fruity.py
+-rw-rw-r--   0 user      (1000) user      (1000)      787 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/igor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2395 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/inkpot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3221 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/lovelace.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2422 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/manni.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5134 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/monokai.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2799 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/murphy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1986 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/native.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5689 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/paraiso_dark.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5693 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/paraiso_light.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2521 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/pastie.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2223 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/perldoc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2528 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/rainbow_dash.py
+-rw-rw-r--   0 user      (1000) user      (1000)      900 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/rrt.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1489 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/sas.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3795 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/solarized.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1293 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/stata_dark.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1322 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/stata_light.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7144 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/tango.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1981 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/trac.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2024 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/vim.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/vs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1549 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/xcode.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6490 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/token.py
+-rw-rw-r--   0 user      (1000) user      (1000)    64749 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/unistring.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11924 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.108213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/
+-rw-rw-r--   0 user      (1000) user      (1000)      577 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2048 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1536 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1486 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/_compat.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1779 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/asn1.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9947 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4668 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/common.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26191 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/key.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2361 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/parallel.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3976 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/pem.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15539 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/pkcs1.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3448 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/pkcs1_v2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5136 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/prime.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2695 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/randnum.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2200 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/transform.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2994 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.108213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/schema/
+-rw-rw-r--   0 user      (1000) user      (1000)     1097 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/schema/LICENSE-MIT
+-rw-rw-r--   0 user      (1000) user      (1000)    30729 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/schema/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)    28963 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/schema/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/snowflake/
+-rw-rw-r--   0 user      (1000) user      (1000)     1066 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/snowflake/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      201 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/snowflake/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4096 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/snowflake/snowflake.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/x256/
+-rw-rw-r--   0 user      (1000) user      (1000)     1079 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/x256/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2553 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/x256/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/x256/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4519 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/x256/x256.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/
+-rw-rw-r--   0 user      (1000) user      (1000)    11314 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/CHANGES
+-rw-rw-r--   0 user      (1000) user      (1000)     1101 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     1548 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/README
+-rw-rw-r--   0 user      (1000) user      (1000)    13170 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4883 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/composer.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28639 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/constructor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3851 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/cyaml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2837 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/dumper.py
+-rw-rw-r--   0 user      (1000) user      (1000)    43006 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/emitter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2533 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2445 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/events.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2061 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/loader.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1440 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25495 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/parser.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6794 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/reader.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14184 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/representer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8999 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/resolver.py
+-rw-rw-r--   0 user      (1000) user      (1000)    51277 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/scanner.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4165 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/serializer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2573 2024-01-11 16:42:02.000000 testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/tokens.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/document/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/document/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2402 2023-06-23 21:23:06.000000 testflows.core-2.1.240306.1133530/testflows/_core/document/convert.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/document/new/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/document/new/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3667 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/document/new/requirements.md
+-rw-rw-r--   0 user      (1000) user      (1000)    13924 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/document/srs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    40891 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/document/style.css
+-rw-rw-r--   0 user      (1000) user      (1000)     5291 2023-07-05 22:42:05.000000 testflows.core-2.1.240306.1133530/testflows/_core/document/toc.py
+-rw-rw-r--   0 user      (1000) user      (1000)      695 2023-06-23 21:23:06.000000 testflows.core-2.1.240306.1133530/testflows/_core/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-06-23 21:23:06.000000 testflows.core-2.1.240306.1133530/testflows/_core/filters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5464 2023-06-23 21:23:06.000000 testflows.core-2.1.240306.1133530/testflows/_core/flags.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16368 2024-01-09 18:10:13.000000 testflows.core-2.1.240306.1133530/testflows/_core/funcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4489 2023-06-23 21:23:06.000000 testflows.core-2.1.240306.1133530/testflows/_core/has.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7821 2023-12-08 03:38:57.000000 testflows.core-2.1.240306.1133530/testflows/_core/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18029 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/io.py
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-12-08 00:28:36.000000 testflows.core-2.1.240306.1133530/testflows/_core/jupyter_notebook.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1672 2023-06-23 21:23:06.000000 testflows.core-2.1.240306.1133530/testflows/_core/message.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10817 2023-12-13 22:43:14.000000 testflows.core-2.1.240306.1133530/testflows/_core/name.py
+-rw-rw-r--   0 user      (1000) user      (1000)    33609 2024-03-05 23:40:08.000000 testflows.core-2.1.240306.1133530/testflows/_core/objects.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/parallel/
+-rw-rw-r--   0 user      (1000) user      (1000)     8507 2023-11-30 14:32:53.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2790 2023-12-08 00:28:03.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/asyncio.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/
+-rw-rw-r--   0 user      (1000) user      (1000)      673 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9857 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/asyncio.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1181 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/future.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16848 2023-11-30 14:32:54.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/process.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6726 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/thread.py
+-rw-rw-r--   0 user      (1000) user      (1000)    38297 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/parallel/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1914 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/serialize.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1258 2023-06-23 21:45:19.000000 testflows.core-2.1.240306.1133530/testflows/_core/temp.py
+-rw-rw-r--   0 user      (1000) user      (1000)   139089 2024-03-06 13:31:11.000000 testflows.core-2.1.240306.1133530/testflows/_core/test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1409 2023-09-21 18:20:55.000000 testflows.core-2.1.240306.1133530/testflows/_core/testtype.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8137 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/tracing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.112213 testflows.core-2.1.240306.1133530/testflows/_core/transform/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.116213 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19603 2023-09-21 18:30:55.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/brisk.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5383 2023-09-17 12:46:18.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/classic.py
+-rw-rw-r--   0 user      (1000) user      (1000)      818 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/collect.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3242 2023-09-17 12:48:51.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/dots.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4968 2023-09-17 12:51:48.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/fails.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15087 2023-09-21 18:31:14.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/flat.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19272 2023-09-21 18:32:22.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/manual.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18153 2023-09-21 18:31:48.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/nice.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1164 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/parse.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21957 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/pipeline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/procedure.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4025 2023-09-17 12:48:23.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/progress.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5088 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/quiet.py
+-rw-rw-r--   0 user      (1000) user      (1000)      905 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/raw.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1686 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/read.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1731 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/read_and_filter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1479 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/read_raw.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.116213 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8339 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/coverage.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4072 2023-09-17 12:55:50.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/fails.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1471 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/metrics.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3448 2023-09-17 12:54:12.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/passing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5391 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/results.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15059 2023-12-15 22:10:12.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/totals.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4476 2023-09-17 13:10:22.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/unstable.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1698 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16566 2023-09-21 18:32:03.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/short.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7262 2023-09-21 18:31:31.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/slick.py
+-rw-rw-r--   0 user      (1000) user      (1000)      987 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/sort.py
+-rw-rw-r--   0 user      (1000) user      (1000)      838 2023-01-26 06:02:55.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/stop.py
+-rw-rw-r--   0 user      (1000) user      (1000)      981 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/tests.py
+-rw-rw-r--   0 user      (1000) user      (1000)      810 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/values.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/_core/transform/log/write.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.116213 testflows.core-2.1.240306.1133530/testflows/_core/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      772 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/enum.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1142 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/format.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1151 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/sort.py
+-rw-rw-r--   0 user      (1000) user      (1000)      855 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/string.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1590 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/strip.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3597 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/timefuncs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1367 2023-06-23 21:23:07.000000 testflows.core-2.1.240306.1133530/testflows/_core/utils/timer.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.116213 testflows.core-2.1.240306.1133530/testflows/combinatorics/
+-rw-rw-r--   0 user      (1000) user      (1000)    10224 2023-07-19 18:52:51.000000 testflows.core-2.1.240306.1133530/testflows/combinatorics/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)      887 2023-07-18 13:53:27.000000 testflows.core-2.1.240306.1133530/testflows/combinatorics/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.116213 testflows.core-2.1.240306.1133530/testflows/core/
+-rw-rw-r--   0 user      (1000) user      (1000)     4696 2024-01-08 23:10:03.000000 testflows.core-2.1.240306.1133530/testflows/core/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      695 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/testflows/core/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      955 2023-12-13 21:23:37.000000 testflows.core-2.1.240306.1133530/testflows/core/name.py
+-rw-rw-r--   0 user      (1000) user      (1000)      844 2023-06-23 21:23:32.000000 testflows.core-2.1.240306.1133530/testflows/core/objects.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1317 2023-06-23 21:23:32.000000 testflows.core-2.1.240306.1133530/testflows/core/parallel.py
+-rw-rw-r--   0 user      (1000) user      (1000)      701 2022-12-28 17:03:42.000000 testflows.core-2.1.240306.1133530/testflows/core/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.116213 testflows.core-2.1.240306.1133530/testflows/exceptions/
+-rw-rw-r--   0 user      (1000) user      (1000)     2403 2023-06-23 21:23:42.000000 testflows.core-2.1.240306.1133530/testflows/exceptions/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.116213 testflows.core-2.1.240306.1133530/testflows/settings/
+-rw-rw-r--   0 user      (1000) user      (1000)     1531 2023-06-23 21:23:47.000000 testflows.core-2.1.240306.1133530/testflows/settings/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.076213 testflows.core-2.1.240306.1133530/testflows.core.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      763 2024-03-06 13:35:31.000000 testflows.core-2.1.240306.1133530/testflows.core.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    25217 2024-03-06 13:35:31.000000 testflows.core-2.1.240306.1133530/testflows.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-06 13:35:31.000000 testflows.core-2.1.240306.1133530/testflows.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-23 21:33:10.000000 testflows.core-2.1.240306.1133530/testflows.core.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-03-06 13:35:31.000000 testflows.core-2.1.240306.1133530/testflows.core.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2024-03-06 13:35:31.000000 testflows.core-2.1.240306.1133530/testflows.core.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     4129 2023-08-15 12:16:12.000000 testflows.core-2.1.240306.1133530/tests/covering_arrays.py
+-rw-rw-r--   0 user      (1000) user      (1000)      296 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/tests/current_time.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     2969 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/decorated_tests_attributes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      812 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/define.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     2671 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/definitions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      624 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/dynamic_tags_reqs_and_attrs.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/eresult_flags.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.076213 testflows.core-2.1.240306.1133530/tests/examples/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/tests/examples/calculator/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/tests/examples/calculator/docker-compose/
+-rw-rw-r--   0 user      (1000) user      (1000)      956 2023-07-04 11:21:39.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/docker-compose/docker-compose.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     2370 2023-08-15 12:16:26.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/regression.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/tests/examples/calculator/requirements/
+-rw-rw-r--   0 user      (1000) user      (1000)     2704 2023-07-04 11:21:39.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/requirements/answer_prompt.png
+-rw-rw-r--   0 user      (1000) user      (1000)    15203 2023-07-04 11:21:39.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/requirements/calculator.png
+-rw-rw-r--   0 user      (1000) user      (1000)    16630 2023-07-04 11:21:39.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/requirements/history.png
+-rw-rw-r--   0 user      (1000) user      (1000)    15904 2023-07-04 11:21:39.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/requirements/inverse.png
+-rw-rw-r--   0 user      (1000) user      (1000)    38461 2023-09-11 11:57:50.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/requirements/requirements.md
+-rw-rw-r--   0 user      (1000) user      (1000)   101852 2023-09-11 11:58:14.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/requirements/requirements.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20300 2023-07-05 22:43:09.000000 testflows.core-2.1.240306.1133530/tests/examples/calculator/steps.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.076213 testflows.core-2.1.240306.1133530/tests/examples/coreutils/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/tests/examples/coreutils/ls/
+-rw-rw-r--   0 user      (1000) user      (1000)     1038 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/examples/coreutils/ls/regression.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/tests/examples/coreutils/ls/requirements/
+-rw-rw-r--   0 user      (1000) user      (1000)     1733 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/tests/examples/coreutils/ls/requirements/SRS001_GNU_Core_Utilities_ls.md
+-rw-rw-r--   0 user      (1000) user      (1000)      683 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/tests/examples/coreutils/ls/requirements/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7824 2023-01-06 01:18:17.000000 testflows.core-2.1.240306.1133530/tests/examples/coreutils/ls/requirements/ls.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1218 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/examples/coreutils/ls/requirements/requirements.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     3171 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/examples.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1924 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/inlineand.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1318 2023-10-01 17:53:33.000000 testflows.core-2.1.240306.1133530/tests/input.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1910 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/onlynamedargs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4157 2023-09-15 13:00:39.000000 testflows.core-2.1.240306.1133530/tests/outlines.py
+-rw-rw-r--   0 user      (1000) user      (1000)      703 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/outside_setup.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1338 2023-11-30 14:32:54.000000 testflows.core-2.1.240306.1133530/tests/parallel.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7657 2023-11-30 15:33:26.000000 testflows.core-2.1.240306.1133530/tests/parallel_async.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1098 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/parallel_loads.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6375 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/parallel_process.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7357 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/parallel_process2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5392 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/parallel_terminate.py
+-rw-rw-r--   0 user      (1000) user      (1000)      667 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/parserfunc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3352 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/repeat_and_retry.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/results.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3804 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/scenario_filtering.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4670 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/service.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     2879 2023-09-17 12:58:29.000000 testflows.core-2.1.240306.1133530/tests/setups_and_teardowns.py
+-rw-rw-r--   0 user      (1000) user      (1000)      599 2023-09-21 18:33:07.000000 testflows.core-2.1.240306.1133530/tests/sketches.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:35:31.120213 testflows.core-2.1.240306.1133530/tests/snapshots/
+-rw-rw-r--   0 user      (1000) user      (1000)   120984 2023-07-16 01:27:13.000000 testflows.core-2.1.240306.1133530/tests/snapshots/covering_arrays.py.snapshot
+-rw-rw-r--   0 user      (1000) user      (1000)     8725 2024-01-11 21:07:27.000000 testflows.core-2.1.240306.1133530/tests/timer_and_timeouts.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/top_async.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2137 2023-09-14 22:14:05.000000 testflows.core-2.1.240306.1133530/tests/using_secrets.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1017 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/xflags_xfails_when.py
+-rw-rw-r--   0 user      (1000) user      (1000)      391 2023-06-23 21:24:13.000000 testflows.core-2.1.240306.1133530/tests/xresult_flags.py
```

### Comparing `testflows.core-2.0.240508.1150015/LICENSE` & `testflows.core-2.1.240306.1133530/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/PKG-INFO` & `testflows.core-2.1.240306.1133530/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: testflows.core
-Version: 2.0.240508.1150015
+Version: 2.1.240306.1133530
 Summary: TestFlows - Core
 Home-page: https://github.com/testflows/testflows-core
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
 
 # [TestFlows.com Open-Source Software Testing Framework] - Core
 
 [TestFlows.com Open-Source Software Testing Framework] Core module.
 
 [TestFlows.com Open-Source Software Testing Framework]: https://testflows.com
-
-
```

### Comparing `testflows.core-2.0.240508.1150015/setup.py` & `testflows.core-2.1.240306.1133530/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows.core",
-    version="2.0.240508.1150015",
+    version="2.1.240306.1133530",
     description="TestFlows - Core",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/testflows/testflows-core",
     classifiers=[
```

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/format.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,27 @@
-# Copyright 2019-2021 Katteli Inc.
+# Copyright 2020 Katteli Inc.
 # TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from datetime import datetime
+def bytesize(nbytes):
+    """Return human readable size in bytes in
+    short form using KB, MB, GB, or TB string.
 
-__author__ = "Vitaliy Zakaznikov"
-__version__ = "2.0.240508.1150015"
-__repository__ = "//None/git@github.com:testflows/TestFlows-Core.git"
-__commit__ = "21d8757adac539fb9b38f5ef5eb8fff8929ad176"
-__branch__ = "master"
-__license__ = f"""
-Copyright 2019-{datetime.now().year} Katteli Inc.
-TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-     http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-
-See testflows/_core/contrib folder in sources for licenses of each third-party module.
-"""
+    Credit: https://stackoverflow.com/questions/14996453/python-libraries-to-calculate-human-readable-filesize-from-bytes
+    """
+    suffixes = ["B", "KB", "MB", "GB", "TB", "PB"]
+    i = 0
+    while nbytes >= 1024 and i < len(suffixes) - 1:
+        nbytes /= 1024.0
+        i += 1
+    f = ("%.2f" % nbytes).rstrip("0").rstrip(".")
+    return "%s %s" % (f, suffixes[i])
```

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/baseobject.py` & `testflows.core-2.1.240306.1133530/testflows/_core/baseobject.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/bin/tfs` & `testflows.core-2.1.240306.1133530/testflows/_core/bin/tfs`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/bin/tfs-worker` & `testflows.core-2.1.240306.1133530/testflows/_core/bin/tfs-worker`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/common.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/common.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/exit.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/exit.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/convert.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/convert.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/new/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/new/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/new/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/new/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/new/requirements.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/new/requirements.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/document/toc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/document/toc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/log.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/log.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/command.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/command.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/metrics.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/metrics.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/compare/results.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/compare/results.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/copyright.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/copyright.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/coverage.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/coverage.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/metrics.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/metrics.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/results.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/results.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/specification.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/specification.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/srs_coverage.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/srs_coverage.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/report/tracebility.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/report/tracebility.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/requirement/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/requirement/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/requirement/generate.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/requirement/generate.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/requirement/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/requirement/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/run.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/run.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/arguments.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/arguments.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/attributes.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/attributes.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/coverage.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/coverage.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/description.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/description.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/details.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/details.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/examples.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/examples.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/fails.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/fails.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/messages.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/messages.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/metrics.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/metrics.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/passing.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/passing.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/procedure.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/procedure.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/requirements.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/requirements.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/result.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/result.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/results.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/results.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/specifications.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/specifications.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/tags.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/tags.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/tests.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/tests.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/totals.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/totals.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/unstable.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/unstable.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/show/version.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/show/version.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/snapshot/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/snapshot/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/snapshot/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/snapshot/rewrite.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/snapshot/rewrite.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/brisk.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/brisk.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/classic.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/classic.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/compact.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/compact.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/compress.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/compress.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/decompress.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/decompress.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/dots.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/dots.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/fails.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/fails.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/handler.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/handler.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/manual.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/manual.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/nice.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/nice.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/pnice.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/pnice.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/raw.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/raw.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/short.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/short.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/handlers/transform/slick.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/handlers/transform/slick.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/parser.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/parser.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/arg/type.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/arg/type.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/colors.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/colors.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/cli/text.py` & `testflows.core-2.1.240306.1133530/testflows/_core/cli/text.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/combinatorics/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/combinatorics/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/combinatorics/covering_array.py` & `testflows.core-2.1.240306.1133530/testflows/_core/combinatorics/covering_array.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/compress.py` & `testflows.core-2.1.240306.1133530/testflows/_core/compress.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/constants.py` & `testflows.core-2.1.240306.1133530/testflows/_core/constants.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/aiomsg/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/aiomsg/header.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/header.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/aiomsg/msgproto.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/aiomsg/msgproto.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/cleanpeg.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/cleanpeg.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/export.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/export.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/arpeggio/peg.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/arpeggio/peg.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/cloudpickle/cloudpickle.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/cloudpickle/cloudpickle_fast.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/markdown2/markdown2.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/markdown2/markdown2.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/decoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/decoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/encoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/encoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/ber/eoo.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/ber/eoo.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/cer/decoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/cer/decoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/cer/encoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/cer/encoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/der/decoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/der/decoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/der/encoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/der/encoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/native/decoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/native/decoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/codec/native/encoder.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/codec/native/encoder.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/binary.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/binary.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/integer.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/integer.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/compat/octets.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/compat/octets.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/debug.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/debug.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/error.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/error.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/base.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/base.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/char.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/char.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/constraint.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/constraint.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/namedtype.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/namedtype.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/namedval.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/namedval.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/opentype.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/opentype.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/tag.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/tag.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/tagmap.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/tagmap.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/univ.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/univ.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pyasn1/type/useful.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pyasn1/type/useful.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/cmdline.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/console.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/console.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/filter.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/filters/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatter.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/_mapping.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/bbcode.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/html.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/img.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/irc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/latex.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/other.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/rtf.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/svg.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/terminal.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/formatters/terminal256.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexer.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_asy_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_cl_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_cocoa_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_csound_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_lasso_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_lua_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_mapping.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_mql_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_openedge_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_php_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_postgres_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_scilab_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_sourcemod_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_stan_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_stata_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_tsql_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_vbscript_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/_vim_builtins.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/actionscript.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/agile.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/algebra.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ambient.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ampl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/apl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/archetype.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/asm.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/automation.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/basic.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/bibtex.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/boa.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/business.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/c_cpp.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/c_like.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/capnproto.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/chapel.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/clean.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/compiled.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/configs.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/console.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/crystal.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/csound.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/css.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/d.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dalvik.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/data.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/diff.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dotnet.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dsls.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/dylan.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ecl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/eiffel.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/elm.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/email.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/erlang.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/esoteric.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ezhil.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/factor.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/fantom.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/felix.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/floscript.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/forth.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/fortran.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/foxpro.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/freefem.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/functional.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/go.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/grammar_notation.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/graph.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/graphics.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/haskell.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/haxe.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/hdl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/hexdump.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/html.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/idl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/igor.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/inferno.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/installers.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/int_fiction.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/iolang.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/j.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/javascript.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/julia.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/jvm.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/lisp.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/make.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/markup.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/math.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/matlab.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/mime.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/mime.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ml.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/modeling.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/modula2.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/monte.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ncl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/nimrod.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/nit.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/nix.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/oberon.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/objective.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ooc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/other.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/parasail.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/parsers.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/pascal.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/pawn.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/perl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/php.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/pony.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/pony.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/praat.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/prolog.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/python.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/qvt.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/r.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rdf.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rebol.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/resource.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rnc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/roboconf.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/robotframework.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/ruby.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/rust.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/sas.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/scdoc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/scripting.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/sgf.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/shell.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/slash.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/smalltalk.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/smv.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/snobol.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/solidity.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/special.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/sql.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/stata.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/supercollider.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/tcl.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/templates.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/teraterm.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/testflows.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/testflows.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/testing.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/text.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/textedit.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/textfmts.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/theorem.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/trafficscript.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/typoscript.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/unicon.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/urbi.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/varnish.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/verification.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/web.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/webmisc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/whiley.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/x10.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/xorg.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/lexers/zig.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/modeline.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/plugin.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/regexopt.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/scanner.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/sphinxext.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/style.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/style.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/abap.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/algol.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/algol_nu.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/arduino.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/autumn.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/borland.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/bw.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/colorful.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/default.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/emacs.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/friendly.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/fruity.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/igor.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/inkpot.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/inkpot.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/lovelace.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/manni.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/monokai.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/murphy.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/native.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/paraiso_dark.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/paraiso_light.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/pastie.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/perldoc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/rainbow_dash.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/rrt.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/sas.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/solarized.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/solarized.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/stata_dark.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/stata_dark.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/stata_light.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/stata_light.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/tango.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/trac.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/vim.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/vs.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/styles/xcode.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/token.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/token.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/unistring.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/pygments/util.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/pygments/util.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/_compat.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/_compat.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/asn1.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/asn1.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/cli.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/cli.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/common.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/common.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/core.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/core.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/key.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/key.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/parallel.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/parallel.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/pem.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/pem.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/pkcs1.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/pkcs1.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/pkcs1_v2.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/pkcs1_v2.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/prime.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/prime.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/randnum.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/randnum.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/transform.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/transform.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/rsa/util.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/rsa/util.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/schema/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/snowflake/snowflake.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/x256/x256.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/x256/x256.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/composer.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/constructor.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/cyaml.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/dumper.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/emitter.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/error.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/error.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/events.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/events.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/loader.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/nodes.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/parser.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/reader.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/representer.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/resolver.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/scanner.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/serializer.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/contrib/yaml/tokens.py` & `testflows.core-2.1.240306.1133530/testflows/_core/contrib/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/document/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/document/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/document/convert.py` & `testflows.core-2.1.240306.1133530/testflows/_core/document/convert.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/document/new/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/document/new/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/document/new/requirements.md` & `testflows.core-2.1.240306.1133530/testflows/_core/document/new/requirements.md`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/document/srs.py` & `testflows.core-2.1.240306.1133530/testflows/_core/document/srs.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/document/style.css` & `testflows.core-2.1.240306.1133530/testflows/_core/document/style.css`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/document/toc.py` & `testflows.core-2.1.240306.1133530/testflows/_core/document/toc.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/exceptions.py` & `testflows.core-2.1.240306.1133530/testflows/_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/filters.py` & `testflows.core-2.1.240306.1133530/testflows/_core/filters.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/flags.py` & `testflows.core-2.1.240306.1133530/testflows/_core/flags.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/funcs.py` & `testflows.core-2.1.240306.1133530/testflows/_core/funcs.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/has.py` & `testflows.core-2.1.240306.1133530/testflows/_core/has.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/init.py` & `testflows.core-2.1.240306.1133530/testflows/_core/init.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/io.py` & `testflows.core-2.1.240306.1133530/testflows/_core/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,27 +56,25 @@
     def __init__(self, test, io):
         self.io = io
         self.test = test
         self.msg_hash = ""
         self.msg_count = 0
         self.prefix = {
             "test_type": str(self.test.type),
-            "test_subtype": (
-                str(self.test.subtype) if self.test.subtype is not None else None
-            ),
+            "test_subtype": str(self.test.subtype)
+            if self.test.subtype is not None
+            else None,
             "test_id": self.test.id_str,
             "test_name": self.test.name,
             "test_flags": int(self.test.flags),
             "test_cflags": int(self.test.cflags),
             "test_level": len(self.test.id),
-            "test_parent_type": (
-                str(self.test.parent_type)
-                if self.test.parent_type is not None
-                else None
-            ),
+            "test_parent_type": str(self.test.parent_type)
+            if self.test.parent_type is not None
+            else None,
         }
 
     def message(self, keyword, message, object_type=0, stream=None):
         """Output message.
 
         :param keyword: keyword
         :param message: message
```

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/jupyter_notebook.py` & `testflows.core-2.1.240306.1133530/testflows/_core/jupyter_notebook.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/message.py` & `testflows.core-2.1.240306.1133530/testflows/_core/message.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/name.py` & `testflows.core-2.1.240306.1133530/testflows/_core/name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Code is based on Python3.6 posixpath.py.
 """
-
 import re
 import functools
 
 sep = "/"
 empty = ""
 dot = "."
 dotdot = ".."
```

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/objects.py` & `testflows.core-2.1.240306.1133530/testflows/_core/objects.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/asyncio.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/asyncio.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/asyncio.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/asyncio.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/future.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/future.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/process.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/process.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/executor/thread.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/executor/thread.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/parallel/service.py` & `testflows.core-2.1.240306.1133530/testflows/_core/parallel/service.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/serialize.py` & `testflows.core-2.1.240306.1133530/testflows/_core/serialize.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/temp.py` & `testflows.core-2.1.240306.1133530/testflows/_core/temp.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/test.py` & `testflows.core-2.1.240306.1133530/testflows/_core/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,35 +486,31 @@
         self.maps = get(maps, list(self.maps))
         self.module = module
         self.action = action
         self.type = get(type, self.type)
         self.subtype = get(subtype, self.subtype)
         self.context = get(
             context,
-            (
-                current_test.context
-                if current_test and self.type < TestType.Test
-                else (Context(current_test.context if current_test else None))
-            ),
+            current_test.context
+            if current_test and self.type < TestType.Test
+            else (Context(current_test.context if current_test else None)),
         )
         self.behavior = get(
             behavior,
             current_test.behavior if current_test and self.type < TestType.Test else [],
         )
         self.pattern = get(
             pattern,
             current_test.pattern if current_test and self.type < TestType.Test else {},
         )
         self.random = get(
             random,
-            (
-                current_test.random
-                if current_test and self.type < TestType.Test
-                else False
-            ),
+            current_test.random
+            if current_test and self.type < TestType.Test
+            else False,
         )
         self.limit = limit
         if action is not None:
             self.behavior.append(basename(self.name))
         self.tags = tags
         self.specifications = {
             s.name: s
@@ -2157,19 +2153,17 @@
             top_test = top()
 
             if not top_test:
                 cli_args = parse_cli_args(
                     self.kwargs,
                     cli_argparser(
                         self.kwargs,
-                        (
-                            argparser
-                            if not isinstance(argparser, ArgumentParser)
-                            else argparser.value
-                        ),
+                        argparser
+                        if not isinstance(argparser, ArgumentParser)
+                        else argparser.value,
                     ),
                 )
                 kwargs["args"].update(
                     {k: v for k, v in cli_args.items() if not k.startswith("_")}
                 )
 
             test = kwargs.pop("test", None)
@@ -2879,17 +2873,15 @@
                         r = _retries.__next__(
                             flags=retry_kwargs_flags,
                             tags=self.tags,
                             **retry_kwargs,
                         )
                     except StopIteration:
                         pass
-                    async with (
-                        r if retry is not None else AsyncNullStep()
-                    ) as retry_iteration:
+                    async with r if retry is not None else AsyncNullStep() as retry_iteration:
                         if retry_iteration is None:
                             retry_iteration = iteration
                         if isinstance(self.repeatable_func, TestOutline):
                             retry_iteration._run_outline_with_no_arguments = (
                                 self.no_arguments
                             )
                             retry_iteration._run_outline = True
@@ -3864,18 +3856,14 @@
 
         self.retry = RetryIteration(
             f"try #{self.number}",
             flags=flags,
             **kwargs,
         )
 
-        # provide retry number and is_last to the user
-        self.retry.retry_number = self.number
-        self.retry.last_retry = bool(flags & LAST_RETRY)
-
         return self.retry
 
 
 def retry(
     func, count=None, timeout=None, delay=0, backoff=1, jitter=None, initial_delay=0
 ):
     """Retry function.
```

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/testtype.py` & `testflows.core-2.1.240306.1133530/testflows/_core/testtype.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/tracing.py` & `testflows.core-2.1.240306.1133530/testflows/_core/tracing.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/brisk.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/brisk.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/classic.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/classic.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/collect.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/collect.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/dots.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/dots.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/fails.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/fails.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/flat.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/flat.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/manual.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/manual.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/nice.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/nice.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/parse.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/parse.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/pipeline.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/pipeline.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/procedure.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/procedure.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/progress.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/progress.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/quiet.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/quiet.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/raw.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/raw.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/read.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/read.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/read_and_filter.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/read_and_filter.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/read_raw.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/read_raw.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/coverage.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,20 +149,18 @@
         for requirement, tests in self.requirements.items():
             if not tests:
                 self.counts.untested += 1
             else:
                 if (
                     sum(
                         [
-                            (
-                                0
-                                if test["result"] is not None
-                                and test["result"]["result_type"] == "OK"
-                                else 1
-                            )
+                            0
+                            if test["result"] is not None
+                            and test["result"]["result_type"] == "OK"
+                            else 1
                             for test in tests
                         ]
                     )
                     == 0
                 ):
                     self.counts.ok += 1
                 else:
```

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/fails.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/fails.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/metrics.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/metrics.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/passing.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/passing.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/results.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/results.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/totals.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/totals.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/unstable.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/unstable.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/report/version.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/report/version.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/short.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/short.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/slick.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/slick.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/sort.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/sort.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/stop.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/stop.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/tests.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/tests.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/values.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/values.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/transform/log/write.py` & `testflows.core-2.1.240306.1133530/testflows/_core/transform/log/write.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/utils/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/utils/enum.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/enum.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/utils/sort.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/sort.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/utils/string.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/string.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/utils/strip.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/strip.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/utils/timefuncs.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/timefuncs.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/_core/utils/timer.py` & `testflows.core-2.1.240306.1133530/testflows/_core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/combinatorics/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/combinatorics/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/core/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/core/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/core/exceptions.py` & `testflows.core-2.1.240306.1133530/testflows/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/core/name.py` & `testflows.core-2.1.240306.1133530/testflows/core/name.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/core/objects.py` & `testflows.core-2.1.240306.1133530/testflows/core/objects.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/core/parallel.py` & `testflows.core-2.1.240306.1133530/testflows/core/parallel.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/core/utils.py` & `testflows.core-2.1.240306.1133530/testflows/core/utils.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/exceptions/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows/settings/__init__.py` & `testflows.core-2.1.240306.1133530/testflows/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.core-2.0.240508.1150015/testflows.core.egg-info/PKG-INFO` & `testflows.core-2.1.240306.1133530/testflows.core.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: testflows.core
-Version: 2.0.240508.1150015
+Version: 2.1.240306.1133530
 Summary: TestFlows - Core
 Home-page: https://github.com/testflows/testflows-core
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
 
 # [TestFlows.com Open-Source Software Testing Framework] - Core
 
 [TestFlows.com Open-Source Software Testing Framework] Core module.
 
 [TestFlows.com Open-Source Software Testing Framework]: https://testflows.com
-
-
```

### Comparing `testflows.core-2.0.240508.1150015/testflows.core.egg-info/SOURCES.txt` & `testflows.core-2.1.240306.1133530/testflows.core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+.gitignore
 LICENSE
 README.md
+install
+package
 setup.py
+.github/pull_request_template.md
+.github/workflows/cla.yml
 testflows.core.egg-info/PKG-INFO
 testflows.core.egg-info/SOURCES.txt
 testflows.core.egg-info/dependency_links.txt
 testflows.core.egg-info/not-zip-safe
 testflows.core.egg-info/requires.txt
 testflows.core.egg-info/top_level.txt
 testflows/_core/__init__.py
@@ -104,28 +109,42 @@
 testflows/_core/cli/arg/handlers/transform/pnice.py
 testflows/_core/cli/arg/handlers/transform/raw.py
 testflows/_core/cli/arg/handlers/transform/short.py
 testflows/_core/cli/arg/handlers/transform/slick.py
 testflows/_core/combinatorics/__init__.py
 testflows/_core/combinatorics/covering_array.py
 testflows/_core/contrib/__init__.py
+testflows/_core/contrib/aiomsg/LICENSE
+testflows/_core/contrib/aiomsg/README.rst
+testflows/_core/contrib/aiomsg/VERSION
 testflows/_core/contrib/aiomsg/__init__.py
 testflows/_core/contrib/aiomsg/header.py
 testflows/_core/contrib/aiomsg/msgproto.py
+testflows/_core/contrib/arpeggio/AUTHORS.md
+testflows/_core/contrib/arpeggio/CHANGELOG.md
+testflows/_core/contrib/arpeggio/LICENSE
+testflows/_core/contrib/arpeggio/README.rst
+testflows/_core/contrib/arpeggio/THANKS.md
 testflows/_core/contrib/arpeggio/__init__.py
 testflows/_core/contrib/arpeggio/cleanpeg.py
 testflows/_core/contrib/arpeggio/export.py
 testflows/_core/contrib/arpeggio/peg.py
 testflows/_core/contrib/arpeggio/utils.py
+testflows/_core/contrib/cloudpickle/LICENSE
 testflows/_core/contrib/cloudpickle/__init__.py
 testflows/_core/contrib/cloudpickle/cloudpickle.py
 testflows/_core/contrib/cloudpickle/cloudpickle_fast.py
 testflows/_core/contrib/cloudpickle/compat.py
+testflows/_core/contrib/markdown2/LICENSE.txt
 testflows/_core/contrib/markdown2/__init__.py
 testflows/_core/contrib/markdown2/markdown2.py
+testflows/_core/contrib/pyasn1/CHANGES.rst
+testflows/_core/contrib/pyasn1/LICENSE.rst
+testflows/_core/contrib/pyasn1/README.md
+testflows/_core/contrib/pyasn1/THANKS.txt
 testflows/_core/contrib/pyasn1/__init__.py
 testflows/_core/contrib/pyasn1/debug.py
 testflows/_core/contrib/pyasn1/error.py
 testflows/_core/contrib/pyasn1/codec/__init__.py
 testflows/_core/contrib/pyasn1/codec/ber/__init__.py
 testflows/_core/contrib/pyasn1/codec/ber/decoder.py
 testflows/_core/contrib/pyasn1/codec/ber/encoder.py
@@ -154,14 +173,19 @@
 testflows/_core/contrib/pyasn1/type/namedtype.py
 testflows/_core/contrib/pyasn1/type/namedval.py
 testflows/_core/contrib/pyasn1/type/opentype.py
 testflows/_core/contrib/pyasn1/type/tag.py
 testflows/_core/contrib/pyasn1/type/tagmap.py
 testflows/_core/contrib/pyasn1/type/univ.py
 testflows/_core/contrib/pyasn1/type/useful.py
+testflows/_core/contrib/pygments/.coveragerc
+testflows/_core/contrib/pygments/.gitignore
+testflows/_core/contrib/pygments/AUTHORS
+testflows/_core/contrib/pygments/CHANGES
+testflows/_core/contrib/pygments/LICENSE
 testflows/_core/contrib/pygments/__init__.py
 testflows/_core/contrib/pygments/__main__.py
 testflows/_core/contrib/pygments/cmdline.py
 testflows/_core/contrib/pygments/console.py
 testflows/_core/contrib/pygments/filter.py
 testflows/_core/contrib/pygments/formatter.py
 testflows/_core/contrib/pygments/lexer.py
@@ -376,14 +400,16 @@
 testflows/_core/contrib/pygments/styles/stata_dark.py
 testflows/_core/contrib/pygments/styles/stata_light.py
 testflows/_core/contrib/pygments/styles/tango.py
 testflows/_core/contrib/pygments/styles/trac.py
 testflows/_core/contrib/pygments/styles/vim.py
 testflows/_core/contrib/pygments/styles/vs.py
 testflows/_core/contrib/pygments/styles/xcode.py
+testflows/_core/contrib/rsa/LICENSE
+testflows/_core/contrib/rsa/README.md
 testflows/_core/contrib/rsa/__init__.py
 testflows/_core/contrib/rsa/_compat.py
 testflows/_core/contrib/rsa/asn1.py
 testflows/_core/contrib/rsa/cli.py
 testflows/_core/contrib/rsa/common.py
 testflows/_core/contrib/rsa/core.py
 testflows/_core/contrib/rsa/key.py
@@ -391,19 +417,27 @@
 testflows/_core/contrib/rsa/pem.py
 testflows/_core/contrib/rsa/pkcs1.py
 testflows/_core/contrib/rsa/pkcs1_v2.py
 testflows/_core/contrib/rsa/prime.py
 testflows/_core/contrib/rsa/randnum.py
 testflows/_core/contrib/rsa/transform.py
 testflows/_core/contrib/rsa/util.py
+testflows/_core/contrib/schema/LICENSE-MIT
+testflows/_core/contrib/schema/README.rst
 testflows/_core/contrib/schema/__init__.py
+testflows/_core/contrib/snowflake/LICENSE
 testflows/_core/contrib/snowflake/__init__.py
 testflows/_core/contrib/snowflake/snowflake.py
+testflows/_core/contrib/x256/LICENSE
+testflows/_core/contrib/x256/README.md
 testflows/_core/contrib/x256/__init__.py
 testflows/_core/contrib/x256/x256.py
+testflows/_core/contrib/yaml/CHANGES
+testflows/_core/contrib/yaml/LICENSE
+testflows/_core/contrib/yaml/README
 testflows/_core/contrib/yaml/__init__.py
 testflows/_core/contrib/yaml/composer.py
 testflows/_core/contrib/yaml/constructor.py
 testflows/_core/contrib/yaml/cyaml.py
 testflows/_core/contrib/yaml/dumper.py
 testflows/_core/contrib/yaml/emitter.py
 testflows/_core/contrib/yaml/error.py
@@ -471,16 +505,63 @@
 testflows/_core/utils/enum.py
 testflows/_core/utils/format.py
 testflows/_core/utils/sort.py
 testflows/_core/utils/string.py
 testflows/_core/utils/strip.py
 testflows/_core/utils/timefuncs.py
 testflows/_core/utils/timer.py
+testflows/combinatorics/README.rst
 testflows/combinatorics/__init__.py
 testflows/core/__init__.py
 testflows/core/exceptions.py
 testflows/core/name.py
 testflows/core/objects.py
 testflows/core/parallel.py
 testflows/core/utils.py
 testflows/exceptions/__init__.py
-testflows/settings/__init__.py
+testflows/settings/__init__.py
+tests/covering_arrays.py
+tests/current_time.py
+tests/decorated_tests_attributes.py
+tests/define.py
+tests/definitions.py
+tests/dynamic_tags_reqs_and_attrs.py
+tests/eresult_flags.py
+tests/examples.py
+tests/inlineand.py
+tests/input.py
+tests/onlynamedargs.py
+tests/outlines.py
+tests/outside_setup.py
+tests/parallel.py
+tests/parallel_async.py
+tests/parallel_loads.py
+tests/parallel_process.py
+tests/parallel_process2.py
+tests/parallel_terminate.py
+tests/parserfunc.py
+tests/repeat_and_retry.py
+tests/results.py
+tests/scenario_filtering.py
+tests/service.py
+tests/setups_and_teardowns.py
+tests/sketches.py
+tests/timer_and_timeouts.py
+tests/top_async.py
+tests/using_secrets.py
+tests/xflags_xfails_when.py
+tests/xresult_flags.py
+tests/examples/calculator/regression.py
+tests/examples/calculator/steps.py
+tests/examples/calculator/docker-compose/docker-compose.yml
+tests/examples/calculator/requirements/answer_prompt.png
+tests/examples/calculator/requirements/calculator.png
+tests/examples/calculator/requirements/history.png
+tests/examples/calculator/requirements/inverse.png
+tests/examples/calculator/requirements/requirements.md
+tests/examples/calculator/requirements/requirements.py
+tests/examples/coreutils/ls/regression.py
+tests/examples/coreutils/ls/requirements/SRS001_GNU_Core_Utilities_ls.md
+tests/examples/coreutils/ls/requirements/__init__.py
+tests/examples/coreutils/ls/requirements/ls.txt
+tests/examples/coreutils/ls/requirements/requirements.py
+tests/snapshots/covering_arrays.py.snapshot
```


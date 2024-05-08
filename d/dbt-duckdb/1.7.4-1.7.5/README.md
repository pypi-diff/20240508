# Comparing `tmp/dbt_duckdb-1.7.4.tar.gz` & `tmp/dbt_duckdb-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_duckdb-1.7.4.tar", last modified: Wed Apr 17 06:01:38 2024, max compression
+gzip compressed data, was "dbt_duckdb-1.7.5.tar", last modified: Wed May  8 05:42:52 2024, max compression
```

## Comparing `dbt_duckdb-1.7.4.tar` & `dbt_duckdb-1.7.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.843292 dbt_duckdb-1.7.4/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)       47 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)    23279 2024-04-17 06:01:38.843066 dbt_duckdb-1.7.4/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)    22265 2024-04-17 05:57:44.000000 dbt_duckdb-1.7.4/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.831895 dbt_duckdb-1.7.4/dbt/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.832136 dbt_duckdb-1.7.4/dbt/adapters/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.834522 dbt_duckdb-1.7.4/dbt/adapters/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)      407 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       18 2024-04-17 05:57:34.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 jwills     (501) staff       (20)      856 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/column.py
--rw-r--r--   0 jwills     (501) staff       (20)     3740 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 jwills     (501) staff       (20)     9883 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/credentials.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.835556 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/
--rw-r--r--   0 jwills     (501) staff       (20)     9673 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     2404 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/buenavista.py
--rw-r--r--   0 jwills     (501) staff       (20)     5462 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/local.py
--rw-r--r--   0 jwills     (501) staff       (20)    11267 2024-04-17 05:42:41.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.838174 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 jwills     (501) staff       (20)     5039 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     1230 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/delta.py
--rw-r--r--   0 jwills     (501) staff       (20)     4951 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 jwills     (501) staff       (20)    12466 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/glue.py
--rw-r--r--   0 jwills     (501) staff       (20)     2386 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 jwills     (501) staff       (20)     1029 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 jwills     (501) staff       (20)     1703 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/motherduck.py
--rw-r--r--   0 jwills     (501) staff       (20)      533 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/pd_utils.py
--rw-r--r--   0 jwills     (501) staff       (20)     1296 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)     1505 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 jwills     (501) staff       (20)     3457 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 jwills     (501) staff       (20)     2445 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.838305 dbt_duckdb-1.7.4/dbt/include/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.838729 dbt_duckdb-1.7.4/dbt/include/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)       52 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       74 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.840206 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/
--rw-r--r--   0 jwills     (501) staff       (20)     7949 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1465 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/catalog.sql
--rw-r--r--   0 jwills     (501) staff       (20)      643 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/columns.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1429 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/incremental_helper.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.840872 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 jwills     (501) staff       (20)     4165 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 jwills     (501) staff       (20)     5315 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2529 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1620 2024-04-03 05:10:12.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/persist_docs.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1849 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1359 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/snapshot_helper.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.841974 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 jwills     (501) staff       (20)       93 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 jwills     (501) staff       (20)      174 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 jwills     (501) staff       (20)      172 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 jwills     (501) staff       (20)      357 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 jwills     (501) staff       (20)      378 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 jwills     (501) staff       (20)      568 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 jwills     (501) staff       (20)      167 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1683 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/upstream.sql
--rw-r--r--   0 jwills     (501) staff       (20)      174 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/dbt/include/duckdb/sample_profiles.yml
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-04-17 06:01:38.842657 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)    23279 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1982 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       88 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        4 2024-04-17 06:01:38.000000 dbt_duckdb-1.7.4/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2024-04-17 06:01:38.843330 dbt_duckdb-1.7.4/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1899 2024-03-07 21:36:58.000000 dbt_duckdb-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.170551 dbt_duckdb-1.7.5/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.170551 dbt_duckdb-1.7.5/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.170551 dbt_duckdb-1.7.5/dbt/adapters/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/buenavista.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/motherduck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/pd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/include/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/incremental_helper.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/snapshot_helper.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/upstream.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 05:42:52.182551 dbt_duckdb-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/setup.py
```

### Comparing `dbt_duckdb-1.7.4/LICENSE` & `dbt_duckdb-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/PKG-INFO` & `dbt_duckdb-1.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.7.4
+Version: 1.7.5
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -19,15 +19,15 @@
 License-File: LICENSE
 Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: duckdb>=0.7.0
 Provides-Extra: glue
 Requires-Dist: boto3; extra == "glue"
 Requires-Dist: mypy-boto3-glue; extra == "glue"
 Provides-Extra: md
-Requires-Dist: duckdb<=0.9.2,>=0.7.0; extra == "md"
+Requires-Dist: duckdb>=0.10.2; extra == "md"
 
 ## dbt-duckdb
 
 [DuckDB](http://duckdb.org) is an embedded database, similar to SQLite, but designed for OLAP-style analytics.
 It is crazy fast and allows you to read and write data stored in CSV, JSON, and Parquet files directly, without requiring you to load
 them into the database first.
 
@@ -229,15 +229,18 @@
 
 One of DuckDB's most powerful features is its ability to read and write CSV, JSON, and Parquet files directly, without needing to import/export
 them from the database first.
 
 #### Reading from external files
 
 You may reference external files in your dbt models either directly or as dbt `source`s by configuring the `external_location`
-meta option on the source:
+in either the `meta` or the `config` option on the source definition. The difference is that settings under the `meta` option
+will be propagated to the documentation for the source generated via `dbt docs generate`, but the settings under the `config`
+option will not be. Any source settings that should be excluded from the docs should be specified via `config`, while any
+options that you would like to be included in the generated documentation should live under `meta`.
 
 ```
 sources:
   - name: external_source
     meta:
       external_location: "s3://my-bucket/my-sources/{name}.parquet"
     tables:
@@ -267,15 +270,15 @@
 sources:
   - name: external_source
     meta:
       external_location: "s3://my-bucket/my-sources/{name}.parquet"
     tables:
       - name: source1
       - name: source2
-        meta:
+        config:
           external_location: "read_parquet(['s3://my-bucket/my-sources/source2a.parquet', 's3://my-bucket/my-sources/source2b.parquet'])"
 ```
 
 In this situation, the `external_location` setting on the `source2` table will take precedence, so a dbt model like:
 
 ```
 SELECT *
@@ -293,15 +296,15 @@
 call, which is helpful in the case that you have an external source that is a CSV file which requires special handling for DuckDB to load it correctly:
 
 ```
 sources:
   - name: flights_source
     tables:
       - name: flights
-        meta:
+        config:
           external_location: "read_csv('flights.csv', types={'FlightDate': 'DATE'}, names=['FlightDate', 'UniqueCarrier'])"
           formatter: oldstyle
 ```
 
 Note that we need to override the default `str.format` string formatting strategy for this example
 because the `types={'FlightDate': 'DATE'}` argument to the `read_csv` function will be interpreted by
 `str.format` as a template to be matched on, which will cause a `KeyError: "'FlightDate'"` when we attempt
```

### Comparing `dbt_duckdb-1.7.4/README.md` & `dbt_duckdb-1.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,18 @@
 
 One of DuckDB's most powerful features is its ability to read and write CSV, JSON, and Parquet files directly, without needing to import/export
 them from the database first.
 
 #### Reading from external files
 
 You may reference external files in your dbt models either directly or as dbt `source`s by configuring the `external_location`
-meta option on the source:
+in either the `meta` or the `config` option on the source definition. The difference is that settings under the `meta` option
+will be propagated to the documentation for the source generated via `dbt docs generate`, but the settings under the `config`
+option will not be. Any source settings that should be excluded from the docs should be specified via `config`, while any
+options that you would like to be included in the generated documentation should live under `meta`.
 
 ```
 sources:
   - name: external_source
     meta:
       external_location: "s3://my-bucket/my-sources/{name}.parquet"
     tables:
@@ -240,15 +243,15 @@
 sources:
   - name: external_source
     meta:
       external_location: "s3://my-bucket/my-sources/{name}.parquet"
     tables:
       - name: source1
       - name: source2
-        meta:
+        config:
           external_location: "read_parquet(['s3://my-bucket/my-sources/source2a.parquet', 's3://my-bucket/my-sources/source2b.parquet'])"
 ```
 
 In this situation, the `external_location` setting on the `source2` table will take precedence, so a dbt model like:
 
 ```
 SELECT *
@@ -266,15 +269,15 @@
 call, which is helpful in the case that you have an external source that is a CSV file which requires special handling for DuckDB to load it correctly:
 
 ```
 sources:
   - name: flights_source
     tables:
       - name: flights
-        meta:
+        config:
           external_location: "read_csv('flights.csv', types={'FlightDate': 'DATE'}, names=['FlightDate', 'UniqueCarrier'])"
           formatter: oldstyle
 ```
 
 Note that we need to override the default `str.format` string formatting strategy for this example
 because the `types={'FlightDate': 'DATE'}` argument to the `read_csv` function will be interpreted by
 `str.format` as a template to be matched on, which will cause a `KeyError: "'FlightDate'"` when we attempt
```

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/column.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/column.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/connections.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,16 +61,23 @@
         # if the connection is in closed or init, there's nothing to do
         if connection.state in {ConnectionState.CLOSED, ConnectionState.INIT}:
             return connection
 
         connection = super(SQLConnectionManager, cls).close(connection)
         return connection
 
-    def cancel(self, connection):
-        pass
+    def cancel(self, connection: Connection):
+        if self._ENV is not None:
+            logger.debug(
+                "cancelling query on connection {}. Details: {}".format(
+                    connection.name, connection
+                )
+            )
+            self._ENV.cancel(connection)
+            logger.debug("query cancelled on connection {}".format(connection.name))
 
     @contextmanager
     def exception_handler(self, sql: str, connection_name="master"):
         try:
             yield
         except dbt.exceptions.DbtRuntimeError:
             raise
```

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/credentials.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,41 +230,43 @@
             "disable_transactions",
         )
 
     def load_settings(self) -> Dict[str, str]:
         settings = self.settings or {}
         if self.use_credential_provider:
             if self.use_credential_provider == "aws":
-                settings.update(_load_aws_credentials(ttl=_get_ttl_hash()))
+                settings.update(
+                    _load_aws_credentials(ttl=_get_ttl_hash(), profile=settings.get("s3_profile")),
+                )
             else:
                 raise ValueError(
                     "Unsupported value for use_credential_provider: "
                     + self.use_credential_provider
                 )
         return settings
 
 
 def _get_ttl_hash(seconds=300):
     return round(time.time() / seconds)
 
 
 @lru_cache()
-def _load_aws_credentials(ttl=None) -> Dict[str, Any]:
+def _load_aws_credentials(ttl=None, profile="default") -> Dict[str, Any]:
     """
     Load AWS credentials from the environment.
 
     This function is cached to prevent unnecessary calls to the AWS API.
 
     :param ttl: Time to live for the cache. If None, the cache will not expire.
     :return: A dictionary containing the AWS credentials which can be used to configure DuckDB settings.
     """
     del ttl  # make mypy happy
     import boto3.session
 
-    session = boto3.session.Session()
+    session = boto3.session.Session(profile_name=profile)
 
     # use STS to verify that the credentials are valid; we will
     # raise a helpful error here if they are not
     sts = session.client("sts")
     sts.get_caller_identity()
 
     # now extract/return them
```

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/__init__.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import duckdb
 
 from ..credentials import DuckDBCredentials
 from ..plugins import BasePlugin
 from ..utils import SourceConfig
 from ..utils import TargetConfig
 from dbt.contracts.connection import AdapterResponse
+from dbt.contracts.connection import Connection
 from dbt.exceptions import DbtRuntimeError
 
 
 def _ensure_event_loop():
     """
     Ensures the current thread has an event loop defined, and creates one if necessary.
     """
@@ -115,14 +116,24 @@
     def get_binding_char(self) -> str:
         return "?"
 
     def supports_comments(self) -> bool:
         return self._supports_comments
 
     @classmethod
+    @abc.abstractmethod
+    def is_cancelable(cls) -> bool:
+        pass
+
+    @classmethod
+    @abc.abstractmethod
+    def cancel(cls, connection: Connection):
+        pass
+
+    @classmethod
     def initialize_db(
         cls, creds: DuckDBCredentials, plugins: Optional[Dict[str, BasePlugin]] = None
     ):
         config = creds.config_options or {}
         plugins = plugins or {}
         for plugin in plugins.values():
             plugin.update_connection_config(creds, config)
```

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/buenavista.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/buenavista.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import psycopg2
 
 from . import Environment
 from .. import credentials
 from .. import utils
 from dbt.contracts.connection import AdapterResponse
+from dbt.contracts.connection import Connection
 
 
 class BVEnvironment(Environment):
     @classmethod
     def _get_conn(cls, dbname: str, remote: credentials.Remote):
         return psycopg2.connect(
             dbname=dbname,
@@ -27,14 +28,21 @@
     def handle(self):
         # Extensions/settings need to be configured per cursor
         conn = self._get_conn(self.creds.database, self.creds.remote)
         cursor = self.initialize_cursor(self.creds, conn.cursor())
         cursor.close()
         return conn
 
+    def is_cancelable(cls):
+        return False
+
+    @classmethod
+    def cancel(cls, connection: Connection):
+        pass
+
     def get_binding_char(self) -> str:
         return "%s"
 
     def submit_python_job(self, handle, parsed_model: dict, compiled_code: str) -> AdapterResponse:
         identifier = parsed_model["alias"]
         payload = {
             "method": "dbt_python_job",
```

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/environments/local.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import threading
 
 from . import Environment
 from .. import credentials
 from .. import utils
 from dbt.contracts.connection import AdapterResponse
+from dbt.contracts.connection import Connection
 from dbt.exceptions import DbtRuntimeError
 
 
 class DuckDBCursorWrapper:
     def __init__(self, cursor):
         self._cursor = cursor
 
@@ -54,14 +55,21 @@
 
     def notify_closed(self):
         with self.lock:
             self.handle_count -= 1
             if self.handle_count == 0 and not self._keep_open:
                 self.close()
 
+    def is_cancelable(cls):
+        return True
+
+    @classmethod
+    def cancel(cls, connection: Connection):
+        connection.handle.cursor().interrupt()
+
     def handle(self):
         # Extensions/settings need to be configured per cursor
         with self.lock:
             if self.conn is None:
                 self.conn = self.initialize_db(self.creds, self._plugins)
             self.handle_count += 1
```

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/impl.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     @classmethod
     def date_function(cls) -> str:
         return "now()"
 
     @classmethod
     def is_cancelable(cls) -> bool:
-        return False
+        return cls.ConnectionManager.env().is_cancelable()
 
     def debug_query(self):
         self.execute("select 1 as id")
 
     @available
     def is_motherduck(self):
         return self.config.credentials.is_motherduck
```

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/__init__.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/delta.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/delta.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/excel.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/excel.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/glue.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/glue.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/motherduck.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/motherduck.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/pd_utils.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/postgres.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/relation.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/adapters/duckdb/utils.py` & `dbt_duckdb-1.7.5/dbt/adapters/duckdb/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/adapters.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/catalog.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/columns.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/incremental_helper.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/incremental_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/external.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/materializations/table.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/persist_docs.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/seed.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/snapshot_helper.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/snapshot_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/dbt_duckdb.egg-info/PKG-INFO` & `dbt_duckdb-1.7.5/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.7.4
+Version: 1.7.5
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -19,15 +19,15 @@
 License-File: LICENSE
 Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: duckdb>=0.7.0
 Provides-Extra: glue
 Requires-Dist: boto3; extra == "glue"
 Requires-Dist: mypy-boto3-glue; extra == "glue"
 Provides-Extra: md
-Requires-Dist: duckdb<=0.9.2,>=0.7.0; extra == "md"
+Requires-Dist: duckdb>=0.10.2; extra == "md"
 
 ## dbt-duckdb
 
 [DuckDB](http://duckdb.org) is an embedded database, similar to SQLite, but designed for OLAP-style analytics.
 It is crazy fast and allows you to read and write data stored in CSV, JSON, and Parquet files directly, without requiring you to load
 them into the database first.
 
@@ -229,15 +229,18 @@
 
 One of DuckDB's most powerful features is its ability to read and write CSV, JSON, and Parquet files directly, without needing to import/export
 them from the database first.
 
 #### Reading from external files
 
 You may reference external files in your dbt models either directly or as dbt `source`s by configuring the `external_location`
-meta option on the source:
+in either the `meta` or the `config` option on the source definition. The difference is that settings under the `meta` option
+will be propagated to the documentation for the source generated via `dbt docs generate`, but the settings under the `config`
+option will not be. Any source settings that should be excluded from the docs should be specified via `config`, while any
+options that you would like to be included in the generated documentation should live under `meta`.
 
 ```
 sources:
   - name: external_source
     meta:
       external_location: "s3://my-bucket/my-sources/{name}.parquet"
     tables:
@@ -267,15 +270,15 @@
 sources:
   - name: external_source
     meta:
       external_location: "s3://my-bucket/my-sources/{name}.parquet"
     tables:
       - name: source1
       - name: source2
-        meta:
+        config:
           external_location: "read_parquet(['s3://my-bucket/my-sources/source2a.parquet', 's3://my-bucket/my-sources/source2b.parquet'])"
 ```
 
 In this situation, the `external_location` setting on the `source2` table will take precedence, so a dbt model like:
 
 ```
 SELECT *
@@ -293,15 +296,15 @@
 call, which is helpful in the case that you have an external source that is a CSV file which requires special handling for DuckDB to load it correctly:
 
 ```
 sources:
   - name: flights_source
     tables:
       - name: flights
-        meta:
+        config:
           external_location: "read_csv('flights.csv', types={'FlightDate': 'DATE'}, names=['FlightDate', 'UniqueCarrier'])"
           formatter: oldstyle
 ```
 
 Note that we need to override the default `str.format` string formatting strategy for this example
 because the `types={'FlightDate': 'DATE'}` argument to the `read_csv` function will be interpreted by
 `str.format` as a template to be matched on, which will cause a `KeyError: "'FlightDate'"` when we attempt
```

### Comparing `dbt_duckdb-1.7.4/dbt_duckdb.egg-info/SOURCES.txt` & `dbt_duckdb-1.7.5/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.4/setup.py` & `dbt_duckdb-1.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     url="https://github.com/jwills/dbt-duckdb",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~=1.7.0",
         "duckdb>=0.7.0",
     ],
-    extras_require={"glue": ["boto3", "mypy-boto3-glue"], "md": ["duckdb>=0.7.0,<=0.9.2"]},
+    extras_require={"glue": ["boto3", "mypy-boto3-glue"], "md": ["duckdb>=0.10.2"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.8",
```


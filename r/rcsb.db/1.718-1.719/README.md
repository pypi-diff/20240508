# Comparing `tmp/rcsb.db-1.718.tar.gz` & `tmp/rcsb_db-1.719.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.db-1.718.tar", last modified: Wed Apr 10 21:05:38 2024, max compression
+gzip compressed data, was "rcsb_db-1.719.tar", last modified: Wed May  8 18:16:48 2024, max compression
```

## Comparing `rcsb.db-1.718.tar` & `rcsb_db-1.719.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/
--rw-r--r--   0 vsts      (1001) docker     (127)    30577 2024-04-10 20:44:31.000000 rcsb.db-1.718/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-10 20:44:31.000000 rcsb.db-1.718/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-10 20:44:31.000000 rcsb.db-1.718/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    25578 2024-04-10 21:05:38.514944 rcsb.db-1.718/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    24032 2024-04-10 20:44:31.000000 rcsb.db-1.718/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.502943 rcsb.db-1.718/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/ETLExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/RepoHoldingsEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13346 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/RepoLoadExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/RepoScanExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/SchemaUpdateExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8990 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/SequenceClustersEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/cockroach/
--rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/CockroachDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/CockroachDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/crate/
--rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/CrateDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/CrateDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/define/
--rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/ContentDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/DataTypeApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15542 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/DataTypeApplicationInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/DataTypeInstanceInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/SchemaDefAccess.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/SchemaDefBuild.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/helpers/
--rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/ContentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/DocumentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/r.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/mongo/
--rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15187 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/DocumentLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/MongoDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    60384 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/PdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/mysql/
--rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19129 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/processors/
--rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/ClusterDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/DataExchangeStatus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/DataTransformFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/RepoHoldingsDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/SchemaDefDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/SchemaDefReShape.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb/db/sql/
--rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/sql/QueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/sql/SqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/sql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb/db/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/CaseNormalizedDict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/ProvenanceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/SchemaProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/TextUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/makePathList.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/unescape.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb/db/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)    22136 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/wf/RepoLoadWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    25578 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 20:48:40.000000 rcsb.db-1.718/rcsb.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      437 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-10 20:44:32.000000 rcsb.db-1.718/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-10 21:05:38.514944 rcsb.db-1.718/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-04-10 20:44:32.000000 rcsb.db-1.718/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.443221 rcsb_db-1.719/
+-rw-r--r--   0 vsts      (1001) docker     (127)    30623 2024-05-08 17:57:49.000000 rcsb_db-1.719/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-08 17:57:49.000000 rcsb_db-1.719/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-05-08 17:57:49.000000 rcsb_db-1.719/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    25578 2024-05-08 18:16:48.443221 rcsb_db-1.719/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    24032 2024-05-08 17:57:49.000000 rcsb_db-1.719/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.431221 rcsb_db-1.719/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.431221 rcsb_db-1.719/rcsb/db/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.431221 rcsb_db-1.719/rcsb/db/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cli/ETLExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cli/RepoHoldingsEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13627 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cli/RepoLoadExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cli/RepoScanExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cli/SchemaUpdateExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8990 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cli/SequenceClustersEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.431221 rcsb_db-1.719/rcsb/db/cockroach/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cockroach/CockroachDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cockroach/CockroachDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cockroach/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/cockroach/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.435221 rcsb_db-1.719/rcsb/db/crate/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/crate/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/crate/CrateDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/crate/CrateDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/crate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.435221 rcsb_db-1.719/rcsb/db/define/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/define/ContentDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/define/DataTypeApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15542 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/define/DataTypeApplicationInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/define/DataTypeInstanceInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/define/SchemaDefAccess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/define/SchemaDefBuild.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/define/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.435221 rcsb_db-1.719/rcsb/db/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/helpers/ContentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/helpers/DocumentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/helpers/r.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.435221 rcsb_db-1.719/rcsb/db/mongo/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mongo/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mongo/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15187 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mongo/DocumentLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mongo/MongoDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    60453 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mongo/PdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mongo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.439221 rcsb_db-1.719/rcsb/db/mysql/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mysql/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mysql/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mysql/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mysql/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mysql/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19129 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mysql/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/mysql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.439221 rcsb_db-1.719/rcsb/db/processors/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/ClusterDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/DataExchangeStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/DataTransformFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/RepoHoldingsDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/SchemaDefDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/SchemaDefReShape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/processors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.439221 rcsb_db-1.719/rcsb/db/sql/
+-rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/sql/QueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/sql/SqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/sql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.439221 rcsb_db-1.719/rcsb/db/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/CaseNormalizedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/ProvenanceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/SchemaProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/TextUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/makePathList.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/utils/unescape.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.439221 rcsb_db-1.719/rcsb/db/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)    22205 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/wf/RepoLoadWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 17:57:49.000000 rcsb_db-1.719/rcsb/db/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 18:16:48.439221 rcsb_db-1.719/rcsb.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    25578 2024-05-08 18:16:48.000000 rcsb_db-1.719/rcsb.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-05-08 18:16:48.000000 rcsb_db-1.719/rcsb.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-08 18:16:48.000000 rcsb_db-1.719/rcsb.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-05-08 18:16:48.000000 rcsb_db-1.719/rcsb.db.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-08 18:01:29.000000 rcsb_db-1.719/rcsb.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      437 2024-05-08 18:16:48.000000 rcsb_db-1.719/rcsb.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-08 18:16:48.000000 rcsb_db-1.719/rcsb.db.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-05-08 17:57:49.000000 rcsb_db-1.719/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-08 18:16:48.443221 rcsb_db-1.719/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-05-08 17:57:49.000000 rcsb_db-1.719/setup.py
```

### Comparing `rcsb.db-1.718/HISTORY.txt` & `rcsb_db-1.719/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -350,7 +350,8 @@
   6-Nov-2023  V1.713 Add maxStepLength argument to RepoLoadWorkflow
  21-Nov-2023  V1.714 Add support in json schema for min and unique items for sub-categories and iterable attributes
  15-Dec-2023  V1.715 Revert setting for mergeValidationReports
  19-Mar-2024  V1.716 Add quality check to PdbxLoader to ensure validation report data are loaded along with the primary data;
                      Begin updating PdbxLoader and RepoLoadEx to support weekly update workflow CLI requirements
  03-Apr-2024  V1.717 Add int_list cifType to DataTypeApplicationInfo
  09-Apr-2024  V1.718 Update RepoLoadExec CLI and RepoLoadWorkflow to support CLI usage from weekly-update workflow
+  6-May-2024  V1.719 Updates to CLI utilities
```

### Comparing `rcsb.db-1.718/LICENSE` & `rcsb_db-1.719/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/PKG-INFO` & `rcsb_db-1.719/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.718
+Version: 1.719
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -235,15 +235,15 @@
                           [--prune_document_size PRUNE_DOCUMENT_SIZE]
                           [--debug] [--mock] [--cache_path CACHE_PATH]
                           [--rebuild_cache] [--rebuild_schema]
                           [--vrpt_repo_path VRPT_REPO_PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
-  --op {pdbx-loader,build-resource-cache,pdbx-db-wiper,pdbx-id-list-splitter,pdbx-loader-check,etl-entity-sequence-clusters,etl-repository-holdings}
+  --op {pdbx_loader,build_resource_cache,pdbx_db_wiper,pdbx_id_list_splitter,pdbx_loader_check,etl_entity_sequence_clusters,etl_repository_holdings}
                         Loading operation to perform
   --load_type {replace,full}
                         Type of load ('replace' for incremental and
                         multi-worker load, 'full' for complete and
                         fresh single-worker load)
   --database {pdbx_core,pdbx_comp_model_core,bird_chem_comp_core,chem_comp,chem_comp_core,bird_chem_comp,bird,bird_family,ihm_dev}
                         Database to load (most common choices are:
@@ -321,65 +321,65 @@
 
 ```bash
 export CONFIG_SUPPORT_TOKEN_ENV=personal_token_used_for_decrypting_config_variables
 export OE_LICENSE=/path/to/oe_license.txt
 export NLTK_DATA=/path/to/nltk_data
 ```
 
-`--op build-resource-cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
+`--op build_resource_cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
 ```bash
-exdb_repo_load_cli --op "build-resource-cache" \
+exdb_repo_load_cli --op "build_resource_cache" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --num_proc 6  \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-db-wiper` - Wipe the pre-existing database (and all of its collections).
+`--op pdbx_db_wiper` - Wipe the pre-existing database (and all of its collections).
 ```bash
-exdb_repo_load_cli --op "pdbx-db-wiper" \
+exdb_repo_load_cli --op "pdbx_db_wiper" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-id-list-splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
+`--op pdbx_id_list_splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
 ```bash
-exdb_repo_load_cli --op "pdbx-id-list-splitter" \
+exdb_repo_load_cli --op "pdbx_id_list_splitter" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 --load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
 --holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
 --num_sublists 10 \
 
 ```
 
-`--op pdbx-loader` - Load a list of entry IDs to ExDB.
+`--op pdbx_loader` - Load a list of entry IDs to ExDB.
 ```bash
-exdb_repo_load_cli --op "pdbx-loader" \
+exdb_repo_load_cli --op "pdbx_loader" \
 --database "pdbx_core" \
 --load_type replace  \
 --config_path /opt/etl-scratch/config/exdb-loader-config.yml \
 --config_name site_info_remote_configuration \
 --num_proc 8  \
 --chunk_size 5  \
 --max_step_length 500 \
 --load_id_list_path "/opt/etl-scratch/work-dir/load_file_lists/pdbx_core_ids-1.txt" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-loader-check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
+`--op pdbx_loader_check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
 ```bash
-exdb_repo_load_cli --op "pdbx-loader-check" \
+exdb_repo_load_cli --op "pdbx_loader_check" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 --load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
 --holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
 --num_sublists 10 \
```

### Comparing `rcsb.db-1.718/README.md` & `rcsb_db-1.719/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                           [--prune_document_size PRUNE_DOCUMENT_SIZE]
                           [--debug] [--mock] [--cache_path CACHE_PATH]
                           [--rebuild_cache] [--rebuild_schema]
                           [--vrpt_repo_path VRPT_REPO_PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
-  --op {pdbx-loader,build-resource-cache,pdbx-db-wiper,pdbx-id-list-splitter,pdbx-loader-check,etl-entity-sequence-clusters,etl-repository-holdings}
+  --op {pdbx_loader,build_resource_cache,pdbx_db_wiper,pdbx_id_list_splitter,pdbx_loader_check,etl_entity_sequence_clusters,etl_repository_holdings}
                         Loading operation to perform
   --load_type {replace,full}
                         Type of load ('replace' for incremental and
                         multi-worker load, 'full' for complete and
                         fresh single-worker load)
   --database {pdbx_core,pdbx_comp_model_core,bird_chem_comp_core,chem_comp,chem_comp_core,bird_chem_comp,bird,bird_family,ihm_dev}
                         Database to load (most common choices are:
@@ -277,65 +277,65 @@
 
 ```bash
 export CONFIG_SUPPORT_TOKEN_ENV=personal_token_used_for_decrypting_config_variables
 export OE_LICENSE=/path/to/oe_license.txt
 export NLTK_DATA=/path/to/nltk_data
 ```
 
-`--op build-resource-cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
+`--op build_resource_cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
 ```bash
-exdb_repo_load_cli --op "build-resource-cache" \
+exdb_repo_load_cli --op "build_resource_cache" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --num_proc 6  \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-db-wiper` - Wipe the pre-existing database (and all of its collections).
+`--op pdbx_db_wiper` - Wipe the pre-existing database (and all of its collections).
 ```bash
-exdb_repo_load_cli --op "pdbx-db-wiper" \
+exdb_repo_load_cli --op "pdbx_db_wiper" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-id-list-splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
+`--op pdbx_id_list_splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
 ```bash
-exdb_repo_load_cli --op "pdbx-id-list-splitter" \
+exdb_repo_load_cli --op "pdbx_id_list_splitter" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 --load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
 --holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
 --num_sublists 10 \
 
 ```
 
-`--op pdbx-loader` - Load a list of entry IDs to ExDB.
+`--op pdbx_loader` - Load a list of entry IDs to ExDB.
 ```bash
-exdb_repo_load_cli --op "pdbx-loader" \
+exdb_repo_load_cli --op "pdbx_loader" \
 --database "pdbx_core" \
 --load_type replace  \
 --config_path /opt/etl-scratch/config/exdb-loader-config.yml \
 --config_name site_info_remote_configuration \
 --num_proc 8  \
 --chunk_size 5  \
 --max_step_length 500 \
 --load_id_list_path "/opt/etl-scratch/work-dir/load_file_lists/pdbx_core_ids-1.txt" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-loader-check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
+`--op pdbx_loader_check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
 ```bash
-exdb_repo_load_cli --op "pdbx-loader-check" \
+exdb_repo_load_cli --op "pdbx_loader_check" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 --load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
 --holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
 --num_sublists 10 \
```

### Comparing `rcsb.db-1.718/rcsb/db/cli/ETLExec.py` & `rcsb_db-1.719/rcsb/db/cli/ETLExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/cli/RepoHoldingsEtlWorker.py` & `rcsb_db-1.719/rcsb/db/cli/RepoHoldingsEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/cli/RepoLoadExec.py` & `rcsb_db-1.719/rcsb/db/cli/RepoLoadExec.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #    12-Dec-2018 - jdw add core_entity_monomer collection support
 #    13-Dec-2018 - jdw add I/HM schema support
 #    23-Nov-2021 - dwp Add pdbx_comp_model_core
 #    19-Mar-2024 - dwp Updating arguments and making compatible with luigi workflow
 #     5-Apr-2024 - dwp Change arguments and execution structure to make more flexible;
 #                      Add arguments and logic to support CLI usage from weekly-update workflow;
 #                      Add support for logging output to a specific file
+#    25-Apr-2024 - dwp Add support for remote config file loading; use underscores instead of hyphens for arg choices
 ##
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import os
@@ -44,22 +45,20 @@
 # logging.basicConfig(level=logging.INFO, format="%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s", stream=sys.stdout)
 logger = logging.getLogger()
 
 
 def main():
     parser = argparse.ArgumentParser()
     #
-    # defaultConfigName = "site_info_configuration"
-    #
     parser.add_argument(
         "--op",
         default=None,
         required=True,
         help="Loading operation to perform",
-        choices=["pdbx-loader", "build-resource-cache", "pdbx-db-wiper", "pdbx-id-list-splitter", "pdbx-loader-check", "etl-entity-sequence-clusters", "etl-repository-holdings"]
+        choices=["pdbx_loader", "build_resource_cache", "pdbx_db_wiper", "pdbx_id_list_splitter", "pdbx_loader_check", "etl_entity_sequence_clusters", "etl_repository_holdings"]
     )
     #
     parser.add_argument(
         "--load_type",
         default="replace",
         help="Type of load ('replace' for incremental and multi-worker load, 'full' for complete and fresh single-worker load)",
         choices=["replace", "full"],
@@ -111,105 +110,104 @@
     parser.add_argument("--cluster_filename_template", default=None, help="Filename template for cluster files (e.g., clusters-by-entity-90.txt)")
     parser.add_argument("--log_file_path", default=None, help="Path to runtime log file output.")
     #
     args = parser.parse_args()
     #
     try:
         op, commonD, loadD = processArguments(args)
-    except Exception as e:
-        logger.exception("Argument processing problem %s", str(e))
-        parser.print_help(sys.stderr)
-        exit(1)
+    except Exception as err:
+        logger.exception("Argument processing problem %s", str(err))
+        raise ValueError("Argument processing problem") from err
+    #
     #
     # Log input arguments
     loadLogD = {k: v for d in [commonD, loadD] for k, v in d.items() if k != "inputIdCodeList"}
     logger.info("running load op %r on loadLogD %r:", op, loadLogD)
-
-    # ----------------------- - ----------------------- - ----------------------- - ----------------------- - ----------------------- -
-    # Run the operation
     #
+    # Run the operation
     okR = False
     rlWf = RepoLoadWorkflow(**commonD)
-    if op in ["pdbx-loader", "etl-entity-sequence-clusters", "etl-repository-holdings"]:
+    if op in ["pdbx_loader", "etl_entity_sequence_clusters", "etl_repository_holdings"]:
         okR = rlWf.load(op, **loadD)
     #
-    elif op == "build-resource-cache":
+    elif op == "build_resource_cache":
         okR = rlWf.buildResourceCache(rebuildCache=True, providerTypeExclude=loadD["providerTypeExclude"])
     #
-    elif op == "pdbx-id-list-splitter":
+    elif op == "pdbx_id_list_splitter":
         okR = rlWf.splitIdList(op, **loadD)
     #
-    elif op == "pdbx-db-wiper":
+    elif op == "pdbx_db_wiper":
         okR = rlWf.removeAndRecreateDbCollections(op, **loadD)
     #
-    elif op == "pdbx-loader-check":
+    elif op == "pdbx_loader_check":
         okR = rlWf.loadCompleteCheck(op, **loadD)
     #
     else:
         logger.error("Unsupported op %r", op)
-
+    #
     logger.info("Operation %r completed with status %r", op, okR)
-
+    #
     if not okR:
         logger.error("Operation %r failed with status %r", op, okR)
-        exit(1)
+        raise ValueError("Operation %r failed" % op)
 
 
 def processArguments(args):
+    # Logging details
     logFilePath = args.log_file_path
     debugFlag = args.debug
     if debugFlag:
         logger.setLevel(logging.DEBUG)
     else:
         logger.setLevel(logging.INFO)
-    #
     if logFilePath:
         logDir = os.path.dirname(logFilePath)
         if not os.path.isdir(logDir):
             os.makedirs(logDir)
         handler = logging.FileHandler(logFilePath, mode="a")
         if debugFlag:
             handler.setLevel(logging.DEBUG)
         else:
             handler.setLevel(logging.INFO)
         formatter = logging.Formatter("%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s")
         handler.setFormatter(formatter)
         logger.addHandler(handler)
     #
-    # Configuration Details
+    # Configuration details
     configPath = args.config_path
     configName = args.config_name
-    if not configPath:
-        configPath = os.getenv("DBLOAD_CONFIG_PATH", None)
-    try:
-        if os.access(configPath, os.R_OK):
-            os.environ["DBLOAD_CONFIG_PATH"] = configPath
-            logger.info("Using configuation path %s (%s)", configPath, configName)
-        else:
-            logger.error("Missing or access issue with config file %r", configPath)
-            exit(1)
-        mockTopPath = os.path.join(TOPDIR, "rcsb", "mock-data") if args.mock else None
-        cfgOb = ConfigUtil(configPath=configPath, defaultSectionName=configName, mockTopPath=mockTopPath)
-        if args.vrpt_repo_path:
-            vrptPath = args.vrpt_repo_path
-            if not os.access(vrptPath, os.R_OK):
-                logger.error("Unreadable validation report repository path %r", vrptPath)
-            envName = cfgOb.get("VRPT_REPO_PATH_ENV", sectionName=configName)
-            os.environ[envName] = vrptPath
-            logger.info("Using alternate validation report path %s", os.getenv(envName))
-    except Exception as e:
-        logger.error("Missing or access issue with config file %r with %s", configPath, str(e))
-        exit(1)
+    if not (configPath and configName):
+        logger.error("Config path and/or name not provided: %r, %r", configPath, configName)
+        raise ValueError("Config path and/or name not provided: %r, %r" % (configPath, configName))
+    mockTopPath = os.path.join(TOPDIR, "rcsb", "mock-data") if args.mock else None
+    logger.info("Using configuration file %r (section %r)", configPath, configName)
+    cfgOb = ConfigUtil(configPath=configPath, defaultSectionName=configName, mockTopPath=mockTopPath)
+    cfgObTmp = cfgOb.exportConfig()
+    logger.info("Length of config object (%r)", len(cfgObTmp))
+    if len(cfgObTmp) == 0:
+        logger.error("Missing or access issue for config file %r", configPath)
+        raise ValueError("Missing or access issue for config file %r" % configPath)
+    else:
+        del cfgObTmp
+    #
+    if args.vrpt_repo_path:
+        vrptPath = args.vrpt_repo_path
+        if not os.access(vrptPath, os.R_OK):
+            logger.error("Unreadable validation report repository path %r", vrptPath)
+            raise ValueError("Unreadable validation report repository path %r" % vrptPath)
+        envName = cfgOb.get("VRPT_REPO_PATH_ENV", sectionName=configName)
+        os.environ[envName] = vrptPath
+        logger.info("Using alternate validation report path %s", os.getenv(envName))
     #
-    # First do any needed argument checking
+    # Do any additional argument checking
     op = args.op
     databaseName = args.database
     if not op:
         raise ValueError("Must supply a value to '--op' argument")
-    if op == "pdbx-loader" and not databaseName:
+    if op == "pdbx_loader" and not databaseName:
         raise ValueError("Must supply a value to '--database' argument for op type 'pdbx-loader")
     #
     if databaseName == "bird_family":  # Not sure if this is relevant anymore
         dataSelectors = ["BIRD_FAMILY_PUBLIC_RELEASE"]
     else:
         dataSelectors = args.data_selectors if args.data_selectors else ["PUBLIC_RELEASE"]
     #
@@ -257,8 +255,12 @@
         "forceReload": args.force_reload,
     }
 
     return op, commonD, loadD
 
 
 if __name__ == "__main__":
-    main()
+    try:
+        main()
+    except Exception as e:
+        logger.exception("Run failed %s", str(e))
+        sys.exit(1)
```

### Comparing `rcsb.db-1.718/rcsb/db/cli/RepoScanExec.py` & `rcsb_db-1.719/rcsb/db/cli/RepoScanExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/cli/SchemaUpdateExec.py` & `rcsb_db-1.719/rcsb/db/cli/SchemaUpdateExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/cli/SequenceClustersEtlWorker.py` & `rcsb_db-1.719/rcsb/db/cli/SequenceClustersEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/cockroach/CockroachDbLoader.py` & `rcsb_db-1.719/rcsb/db/cockroach/CockroachDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/cockroach/CockroachDbUtil.py` & `rcsb_db-1.719/rcsb/db/cockroach/CockroachDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/cockroach/Connection.py` & `rcsb_db-1.719/rcsb/db/cockroach/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/crate/Connection.py` & `rcsb_db-1.719/rcsb/db/crate/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/crate/CrateDbLoader.py` & `rcsb_db-1.719/rcsb/db/crate/CrateDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/crate/CrateDbUtil.py` & `rcsb_db-1.719/rcsb/db/crate/CrateDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/define/ContentDefinition.py` & `rcsb_db-1.719/rcsb/db/define/ContentDefinition.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/define/DataTypeApiProvider.py` & `rcsb_db-1.719/rcsb/db/define/DataTypeApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/define/DataTypeApplicationInfo.py` & `rcsb_db-1.719/rcsb/db/define/DataTypeApplicationInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/define/DataTypeInstanceInfo.py` & `rcsb_db-1.719/rcsb/db/define/DataTypeInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/define/SchemaDefAccess.py` & `rcsb_db-1.719/rcsb/db/define/SchemaDefAccess.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/define/SchemaDefBuild.py` & `rcsb_db-1.719/rcsb/db/define/SchemaDefBuild.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/helpers/ContentDefinitionHelper.py` & `rcsb_db-1.719/rcsb/db/helpers/ContentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/helpers/DocumentDefinitionHelper.py` & `rcsb_db-1.719/rcsb/db/helpers/DocumentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/helpers/r.py` & `rcsb_db-1.719/rcsb/db/helpers/r.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mongo/Connection.py` & `rcsb_db-1.719/rcsb/db/mongo/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mongo/ConnectionBase.py` & `rcsb_db-1.719/rcsb/db/mongo/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mongo/DocumentLoader.py` & `rcsb_db-1.719/rcsb/db/mongo/DocumentLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mongo/MongoDbUtil.py` & `rcsb_db-1.719/rcsb/db/mongo/MongoDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mongo/PdbxLoader.py` & `rcsb_db-1.719/rcsb/db/mongo/PdbxLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
             statusStartTimestamp = desp.setStartTime()
             #
             logger.info("Beginning load operation (%r) for database %s", loadType, databaseName)
             startTime = self.__begin(message="loading operation")
             #
             # -- Check database to see if any entries have already been loaded, and determine the delta for the current load
             inputIdCodeList = inputIdCodeList if inputIdCodeList else []
+            inputIdCodeList = [id.upper() for id in inputIdCodeList]
             if databaseName in ["pdbx_core", "pdbx_comp_model_core"]:
                 totalIdsAlreadyLoaded = self.__getLoadedRcsbIdList(databaseName=databaseName, collectionName=databaseName + "_entry")
                 # Get the list of IDs from only the given sublist that are already loaded
                 subsetIdsAlreadyLoaded = list(set(totalIdsAlreadyLoaded).intersection(set(inputIdCodeList)))
                 if not forceReload:
                     # Get a list of the delta between the two lists—-i.e., the entry IDs needed to be loaded
                     idCodesToLoadL = list(set(inputIdCodeList) ^ set(subsetIdsAlreadyLoaded))
```

### Comparing `rcsb.db-1.718/rcsb/db/mysql/Connection.py` & `rcsb_db-1.719/rcsb/db/mysql/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mysql/ConnectionBase.py` & `rcsb_db-1.719/rcsb/db/mysql/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mysql/MyDbAdapter.py` & `rcsb_db-1.719/rcsb/db/mysql/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mysql/MyDbUtil.py` & `rcsb_db-1.719/rcsb/db/mysql/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mysql/MysqlSchemaImporter.py` & `rcsb_db-1.719/rcsb/db/mysql/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/mysql/SchemaDefLoader.py` & `rcsb_db-1.719/rcsb/db/mysql/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/processors/ClusterDataPrep.py` & `rcsb_db-1.719/rcsb/db/processors/ClusterDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/processors/DataExchangeStatus.py` & `rcsb_db-1.719/rcsb/db/processors/DataExchangeStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/processors/DataTransformFactory.py` & `rcsb_db-1.719/rcsb/db/processors/DataTransformFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/processors/RepoHoldingsDataPrep.py` & `rcsb_db-1.719/rcsb/db/processors/RepoHoldingsDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py` & `rcsb_db-1.719/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/processors/SchemaDefDataPrep.py` & `rcsb_db-1.719/rcsb/db/processors/SchemaDefDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/processors/SchemaDefReShape.py` & `rcsb_db-1.719/rcsb/db/processors/SchemaDefReShape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/sql/QueryDirectives.py` & `rcsb_db-1.719/rcsb/db/sql/QueryDirectives.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/sql/SqlGen.py` & `rcsb_db-1.719/rcsb/db/sql/SqlGen.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/CaseNormalizedDict.py` & `rcsb_db-1.719/rcsb/db/utils/CaseNormalizedDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/PdbxSchemaMapReader.py` & `rcsb_db-1.719/rcsb/db/utils/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/ProvenanceProvider.py` & `rcsb_db-1.719/rcsb/db/utils/ProvenanceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/SchemaProvider.py` & `rcsb_db-1.719/rcsb/db/utils/SchemaProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/TextUtil.py` & `rcsb_db-1.719/rcsb/db/utils/TextUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/TimeUtil.py` & `rcsb_db-1.719/rcsb/db/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/makePathList.py` & `rcsb_db-1.719/rcsb/db/utils/makePathList.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/utils/unescape.py` & `rcsb_db-1.719/rcsb/db/utils/unescape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/rcsb/db/wf/RepoLoadWorkflow.py` & `rcsb_db-1.719/rcsb/db/wf/RepoLoadWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 logger = logging.getLogger(__name__)
 
 
 class RepoLoadWorkflow(object):
     def __init__(self, **kwargs):
         #  Configuration Details
         configPath = kwargs.get("configPath", "exdb-config-example.yml")
-        self.__configName = kwargs.get("configName", "site_info_configuration")
+        self.__configName = kwargs.get("configName", "site_info_remote_configuration")
         mockTopPath = kwargs.get("mockTopPath", None)
         self.__cfgOb = ConfigUtil(configPath=configPath, defaultSectionName=self.__configName, mockTopPath=mockTopPath)
         #
         self.__cachePath = kwargs.get("cachePath", ".")
         self.__cachePath = os.path.abspath(self.__cachePath)
         self.__debugFlag = kwargs.get("debugFlag", False)
         if self.__debugFlag:
@@ -56,15 +56,15 @@
         #
 
     def load(self, op, **kwargs):
         # if not self.__cacheStatus:
         #    logger.error("Resource cache test or rebuild has failed - exiting")
         #    return False
         # argument processing
-        if op not in ["pdbx-loader", "etl-repository-holdings", "etl-entity-sequence-clusters"]:
+        if op not in ["pdbx_loader", "etl_repository_holdings", "etl_entity_sequence_clusters"]:
             logger.error("Unsupported operation %r - exiting", op)
             return False
         try:
             databaseName = kwargs.get("databaseName", None)
             databaseNameList = self.__cfgOb.get("DATABASE_NAMES_ALL", sectionName="database_catalog_configuration").split(",")
             collectionNameList = kwargs.get("collectionNameList", None)
             loadType = kwargs.get("loadType", "replace")  # or "full"
@@ -108,15 +108,15 @@
             sandboxPath = self.__cfgOb.getPath("RCSB_EXCHANGE_SANDBOX_PATH", sectionName=self.__configName)
 
         except Exception as e:
             logger.exception("Argument and configuration processing failing with %s", str(e))
             return False
         #
 
-        if op == "pdbx-loader" and dbType == "mongo" and databaseName in databaseNameList:
+        if op == "pdbx_loader" and dbType == "mongo" and databaseName in databaseNameList:
             okS = True
             try:
                 inputPathList, inputIdCodeList = None, None
                 if loadIdListPath:
                     mu = MarshalUtil(workPath=self.__cachePath)
                     inputIdCodeList = mu.doImport(loadIdListPath, fmt="list")
                     if not inputIdCodeList:
@@ -163,29 +163,29 @@
                     updateSchemaOnReplace=updateSchemaOnReplace,
                     rebuildCache=rebuildCache,
                     forceReload=forceReload,
                 )
                 okS = self.loadStatus(mw.getLoadStatus(), readBackCheck=readBackCheck)
             except Exception as e:
                 logger.exception("Operation %r database %r failing with %s", op, databaseName, str(e))
-        elif op == "etl-entity-sequence-clusters" and dbType == "mongo":
+        elif op == "etl_entity_sequence_clusters" and dbType == "mongo":
             cw = SequenceClustersEtlWorker(
                 self.__cfgOb,
                 numProc=numProc,
                 chunkSize=chunkSize,
                 maxStepLength=maxStepLength,
                 documentLimit=documentLimit,
                 verbose=self.__debugFlag,
                 readBackCheck=readBackCheck,
                 workPath=self.__cachePath,
                 clusterFileNameTemplate=clusterFileNameTemplate,
             )
             ok = cw.etl(dataSetId, seqDataLocator, loadType=loadType)
             okS = self.loadStatus(cw.getLoadStatus(), readBackCheck=readBackCheck)
-        elif op == "etl-repository-holdings" and dbType == "mongo":
+        elif op == "etl_repository_holdings" and dbType == "mongo":
             rhw = RepoHoldingsEtlWorker(
                 self.__cfgOb,
                 sandboxPath,
                 self.__cachePath,
                 numProc=numProc,
                 chunkSize=chunkSize,
                 maxStepLength=maxStepLength,
@@ -209,15 +209,15 @@
             databaseName = self.__cfgOb.get("DATABASE_NAME", sectionName=sectionName)
             collectionName = self.__cfgOb.get("COLLECTION_UPDATE_STATUS", sectionName=sectionName)
             ret = dl.load(databaseName, collectionName, loadType="append", documentList=statusList, indexAttributeList=["update_id", "database_name", "object_name"], keyNames=None)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ret
 
-    def buildResourceCache(self, rebuildCache=False, providerTypeExclude=None):
+    def buildResourceCache(self, rebuildCache=False, providerTypeExclude=None, restoreUseStash=True, restoreUseGit=True):
         """Generate and cache resource dependencies."""
         ret = False
         try:
             # First make sure the CACHE directory exists
             if not os.path.isdir(self.__cachePath):
                 logger.info("Cache directory %s doesn't exist. Creating it", self.__cachePath)
                 os.makedirs(self.__cachePath)
@@ -226,27 +226,27 @@
 
             # Now build the cache
             useCache = not rebuildCache
             rP = DictMethodResourceProvider(
                 self.__cfgOb,
                 configName=self.__configName,
                 cachePath=self.__cachePath,
-                restoreUseStash=True,
-                restoreUseGit=True,
+                restoreUseStash=restoreUseStash,
+                restoreUseGit=restoreUseGit,
                 providerTypeExclude=providerTypeExclude,
             )
             ret = rP.cacheResources(useCache=useCache, doBackup=False, useStash=False, useGit=False)
             logger.info("useCache %r cache reload status (%r)", useCache, ret)
 
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ret
 
     def removeAndRecreateDbCollections(self, op, **kwargs):
-        if op not in ["pdbx-db-wiper"]:
+        if op not in ["pdbx_db_wiper"]:
             logger.error("Unsupported operation %r - exiting", op)
             return False
         try:
             schemaLevel = kwargs.get("schemaLevel", "min") if kwargs.get("schemaLevel") in ["min", "full"] else "min"
             dbType = kwargs.get("dbType", "mongo")
             #
             databaseName = kwargs.get("databaseName", None)
@@ -274,15 +274,15 @@
                 logger.exception("Operation %r database %r failing with %s", op, databaseName, str(e))
 
         logger.info("Completed operation %r with status %r", op, ok)
 
         return ok
 
     def splitIdList(self, op, **kwargs):
-        if op not in ["pdbx-id-list-splitter"]:
+        if op not in ["pdbx_id_list_splitter"]:
             logger.error("Unsupported operation %r - exiting", op)
             return False
 
         databaseName = kwargs.get("databaseName")
         holdingsFilePath = kwargs.get("holdingsFilePath", None)  # For CSMs: http://computed-models-internal-%s.rcsb.org/staging/holdings/computed-models-holdings-list.json
         loadFileListDir = kwargs.get("loadFileListDir")  # ExchangeDbConfig().loadFileListsDir
         loadFileListPrefix = databaseName + "_ids"  # pdbx_core_ids or pdbx_comp_model_core_ids
@@ -380,15 +380,15 @@
         ok = mU.doExport(mappingFilePath, filePathMappingD, fmt="json", indent=4)
         if not ok:
             raise ValueError("Failed to export mappingFilePath %r" % mappingFilePath)
 
         return filePathMappingD
 
     def loadCompleteCheck(self, op, **kwargs):
-        if op not in ["pdbx-loader-check"]:
+        if op not in ["pdbx_loader_check"]:
             logger.error("Unsupported operation %r - exiting", op)
             return False
         try:
             databaseName = kwargs.get("databaseName", None)
             holdingsFilePath = kwargs.get("holdingsFilePath", None)
             completeIdCodeList, completeIdCodeCount = self.__getCompleteIdListCount(databaseName, holdingsFilePath)
             if not (completeIdCodeList or completeIdCodeCount):
```

### Comparing `rcsb.db-1.718/rcsb.db.egg-info/PKG-INFO` & `rcsb_db-1.719/rcsb.db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.718
+Version: 1.719
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -235,15 +235,15 @@
                           [--prune_document_size PRUNE_DOCUMENT_SIZE]
                           [--debug] [--mock] [--cache_path CACHE_PATH]
                           [--rebuild_cache] [--rebuild_schema]
                           [--vrpt_repo_path VRPT_REPO_PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
-  --op {pdbx-loader,build-resource-cache,pdbx-db-wiper,pdbx-id-list-splitter,pdbx-loader-check,etl-entity-sequence-clusters,etl-repository-holdings}
+  --op {pdbx_loader,build_resource_cache,pdbx_db_wiper,pdbx_id_list_splitter,pdbx_loader_check,etl_entity_sequence_clusters,etl_repository_holdings}
                         Loading operation to perform
   --load_type {replace,full}
                         Type of load ('replace' for incremental and
                         multi-worker load, 'full' for complete and
                         fresh single-worker load)
   --database {pdbx_core,pdbx_comp_model_core,bird_chem_comp_core,chem_comp,chem_comp_core,bird_chem_comp,bird,bird_family,ihm_dev}
                         Database to load (most common choices are:
@@ -321,65 +321,65 @@
 
 ```bash
 export CONFIG_SUPPORT_TOKEN_ENV=personal_token_used_for_decrypting_config_variables
 export OE_LICENSE=/path/to/oe_license.txt
 export NLTK_DATA=/path/to/nltk_data
 ```
 
-`--op build-resource-cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
+`--op build_resource_cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
 ```bash
-exdb_repo_load_cli --op "build-resource-cache" \
+exdb_repo_load_cli --op "build_resource_cache" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --num_proc 6  \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-db-wiper` - Wipe the pre-existing database (and all of its collections).
+`--op pdbx_db_wiper` - Wipe the pre-existing database (and all of its collections).
 ```bash
-exdb_repo_load_cli --op "pdbx-db-wiper" \
+exdb_repo_load_cli --op "pdbx_db_wiper" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-id-list-splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
+`--op pdbx_id_list_splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
 ```bash
-exdb_repo_load_cli --op "pdbx-id-list-splitter" \
+exdb_repo_load_cli --op "pdbx_id_list_splitter" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 --load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
 --holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
 --num_sublists 10 \
 
 ```
 
-`--op pdbx-loader` - Load a list of entry IDs to ExDB.
+`--op pdbx_loader` - Load a list of entry IDs to ExDB.
 ```bash
-exdb_repo_load_cli --op "pdbx-loader" \
+exdb_repo_load_cli --op "pdbx_loader" \
 --database "pdbx_core" \
 --load_type replace  \
 --config_path /opt/etl-scratch/config/exdb-loader-config.yml \
 --config_name site_info_remote_configuration \
 --num_proc 8  \
 --chunk_size 5  \
 --max_step_length 500 \
 --load_id_list_path "/opt/etl-scratch/work-dir/load_file_lists/pdbx_core_ids-1.txt" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 
 ```
 
-`--op pdbx-loader-check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
+`--op pdbx_loader_check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
 ```bash
-exdb_repo_load_cli --op "pdbx-loader-check" \
+exdb_repo_load_cli --op "pdbx_loader_check" \
 --database "pdbx_core" \
 --config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
 --config_name "site_info_remote_configuration" \
 --cache_path "/opt/etl-scratch/data/CACHE" \
 --load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
 --holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
 --num_sublists 10 \
```

### Comparing `rcsb.db-1.718/rcsb.db.egg-info/SOURCES.txt` & `rcsb_db-1.719/rcsb.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/requirements.txt` & `rcsb_db-1.719/requirements.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.718/setup.py` & `rcsb_db-1.719/setup.py`

 * *Files identical despite different names*


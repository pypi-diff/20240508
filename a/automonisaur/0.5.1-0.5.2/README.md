# Comparing `tmp/automonisaur-0.5.1.tar.gz` & `tmp/automonisaur-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automonisaur-0.5.1.tar", last modified: Wed Apr  3 01:57:19 2024, max compression
+gzip compressed data, was "automonisaur-0.5.2.tar", last modified: Wed May  8 09:52:49 2024, max compression
```

## Comparing `automonisaur-0.5.1.tar` & `automonisaur-0.5.2.tar`

### file list

```diff
@@ -1,411 +1,416 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.302019 automonisaur-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 01:57:15.000000 automonisaur-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 01:57:19.302019 automonisaur-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-03 01:57:15.000000 automonisaur-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.254018 automonisaur-0.5.1/automon/
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.258018 automonisaur-0.5.1/automon/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/assertions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.258018 automonisaur-0.5.1/automon/helpers/asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/asyncioWrapper/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.258018 automonisaur-0.5.1/automon/helpers/cryptography/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/cryptography/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/cryptography/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/httpWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.258018 automonisaur-0.5.1/automon/helpers/mathWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/mathWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/mathWrapper/file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.258018 automonisaur-0.5.1/automon/helpers/osWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/osWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/osWrapper/environ.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.258018 automonisaur-0.5.1/automon/helpers/subprocessWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.258018 automonisaur-0.5.1/automon/helpers/subprocessWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/subprocessWrapper/tests/test_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_sleeper.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/tests/test_sleeper_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/helpers/threadingWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/threadingWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/threadingWrapper/initialize_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/helpers/threadingWrapper/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/beautifulsoupWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/beautifulsoupWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/beautifulsoupWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/cryptocurrency/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/cryptocurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/cryptocurrency/accounting.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/cryptocurrency/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/cryptocurrency/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/cryptocurrency/robinhood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/cryptocurrency/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/cryptocurrency/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/cryptocurrency/tests/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/datadogWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/datadogWrapper/api/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/api/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/datadogWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datadogWrapper/tests/test_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/datascience/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datascience/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.262019 automonisaur-0.5.1/automon/integrations/datascience/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datascience/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datascience/pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datascience/pandas/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datascience/pandas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/datascience/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datascience/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/datascience/tests/test_datascience.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/elasticsearch/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/facebook/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/flaskWrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/flaskWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/flaskWrapper/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/flaskWrapper/auth_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/flaskWrapper/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/flaskWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/flaskWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/flaskWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/flaskWrapper/tests/test_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/geoip/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/geoip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/geoip/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/geoip/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/geoip/tests/test_geoip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.266018 automonisaur-0.5.1/automon/integrations/google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/auth/tests/test_config_Credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/auth/tests/test_google_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/gmail/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/gmail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/gmail/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/gmail/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/gmail/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/gmail/v1/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/people/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/people/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/people/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/sheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/sheets/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/sheets/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/sheets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/sheets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/sheets/tests/test_google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/google/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/google/tests/test_google_contacts_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.270018 automonisaur-0.5.1/automon/integrations/grok/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/grok/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/grok/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/grok/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/grok/tests/test_grok.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/stories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/instagram/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/tests/test_instagram.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/tests/test_instagram_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/tests/test_instagram_browser_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/tests/test_instagram_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/instagram/xpaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/ldap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/ldap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/mac/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/mac/airport/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/airport/airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/airport/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/airport/ssid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/mac/airport/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/airport/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/airport/tests/test_airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/airport/tests/test_airport_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/mac/macchanger/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/macchanger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/macchanger/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.274018 automonisaur-0.5.1/automon/integrations/mac/macchanger/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/macchanger/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/macchanger/tests/test_macchanger.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.278019 automonisaur-0.5.1/automon/integrations/minioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.278019 automonisaur-0.5.1/automon/integrations/minioWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/tests/test_minio_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/tests/test_minio_client_public.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/minioWrapper/tests/test_minio_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.278019 automonisaur-0.5.1/automon/integrations/neo4jWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/cypher.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.278019 automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.278019 automonisaur-0.5.1/automon/integrations/nest_asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nest_asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nest_asyncioWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.278019 automonisaur-0.5.1/automon/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nmap/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nmap/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nmap/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/nmap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nmap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nmap/tests/test_nmap_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/nmap/tests/test_nmap_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/test/test_client_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/test/test_memory_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/openvpn/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openvpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/openvpn/openvpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/psutilWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/psutilWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/psutilWrapper/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/requestsWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/requestsWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.282019 automonisaur-0.5.1/automon/integrations/scrapyWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/scrapyWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/scrapyWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/seleniumWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17113 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/browser_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/browser_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/config_window_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_new_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/seleniumWrapper/webdriver_chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/sentryio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/sentryio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/sentryio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/sentryio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/sentryio/tests/test_sentryio.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/sentryio/tests/test_sentryio_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/shodan/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/shodan/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/shodan/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/shodan/tests/test_shodan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/slackWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/bots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/slack_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/slack_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.286018 automonisaur-0.5.1/automon/integrations/slackWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/slackWrapper/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.290018 automonisaur-0.5.1/automon/integrations/snmp/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/snmp/generate_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.290018 automonisaur-0.5.1/automon/integrations/splunk/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.290018 automonisaur-0.5.1/automon/integrations/splunk/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk/tests/test_splunk_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk/tests/test_splunk_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.290018 automonisaur-0.5.1/automon/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.290018 automonisaur-0.5.1/automon/integrations/splunk_soar/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.290018 automonisaur-0.5.1/automon/integrations/splunk_soar/integration/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/integration/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/integration/servicenow/ticket.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/phantom_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.290018 automonisaur-0.5.1/automon/integrations/splunk_soar/rest/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/rest/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.294018 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/dino.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_uat.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/splunk_soar/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.294018 automonisaur-0.5.1/automon/integrations/swift/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swift/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swift/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swift/iterables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/integrations/swift/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swift/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swift/tests/test_swift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/api/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/integrations/vds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/vds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/vds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/vds/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/integrations/vds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/vds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/integrations/vds/tests/test_vds.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/liveliness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)      317 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/log/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.298019 automonisaur-0.5.1/automon/log/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/log/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 01:57:15.000000 automonisaur-0.5.1/automon/log/tests/test_logger_builtin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:57:19.302019 automonisaur-0.5.1/automonisaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 01:57:19.000000 automonisaur-0.5.1/automonisaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-04-03 01:57:19.000000 automonisaur-0.5.1/automonisaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:57:19.000000 automonisaur-0.5.1/automonisaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 01:57:19.000000 automonisaur-0.5.1/automonisaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:57:19.302019 automonisaur-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-03 01:57:15.000000 automonisaur-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 09:52:45.000000 automonisaur-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-08 09:52:49.011735 automonisaur-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-08 09:52:45.000000 automonisaur-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.963735 automonisaur-0.5.2/automon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/assertions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/asyncioWrapper/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/cryptography/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/cryptography/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/cryptography/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/httpWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/mathWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/mathWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/mathWrapper/file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/osWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/osWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/osWrapper/environ.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/subprocessWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_sleeper_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/helpers/threadingWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/threadingWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/threadingWrapper/initialize_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/threadingWrapper/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/cryptocurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/robinhood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datadogWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/client_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/config_opentelemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_client_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_config_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datascience/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datascience/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datascience/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/tests/test_datascience.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/facebook/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/flaskWrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/auth_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/test_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/geoip/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/geoip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/geoip/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/geoip/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/geoip/tests/test_geoip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/tests/test_config_Credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/tests/test_google_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/gmail/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/gmail/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/v1/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/people/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/people/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/sheets/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/sheets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/tests/test_google_contacts_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/grok/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/grok/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/grok/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/grok/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/grok/tests/test_grok.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/stories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/instagram/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/xpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/ldap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/ldap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/airport/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/ssid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/airport/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/macchanger/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/test_macchanger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/minioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/neo4jWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/nmap/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/nmap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/tests/test_nmap_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/tests/test_nmap_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_client_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_memory_trace_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_memory_trace_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/openvpn/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openvpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openvpn/openvpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/psutilWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/psutilWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/psutilWrapper/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/requestsWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/scrapyWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/scrapyWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/scrapyWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/seleniumWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17113 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/config_window_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_new_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/webdriver_chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/sentryio/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/sentryio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/shodan/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/shodan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/shodan/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/shodan/tests/test_shodan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/slackWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/bots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/slack_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/slack_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/slackWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/snmp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/snmp/generate_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/splunk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/splunk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/ticket.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/phantom_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/rest/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swift/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/tests/test_swift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/integrations/vds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/integrations/vds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/tests/test_vds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/liveliness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/log/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/tests/test_logger_builtin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automonisaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:52:49.011735 automonisaur-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 09:52:45.000000 automonisaur-0.5.2/setup.py
```

### Comparing `automonisaur-0.5.1/LICENSE` & `automonisaur-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/PKG-INFO` & `automonisaur-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.5.1
+Version: 0.5.2
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](https://github.com/TheShellLand/automonisaur/raw/master/docs/images/sauruspark.gif)
 
 # Automonisaur: Core Libraries
 
@@ -67,15 +67,15 @@
 | Python          | logging<br/>requests                                        |
 | SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
 
-- python >= 3.8
+- python >= 3.10
 
 _Note: install requirements.txt to use all integrations_
 
 #### install core library
 
 ```shell script
 /bin/bash install.sh
```

### Comparing `automonisaur-0.5.1/README.md` & `automonisaur-0.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 | Python          | logging<br/>requests                                        |
 | SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
 
-- python >= 3.8
+- python >= 3.10
 
 _Note: install requirements.txt to use all integrations_
 
 #### install core library
 
 ```shell script
 /bin/bash install.sh
```

### Comparing `automonisaur-0.5.1/automon/helpers/assertions.py` & `automonisaur-0.5.2/automon/helpers/assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/markdown.py` & `automonisaur-0.5.2/automon/helpers/markdown.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/networking.py` & `automonisaur-0.5.2/automon/helpers/networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/osWrapper/environ.py` & `automonisaur-0.5.2/automon/helpers/osWrapper/environ.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/sanitation.py` & `automonisaur-0.5.2/automon/helpers/sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/sleeper.py` & `automonisaur-0.5.2/automon/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/subprocessWrapper/run.py` & `automonisaur-0.5.2/automon/helpers/subprocessWrapper/run.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/subprocessWrapper/tests/test_runner.py` & `automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/tests/test_assertions.py` & `automonisaur-0.5.2/automon/helpers/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/tests/test_networking.py` & `automonisaur-0.5.2/automon/helpers/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/tests/test_sanitation.py` & `automonisaur-0.5.2/automon/helpers/tests/test_sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/tests/test_sleeper.py` & `automonisaur-0.5.2/automon/helpers/tests/test_sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/threadingWrapper/initialize_threading.py` & `automonisaur-0.5.2/automon/helpers/threadingWrapper/initialize_threading.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/helpers/threadingWrapper/worker_thread.py` & `automonisaur-0.5.2/automon/helpers/threadingWrapper/worker_thread.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/beautifulsoupWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/cryptocurrency/accounting.py` & `automonisaur-0.5.2/automon/integrations/cryptocurrency/accounting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/cryptocurrency/coinbase.py` & `automonisaur-0.5.2/automon/integrations/cryptocurrency/coinbase.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/cryptocurrency/other.py` & `automonisaur-0.5.2/automon/integrations/cryptocurrency/other.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/cryptocurrency/robinhood.py` & `automonisaur-0.5.2/automon/integrations/cryptocurrency/robinhood.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/cryptocurrency/tests/test_crypto.py` & `automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/datadogWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/datadogWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/datadogWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/datadogWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/datadogWrapper/tests/test_log.py` & `automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_log.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
             asyncio.run(self.client_tracer.config.test())
 
             spans = asyncio.run(self.client_tracer.to_datadog())
             for span in spans:
                 asyncio.run(
                     self.client.log(
-                        ddsource=span['datadog']['ddsource'],
-                        ddtags=span['datadog']['ddtags'],
-                        hostname=span['datadog']['hostname'],
-                        service=span['datadog']['service'],
-                        message=span['datadog']['message'],
+                        ddsource=span['ddsource'],
+                        ddtags=span['ddtags'],
+                        hostname=span['hostname'],
+                        service=span['service'],
+                        message=span['message'],
                     ))
 
             pass
 
     if __name__ == '__main__':
         unittest.main()
```

### Comparing `automonisaur-0.5.1/automon/integrations/datascience/pandas/pandas.py` & `automonisaur-0.5.2/automon/integrations/datascience/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/datascience/tests/test_datascience.py` & `automonisaur-0.5.2/automon/integrations/datascience/tests/test_datascience.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/cleanup.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/cleanup.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/client.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/config.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/jvm.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/jvm.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/metrics.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/metrics.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/snapshots.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/snapshots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py` & `automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/facebook/groups.py` & `automonisaur-0.5.2/automon/integrations/facebook/groups.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/flaskWrapper/auth.py` & `automonisaur-0.5.2/automon/integrations/flaskWrapper/auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/flaskWrapper/boilerplate.py` & `automonisaur-0.5.2/automon/integrations/flaskWrapper/boilerplate.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/flaskWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/flaskWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/flaskWrapper/tests/test_flask.py` & `automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/auth/client.py` & `automonisaur-0.5.2/automon/integrations/google/auth/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/auth/config.py` & `automonisaur-0.5.2/automon/integrations/google/auth/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/gmail/v1/client.py` & `automonisaur-0.5.2/automon/integrations/google/gmail/v1/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/gmail/v1/config.py` & `automonisaur-0.5.2/automon/integrations/google/gmail/v1/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/people/client.py` & `automonisaur-0.5.2/automon/integrations/google/people/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/people/config.py` & `automonisaur-0.5.2/automon/integrations/google/people/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/people/person.py` & `automonisaur-0.5.2/automon/integrations/google/people/person.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/people/results.py` & `automonisaur-0.5.2/automon/integrations/google/people/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/people/urls.py` & `automonisaur-0.5.2/automon/integrations/google/people/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/sheets/client.py` & `automonisaur-0.5.2/automon/integrations/google/sheets/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/sheets/config.py` & `automonisaur-0.5.2/automon/integrations/google/sheets/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/sheets/tests/test_google_sheets.py` & `automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py` & `automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/google/sheets/tests/test_google_sheets_clear.py` & `automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_clear.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/grok/__init__.py` & `automonisaur-0.5.2/automon/integrations/grok/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/instagram/client.py` & `automonisaur-0.5.2/automon/integrations/instagram/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/instagram/client_browser.py` & `automonisaur-0.5.2/automon/integrations/instagram/client_browser.py`

 * *Files 5% similar despite different names*

```diff
@@ -236,18 +236,18 @@
     def login(self) -> str:
         return self.config.login
 
     async def start(self):
         self.useragent = await self.browser.get_random_user_agent()
 
         if self.headless:
-            await self.browser.config.webdriver_wrapper.in_headless()
-            await self.browser.config.webdriver_wrapper.set_user_agent(self.useragent)
+            self.browser.config.webdriver_wrapper.in_headless()
+            self.browser.config.webdriver_wrapper.set_user_agent(self.useragent)
         else:
-            await self.browser.config.webdriver_wrapper.set_user_agent(self.useragent)
+            self.browser.config.webdriver_wrapper.set_user_agent(self.useragent)
 
     @property
     def urls(self):
         return Urls()
 
     @property
     def xpaths(self):
```

### Comparing `automonisaur-0.5.1/automon/integrations/instagram/config.py` & `automonisaur-0.5.2/automon/integrations/instagram/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/instagram/stories.py` & `automonisaur-0.5.2/automon/integrations/instagram/stories.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/instagram/tests/test_instagram_browser.py` & `automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/instagram/tests/test_instagram_browser_auth.py` & `automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser_auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/instagram/xpaths.py` & `automonisaur-0.5.2/automon/integrations/instagram/xpaths.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/ldap/client.py` & `automonisaur-0.5.2/automon/integrations/ldap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/mac/airport/airport.py` & `automonisaur-0.5.2/automon/integrations/mac/airport/airport.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,18 @@
             self._scan_output = self._runner.stdout
             self._scan_error = self._runner.stderr
             return True
 
         return False
 
     async def scan_channel(self, channel: int = None):
-        return self.scan(channel=channel)
+        return await self.scan(channel=channel)
 
     async def scan_summary(self, channel: int = None, args: str = None, output: bool = True):
-        if self.scan(channel=channel, args=args):
+        if await self.scan(channel=channel, args=args):
             if output:
                 logger.info(f'{self._scan_output}')
             return True
         return False
 
     @property
     def ssids(self):
```

### Comparing `automonisaur-0.5.1/automon/integrations/mac/airport/scan.py` & `automonisaur-0.5.2/automon/integrations/mac/airport/scan.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/mac/airport/ssid.py` & `automonisaur-0.5.2/automon/integrations/mac/airport/ssid.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/mac/airport/tests/test_airport.py` & `automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/mac/airport/tests/test_airport_neo4j.py` & `automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport_neo4j.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import sys
+import asyncio
 import unittest
 
 from automon.integrations.mac.airport import Airport
 
 from automon.integrations.neo4jWrapper import Neo4jClient
 
 
 class AirportToNeo4jTest(unittest.TestCase):
     a = Airport()
     n = Neo4jClient()
 
     def test_scan_xml(self):
-        if self.a.isReady():
-            test = self.a.scan_xml()
+        if asyncio.run(self.a.isReady()):
+            test = asyncio.run(self.a.scan_xml())
             if test:
                 self.assertTrue(test)
 
         if self.n.isConnected():
             # self.n.delete_all()
             for bssid in self.a.ssids:
                 flatten = bssid._ssid
```

### Comparing `automonisaur-0.5.1/automon/integrations/mac/macchanger/client.py` & `automonisaur-0.5.2/automon/integrations/mac/macchanger/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/mac/macchanger/tests/test_macchanger.py` & `automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/test_macchanger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/minioWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/minioWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/minioWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/minioWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/minioWrapper/object.py` & `automonisaur-0.5.2/automon/integrations/minioWrapper/object.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/minioWrapper/tests/test_minio_client.py` & `automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/minioWrapper/tests/test_minio_client_public.py` & `automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py` & `automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/clientAsync.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/cypher.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/results.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/results.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from neo4j.work.summary import ResultSummary
+from neo4j import ResultSummary
 
 from automon import log
 
 logger = log.logging.getLogger(__name__)
 logger.setLevel(log.DEBUG)
```

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py` & `automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/nest_asyncioWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/nmap/client.py` & `automonisaur-0.5.2/automon/integrations/nmap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/nmap/config.py` & `automonisaur-0.5.2/automon/integrations/nmap/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/nmap/output.py` & `automonisaur-0.5.2/automon/integrations/nmap/output.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/nmap/tests/test_nmap_client.py` & `automonisaur-0.5.2/automon/integrations/nmap/tests/test_nmap_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/openTelemetryWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 import asyncio
+import opentelemetry
 
-from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 from opentelemetry.sdk.trace.export.in_memory_span_exporter import InMemorySpanExporter
 
 from automon.log import logging
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class OpenTelemetryConfig(object):
     def __init__(self):
+        self.opentelemetry = opentelemetry
         self.provider = TracerProvider()
         self.memory_processor = InMemorySpanExporter()
         self.processor = SimpleSpanProcessor(self.memory_processor)
         self.provider.add_span_processor(self.processor)
 
-        trace.set_tracer_provider(self.provider)
+        opentelemetry.trace.set_tracer_provider(self.provider)
 
-        self.tracer = trace.get_tracer(__name__)
+        self.tracer = opentelemetry.trace.get_tracer(__name__)
 
         self.queue_consumer = asyncio.Queue()
         self.queue_producer = asyncio.Queue()
 
     async def clear(self):
+        logger.debug('clear')
         return self.memory_processor.clear()
 
+    @property
+    def get_current_span(self):
+        logger.debug('get_current_span')
+        return opentelemetry.trace.get_current_span()
+
     async def is_ready(self):
         if self.provider and self.memory_processor and self.processor:
             return True
 
     async def get_finished_spans(self):
+        logger.debug('get_finished_spans')
         return self.memory_processor.get_finished_spans()
 
     async def pop_finished_spans(self):
         """ideal is to lock, pop spans, and clear"""
         spans = await self.get_finished_spans()
         clear = await self.clear()
         return spans
 
     async def test(self):
-        with self.tracer.start_as_current_span("rootSpan"):
-            with self.tracer.start_as_current_span("childSpan"):
-                print("Hello world!")
+        with self.tracer.start_as_current_span(name="rootSpan") as trace_root:
+            trace_root.add_event('AAAAAAAA')
+            with self.tracer.start_as_current_span(name="childSpan") as trace_child:
+                trace_child.add_event('AAAAAAAA')
+                trace_child.add_event('BBBBBBBB')
 
         return True
```

### Comparing `automonisaur-0.5.1/automon/integrations/openvpn/openvpn.py` & `automonisaur-0.5.2/automon/integrations/openvpn/openvpn.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/requestsWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/requestsWrapper/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,25 +32,25 @@
 
     async def _log_result(self):
         if self.status_code == 200:
             msg = [
                 self.response.request.method,
                 self.response.url,
                 f'{round(len(self.content) / 1024, 2)} KB',
-                self.status_code,
+                f'{self.status_code}',
             ]
             msg = ' '.join(msg)
             return logger.debug(msg)
 
         msg = [
             self.response.request.method,
             self.response.url,
             f'{round(len(self.content) / 1024, 2)} KB',
-            self.status_code,
-            self.content
+            f'{self.status_code}',
+            f'{self.content}'
         ]
 
         msg = ' '.join(msg)
         return logger.error(msg)
 
     async def _params(self, url, data, headers):
         if url is None:
```

### Comparing `automonisaur-0.5.1/automon/integrations/requestsWrapper/rest.py` & `automonisaur-0.5.2/automon/integrations/requestsWrapper/rest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/requestsWrapper/tests/test_requests.py` & `automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/actions.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/actions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/browser.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/browser_types.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser_types.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/config_window_size.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/config_window_size.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_browser_headless.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_headless.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 browser = SeleniumBrowser()
 browser.config.webdriver_wrapper = ChromeWrapper()
 browser.config.webdriver_wrapper.enable_defaults()
 browser.config.webdriver_wrapper.enable_headless()
 
 
 class SeleniumClientTest(unittest.TestCase):
+    if asyncio.run(browser.run()):
 
-    def test(self):
+        def test(self):
 
-        if asyncio.run(browser.run()):
             asyncio.run(browser.set_window_size(device_type='web-large'))
 
             if asyncio.run(browser.get('http://bing.com')):
                 self.assertTrue(asyncio.run(browser.save_screenshot()))
                 self.assertTrue(asyncio.run(browser.save_screenshot()))
                 self.assertTrue(asyncio.run(browser.save_screenshot(folder='./')))
```

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import unittest
+import asyncio
 
 from automon.integrations.seleniumWrapper import SeleniumBrowser, ChromeWrapper
 
 browser = SeleniumBrowser()
 browser.config.webdriver_wrapper = ChromeWrapper()
 browser.config.webdriver_wrapper.enable_defaults()
 browser.config.webdriver_wrapper.enable_headless()
 
 agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:112.0) Gecko/20100101 Firefox/112.0'
 
 browser.config.webdriver_wrapper.set_user_agent(agent)
 
 
 class SeleniumClientTest(unittest.TestCase):
-    async def test_user_agent(self):
-        if await browser.run():
+    if asyncio.run(browser.run()):
+        def test_user_agent(self):
             self.assertEqual(browser.user_agent, agent)
-
-            await browser.quit()
+            asyncio.run(browser.quit())
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/tests/test_user_agent.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_user_agent.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/user_agents.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/user_agents.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/seleniumWrapper/webdriver_chrome.py` & `automonisaur-0.5.2/automon/integrations/seleniumWrapper/webdriver_chrome.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         self._chrome_options = selenium.webdriver.ChromeOptions()
         self._chromedriver_path = environ_list('SELENIUM_CHROMEDRIVER_PATH')
         self._ChromeService = None
         self._window_size = set_window_size()
 
         self.update_paths(self.chromedriver_path)
 
+        logger.error('missing SELENIUM_CHROMEDRIVER_PATH')
+
     def __repr__(self):
         if self._webdriver:
             return str(dict(
                 name=self.webdriver.name,
                 window_size=self.window_size,
                 browserVersion=self.browserVersion,
                 chromedriverVersion=self.chromedriverVersion,
@@ -69,106 +71,106 @@
     def webdriver(self) -> selenium.webdriver.Chrome:
         return self._webdriver
 
     @property
     def window_size(self):
         return self._window_size
 
-    async def disable_certificate_verification(self):
+    def disable_certificate_verification(self):
         logger.warning('Certificates are not verified')
         self.chrome_options.add_argument('--ignore-certificate-errors')
         logger.debug(str(dict(
             add_argument='--ignore-certificate-errors'
         )))
         return self
 
-    async def disable_extensions(self):
+    def disable_extensions(self):
         self.chrome_options.add_argument("--disable-extensions")
         logger.debug(str(dict(
             add_argument=f'--disable-extensions'
         )))
         return self
 
-    async def disable_infobars(self):
+    def disable_infobars(self):
         self.chrome_options.add_argument("--disable-infobars")
         logger.debug(str(dict(
             add_argument=f'--disable-infobars'
         )))
         return self
 
-    async def disable_notifications(self):
+    def disable_notifications(self):
         """Pass the argument 1 to allow and 2 to block
 
         """
         self.chrome_options.add_experimental_option(
             "prefs", {"profile.default_content_setting_values.notifications": 2}
         )
 
         logger.debug(str(dict(
             add_experimental_option=("prefs", {"profile.default_content_setting_values.notifications": 2})
         )))
         return self
 
-    async def disable_sandbox(self):
+    def disable_sandbox(self):
         self.chrome_options.add_argument('--no-sandbox')
         logger.debug(str(dict(
             add_argument=f'--no-sandbox'
         )))
         return self
 
-    async def disable_shm(self):
+    def disable_shm(self):
         logger.warning('Disabled shm will use disk I/O, and will be slow')
         self.chrome_options.add_argument('--disable-dev-shm-usage')
         logger.debug(str(dict(
             add_argument=f'--disable-dev-shm-usage'
         )))
         return self
 
-    async def enable_bigshm(self):
+    def enable_bigshm(self):
         logger.warning('Big shm not yet implemented')
         return self
 
-    async def enable_defaults(self):
-        await self.enable_maximized()
+    def enable_defaults(self):
+        self.enable_maximized()
         return self
 
-    async def enable_fullscreen(self):
+    def enable_fullscreen(self):
         self.chrome_options.add_argument("--start-fullscreen")
         logger.debug(str(dict(
             add_argument=f'--start-fullscreen'
         )))
         return self
 
-    async def enable_headless(self):
+    def enable_headless(self):
         self.chrome_options.add_argument('headless')
         logger.debug(str(dict(
             add_argument='headless'
         )))
         return self
 
-    async def enable_notifications(self):
+    def enable_notifications(self):
         """Pass the argument 1 to allow and 2 to block
 
         """
         self.chrome_options.add_experimental_option(
             "prefs", {"profile.default_content_setting_values.notifications": 1}
         )
         logger.debug(str(dict(
             add_experimental_option=("prefs", {"profile.default_content_setting_values.notifications": 1})
         )))
         return self
 
-    async def enable_maximized(self):
+    def enable_maximized(self):
         self.chrome_options.add_argument('--start-maximized')
         logger.debug(str(dict(
             add_argument='--start-maximized'
         )))
         return self
 
-    async def enable_translate(self, native_language: str = 'en'):
+    def enable_translate(self, native_language: str = 'en'):
         prefs = {
             "translate_whitelists": {"your native language": native_language},
             "translate": {"enabled": "True"}
         }
         self.chrome_options.add_experimental_option(
             name="prefs",
             value=prefs,
@@ -186,123 +188,123 @@
         """close
 
         """
         result = self.webdriver.close()
         logger.info(f'{result}')
         return result
 
-    async def in_docker(self):
+    def in_docker(self):
         """Chrome best used with docker
 
         """
-        await self.enable_defaults()
-        await self.enable_headless()
-        await self.disable_sandbox()
-        await self.disable_infobars()
-        await self.disable_extensions()
-        await self.disable_notifications()
+        self.enable_defaults()
+        self.enable_headless()
+        self.disable_sandbox()
+        self.disable_infobars()
+        self.disable_extensions()
+        self.disable_notifications()
         return self
 
-    async def in_headless(self):
+    def in_headless(self):
         """alias to headless sandboxed
 
         """
-        return await self.in_headless_sandboxed()
+        return self.in_headless_sandboxed()
 
-    async def in_headless_sandboxed(self):
+    def in_headless_sandboxed(self):
         """Headless Chrome with sandbox enabled
 
         """
         logger.warning(
             'Docker does not support sandbox option. '
             'Default shm size is 64m, which will cause chrome driver to crash.'
         )
 
-        await self.enable_defaults()
-        await self.enable_headless()
+        self.enable_defaults()
+        self.enable_headless()
         return self
 
-    async def in_headless_sandbox_disabled(self):
+    def in_headless_sandbox_disabled(self):
         """Headless Chrome with sandbox disabled
 
         """
         logger.warning('Default shm size is 64m, which will cause chrome driver to crash.')
 
-        await self.enable_defaults()
-        await self.enable_headless()
-        await self.disable_sandbox()
+        self.enable_defaults()
+        self.enable_headless()
+        self.disable_sandbox()
         return self
 
-    async def in_headless_sandbox_disabled_certificate_unverified(self):
+    def in_headless_sandbox_disabled_certificate_unverified(self):
         """Headless Chrome with sandbox disabled with no certificate verification
 
         """
         logger.warning('Default shm size is 64m, which will cause chrome driver to crash.')
 
-        await self.enable_defaults()
-        await self.enable_headless()
-        await self.disable_sandbox()
-        await self.disable_certificate_verification()
+        self.enable_defaults()
+        self.enable_headless()
+        self.disable_sandbox()
+        self.disable_certificate_verification()
         return self
 
-    async def in_headless_sandbox_disabled_shm_disabled(self):
+    def in_headless_sandbox_disabled_shm_disabled(self):
         """Headless Chrome with sandbox disabled
 
         """
-        await self.enable_defaults()
-        await self.enable_headless()
-        await self.disable_sandbox()
-        await self.disable_shm()
+        self.enable_defaults()
+        self.enable_headless()
+        self.disable_sandbox()
+        self.disable_shm()
         return self
 
-    async def in_headless_sandbox_disabled_bigshm(self):
+    def in_headless_sandbox_disabled_bigshm(self):
         """Headless Chrome with sandbox disabled
 
         """
         logger.warning('Larger shm option is not implemented')
 
-        await self.enable_defaults()
-        await self.enable_headless()
-        await self.enable_bigshm()
-        await self.disable_sandbox()
+        self.enable_defaults()
+        self.enable_headless()
+        self.enable_bigshm()
+        self.disable_sandbox()
         return self
 
-    async def in_remote_driver(self, host: str = '127.0.0.1', port: str = '4444', executor_path: str = '/wd/hub'):
+    def in_remote_driver(self, host: str = '127.0.0.1', port: str = '4444', executor_path: str = '/wd/hub'):
         """Remote Selenium
 
         """
         logger.info(
             f'Remote WebDriver Hub URL: http://{host}:{port}{executor_path}/static/resource/hub.html')
 
         selenium.webdriver.Remote(
             command_executor=f'http://{host}:{port}{executor_path}',
             desired_capabilities=selenium.webdriver.common.desired_capabilities.DesiredCapabilities.CHROME
         )
         return self
 
-    async def in_sandbox(self):
+    def in_sandbox(self):
         """Chrome with sandbox enabled
 
         """
         logger.warning(
             'Docker does not support sandbox option. '
             'Default shm size is 64m, which will cause chrome driver to crash.'
         )
 
-        await self.enable_defaults()
+        self.enable_defaults()
         return self
 
-    async def in_sandbox_disabled(self):
+    def in_sandbox_disabled(self):
         """Chrome with sandbox disabled
 
         """
         logger.warning('Default shm size is 64m, which will cause chrome driver to crash.')
 
-        await self.enable_defaults()
-        await self.disable_sandbox()
+        self.enable_defaults()
+        self.disable_sandbox()
         return self
 
     async def run(self) -> selenium.webdriver.Chrome:
         try:
             if self.chromedriver_path:
                 self._ChromeService = selenium.webdriver.ChromeService(
                     executable_path=self.chromedriver_path
@@ -329,43 +331,43 @@
 
     async def set_chromedriver(self, chromedriver_path: str):
         logger.debug(f'{chromedriver_path}')
         self._chromedriver_path.append(chromedriver_path)
         self.update_paths(chromedriver_path)
         return self
 
-    async def set_locale(self, locale: str = 'en'):
+    def set_locale(self, locale: str = 'en'):
         self.chrome_options.add_argument(f"--lang={locale}")
         logger.debug(str(dict(
             add_argument=f"--lang={locale}"
         )))
         return self
 
-    async def set_locale_experimental(self, locale: str = 'en-US'):
+    def set_locale_experimental(self, locale: str = 'en-US'):
         self.chrome_options.add_experimental_option(
             name='prefs',
             value={'intl.accept_languages': locale}
         )
 
         logger.debug(str(dict(
             add_experimental_option=dict(
                 name='prefs',
                 value={'intl.accept_languages': locale}
             )
         )))
         return self
 
-    async def set_user_agent(self, user_agent: str):
+    def set_user_agent(self, user_agent: str):
         self.chrome_options.add_argument(f"user-agent={user_agent}")
         logger.debug(str(dict(
             add_argument=f"user-agent={user_agent}"
         )))
         return self
 
-    async def set_window_size(self, *args, **kwargs):
+    def set_window_size(self, *args, **kwargs):
         self._window_size = set_window_size(*args, **kwargs)
         width, height = self.window_size
         self.webdriver.set_window_size(width=width, height=height)
         logger.debug(f'{width}, {height}')
         return self
 
     async def start(self):
@@ -393,15 +395,17 @@
                 logger.debug(str(dict(
                     SELENIUM_CHROMEDRIVER_PATH=path,
                     PATH=os.environ['PATH']
                 )))
 
                 return True
 
-        logger.error(f'chrome driver not found: {path}')
+        logger.error(dict(
+            chromedriver_path=path
+        ))
 
     async def quit(self):
         """quit
 
         """
         result = self.webdriver.quit()
         logger.info(f'{result}')
```

### Comparing `automonisaur-0.5.1/automon/integrations/sentryio/client.py` & `automonisaur-0.5.2/automon/integrations/sentryio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
             sample_rate=self.config.sample_rate,
             max_breadcrumbs=self.config.max_breadcrumbs,
             attach_stacktrace=self.config.attach_stacktrace,
             send_default_pii=self.config.send_default_pii,
             server_name=self.config.server_name,
             in_app_include=self.config.in_app_include,
             in_app_exclude=self.config.in_app_exclude,
-            request_bodies=self.config.request_bodies,
-            with_locals=self.config.with_locals,
             ca_certs=self.config.ca_certs,
             integrations=self.config.integrations,
             default_integrations=self.config.default_integrations,
             before_send=self.config.before_send,
             before_breadcrumb=self.config.before_breadcrumb,
             transport=self.config.transport,
             http_proxy=self.config.http_proxy,
```

### Comparing `automonisaur-0.5.1/automon/integrations/sentryio/config.py` & `automonisaur-0.5.2/automon/integrations/sentryio/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,17 @@
         self.sample_rate = sample_rate or 1.0
         self.max_breadcrumbs = None
         self.attach_stacktrace = None
         self.send_default_pii = None
         self.server_name = None
         self.in_app_include = None
         self.in_app_exclude = None
+        # depreciated
         self.request_bodies = request_bodies or 'always'
+        # depreciated
         self.with_locals = None
         self.ca_certs = None
 
         # integration configuration
         self.integrations = None
         self.default_integrations = None
```

### Comparing `automonisaur-0.5.1/automon/integrations/sentryio/tests/test_sentryio.py` & `automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/sentryio/tests/test_sentryio_callback.py` & `automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio_callback.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/shodan/__init__.py` & `automonisaur-0.5.2/automon/integrations/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/bots.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/bots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/clientAsync.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/error.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/slack_formatting.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/slack_formatting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/slack_logger.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/slack_logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/slackWrapper/tests/test_slack.py` & `automonisaur-0.5.2/automon/integrations/slackWrapper/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/snmp/generate_maps.py` & `automonisaur-0.5.2/automon/integrations/snmp/generate_maps.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk/client.py` & `automonisaur-0.5.2/automon/integrations/splunk/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk/config.py` & `automonisaur-0.5.2/automon/integrations/splunk/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk/helpers.py` & `automonisaur-0.5.2/automon/integrations/splunk/helpers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk/tests/test_splunk_client.py` & `automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk/tests/test_splunk_config.py` & `automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/client.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/config.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/datatypes.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/datatypes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/integration/servicenow/ticket.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/ticket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/phantom_unittest.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/phantom_unittest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/responses.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/responses.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/rest/urls.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/rest/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/rules.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/rules.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/tests/dino.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/dino.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_uat.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/splunk_soar/vault.py` & `automonisaur-0.5.2/automon/integrations/splunk_soar/vault.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swift/client.py` & `automonisaur-0.5.2/automon/integrations/swift/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swift/config.py` & `automonisaur-0.5.2/automon/integrations/swift/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swift/error.py` & `automonisaur-0.5.2/automon/integrations/swift/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swift/iterables.py` & `automonisaur-0.5.2/automon/integrations/swift/iterables.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swift/tests/test_swift.py` & `automonisaur-0.5.2/automon/integrations/swift/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/api/v2.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/v2.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/client.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,18 @@
 
         response = await self.requests.get(url=url)
         logs_job = await self.requests.to_dict()
 
         return logs_job
 
     async def logging_recent(self, level: str = 'Debug'):
-        """finds the recent logs"""
+        """gets logs but needs to get it from a task run id
+
+        this is broken
+        """
         url = f'{self.host}/{Logging.recent}'
 
         request_body = {
             "level": [
                 level
             ]
         }
@@ -256,14 +259,17 @@
         """delete all records in application"""
         url = f'{self.host}/{Record.api(appId)}'
 
         response = await self.requests.delete(
             url=url
         )
 
+        if self.requests.status_code == 204 or self.requests.status_code == 404:
+            return True
+
         return response
 
     async def record_get(self, appId: str, id: str):
         """get a record"""
         url = f'{self.host}/{Record.get(appId=appId, id=id)}'
 
         response = await self.requests.get(
```

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/config.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_app.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_app.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_record.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,37 +7,37 @@
 client = SwimlaneClientRest()
 
 
 class MyTestCase(unittest.TestCase):
     def test_login(self):
         if asyncio.run(client.is_ready()):
             if asyncio.run(client.login_token()):
-                self.assertTrue(asyncio.run(
-                    client.app_list()
-                ))
+                appId = client.config.appId
 
-                key = 'a7m4r'       # json
-                value = json.dumps(dict(
+                key = 'a1qio'  # base64
+                value = dict(
                     key='value',
                     key2='value2',
-                ))
+                )
+
+                value = 'value'
 
                 record_new = asyncio.run(
                     client.record_create(
-                        appId=client.config.appId,
+                        appId=appId,
                         key=key,
                         value=value)
                 )
 
                 self.assertTrue(record_new)
 
                 record_id = record_new.get('id')
 
                 record_get = asyncio.run(
-                    client.record_get(appId=client.config.appId, id=record_id))
+                    client.record_get(appId=appId, id=record_id))
 
                 self.assertTrue(record_get)
 
                 pass
 
 
 if __name__ == '__main__':
```

### Comparing `automonisaur-0.5.1/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py` & `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 
 class MyTestCase(unittest.TestCase):
     def test_login(self):
         if asyncio.run(client.is_ready()):
             if asyncio.run(client.login()):
                 app_id = client.config.appId
-                delete_all = asyncio.run(
-                    client.record_delete_all(appId=app_id)
+                fields = asyncio.run(
+                    client.record_resolve_fields(appId=app_id)
                 )
 
-                self.assertTrue(delete_all)
+                self.assertTrue(fields)
 
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `automonisaur-0.5.1/automon/integrations/vds/client.py` & `automonisaur-0.5.2/automon/integrations/vds/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/integrations/vds/config.py` & `automonisaur-0.5.2/automon/integrations/vds/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/log/attributes.py` & `automonisaur-0.5.2/automon/log/attributes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/log/logger.py` & `automonisaur-0.5.2/automon/log/logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automon/log/tests/test_logger_builtin.py` & `automonisaur-0.5.2/automon/log/tests/test_logger_builtin.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.1/automonisaur.egg-info/PKG-INFO` & `automonisaur-0.5.2/automonisaur.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.5.1
+Version: 0.5.2
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](https://github.com/TheShellLand/automonisaur/raw/master/docs/images/sauruspark.gif)
 
 # Automonisaur: Core Libraries
 
@@ -67,15 +67,15 @@
 | Python          | logging<br/>requests                                        |
 | SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
 
-- python >= 3.8
+- python >= 3.10
 
 _Note: install requirements.txt to use all integrations_
 
 #### install core library
 
 ```shell script
 /bin/bash install.sh
```

### Comparing `automonisaur-0.5.1/automonisaur.egg-info/SOURCES.txt` & `automonisaur-0.5.2/automonisaur.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,20 +50,24 @@
 automon/integrations/cryptocurrency/coinbase.py
 automon/integrations/cryptocurrency/other.py
 automon/integrations/cryptocurrency/robinhood.py
 automon/integrations/cryptocurrency/tests/__init__.py
 automon/integrations/cryptocurrency/tests/test_crypto.py
 automon/integrations/datadogWrapper/__init__.py
 automon/integrations/datadogWrapper/client.py
+automon/integrations/datadogWrapper/client_opentelemetry.py
 automon/integrations/datadogWrapper/config.py
+automon/integrations/datadogWrapper/config_opentelemetry.py
 automon/integrations/datadogWrapper/api/__init__.py
 automon/integrations/datadogWrapper/api/v1.py
 automon/integrations/datadogWrapper/api/v2.py
 automon/integrations/datadogWrapper/tests/__init__.py
 automon/integrations/datadogWrapper/tests/test_auth.py
+automon/integrations/datadogWrapper/tests/test_client_opentelemetry.py
+automon/integrations/datadogWrapper/tests/test_config_opentelemetry.py
 automon/integrations/datadogWrapper/tests/test_log.py
 automon/integrations/datascience/__init__.py
 automon/integrations/datascience/pandas/__init__.py
 automon/integrations/datascience/pandas/dataframe.py
 automon/integrations/datascience/pandas/pandas.py
 automon/integrations/datascience/pandas/series.py
 automon/integrations/datascience/tests/__init__.py
@@ -184,15 +188,16 @@
 automon/integrations/nmap/tests/test_nmap_client.py
 automon/integrations/nmap/tests/test_nmap_config.py
 automon/integrations/openTelemetryWrapper/__init__.py
 automon/integrations/openTelemetryWrapper/client.py
 automon/integrations/openTelemetryWrapper/config.py
 automon/integrations/openTelemetryWrapper/test/__init__.py
 automon/integrations/openTelemetryWrapper/test/test_client_ready.py
-automon/integrations/openTelemetryWrapper/test/test_memory_trace.py
+automon/integrations/openTelemetryWrapper/test/test_memory_trace_client_test.py
+automon/integrations/openTelemetryWrapper/test/test_memory_trace_config.py
 automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
 automon/integrations/openvpn/__init__.py
 automon/integrations/openvpn/openvpn.py
 automon/integrations/psutilWrapper/__init__.py
 automon/integrations/psutilWrapper/cpu.py
 automon/integrations/requestsWrapper/__init__.py
 automon/integrations/requestsWrapper/client.py
```

### Comparing `automonisaur-0.5.1/setup.py` & `automonisaur-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="automonisaur",
-    version="0.5.1",
+    version="0.5.2",
     author="naisanza",
     author_email="naisanza@gmail.com",
     description="Core libraries for automonisaur",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheShellLand/automonisaur",
     packages=setuptools.find_packages(),
     tests_require=["pytest"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.10',
     install_requires=[]
 )
```


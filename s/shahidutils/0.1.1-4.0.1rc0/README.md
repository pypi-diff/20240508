# Comparing `tmp/shahidutils-0.1.1.tar.gz` & `tmp/shahidutils-4.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shahidutils-0.1.1.tar", max compression
+gzip compressed data, was "shahidutils-4.0.1rc0.tar", max compression
```

## Comparing `shahidutils-0.1.1.tar` & `shahidutils-4.0.1rc0.tar`

### file list

```diff
@@ -1,4 +1,83 @@
--rw-r--r--   0        0        0        0 2023-08-01 00:59:58.317280 shahidutils-0.1.1/README.md
--rw-r--r--   0        0        0      274 2023-08-01 01:03:56.676471 shahidutils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      260 2023-08-01 01:02:33.758937 shahidutils-0.1.1/shahidutils/__init__.py
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 shahidutils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      541 2024-04-23 11:15:13.198294 shahidutils-4.0.1rc0/README.md
+-rw-r--r--   0        0        0     9118 2024-05-08 19:42:01.328600 shahidutils-4.0.1rc0/pyproject.toml
+-rw-r--r--   0        0        0     1518 2024-05-08 14:22:55.912886 shahidutils-4.0.1rc0/src/shahidutils/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-05-07 21:06:09.633484 shahidutils-4.0.1rc0/src/shahidutils/__main__.py
+-rw-r--r--   0        0        0      303 2024-05-07 21:06:09.636818 shahidutils-4.0.1rc0/src/shahidutils/__metadata__.py
+-rw-r--r--   0        0        0     1917 2024-05-07 21:06:09.636818 shahidutils-4.0.1rc0/src/shahidutils/cli.py
+-rw-r--r--   0        0        0      145 2024-05-01 00:42:09.787476 shahidutils-4.0.1rc0/src/shahidutils/conf/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-22 07:55:45.112116 shahidutils-4.0.1rc0/src/shahidutils/conf/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      367 2024-05-01 00:42:10.267481 shahidutils-4.0.1rc0/src/shahidutils/conf/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1542 2024-04-22 07:55:45.112116 shahidutils-4.0.1rc0/src/shahidutils/conf/__pycache__/_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1613 2024-05-07 21:07:27.377647 shahidutils-4.0.1rc0/src/shahidutils/conf/__pycache__/_config.cpython-312.pyc
+-rw-r--r--   0        0        0     7362 2024-05-07 21:07:27.574316 shahidutils-4.0.1rc0/src/shahidutils/conf/__pycache__/_logging.cpython-312.pyc
+-rw-r--r--   0        0        0      659 2024-04-06 00:23:56.855886 shahidutils-4.0.1rc0/src/shahidutils/conf/__pycache__/config.cpython-312.pyc
+-rw-r--r--   0        0        0     1625 2024-05-07 21:06:09.633484 shahidutils-4.0.1rc0/src/shahidutils/conf/_config.py
+-rw-r--r--   0        0        0     5219 2024-05-07 21:06:09.636818 shahidutils-4.0.1rc0/src/shahidutils/conf/_logging.py
+-rw-r--r--   0        0        0      522 2024-04-19 02:02:49.262026 shahidutils-4.0.1rc0/src/shahidutils/conf/_meta.toml
+-rw-r--r--   0        0        0        0 2024-04-06 00:17:18.731859 shahidutils-4.0.1rc0/src/shahidutils/conf/dynaconf_validators.toml
+-rw-r--r--   0        0        0      516 2024-04-18 17:22:58.924608 shahidutils-4.0.1rc0/src/shahidutils/conf/shahidutils_logger.toml
+-rw-r--r--   0        0        0      470 2024-04-19 02:00:55.970513 shahidutils-4.0.1rc0/src/shahidutils/conf/shahidutils_secrets.toml
+-rw-r--r--   0        0        0     1478 2024-04-18 09:13:00.603438 shahidutils-4.0.1rc0/src/shahidutils/conf/shahidutils_settings.toml
+-rw-r--r--   0        0        0     4200 2024-05-07 21:06:09.636818 shahidutils-4.0.1rc0/src/shahidutils/exceptions.py
+-rw-r--r--   0        0        0      154 2024-05-07 06:47:44.693742 shahidutils-4.0.1rc0/src/shahidutils/models/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-22 07:55:45.118783 shahidutils-4.0.1rc0/src/shahidutils/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      405 2024-05-07 06:47:45.967088 shahidutils-4.0.1rc0/src/shahidutils/models/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2536 2024-04-29 13:49:50.483102 shahidutils-4.0.1rc0/src/shahidutils/models/__pycache__/_slack_blocks.cpython-312.pyc
+-rw-r--r--   0        0        0     2116 2024-04-18 05:04:00.955426 shahidutils-4.0.1rc0/src/shahidutils/models/__pycache__/slack_blocks.cpython-312.pyc
+-rw-r--r--   0        0        0       64 2024-04-29 21:29:52.326250 shahidutils-4.0.1rc0/src/shahidutils/models/_slack_blocks/__init__.py
+-rw-r--r--   0        0        0     2408 2024-05-08 09:08:59.404373 shahidutils-4.0.1rc0/src/shahidutils/models/_slack_blocks/_slack_blocks.py
+-rw-r--r--   0        0        0      255 2024-04-30 20:22:56.900361 shahidutils-4.0.1rc0/src/shahidutils/models/assets/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-30 20:22:58.083709 shahidutils-4.0.1rc0/src/shahidutils/models/assets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2232 2024-05-07 04:58:46.055623 shahidutils-4.0.1rc0/src/shahidutils/models/assets/__pycache__/asset.cpython-312.pyc
+-rw-r--r--   0        0        0     3775 2024-05-07 05:06:46.067742 shahidutils-4.0.1rc0/src/shahidutils/models/assets/__pycache__/asset_azure.cpython-312.pyc
+-rw-r--r--   0        0        0     4666 2024-05-07 05:03:27.492213 shahidutils-4.0.1rc0/src/shahidutils/models/assets/__pycache__/asset_old.cpython-312.pyc
+-rw-r--r--   0        0        0     8975 2024-05-07 21:07:28.437658 shahidutils-4.0.1rc0/src/shahidutils/models/assets/__pycache__/asset_vod.cpython-312.pyc
+-rw-r--r--   0        0        0     4369 2024-05-07 08:06:38.353998 shahidutils-4.0.1rc0/src/shahidutils/models/assets/_common_super.py
+-rw-r--r--   0        0        0     2147 2024-05-07 05:06:44.867729 shahidutils-4.0.1rc0/src/shahidutils/models/assets/asset_azure.py
+-rw-r--r--   0        0        0     1823 2024-05-07 18:07:55.358836 shahidutils-4.0.1rc0/src/shahidutils/models/assets/asset_factory.py
+-rw-r--r--   0        0        0     2798 2024-05-07 05:03:26.175531 shahidutils-4.0.1rc0/src/shahidutils/models/assets/asset_old.py
+-rw-r--r--   0        0        0     4806 2024-05-07 21:06:09.636818 shahidutils-4.0.1rc0/src/shahidutils/models/assets/asset_vod.py
+-rw-r--r--   0        0        0      181 2024-05-07 21:06:09.633484 shahidutils-4.0.1rc0/src/shahidutils/services/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-22 07:55:45.118783 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      253 2024-05-07 21:07:27.580983 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5815 2024-04-30 21:49:56.341726 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/_common.cpython-312.pyc
+-rw-r--r--   0        0        0     4101 2024-04-23 04:32:26.718092 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/_lambda.cpython-312.pyc
+-rw-r--r--   0        0        0      739 2024-04-14 03:29:15.309429 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/_netutils.cpython-312.pyc
+-rw-r--r--   0        0        0     3466 2024-04-22 08:01:22.009352 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/_opensearch.cpython-311.pyc
+-rw-r--r--   0        0        0     6274 2024-04-23 07:35:59.963090 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/_opensearch.cpython-312.pyc
+-rw-r--r--   0        0        0      356 2024-04-22 12:21:09.092310 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/_s3.cpython-312.pyc
+-rw-r--r--   0        0        0     2336 2024-04-18 15:32:18.143166 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/lambda_.cpython-312.pyc
+-rw-r--r--   0        0        0      672 2024-04-14 03:30:24.943578 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/netutils.cpython-312.pyc
+-rw-r--r--   0        0        0     4546 2024-04-18 21:09:36.770851 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/opensearch.cpython-312.pyc
+-rw-r--r--   0        0        0     2337 2024-04-18 21:19:32.348298 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/s_lambda.cpython-312.pyc
+-rw-r--r--   0        0        0     4548 2024-04-18 21:19:41.775047 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/s_opensearch.cpython-312.pyc
+-rw-r--r--   0        0        0     3513 2024-04-22 23:23:41.690279 shahidutils-4.0.1rc0/src/shahidutils/services/__pycache__/shahidquery.cpython-312.pyc
+-rw-r--r--   0        0        0     4179 2024-04-30 21:49:55.741720 shahidutils-4.0.1rc0/src/shahidutils/services/_common.py
+-rw-r--r--   0        0        0      266 2024-05-01 01:17:59.897590 shahidutils-4.0.1rc0/src/shahidutils/services/lambda_/__init__.py
+-rw-r--r--   0        0        0      421 2024-05-01 01:18:11.071044 shahidutils-4.0.1rc0/src/shahidutils/services/lambda_/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4751 2024-05-01 00:01:35.478560 shahidutils-4.0.1rc0/src/shahidutils/services/lambda_/__pycache__/_lambda.cpython-312.pyc
+-rw-r--r--   0        0        0     3775 2024-05-01 00:01:34.758552 shahidutils-4.0.1rc0/src/shahidutils/services/lambda_/_lambda.py
+-rw-r--r--   0        0        0       81 2024-04-23 07:52:54.893737 shahidutils-4.0.1rc0/src/shahidutils/services/opensearch/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-23 07:52:55.573747 shahidutils-4.0.1rc0/src/shahidutils/services/opensearch/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    11532 2024-05-08 10:29:14.414380 shahidutils-4.0.1rc0/src/shahidutils/services/opensearch/__pycache__/_opensearch.cpython-312.pyc
+-rw-r--r--   0        0        0    10539 2024-05-08 10:29:13.631039 shahidutils-4.0.1rc0/src/shahidutils/services/opensearch/_opensearch.py
+-rw-r--r--   0        0        0      777 2024-05-08 14:22:21.505836 shahidutils-4.0.1rc0/src/shahidutils/services/s3/__init__.py
+-rw-r--r--   0        0        0     5272 2024-05-08 10:58:00.252710 shahidutils-4.0.1rc0/src/shahidutils/services/s3/_parsing.py
+-rw-r--r--   0        0        0     4259 2024-05-08 09:18:18.007091 shahidutils-4.0.1rc0/src/shahidutils/services/s3/_s3.py
+-rw-r--r--   0        0        0      181 2024-05-08 14:23:19.833150 shahidutils-4.0.1rc0/src/shahidutils/services/sqs/__init__.py
+-rw-r--r--   0        0        0     3255 2024-05-08 14:27:28.609243 shahidutils-4.0.1rc0/src/shahidutils/services/sqs/_sqs.py
+-rw-r--r--   0        0        0      137 2024-04-18 20:01:03.998313 shahidutils-4.0.1rc0/src/shahidutils/utilities/__init__.py
+-rw-r--r--   0        0        0      211 2024-04-22 07:55:45.245452 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      199 2024-04-18 20:01:05.118337 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7063 2024-04-18 17:22:13.274192 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/_logging.cpython-312.pyc
+-rw-r--r--   0        0        0      740 2024-04-14 03:25:19.416594 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/_netutils.cpython-312.pyc
+-rw-r--r--   0        0        0     3300 2024-04-06 03:13:08.929135 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/_parsing.cpython-312.pyc
+-rw-r--r--   0        0        0      302 2024-04-18 20:00:59.121539 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/_utils.cpython-312.pyc
+-rw-r--r--   0        0        0     6209 2024-04-05 15:38:30.119922 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/conf.cpython-312.pyc
+-rw-r--r--   0        0        0      673 2024-03-29 11:27:10.367780 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/logging.cpython-312.pyc
+-rw-r--r--   0        0        0     3178 2024-05-07 21:07:28.557660 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/media_notify.cpython-312.pyc
+-rw-r--r--   0        0        0      731 2024-04-17 04:40:42.207820 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/netutils.cpython-312.pyc
+-rw-r--r--   0        0        0     3587 2024-05-07 21:07:28.530993 shahidutils-4.0.1rc0/src/shahidutils/utilities/__pycache__/parsing.cpython-312.pyc
+-rw-r--r--   0        0        0     2518 2024-05-07 21:06:09.636818 shahidutils-4.0.1rc0/src/shahidutils/utilities/media_notify.py
+-rw-r--r--   0        0        0     3106 2024-05-07 21:06:09.636818 shahidutils-4.0.1rc0/src/shahidutils/utilities/parsing.py
+-rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 shahidutils-4.0.1rc0/PKG-INFO
```


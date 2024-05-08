# Comparing `tmp/challtools-0.4.8.tar.gz` & `tmp/challtools-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challtools-0.4.8.tar", last modified: Sun Feb 26 13:18:19 2023, max compression
+gzip compressed data, was "challtools-0.4.9.tar", last modified: Wed May  8 13:30:06 2024, max compression
```

## Comparing `challtools-0.4.8.tar` & `challtools-0.4.9.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-02-26 13:18:09.000000 challtools-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-02-26 13:18:19.440101 challtools-0.4.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4383 2023-02-26 13:18:09.000000 challtools-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13514 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/challenge.schema.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    23951 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3064 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/codes.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.432101 challtools-0.4.8/challtools/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/templates/default/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/default/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/default/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/templates/flask/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/flask/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/flask/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/templates/flask/container/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/flask/container/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/flask/container/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/flask/container/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/templates/php/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/php/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/php/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/templates/php/container/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/php/container/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/php/container/index.php
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/templates/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/ssh/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/ssh/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools/templates/ssh/container/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/ssh/container/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/ssh/container/service
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/ssh/container/sshd_config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/challtools/templates/tcp_nsjail/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_nsjail/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_nsjail/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/challtools/templates/tcp_nsjail/container/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_nsjail/container/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_nsjail/container/service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/challtools/templates/tcp_xinetd/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_xinetd/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_xinetd/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/challtools/templates/tcp_xinetd/container/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_xinetd/container/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_xinetd/container/service
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tcp_xinetd/container/xinetd_config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/challtools/templates/tls_nsjail/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tls_nsjail/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tls_nsjail/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/challtools/templates/tls_nsjail/container/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tls_nsjail/container/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tls_nsjail/container/haproxy.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/templates/tls_nsjail/container/service
--rwxr-xr-x   0 runner    (1001) docker     (123)    28290 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9200 2023-02-26 13:18:09.000000 challtools-0.4.8/challtools/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.436101 challtools-0.4.8/challtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-02-26 13:18:19.000000 challtools-0.4.8/challtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-26 13:18:19.000000 challtools-0.4.8/challtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 13:18:19.000000 challtools-0.4.8/challtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-26 13:18:19.000000 challtools-0.4.8/challtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-26 13:18:19.000000 challtools-0.4.8/challtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-26 13:18:19.000000 challtools-0.4.8/challtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-26 13:18:19.440101 challtools-0.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-02-26 13:18:09.000000 challtools-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 13:18:19.440101 challtools-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-02-26 13:18:09.000000 challtools-0.4.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-02-26 13:18:09.000000 challtools-0.4.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-08 13:30:00.000000 challtools-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-08 13:30:06.889691 challtools-0.4.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4383 2024-05-08 13:30:00.000000 challtools-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.885691 challtools-0.4.9/challtools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13514 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/challenge.schema.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24039 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4179 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/codes.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      299 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.881691 challtools-0.4.9/challtools/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.885691 challtools-0.4.9/challtools/templates/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/default/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/default/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.885691 challtools-0.4.9/challtools/templates/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/flask/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/flask/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.885691 challtools-0.4.9/challtools/templates/flask/container/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/flask/container/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/flask/container/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/flask/container/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.885691 challtools-0.4.9/challtools/templates/php/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/php/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/php/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.885691 challtools-0.4.9/challtools/templates/php/container/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/php/container/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/php/container/index.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.885691 challtools-0.4.9/challtools/templates/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/ssh/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/ssh/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools/templates/ssh/container/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/ssh/container/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/ssh/container/service
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/ssh/container/sshd_config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools/templates/tcp_nsjail/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_nsjail/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_nsjail/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools/templates/tcp_nsjail/container/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_nsjail/container/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_nsjail/container/service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools/templates/tcp_xinetd/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_xinetd/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_xinetd/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools/templates/tcp_xinetd/container/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_xinetd/container/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_xinetd/container/service
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tcp_xinetd/container/xinetd_config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools/templates/tls_nsjail/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tls_nsjail/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tls_nsjail/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools/templates/tls_nsjail/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tls_nsjail/container/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tls_nsjail/container/haproxy.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/templates/tls_nsjail/container/service
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28418 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11125 2024-05-08 13:30:00.000000 challtools-0.4.9/challtools/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/challtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-08 13:30:06.000000 challtools-0.4.9/challtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-08 13:30:06.000000 challtools-0.4.9/challtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:30:06.000000 challtools-0.4.9/challtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 13:30:06.000000 challtools-0.4.9/challtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 13:30:06.000000 challtools-0.4.9/challtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 13:30:06.000000 challtools-0.4.9/challtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:30:06.889691 challtools-0.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2024-05-08 13:30:00.000000 challtools-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:06.889691 challtools-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-08 13:30:00.000000 challtools-0.4.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-08 13:30:00.000000 challtools-0.4.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-08 13:30:00.000000 challtools-0.4.9/tests/test_validator.py
```

### Comparing `challtools-0.4.8/LICENSE` & `challtools-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `challtools-0.4.8/PKG-INFO` & `challtools-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: challtools
-Version: 0.4.8
+Version: 0.4.9
 Summary: A tool for managing CTF challenges and challenge repositories using the OpenChallSpec
 Home-page: https://github.com/mateuszdrwal/challtools
 Author: Mateusz Drwal
 Author-email: me@mateuszdrwal.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML
+Requires-Dist: jsonschema>=3.0.0
+Requires-Dist: docker!=3.1.2,!=5.0.0,>=2.3.0
+Requires-Dist: requests>=2.0.0
+Requires-Dist: pypiwin32; platform_system == "Windows"
+Requires-Dist: argcomplete>=2.0.0
 
 # challtools
 
 challtools is a tool that manages CTF challenges and challenge repositories using the [OpenChallSpec](https://openchallspec.readthedocs.io/) challenge format.
 
 ## Installation
```

### Comparing `challtools-0.4.8/README.md` & `challtools-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `challtools-0.4.8/challtools/challenge.schema.json` & `challtools-0.4.9/challtools/challenge.schema.json`

 * *Files identical despite different names*

### Comparing `challtools-0.4.8/challtools/cli.py` & `challtools-0.4.9/challtools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -601,14 +601,16 @@
         "score": config["score"],
         "challenge_id": config["challenge_id"],
         "flag_format_prefix": config["flag_format_prefix"],
         "flag_format_suffix": config["flag_format_suffix"],
         "file_urls": file_urls,
         "flags": config["flags"],
         "order": config["custom"].get("order"),
+        "custom": config["custom"],
+        "human_metadata": config["human_metadata"],
         "services": [
             {
                 "hyperlink": service_types[c["type"]]["hyperlink"],
                 "user_display": format_user_service(config, c["type"], **c),
             }
             for c in config["predefined_services"]
         ],
```

### Comparing `challtools-0.4.8/challtools/codes.yml` & `challtools-0.4.9/challtools/codes.yml`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,34 @@
   formatted_message: "The file {file} is configured as a downloadable file however it does not exist on the filesystem, and is not recognized as an URL."
   docs_message: A file configured as a downloadable file does not exist on the filesystem and is not recognized as an URL.
 A004:
   name: Challenge ID missing
   level: 3
   formatted_message: 'This challenge is missing a challenge ID, which is recommended and required by some systems. Generate one using "challtools ensureid" or add a "challenge_id" to the challenge configuration manually.'
   docs_message: The challenge is missing a challenge ID which is generally recommended and may be required by some systems. Generate one using "challtools ensureid" or add a "challenge_id" to the challenge configuration manually.
+A005:
+  name: Missing flag regex anchors
+  level: 3
+  formatted_message: 'The following regex flag is missing anchors (''^'', ''$'') in the challenge configuration file (challenge.yml): "{flag}".'
+  docs_message: A regex flag missing anchors ('^', '$') n the challenge configuration file (challenge.yml)
+A006:
+  name: Duplicate custom_service_types types
+  level: 4
+  formatted_message: 'The following custom service type contains a duplicate type (challenge.yml): "{type}".'
+  docs_message: A custom service type contains a duplicate type (challenge.yml)
+A007:
+  name: Missing predefined_service display format option
+  level: 4
+  formatted_message: 'The following predefined_service is missing a display format option (challenge.yml): {service}: "{option}".'
+  docs_message: A predefined_service is missing a display format option (challenge.yml)
+A008:
+  name: Missing service type
+  level: 4
+  formatted_message: 'The following predefined_service is referencing a missing service type (challenge.yml): "{service_type}".'
+  docs_message: A predefined_service is referencing a missing service type (challenge.yml)
 
 # challtools messages
 B001:
   name: No CTF config
   level: 2
   formatted_message: No CTF configuration file (ctf.yml) detected in the current directory or any parent directory.
   docs_message: No CTF configuration file (ctf.yml) detected in the current directory or any parent directory.
```

### Comparing `challtools-0.4.8/challtools/templates/ssh/container/sshd_config` & `challtools-0.4.9/challtools/templates/ssh/container/sshd_config`

 * *Files identical despite different names*

### Comparing `challtools-0.4.8/challtools/templates/tls_nsjail/container/Dockerfile` & `challtools-0.4.9/challtools/templates/tls_nsjail/container/Dockerfile`

 * *Files identical despite different names*

### Comparing `challtools-0.4.8/challtools/utils.py` & `challtools-0.4.9/challtools/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,14 +437,16 @@
                 for line in chunk.strip().split(b"\n"):
                     decoded = json.loads(line)
                     # TODO process progress bars for pulling
                     if "error" in decoded:
                         raise CriticalException(decoded["error"])
                     if "stream" in decoded:
                         print(decoded["stream"], end="")
+                    if list(decoded.keys()) == ["message"]:
+                        raise CriticalException(decoded["message"])
 
         except docker.errors.APIError as e:
             raise CriticalException(e.explanation)
 
     elif imagepath.is_file():
         print(f'{BOLD}Interpreting "{image}" as an image archive{CLEAR}')
         print(f"{BOLD}Importing image...{CLEAR}")
```

### Comparing `challtools-0.4.8/challtools/validator.py` & `challtools-0.4.9/challtools/validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from copy import deepcopy
 import json
 from pathlib import Path
 import pkg_resources
 import yaml
+import re
 from jsonschema import validate, ValidationError, Draft7Validator, validators
 
 with pkg_resources.resource_stream("challtools", "codes.yml") as f:
     codes = yaml.safe_load(f)
 
 with pkg_resources.resource_stream("challtools", "challenge.schema.json") as f:
     schema = json.load(f)
@@ -102,15 +103,15 @@
 
             self._raise_code(
                 "A002",
                 path,
                 message=e.message,
             )
             return (
-                True,
+                False,
                 self.messages,
             )  # stop validation here in case of schema violations
 
         ### normalizing config
         self.normalized_config = deepcopy(self.config)
         # insterting defaults
         DefaultValidatingDraft7Validator(schema).validate(self.normalized_config)
@@ -172,14 +173,57 @@
                 if not (self.challdir / Path(file)).exists() and not is_url(file):
                     self._raise_code("A003", "downloadable_files", file=file)
 
         # A004
         if not self.normalized_config["challenge_id"]:
             self._raise_code("A004", "challenge_id")
 
+        # A005 validate regex flag contains anchors
+        for flag in self.normalized_config["flags"]:
+            if flag["type"] != "regex":
+                continue
+            if not (flag["flag"].startswith("^") and flag["flag"].endswith("$")):
+                self._raise_code("A005", "flags", flag=flag["flag"])
+
+        # A006 duplicate custom_service_types type
+        type_names = set()
+        for custom_service_type in self.normalized_config["custom_service_types"]:
+            type_name = custom_service_type["type"]
+            if type_name in type_names:
+                self._raise_code("A006", "custom_service_types", type=type_name)
+            type_names.add(type_name)
+
+        # A007 missing predefined_service display format option
+        service_types = [
+            {"type": "website", "display": "{url}"},
+            {"type": "tcp", "display": "nc {host} {port}"},
+        ] + self.normalized_config["custom_service_types"]
+        for predefined_service in self.normalized_config["predefined_services"]:
+            service_type = predefined_service["type"]
+            type_candidate = [
+                service for service in service_types if service["type"] == service_type
+            ]
+            # A008 missing service type
+            if not type_candidate:
+                self._raise_code(
+                    "A008",
+                    "predefined_services",
+                    service_type=service_type,
+                )
+                continue
+            string = type_candidate[0]["display"]
+            for format_option in re.findall(r"(?<=\{)[^{}]+(?=\})", string):
+                if not format_option in predefined_service:
+                    self._raise_code(
+                        "A007",
+                        "predefined_services",
+                        service=service_type,
+                        option=format_option,
+                    )
+
         ### CTF config validation
         # if no ctf config was provided to the validator we assume it does not exist and issue B001. not ideal as there might be other reasons for why the ctf config is not provided, but works for now
         if self.ctf_config == None:
             self._raise_code("B001")
         else:
             # B002 validate correct challenge names
             if "categories" in self.ctf_config:
```

### Comparing `challtools-0.4.8/challtools.egg-info/PKG-INFO` & `challtools-0.4.9/challtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: challtools
-Version: 0.4.8
+Version: 0.4.9
 Summary: A tool for managing CTF challenges and challenge repositories using the OpenChallSpec
 Home-page: https://github.com/mateuszdrwal/challtools
 Author: Mateusz Drwal
 Author-email: me@mateuszdrwal.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML
+Requires-Dist: jsonschema>=3.0.0
+Requires-Dist: docker!=3.1.2,!=5.0.0,>=2.3.0
+Requires-Dist: requests>=2.0.0
+Requires-Dist: pypiwin32; platform_system == "Windows"
+Requires-Dist: argcomplete>=2.0.0
 
 # challtools
 
 challtools is a tool that manages CTF challenges and challenge repositories using the [OpenChallSpec](https://openchallspec.readthedocs.io/) challenge format.
 
 ## Installation
```

### Comparing `challtools-0.4.8/challtools.egg-info/SOURCES.txt` & `challtools-0.4.9/challtools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,8 +41,9 @@
 challtools/templates/tcp_xinetd/container/xinetd_config
 challtools/templates/tls_nsjail/DESCRIPTION
 challtools/templates/tls_nsjail/challenge.yml
 challtools/templates/tls_nsjail/container/Dockerfile
 challtools/templates/tls_nsjail/container/haproxy.cfg
 challtools/templates/tls_nsjail/container/service
 tests/test_cli.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_validator.py
```

### Comparing `challtools-0.4.8/setup.py` & `challtools-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name="challtools",
-    version="0.4.8",
+    version="0.4.9",
     author="Mateusz Drwal",
     author_email="me@mateuszdrwal.com",
     description="A tool for managing CTF challenges and challenge repositories using the OpenChallSpec",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/mateuszdrwal/challtools",
     packages=setuptools.find_packages(),
```

### Comparing `challtools-0.4.8/tests/test_cli.py` & `challtools-0.4.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `challtools-0.4.8/tests/test_utils.py` & `challtools-0.4.9/tests/test_utils.py`

 * *Files identical despite different names*


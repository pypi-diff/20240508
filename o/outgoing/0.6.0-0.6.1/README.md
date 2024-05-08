# Comparing `tmp/outgoing-0.6.0.tar.gz` & `tmp/outgoing-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outgoing-0.6.0.tar", last modified: Mon Oct 30 19:54:31 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `outgoing-0.6.0.tar` & `outgoing-0.6.1.tar`

### file list

```diff
@@ -1,72 +1,54 @@
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.400586 outgoing-0.6.0/
--rw-r--r--   0 jwodder    (501) staff       (20)     2223 2023-10-30 19:54:25.000000 outgoing-0.6.0/CHANGELOG.md
--rw-r--r--   0 jwodder    (501) staff       (20)     1095 2023-10-30 19:54:25.000000 outgoing-0.6.0/LICENSE
--rw-r--r--   0 jwodder    (501) staff       (20)      126 2021-02-24 16:08:16.000000 outgoing-0.6.0/MANIFEST.in
--rw-r--r--   0 jwodder    (501) staff       (20)     5732 2023-10-30 19:54:31.400310 outgoing-0.6.0/PKG-INFO
--rw-r--r--   0 jwodder    (501) staff       (20)     3935 2022-10-16 02:57:47.000000 outgoing-0.6.0/README.rst
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.375608 outgoing-0.6.0/docs/
--rw-r--r--   0 jwodder    (501) staff       (20)     2349 2023-10-30 19:54:25.000000 outgoing-0.6.0/docs/changelog.rst
--rw-r--r--   0 jwodder    (501) staff       (20)     1901 2021-03-14 22:50:52.000000 outgoing-0.6.0/docs/command.rst
--rw-r--r--   0 jwodder    (501) staff       (20)      982 2023-10-30 19:54:25.000000 outgoing-0.6.0/docs/conf.py
--rw-r--r--   0 jwodder    (501) staff       (20)     9643 2023-10-08 22:14:21.000000 outgoing-0.6.0/docs/configuration.rst
--rw-r--r--   0 jwodder    (501) staff       (20)     1410 2023-10-30 19:53:32.000000 outgoing-0.6.0/docs/ext-utilities.rst
--rw-r--r--   0 jwodder    (501) staff       (20)      544 2021-03-08 21:01:06.000000 outgoing-0.6.0/docs/extensions.rst
--rw-r--r--   0 jwodder    (501) staff       (20)     3449 2022-10-16 02:57:47.000000 outgoing-0.6.0/docs/index.rst
--rw-r--r--   0 jwodder    (501) staff       (20)     1336 2021-09-27 19:58:38.000000 outgoing-0.6.0/docs/pyapi.rst
--rw-r--r--   0 jwodder    (501) staff       (20)       59 2023-10-04 16:12:50.000000 outgoing-0.6.0/docs/requirements.txt
--rw-r--r--   0 jwodder    (501) staff       (20)     3523 2021-03-06 22:39:37.000000 outgoing-0.6.0/docs/writing-exts.rst
--rw-r--r--   0 jwodder    (501) staff       (20)       91 2022-07-07 12:48:58.000000 outgoing-0.6.0/pyproject.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     2926 2023-10-30 19:54:31.401902 outgoing-0.6.0/setup.cfg
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.366156 outgoing-0.6.0/src/
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.379647 outgoing-0.6.0/src/outgoing/
--rw-r--r--   0 jwodder    (501) staff       (20)     1681 2023-10-30 19:54:25.000000 outgoing-0.6.0/src/outgoing/__init__.py
--rw-r--r--   0 jwodder    (501) staff       (20)     3023 2023-10-17 19:56:10.000000 outgoing-0.6.0/src/outgoing/__main__.py
--rw-r--r--   0 jwodder    (501) staff       (20)     9837 2023-10-30 19:53:32.000000 outgoing-0.6.0/src/outgoing/config.py
--rw-r--r--   0 jwodder    (501) staff       (20)     9571 2023-10-30 19:53:32.000000 outgoing-0.6.0/src/outgoing/core.py
--rw-r--r--   0 jwodder    (501) staff       (20)     2049 2022-10-16 17:04:05.000000 outgoing-0.6.0/src/outgoing/errors.py
--rw-r--r--   0 jwodder    (501) staff       (20)     4593 2023-10-30 19:53:32.000000 outgoing-0.6.0/src/outgoing/passwords.py
--rw-r--r--   0 jwodder    (501) staff       (20)        0 2021-02-24 16:08:16.000000 outgoing-0.6.0/src/outgoing/py.typed
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.386308 outgoing-0.6.0/src/outgoing/senders/
--rw-r--r--   0 jwodder    (501) staff       (20)        0 2021-02-24 19:31:09.000000 outgoing-0.6.0/src/outgoing/senders/__init__.py
--rw-r--r--   0 jwodder    (501) staff       (20)      933 2022-10-16 16:59:58.000000 outgoing-0.6.0/src/outgoing/senders/command.py
--rw-r--r--   0 jwodder    (501) staff       (20)     3589 2023-10-30 19:53:32.000000 outgoing-0.6.0/src/outgoing/senders/mailboxes.py
--rw-r--r--   0 jwodder    (501) staff       (20)      457 2021-03-14 21:18:05.000000 outgoing-0.6.0/src/outgoing/senders/null.py
--rw-r--r--   0 jwodder    (501) staff       (20)     2435 2023-10-30 19:53:32.000000 outgoing-0.6.0/src/outgoing/senders/smtp.py
--rw-r--r--   0 jwodder    (501) staff       (20)     2227 2023-10-30 19:53:32.000000 outgoing-0.6.0/src/outgoing/util.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.382897 outgoing-0.6.0/src/outgoing.egg-info/
--rw-r--r--   0 jwodder    (501) staff       (20)     5732 2023-10-30 19:54:31.000000 outgoing-0.6.0/src/outgoing.egg-info/PKG-INFO
--rw-r--r--   0 jwodder    (501) staff       (20)     1548 2023-10-30 19:54:31.000000 outgoing-0.6.0/src/outgoing.egg-info/SOURCES.txt
--rw-r--r--   0 jwodder    (501) staff       (20)        1 2023-10-30 19:54:31.000000 outgoing-0.6.0/src/outgoing.egg-info/dependency_links.txt
--rw-r--r--   0 jwodder    (501) staff       (20)      661 2023-10-30 19:54:31.000000 outgoing-0.6.0/src/outgoing.egg-info/entry_points.txt
--rw-r--r--   0 jwodder    (501) staff       (20)      260 2023-10-30 19:54:31.000000 outgoing-0.6.0/src/outgoing.egg-info/requires.txt
--rw-r--r--   0 jwodder    (501) staff       (20)        9 2023-10-30 19:54:31.000000 outgoing-0.6.0/src/outgoing.egg-info/top_level.txt
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.389414 outgoing-0.6.0/test/
--rw-r--r--   0 jwodder    (501) staff       (20)     1268 2021-10-31 20:50:06.000000 outgoing-0.6.0/test/conftest.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.389932 outgoing-0.6.0/test/data/
--rw-r--r--   0 jwodder    (501) staff       (20)      603 2023-06-20 12:20:45.000000 outgoing-0.6.0/test/data/Hunter2Keyring.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.391412 outgoing-0.6.0/test/test_config/
--rw-r--r--   0 jwodder    (501) staff       (20)     7392 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_config/test_netrc_config.py
--rw-r--r--   0 jwodder    (501) staff       (20)     7745 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_config/test_password.py
--rw-r--r--   0 jwodder    (501) staff       (20)     3567 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_config/test_paths.py
--rw-r--r--   0 jwodder    (501) staff       (20)     8146 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_from_config_file.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1662 2021-03-01 17:10:51.000000 outgoing-0.6.0/test/test_from_dict.py
--rw-r--r--   0 jwodder    (501) staff       (20)     2638 2022-10-30 17:30:34.000000 outgoing-0.6.0/test/test_lookup_netrc.py
--rw-r--r--   0 jwodder    (501) staff       (20)     6313 2023-10-10 23:41:16.000000 outgoing-0.6.0/test/test_main.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.394835 outgoing-0.6.0/test/test_passwords/
--rw-r--r--   0 jwodder    (501) staff       (20)      963 2021-03-04 01:45:15.000000 outgoing-0.6.0/test/test_passwords/test_base64.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1067 2021-03-07 01:00:42.000000 outgoing-0.6.0/test/test_passwords/test_basics.py
--rw-r--r--   0 jwodder    (501) staff       (20)     4964 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_passwords/test_dotenv.py
--rw-r--r--   0 jwodder    (501) staff       (20)      968 2021-03-07 03:17:28.000000 outgoing-0.6.0/test/test_passwords/test_env.py
--rw-r--r--   0 jwodder    (501) staff       (20)     2439 2021-03-08 04:09:07.000000 outgoing-0.6.0/test/test_passwords/test_file.py
--rw-r--r--   0 jwodder    (501) staff       (20)     8444 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_passwords/test_keyring.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-30 19:54:31.399268 outgoing-0.6.0/test/test_senders/
--rw-r--r--   0 jwodder    (501) staff       (20)     3636 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_babyl.py
--rw-r--r--   0 jwodder    (501) staff       (20)     2824 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_command.py
--rw-r--r--   0 jwodder    (501) staff       (20)     6694 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_maildir.py
--rw-r--r--   0 jwodder    (501) staff       (20)     3809 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_mbox.py
--rw-r--r--   0 jwodder    (501) staff       (20)     9814 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_mh.py
--rw-r--r--   0 jwodder    (501) staff       (20)     3833 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_mmdf.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1055 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_null.py
--rw-r--r--   0 jwodder    (501) staff       (20)    16406 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_senders/test_smtp.py
--rw-r--r--   0 jwodder    (501) staff       (20)      998 2023-10-30 19:53:32.000000 outgoing-0.6.0/test/test_util.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1848 2023-10-30 19:53:32.000000 outgoing-0.6.0/tox.ini
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 outgoing-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 outgoing-0.6.1/tox.ini
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/changelog.rst
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/command.rst
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/conf.py
+-rw-r--r--   0        0        0     9643 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/configuration.rst
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/ext-utilities.rst
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/extensions.rst
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/index.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/pyapi.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 outgoing-0.6.1/docs/writing-exts.rst
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/__init__.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/__main__.py
+-rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/config.py
+-rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/core.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/errors.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/passwords.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/py.typed
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/senders/__init__.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/senders/command.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/senders/mailboxes.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/senders/null.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 outgoing-0.6.1/src/outgoing/senders/smtp.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/conftest.py
+-rw-r--r--   0        0        0     8158 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_from_config_file.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_from_dict.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_lookup_netrc.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_main.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_util.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/data/Hunter2Keyring.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_config/test_netrc_config.py
+-rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_config/test_password.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_config/test_paths.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_passwords/test_base64.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_passwords/test_basics.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_passwords/test_dotenv.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_passwords/test_env.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_passwords/test_file.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_passwords/test_keyring.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_babyl.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_command.py
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_maildir.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_mbox.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_mh.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_mmdf.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_null.py
+-rw-r--r--   0        0        0    16406 2020-02-02 00:00:00.000000 outgoing-0.6.1/test/test_senders/test_smtp.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 outgoing-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 outgoing-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 outgoing-0.6.1/README.rst
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 outgoing-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 outgoing-0.6.1/PKG-INFO
```

### Comparing `outgoing-0.6.0/CHANGELOG.md` & `outgoing-0.6.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v0.6.1 (2024-05-08)
+-------------------
+- Support platformdirs v4.0
+- Migrated from setuptools to hatch
+- Drop support for Python 3.7
+
 v0.6.0 (2023-10-30)
 -------------------
 - Support python-dotenv v1.0
 - Always read JSON configuration files using UTF-8 encoding
 - Always read files for the "file" password method using UTF-8 encoding
 - Support Python 3.12
 - Correct the default Linux config file location listed in the README
```

### Comparing `outgoing-0.6.0/LICENSE` & `outgoing-0.6.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021-2023 John Thorvald Wodder II
+Copyright (c) 2021-2024 John Thorvald Wodder II
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `outgoing-0.6.0/PKG-INFO` & `outgoing-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: outgoing
-Version: 0.6.0
+Version: 0.6.1
 Summary: Common interface for multiple e-mail methods
-Home-page: https://github.com/jwodder/outgoing
-Author: John Thorvald Wodder II
-Author-email: outgoing@varonathe.org
-License: MIT
 Project-URL: Source Code, https://github.com/jwodder/outgoing
 Project-URL: Bug Tracker, https://github.com/jwodder/outgoing/issues
 Project-URL: Documentation, https://outgoing.readthedocs.io
+Author-email: John Thorvald Wodder II <outgoing@varonathe.org>
+License-Expression: MIT
+License-File: LICENSE
 Keywords: e-mail,email,mailbox,mbox,send mail,sendmail,smtp
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Communications :: Email
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: click>=8.0
+Requires-Python: >=3.8
 Requires-Dist: click-loglevel~=0.5
-Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
+Requires-Dist: click>=8.0
+Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: keyring>=21.7
 Requires-Dist: morecontext~=0.4
-Requires-Dist: platformdirs~=3.0
+Requires-Dist: platformdirs<5.0,>=3.0
 Requires-Dist: pydantic~=2.0
 Requires-Dist: python-dotenv<2.0,>=0.11
-Requires-Dist: tomli<3.0,>=1.2; python_version < "3.11"
-Requires-Dist: typing_extensions; python_version < "3.9"
+Requires-Dist: tomli<3.0,>=1.2; python_version < '3.11'
+Requires-Dist: typing-extensions; python_version < '3.9'
+Description-Content-Type: text/x-rst
+
+|repostatus| |ci-status| |coverage| |pyversions| |license|
 
-.. image:: http://www.repostatus.org/badges/latest/active.svg
-    :target: http://www.repostatus.org/#active
+.. |repostatus| image:: https://www.repostatus.org/badges/latest/active.svg
+    :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/outgoing/workflows/Test/badge.svg?branch=master
-    :target: https://github.com/jwodder/outgoing/actions?workflow=Test
+.. |ci-status| image:: https://github.com/jwodder/outgoing/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jwodder/outgoing/actions/workflows/test.yml
     :alt: CI Status
 
-.. image:: https://codecov.io/gh/jwodder/outgoing/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/jwodder/outgoing/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/outgoing
 
-.. image:: https://img.shields.io/pypi/pyversions/outgoing.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/outgoing.svg
     :target: https://pypi.org/project/outgoing/
 
-.. image:: https://img.shields.io/github/license/jwodder/outgoing.svg
+.. |license| image:: https://img.shields.io/github/license/jwodder/outgoing.svg
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 `GitHub <https://github.com/jwodder/outgoing>`_
 | `PyPI <https://pypi.org/project/outgoing/>`_
 | `Documentation <https://outgoing.readthedocs.io>`_
 | `Issues <https://github.com/jwodder/outgoing/issues>`_
@@ -75,15 +74,15 @@
 
 See `the documentation <https://outgoing.readthedocs.io>`_ for more
 information.
 
 
 Installation
 ============
-``outgoing`` requires Python 3.7 or higher.  Just use `pip
+``outgoing`` requires Python 3.8 or higher.  Just use `pip
 <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to install
 ``outgoing`` and its dependencies::
 
     python3 -m pip install outgoing
 
 
 Examples
```

### Comparing `outgoing-0.6.0/README.rst` & `outgoing-0.6.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-.. image:: http://www.repostatus.org/badges/latest/active.svg
-    :target: http://www.repostatus.org/#active
+|repostatus| |ci-status| |coverage| |pyversions| |license|
+
+.. |repostatus| image:: https://www.repostatus.org/badges/latest/active.svg
+    :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/outgoing/workflows/Test/badge.svg?branch=master
-    :target: https://github.com/jwodder/outgoing/actions?workflow=Test
+.. |ci-status| image:: https://github.com/jwodder/outgoing/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jwodder/outgoing/actions/workflows/test.yml
     :alt: CI Status
 
-.. image:: https://codecov.io/gh/jwodder/outgoing/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/jwodder/outgoing/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/outgoing
 
-.. image:: https://img.shields.io/pypi/pyversions/outgoing.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/outgoing.svg
     :target: https://pypi.org/project/outgoing/
 
-.. image:: https://img.shields.io/github/license/jwodder/outgoing.svg
+.. |license| image:: https://img.shields.io/github/license/jwodder/outgoing.svg
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 `GitHub <https://github.com/jwodder/outgoing>`_
 | `PyPI <https://pypi.org/project/outgoing/>`_
 | `Documentation <https://outgoing.readthedocs.io>`_
 | `Issues <https://github.com/jwodder/outgoing/issues>`_
@@ -33,15 +35,15 @@
 
 See `the documentation <https://outgoing.readthedocs.io>`_ for more
 information.
 
 
 Installation
 ============
-``outgoing`` requires Python 3.7 or higher.  Just use `pip
+``outgoing`` requires Python 3.8 or higher.  Just use `pip
 <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to install
 ``outgoing`` and its dependencies::
 
     python3 -m pip install outgoing
 
 
 Examples
```

### Comparing `outgoing-0.6.0/docs/changelog.rst` & `outgoing-0.6.1/docs/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. currentmodule:: outgoing
 
 Changelog
 =========
 
+v0.6.1 (2024-05-08)
+-------------------
+- Support platformdirs v4.0
+- Migrated from setuptools to hatch
+- Drop support for Python 3.7
+
 v0.6.0 (2023-10-30)
 -------------------
 - Support python-dotenv v1.0
 - Always read JSON configuration files using UTF-8 encoding
 - Always read files for the "file" password method using UTF-8 encoding
 - Support Python 3.12
 - Correct the default Linux config file location listed in the README
```

### Comparing `outgoing-0.6.0/docs/command.rst` & `outgoing-0.6.1/docs/command.rst`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/docs/conf.py` & `outgoing-0.6.1/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from outgoing import __version__
 
 project = "outgoing"
 author = "John Thorvald Wodder II"
-copyright = "2021-2023 John Thorvald Wodder II"  # noqa: A001
+copyright = "2021-2024 John Thorvald Wodder II"  # noqa: A001
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx_copybutton",
 ]
```

### Comparing `outgoing-0.6.0/docs/configuration.rst` & `outgoing-0.6.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/docs/ext-utilities.rst` & `outgoing-0.6.1/docs/ext-utilities.rst`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/docs/extensions.rst` & `outgoing-0.6.1/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/docs/index.rst` & `outgoing-0.6.1/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ``outgoing`` itself provides support for only basic sending methods; additional
 methods are provided by :doc:`extension packages <extensions>`.
 
 
 Installation
 ============
-``outgoing`` requires Python 3.7 or higher.  Just use `pip
+``outgoing`` requires Python 3.8 or higher.  Just use `pip
 <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to install
 ``outgoing`` and its dependencies::
 
     python3 -m pip install outgoing
 
 
 .. _examples:
```

### Comparing `outgoing-0.6.0/docs/pyapi.rst` & `outgoing-0.6.1/docs/pyapi.rst`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/docs/writing-exts.rst` & `outgoing-0.6.1/docs/writing-exts.rst`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/setup.cfg` & `outgoing-0.6.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,119 @@
-[metadata]
-name = outgoing
-version = attr:outgoing.__version__
-description = Common interface for multiple e-mail methods
-long_description = file:README.rst
-long_description_content_type = text/x-rst
-author = John Thorvald Wodder II
-author_email = outgoing@varonathe.org
-license = MIT
-license_files = LICENSE
-url = https://github.com/jwodder/outgoing
-keywords = 
-	e-mail
-	email
-	mailbox
-	mbox
-	send mail
-	sendmail
-	smtp
-classifiers = 
-	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: 3.12
-	Programming Language :: Python :: Implementation :: CPython
-	Programming Language :: Python :: Implementation :: PyPy
-	License :: OSI Approved :: MIT License
-	Intended Audience :: Developers
-	Intended Audience :: Information Technology
-	Intended Audience :: System Administrators
-	Topic :: Communications :: Email
-	Typing :: Typed
-project_urls = 
-	Source Code = https://github.com/jwodder/outgoing
-	Bug Tracker = https://github.com/jwodder/outgoing/issues
-	Documentation = https://outgoing.readthedocs.io
-
-[options]
-packages = find:
-package_dir = 
-	=src
-include_package_data = True
-python_requires = >=3.7
-install_requires = 
-	click          >= 8.0
-	click-loglevel ~= 0.5
-	importlib-metadata >= 3.6; python_version < "3.10"
-	keyring        >= 21.7
-	morecontext    ~= 0.4
-	platformdirs   ~= 3.0
-	pydantic       ~= 2.0
-	python-dotenv  >= 0.11, < 2.0
-	tomli          >= 1.2, < 3.0; python_version < "3.11"
-	typing_extensions; python_version < "3.9"
-
-[options.packages.find]
-where = src
-
-[options.entry_points]
-console_scripts = 
-	outgoing = outgoing.__main__:main
-outgoing.senders = 
-	babyl = outgoing.senders.mailboxes:BabylSender
-	command = outgoing.senders.command:CommandSender
-	maildir = outgoing.senders.mailboxes:MaildirSender
-	mbox = outgoing.senders.mailboxes:MboxSender
-	mh = outgoing.senders.mailboxes:MHSender
-	mmdf = outgoing.senders.mailboxes:MMDFSender
-	null = outgoing.senders.null:NullSender
-	smtp = outgoing.senders.smtp:SMTPSender
-outgoing.password_schemes = 
-	dotenv = outgoing.passwords:dotenv_scheme
-	base64 = outgoing.passwords:base64_scheme
-	env = outgoing.passwords:env_scheme
-	file = outgoing.passwords:file_scheme
-	keyring = outgoing.passwords:keyring_scheme
-
-[mypy]
-allow_incomplete_defs = False
-allow_untyped_defs = False
-ignore_missing_imports = False
-no_implicit_optional = True
-implicit_reexport = False
-local_partial_types = True
-pretty = True
-show_error_codes = True
-show_traceback = True
-strict_equality = True
-warn_redundant_casts = True
-warn_return_any = True
-warn_unreachable = True
-plugins = pydantic.mypy
-exclude = test/data/
-
-[pydantic-mypy]
-init_forbid_extra = True
-warn_untypes_fields = True
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "outgoing"
+dynamic = ["version"]
+description = "Common interface for multiple e-mail methods"
+readme = "README.rst"
+requires-python = ">=3.8"
+license = "MIT"
+license-files = { paths = ["LICENSE"] }
+authors = [
+    { name = "John Thorvald Wodder II", email = "outgoing@varonathe.org" }
+]
+
+keywords = [
+    "e-mail",
+    "email",
+    "mailbox",
+    "mbox",
+    "send mail",
+    "sendmail",
+    "smtp",
+]
+
+classifiers = [
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "License :: OSI Approved :: MIT License",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: System Administrators",
+    "Topic :: Communications :: Email",
+    "Typing :: Typed",
+]
+
+dependencies = [
+    "click          >= 8.0",
+    "click-loglevel ~= 0.5",
+    "importlib-metadata >= 3.6; python_version < '3.10'",
+    "keyring        >= 21.7",
+    "morecontext    ~= 0.4",
+    "platformdirs   >= 3.0, < 5.0",
+    "pydantic       ~= 2.0",
+    "python-dotenv  >= 0.11, < 2.0",
+    "tomli          >= 1.2, < 3.0; python_version < '3.11'",
+    "typing_extensions; python_version < '3.9'",
+]
+
+[project.scripts]
+outgoing = "outgoing.__main__:main"
+
+[project.entry-points."outgoing.senders"]
+babyl = "outgoing.senders.mailboxes:BabylSender"
+command = "outgoing.senders.command:CommandSender"
+maildir = "outgoing.senders.mailboxes:MaildirSender"
+mbox = "outgoing.senders.mailboxes:MboxSender"
+mh = "outgoing.senders.mailboxes:MHSender"
+mmdf = "outgoing.senders.mailboxes:MMDFSender"
+null = "outgoing.senders.null:NullSender"
+smtp = "outgoing.senders.smtp:SMTPSender"
+
+[project.entry-points."outgoing.password_schemes"]
+dotenv = "outgoing.passwords:dotenv_scheme"
+base64 = "outgoing.passwords:base64_scheme"
+env = "outgoing.passwords:env_scheme"
+file = "outgoing.passwords:file_scheme"
+keyring = "outgoing.passwords:keyring_scheme"
+
+[project.urls]
+"Source Code" = "https://github.com/jwodder/outgoing"
+"Bug Tracker" = "https://github.com/jwodder/outgoing/issues"
+"Documentation" = "https://outgoing.readthedocs.io"
+
+[tool.hatch.version]
+path = "src/outgoing/__init__.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/docs",
+    "/src",
+    "/test",
+    "CHANGELOG.*",
+    "CONTRIBUTORS.*",
+    "tox.ini",
+]
+
+[tool.hatch.envs.default]
+python = "3"
+
+[tool.mypy]
+allow_incomplete_defs = false
+allow_untyped_defs = false
+ignore_missing_imports = false
+# <https://github.com/python/mypy/issues/7773>:
+no_implicit_optional = true
+implicit_reexport = false
+local_partial_types = true
+pretty = true
+show_error_codes = true
+show_traceback = true
+strict_equality = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unreachable = true
+plugins = ["pydantic.mypy"]
+exclude = "test/data/"
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+warn_required_dynamic_aliases = true
```

### Comparing `outgoing-0.6.0/src/outgoing/__init__.py` & `outgoing-0.6.1/src/outgoing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ``outgoing`` itself provides support for only basic sending methods; additional
 methods are provided by other packages.
 
 Visit <https://github.com/jwodder/outgoing> or <https://outgoing.rtfd.io> for
 more information.
 """
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __author__ = "John Thorvald Wodder II"
 __author_email__ = "outgoing@varonathe.org"
 __license__ = "MIT"
 __url__ = "https://github.com/jwodder/outgoing"
 
 from .config import (
     DirectoryPath,
```

### Comparing `outgoing-0.6.0/src/outgoing/__main__.py` & `outgoing-0.6.1/src/outgoing/__main__.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/src/outgoing/config.py` & `outgoing-0.6.1/src/outgoing/config.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/src/outgoing/core.py` & `outgoing-0.6.1/src/outgoing/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,22 @@
     - Sender objects can be used as context managers, and their ``__enter__``
       methods return ``self``.
 
     - Within its own context, calling a sender's ``send(msg:
       email.message.EmailMessage)`` method sends the given e-mail.
     """
 
-    def __enter__(self) -> Self:
-        ...
+    def __enter__(self) -> Self: ...
 
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
-        ...
+    ) -> Optional[bool]: ...
 
     def send(self, msg: EmailMessage) -> Any:
         """Send ``msg`` or raise an exception if that's not possible"""
         ...
 
 
 def get_default_configpath() -> Path:
```

### Comparing `outgoing-0.6.0/src/outgoing/errors.py` & `outgoing-0.6.1/src/outgoing/errors.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/src/outgoing/passwords.py` & `outgoing-0.6.1/src/outgoing/passwords.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/src/outgoing/senders/command.py` & `outgoing-0.6.1/src/outgoing/senders/command.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/src/outgoing/senders/mailboxes.py` & `outgoing-0.6.1/src/outgoing/senders/mailboxes.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 log = logging.getLogger(__name__)
 
 
 class MailboxSender(OpenClosable):  # ABC inherited from OpenClosable
     _mbox: Optional[mailbox.Mailbox] = PrivateAttr(None)
 
     @abstractmethod
-    def _makebox(self) -> mailbox.Mailbox:
-        ...
+    def _makebox(self) -> mailbox.Mailbox: ...
 
     @abstractmethod
-    def _describe(self) -> str:
-        ...
+    def _describe(self) -> str: ...
 
     def open(self) -> None:
         log.debug("Opening %s", self._describe())
         self._mbox = self._makebox()
         self._mbox.lock()
 
     def close(self) -> None:
```

### Comparing `outgoing-0.6.0/src/outgoing/senders/smtp.py` & `outgoing-0.6.1/src/outgoing/senders/smtp.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/src/outgoing/util.py` & `outgoing-0.6.1/src/outgoing/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,18 @@
     .. _reentrant: https://docs.python.org/3/library/contextlib.html
                    #reentrant-cms
     """
 
     _context_depth: int = PrivateAttr(0)
 
     @abstractmethod
-    def open(self) -> None:
-        ...
+    def open(self) -> None: ...
 
     @abstractmethod
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
     def __enter__(self) -> Self:
         if self._context_depth == 0:
             self.open()
         self._context_depth += 1
         return self
```

### Comparing `outgoing-0.6.0/test/conftest.py` & `outgoing-0.6.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/data/Hunter2Keyring.py` & `outgoing-0.6.1/test/data/Hunter2Keyring.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_config/test_netrc_config.py` & `outgoing-0.6.1/test/test_config/test_netrc_config.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_config/test_password.py` & `outgoing-0.6.1/test/test_config/test_password.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_config/test_paths.py` & `outgoing-0.6.1/test/test_config/test_paths.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_from_config_file.py` & `outgoing-0.6.1/test/test_from_config_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,25 @@
     defconf = get_default_configpath()
     defconf.parent.mkdir(parents=True, exist_ok=True)
     defconf.write_text('[outgoing]\nmethod = "mbox"\npath = "inbox"\n')
     with pytest.raises(MissingConfigError) as excinfo:
         from_config_file(tmp_home / "foo.toml", fallback=False)
     assert (
         str(excinfo.value)
-        == f"outgoing configuration not found in files: {tmp_home/'foo.toml'}"
+        == f"outgoing configuration not found in files: {tmp_home / 'foo.toml'}"
     )
 
 
 def test_from_nonexistent_custom_config_file_no_default(tmp_home: Path) -> None:
     defconf = get_default_configpath()
     with pytest.raises(MissingConfigError) as excinfo:
         from_config_file(tmp_home / "foo.toml")
     assert (
         str(excinfo.value) == f"outgoing configuration not found in files: {defconf},"
-        f" {tmp_home/'foo.toml'}"
+        f" {tmp_home / 'foo.toml'}"
     )
 
 
 @pytest.mark.usefixtures("tmp_home")
 @pytest.mark.parametrize("fallback", [False, True])
 def test_from_nonexistent_default_config_file(fallback: bool) -> None:
     defconf = get_default_configpath()
@@ -99,15 +99,15 @@
 
 
 def test_from_unknown_ext(tmp_path: Path) -> None:
     with pytest.raises(InvalidConfigError) as excinfo:
         from_config_file(tmp_path / "foo.xyz")
     assert (
         str(excinfo.value)
-        == f"{tmp_path/'foo.xyz'}: Invalid configuration: Unsupported file extension"
+        == f"{tmp_path / 'foo.xyz'}: Invalid configuration: Unsupported file extension"
     )
 
 
 def test_from_custom_section(tmp_path: Path) -> None:
     (tmp_path / "foo.toml").write_text(
         "[outgoing]\n"
         'method = "mbox"\n'
@@ -166,30 +166,30 @@
     (tmp_home / "foo.toml").write_text(
         '[sender]\nmethod = "maildir"\npath = "dirmail"\n'
     )
     with pytest.raises(MissingConfigError) as excinfo:
         from_config_file(tmp_home / "foo.toml", fallback=False)
     assert (
         str(excinfo.value)
-        == f"outgoing configuration not found in files: {tmp_home/'foo.toml'}"
+        == f"outgoing configuration not found in files: {tmp_home / 'foo.toml'}"
     )
 
 
 def test_from_no_section_in_custom_config_file_or_default(tmp_home: Path) -> None:
     defconf = get_default_configpath()
     defconf.parent.mkdir(parents=True, exist_ok=True)
     defconf.write_text('[sender]\nmethod = "mbox"\npath = "inbox"\n')
     (tmp_home / "foo.toml").write_text(
         '[sender]\nmethod = "maildir"\npath = "dirmail"\n'
     )
     with pytest.raises(MissingConfigError) as excinfo:
         from_config_file(tmp_home / "foo.toml")
     assert (
         str(excinfo.value) == f"outgoing configuration not found in files: {defconf},"
-        f" {tmp_home/'foo.toml'}"
+        f" {tmp_home / 'foo.toml'}"
     )
 
 
 @pytest.mark.usefixtures("tmp_home")
 @pytest.mark.parametrize("fallback", [False, True])
 def test_from_no_section_default_config_file(fallback: bool) -> None:
     defconf = get_default_configpath()
@@ -226,10 +226,10 @@
     (tmp_path / "foo.toml").write_text(
         '[[outgoing]]\nmethod = "mbox"\npath = "inbox"\n'
     )
     with pytest.raises(InvalidConfigError) as excinfo:
         from_config_file(tmp_path / "foo.toml")
     assert (
         str(excinfo.value)
-        == f"{tmp_path/'foo.toml'}: Invalid configuration: Section must be a"
+        == f"{tmp_path / 'foo.toml'}: Invalid configuration: Section must be a"
         " dict/object"
     )
```

### Comparing `outgoing-0.6.0/test/test_from_dict.py` & `outgoing-0.6.1/test/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_lookup_netrc.py` & `outgoing-0.6.1/test/test_lookup_netrc.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_main.py` & `outgoing-0.6.1/test/test_main.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_passwords/test_base64.py` & `outgoing-0.6.1/test/test_passwords/test_base64.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_passwords/test_basics.py` & `outgoing-0.6.1/test/test_passwords/test_basics.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_passwords/test_dotenv.py` & `outgoing-0.6.1/test/test_passwords/test_dotenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,27 +88,27 @@
     (tmp_path / "foo.txt").write_text("SECRET=hunter2\n")
     with pytest.raises(InvalidPasswordError) as excinfo:
         resolve_password(
             {"dotenv": {"key": "HIDDEN", "file": str(tmp_path / "foo.txt")}}
         )
     assert (
         str(excinfo.value)
-        == f"Invalid password configuration: key 'HIDDEN' not in {tmp_path/'foo.txt'}"
+        == f"Invalid password configuration: key 'HIDDEN' not in {tmp_path / 'foo.txt'}"
     )
 
 
 def test_dotenv_password_no_value(tmp_path: Path) -> None:
     (tmp_path / "foo.txt").write_text("SECRET\n")
     with pytest.raises(InvalidPasswordError) as excinfo:
         resolve_password(
             {"dotenv": {"key": "SECRET", "file": str(tmp_path / "foo.txt")}}
         )
     assert (
         str(excinfo.value) == "Invalid password configuration: key 'SECRET' in"
-        f" {tmp_path/'foo.txt'} does not have a value"
+        f" {tmp_path / 'foo.txt'} does not have a value"
     )
 
 
 def test_dotenv_invalid_spec_type() -> None:
     with pytest.raises(InvalidPasswordError) as excinfo:
         resolve_password({"dotenv": "SECRET"})
     assert (
```

### Comparing `outgoing-0.6.0/test/test_passwords/test_env.py` & `outgoing-0.6.1/test/test_passwords/test_env.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_passwords/test_file.py` & `outgoing-0.6.1/test/test_passwords/test_file.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_passwords/test_keyring.py` & `outgoing-0.6.1/test/test_passwords/test_keyring.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_senders/test_babyl.py` & `outgoing-0.6.1/test/test_senders/test_babyl.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,26 +50,26 @@
     inbox.close()
     assert len(msgs) == 1
     assert email2dict(test_email1) == email2dict(msgs[0])
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening Babyl mailbox at {tmp_path/'inbox'}",
+            f"Opening Babyl mailbox at {tmp_path / 'inbox'}",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to Babyl mailbox at"
-            f" {tmp_path/'inbox'}",
+            f" {tmp_path / 'inbox'}",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing Babyl mailbox at {tmp_path/'inbox'}",
+            f"Closing Babyl mailbox at {tmp_path / 'inbox'}",
         ),
     ]
 
 
 def test_babyl_send_extant_path(
     monkeypatch: pytest.MonkeyPatch,
     test_email1: EmailMessage,
```

### Comparing `outgoing-0.6.0/test/test_senders/test_command.py` & `outgoing-0.6.1/test/test_senders/test_command.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_senders/test_maildir.py` & `outgoing-0.6.1/test/test_senders/test_maildir.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,26 @@
     msgs = list(inbox)
     assert len(msgs) == 1
     assert email2dict(test_email1) == email2dict(msgs[0])
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening Maildir at {tmp_path/'inbox'}, root folder",
+            f"Opening Maildir at {tmp_path / 'inbox'}, root folder",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to Maildir at"
-            f" {tmp_path/'inbox'}, root folder",
+            f" {tmp_path / 'inbox'}, root folder",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing Maildir at {tmp_path/'inbox'}, root folder",
+            f"Closing Maildir at {tmp_path / 'inbox'}, root folder",
         ),
     ]
 
 
 def test_maildir_send_folder_new_path(
     caplog: pytest.LogCaptureFixture,
     monkeypatch: pytest.MonkeyPatch,
@@ -100,26 +100,26 @@
     msgs = list(work)
     assert len(msgs) == 1
     assert email2dict(test_email1) == email2dict(msgs[0])
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening Maildir at {tmp_path/'inbox'}, folder 'work'",
+            f"Opening Maildir at {tmp_path / 'inbox'}, folder 'work'",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to Maildir at"
-            f" {tmp_path/'inbox'}, folder 'work'",
+            f" {tmp_path / 'inbox'}, folder 'work'",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing Maildir at {tmp_path/'inbox'}, folder 'work'",
+            f"Closing Maildir at {tmp_path / 'inbox'}, folder 'work'",
         ),
     ]
 
 
 def test_maildir_send_no_folder_extant_path(
     monkeypatch: pytest.MonkeyPatch,
     test_email1: EmailMessage,
```

### Comparing `outgoing-0.6.0/test/test_senders/test_mbox.py` & `outgoing-0.6.1/test/test_senders/test_mbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,26 @@
     msgdict = email2dict(msgs[0])
     msgdict["unixfrom"] = None
     assert email2dict(test_email1) == msgdict
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening mbox at {tmp_path/'inbox'}",
+            f"Opening mbox at {tmp_path / 'inbox'}",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to mbox at"
-            f" {tmp_path/'inbox'}",
+            f" {tmp_path / 'inbox'}",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing mbox at {tmp_path/'inbox'}",
+            f"Closing mbox at {tmp_path / 'inbox'}",
         ),
     ]
 
 
 def test_mbox_send_extant_path(
     monkeypatch: pytest.MonkeyPatch,
     test_email1: EmailMessage,
```

### Comparing `outgoing-0.6.0/test/test_senders/test_mh.py` & `outgoing-0.6.1/test/test_senders/test_mh.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,26 @@
     msgs = list(inbox)
     assert len(msgs) == 1
     assert email2dict(test_email1) == email2dict(msgs[0])
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening MH mailbox at {tmp_path/'inbox'}, root folder",
+            f"Opening MH mailbox at {tmp_path / 'inbox'}, root folder",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to MH mailbox at"
-            f" {tmp_path/'inbox'}, root folder",
+            f" {tmp_path / 'inbox'}, root folder",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing MH mailbox at {tmp_path/'inbox'}, root folder",
+            f"Closing MH mailbox at {tmp_path / 'inbox'}, root folder",
         ),
     ]
 
 
 def test_mh_send_folder_str_new_path(
     caplog: pytest.LogCaptureFixture,
     monkeypatch: pytest.MonkeyPatch,
@@ -100,26 +100,26 @@
     msgs = list(work)
     assert len(msgs) == 1
     assert email2dict(test_email1) == email2dict(msgs[0])
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening MH mailbox at {tmp_path/'inbox'}, folder 'work'",
+            f"Opening MH mailbox at {tmp_path / 'inbox'}, folder 'work'",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to MH mailbox at"
-            f" {tmp_path/'inbox'}, folder 'work'",
+            f" {tmp_path / 'inbox'}, folder 'work'",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing MH mailbox at {tmp_path/'inbox'}, folder 'work'",
+            f"Closing MH mailbox at {tmp_path / 'inbox'}, folder 'work'",
         ),
     ]
 
 
 def test_mh_send_folder_list_new_path(
     caplog: pytest.LogCaptureFixture,
     monkeypatch: pytest.MonkeyPatch,
@@ -146,26 +146,26 @@
     msgs = list(work)
     assert len(msgs) == 1
     assert email2dict(test_email1) == email2dict(msgs[0])
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening MH mailbox at {tmp_path/'inbox'}, folder 'important'/'work'",
+            f"Opening MH mailbox at {tmp_path / 'inbox'}, folder 'important'/'work'",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to MH mailbox at"
-            f" {tmp_path/'inbox'}, folder 'important'/'work'",
+            f" {tmp_path / 'inbox'}, folder 'important'/'work'",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing MH mailbox at {tmp_path/'inbox'}, folder 'important'/'work'",
+            f"Closing MH mailbox at {tmp_path / 'inbox'}, folder 'important'/'work'",
         ),
     ]
 
 
 def test_mh_send_no_folder_extant_path(
     monkeypatch: pytest.MonkeyPatch,
     test_email1: EmailMessage,
```

### Comparing `outgoing-0.6.0/test/test_senders/test_mmdf.py` & `outgoing-0.6.1/test/test_senders/test_mmdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,26 @@
     msgdict = email2dict(msgs[0])
     msgdict["unixfrom"] = None
     assert email2dict(test_email1) == msgdict
     assert caplog.record_tuples == [
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Opening MMDF mailbox at {tmp_path/'inbox'}",
+            f"Opening MMDF mailbox at {tmp_path / 'inbox'}",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.INFO,
             f"Adding e-mail {test_email1['Subject']!r} to MMDF mailbox at"
-            f" {tmp_path/'inbox'}",
+            f" {tmp_path / 'inbox'}",
         ),
         (
             "outgoing.senders.mailboxes",
             logging.DEBUG,
-            f"Closing MMDF mailbox at {tmp_path/'inbox'}",
+            f"Closing MMDF mailbox at {tmp_path / 'inbox'}",
         ),
     ]
 
 
 def test_mmdf_send_extant_path(
     monkeypatch: pytest.MonkeyPatch,
     test_email1: EmailMessage,
```

### Comparing `outgoing-0.6.0/test/test_senders/test_null.py` & `outgoing-0.6.1/test/test_senders/test_null.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_senders/test_smtp.py` & `outgoing-0.6.1/test/test_senders/test_smtp.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/test/test_util.py` & `outgoing-0.6.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `outgoing-0.6.0/tox.ini` & `outgoing-0.6.1/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = lint,typing,py37,py38,py39,py310,py311,py312,pypy3
+envlist = lint,typing,py38,py39,py310,py311,py312,pypy3
 skip_missing_interpreters = True
 isolated_build = True
 minversion = 3.3.0
 
 [testenv]
 deps =
     mailbits
@@ -58,21 +58,20 @@
 exclude_lines =
     pragma: no cover
     if TYPE_CHECKING:
     \.\.\.
 
 [flake8]
 doctests = True
-exclude = .*/,build/,dist/,test/data,venv/
-hang-closing = False
+extend-exclude = build/,dist/,test/data,venv/
 max-doc-length = 100
 max-line-length = 80
 unused-arguments-ignore-stub-functions = True
-select = A,B,B902,B950,C,E,E242,F,U100,W
-ignore = A003,B005,E203,E262,E266,E501,W503
+extend-select = B901,B902,B950
+ignore = A003,A005,B005,E203,E262,E266,E501,E704,U101,W503
 
 [isort]
 atomic = True
 classes = IO
 force_sort_within_sections = True
 honor_noqa = True
 lines_between_sections = 0
```


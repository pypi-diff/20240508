# Comparing `tmp/thesilent-0.0.980.tar.gz` & `tmp/TheSilent-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thesilent-0.0.980.tar", last modified: Wed May  8 21:17:18 2024, max compression
+gzip compressed data, was "TheSilent-0.0.99.tar", last modified: Mon Jan  9 15:25:09 2023, max compression
```

## Comparing `thesilent-0.0.980.tar` & `TheSilent-0.0.99.tar`

### file list

```diff
@@ -1,22 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 21:17:18.284210 thesilent-0.0.980/
--rw-rw-rw-   0        0        0      583 2024-05-08 21:17:18.283210 thesilent-0.0.980/PKG-INFO
--rw-rw-rw-   0        0        0       70 2024-05-08 21:15:17.000000 thesilent-0.0.980/README.md
--rw-rw-rw-   0        0        0      650 2024-05-08 21:15:36.000000 thesilent-0.0.980/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 21:17:18.284210 thesilent-0.0.980/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 21:17:18.222663 thesilent-0.0.980/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 21:17:18.257210 thesilent-0.0.980/src/TheSilent/
--rw-rw-rw-   0        0        0        0 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/__init__.py
--rw-rw-rw-   0        0        0      167 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/clear.py
--rw-rw-rw-   0        0        0    16161 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/cobra.py
--rw-rw-rw-   0        0        0     1468 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/evasion.py
--rw-rw-rw-   0        0        0     2206 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/fingerprint_scanner.py
--rw-rw-rw-   0        0        0    80557 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/http_scanners.py
--rw-rw-rw-   0        0        0     2667 2024-05-08 11:01:11.000000 thesilent-0.0.980/src/TheSilent/kitten_crawler.py
--rw-rw-rw-   0        0        0    23369 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/payloads.py
--rw-rw-rw-   0        0        0     5234 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/puppy_requests.py
--rw-rw-rw-   0        0        0      646 2024-05-08 21:15:23.000000 thesilent-0.0.980/src/TheSilent/return_user_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-08 21:17:18.282211 thesilent-0.0.980/src/TheSilent.egg-info/
--rw-rw-rw-   0        0        0      583 2024-05-08 21:17:18.000000 thesilent-0.0.980/src/TheSilent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2024-05-08 21:17:18.000000 thesilent-0.0.980/src/TheSilent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 21:17:18.000000 thesilent-0.0.980/src/TheSilent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 21:17:18.000000 thesilent-0.0.980/src/TheSilent.egg-info/top_level.txt
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.786667 TheSilent-0.0.99/
+-rw-r--r--   0 linux     (1000) linux     (1000)      643 2023-01-09 15:25:09.786667 TheSilent-0.0.99/PKG-INFO
+-rw-r--r--   0 linux     (1000) linux     (1000)      101 2023-01-06 01:24:13.000000 TheSilent-0.0.99/README.md
+-rw-r--r--   0 linux     (1000) linux     (1000)      735 2023-01-09 15:05:42.000000 TheSilent-0.0.99/pyproject.toml
+-rw-r--r--   0 linux     (1000) linux     (1000)       38 2023-01-09 15:25:09.786667 TheSilent-0.0.99/setup.cfg
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.777667 TheSilent-0.0.99/src/
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.785667 TheSilent-0.0.99/src/TheSilent/
+-rw-r--r--   0 linux     (1000) linux     (1000)      762 2023-01-08 22:12:06.000000 TheSilent-0.0.99/src/TheSilent/TheSilent.py
+-rw-r--r--   0 linux     (1000) linux     (1000)        0 2023-01-06 01:24:13.000000 TheSilent-0.0.99/src/TheSilent/__init__.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1324 2023-01-08 22:09:59.000000 TheSilent-0.0.99/src/TheSilent/arp_void.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     6976 2023-01-08 22:10:13.000000 TheSilent-0.0.99/src/TheSilent/brute_force_hash.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      167 2023-01-08 20:46:15.000000 TheSilent-0.0.99/src/TheSilent/clear.py
+-rw-r--r--   0 linux     (1000) linux     (1000)    17412 2023-01-08 22:10:20.000000 TheSilent-0.0.99/src/TheSilent/dictionary_hash.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     7894 2023-01-08 22:10:23.000000 TheSilent-0.0.99/src/TheSilent/email_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1247 2023-01-08 21:08:17.000000 TheSilent-0.0.99/src/TheSilent/form_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1812 2023-01-08 22:10:31.000000 TheSilent-0.0.99/src/TheSilent/ftp_cracker.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      781 2023-01-08 22:10:35.000000 TheSilent-0.0.99/src/TheSilent/hex_viewer.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     9590 2023-01-09 15:24:17.000000 TheSilent-0.0.99/src/TheSilent/link_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     5982 2023-01-08 22:10:47.000000 TheSilent-0.0.99/src/TheSilent/login_cracker.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     5074 2023-01-08 22:10:51.000000 TheSilent-0.0.99/src/TheSilent/nmap.py
+-rw-r--r--   0 linux     (1000) linux     (1000)    19506 2023-01-08 22:10:56.000000 TheSilent-0.0.99/src/TheSilent/packet_sniffer.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     2541 2023-01-08 22:11:02.000000 TheSilent-0.0.99/src/TheSilent/port_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1833 2023-01-08 22:11:07.000000 TheSilent-0.0.99/src/TheSilent/secure_overwrite.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      800 2023-01-08 22:11:13.000000 TheSilent-0.0.99/src/TheSilent/security_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)      831 2023-01-08 22:11:18.000000 TheSilent-0.0.99/src/TheSilent/source_code_viewer.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     9363 2023-01-08 22:11:23.000000 TheSilent-0.0.99/src/TheSilent/sql_injection_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1307 2023-01-08 22:11:27.000000 TheSilent-0.0.99/src/TheSilent/subdomain_scanner.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     1366 2023-01-08 22:11:32.000000 TheSilent-0.0.99/src/TheSilent/subdomain_takeover.py
+-rw-r--r--   0 linux     (1000) linux     (1000)     7212 2023-01-09 15:19:41.000000 TheSilent-0.0.99/src/TheSilent/xss_scanner.py
+drwxr-xr-x   0 linux     (1000) linux     (1000)        0 2023-01-09 15:25:09.786667 TheSilent-0.0.99/src/TheSilent.egg-info/
+-rw-r--r--   0 linux     (1000) linux     (1000)      643 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/PKG-INFO
+-rw-r--r--   0 linux     (1000) linux     (1000)      883 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/SOURCES.txt
+-rw-r--r--   0 linux     (1000) linux     (1000)        1 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/dependency_links.txt
+-rw-r--r--   0 linux     (1000) linux     (1000)       23 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/requires.txt
+-rw-r--r--   0 linux     (1000) linux     (1000)       10 2023-01-09 15:25:09.000000 TheSilent-0.0.99/src/TheSilent.egg-info/top_level.txt
```


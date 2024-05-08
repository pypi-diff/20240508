# Comparing `tmp/batou_ext-2.4.7.tar.gz` & `tmp/batou_ext-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou_ext-2.4.7.tar", last modified: Mon Apr 29 08:52:23 2024, max compression
+gzip compressed data, was "batou_ext-2.4.8.tar", last modified: Wed May  8 12:04:49 2024, max compression
```

## Comparing `batou_ext-2.4.7.tar` & `batou_ext-2.4.8.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.112029 batou_ext-2.4.7/
--rw-r--r--   0 zagy       (501) staff       (20)     2244 2024-04-29 08:52:22.000000 batou_ext-2.4.7/CHANGES.md
--rw-r--r--   0 zagy       (501) staff       (20)     1608 2024-04-29 08:52:22.000000 batou_ext-2.4.7/LICENSE.txt
--rw-r--r--   0 zagy       (501) staff       (20)      144 2024-04-29 08:52:22.000000 batou_ext-2.4.7/MANIFEST.in
--rw-r--r--   0 zagy       (501) staff       (20)     4474 2024-04-29 08:52:23.111944 batou_ext-2.4.7/PKG-INFO
--rw-r--r--   0 zagy       (501) staff       (20)     1163 2024-04-29 08:52:22.000000 batou_ext-2.4.7/README.md
--rw-r--r--   0 zagy       (501) staff       (20)      121 2024-04-29 08:52:22.000000 batou_ext-2.4.7/pyproject.toml
--rw-r--r--   0 zagy       (501) staff       (20)      491 2024-04-29 08:52:23.112329 batou_ext-2.4.7/setup.cfg
--rw-r--r--   0 zagy       (501) staff       (20)     1737 2024-04-29 08:52:22.000000 batou_ext-2.4.7/setup.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.097672 batou_ext-2.4.7/src/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.104041 batou_ext-2.4.7/src/batou_ext/
--rw-r--r--   0 zagy       (501) staff       (20)       23 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     1213 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/acl.py
--rw-r--r--   0 zagy       (501) staff       (20)     1080 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/archive.py
--rw-r--r--   0 zagy       (501) staff       (20)     3560 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/config.py
--rw-r--r--   0 zagy       (501) staff       (20)     6795 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/cron.py
--rw-r--r--   0 zagy       (501) staff       (20)    10472 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/fcio.py
--rw-r--r--   0 zagy       (501) staff       (20)     5087 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/file.py
--rw-r--r--   0 zagy       (501) staff       (20)     1498 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/geoip.py
--rw-r--r--   0 zagy       (501) staff       (20)     8165 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/git.py
--rw-r--r--   0 zagy       (501) staff       (20)      616 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/htpasswd.py
--rw-r--r--   0 zagy       (501) staff       (20)     9614 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/http.py
--rw-r--r--   0 zagy       (501) staff       (20)     4162 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/jenkins.py
--rw-r--r--   0 zagy       (501) staff       (20)      714 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/journalbeat.py
--rw-r--r--   0 zagy       (501) staff       (20)      831 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/keypair.py
--rw-r--r--   0 zagy       (501) staff       (20)     5641 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mail.py
--rw-r--r--   0 zagy       (501) staff       (20)      245 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mailhog.py
--rw-r--r--   0 zagy       (501) staff       (20)      972 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/memcached.py
--rw-r--r--   0 zagy       (501) staff       (20)     3325 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mirror.py
--rw-r--r--   0 zagy       (501) staff       (20)     1512 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mysql.py
--rw-r--r--   0 zagy       (501) staff       (20)      617 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/nfs.py
--rw-r--r--   0 zagy       (501) staff       (20)    24116 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/nix.py
--rw-r--r--   0 zagy       (501) staff       (20)     2214 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/nixos.py
--rw-r--r--   0 zagy       (501) staff       (20)     6111 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/oci.py
--rw-r--r--   0 zagy       (501) staff       (20)     3923 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/php.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.105528 batou_ext-2.4.7/src/batou_ext/postfixadmin/
--rw-r--r--   0 zagy       (501) staff       (20)     1997 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/__init__.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.105750 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/
--rw-r--r--   0 zagy       (501) staff       (20)      751 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/database.conf
--rw-r--r--   0 zagy       (501) staff       (20)      447 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/local.conf
--rw-r--r--   0 zagy       (501) staff       (20)      584 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot.py
--rw-r--r--   0 zagy       (501) staff       (20)      576 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/goceptnet.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.106798 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/
--rw-r--r--   0 zagy       (501) staff       (20)      668 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/local.cf
--rw-r--r--   0 zagy       (501) staff       (20)      369 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
--rw-r--r--   0 zagy       (501) staff       (20)      371 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
--rw-r--r--   0 zagy       (501) staff       (20)      376 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
--rw-r--r--   0 zagy       (501) staff       (20)      457 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
--rw-r--r--   0 zagy       (501) staff       (20)     1541 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.107102 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfixadmin/
--rw-r--r--   0 zagy       (501) staff       (20)      864 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfixadmin/config.local.php
--rw-r--r--   0 zagy       (501) staff       (20)      607 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postgres.py
--rw-r--r--   0 zagy       (501) staff       (20)     5294 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postgres.py
--rw-r--r--   0 zagy       (501) staff       (20)     3296 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/python.py
--rw-r--r--   0 zagy       (501) staff       (20)     5691 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/rabbitmq.py
--rw-r--r--   0 zagy       (501) staff       (20)     1268 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/redis.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.109884 batou_ext-2.4.7/src/batou_ext/resources/
--rw-r--r--   0 zagy       (501) staff       (20)      541 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/cert.sh
--rw-r--r--   0 zagy       (501) staff       (20)      388 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/check_systemd_unit.py
--rw-r--r--   0 zagy       (501) staff       (20)      117 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/cron-wrapper.sh
--rw-r--r--   0 zagy       (501) staff       (20)      200 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/geoip-update.sh
--rw-r--r--   0 zagy       (501) staff       (20)     1552 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/http-watchdog.nix
--rw-r--r--   0 zagy       (501) staff       (20)      203 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/journalbeat.nix
--rw-r--r--   0 zagy       (501) staff       (20)      955 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/loader.c
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110033 batou_ext-2.4.7/src/batou_ext/resources/mailhog/
--rw-r--r--   0 zagy       (501) staff       (20)     1371 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/mailhog/mailhog.nix
--rw-r--r--   0 zagy       (501) staff       (20)      946 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/mirror.conf
--rw-r--r--   0 zagy       (501) staff       (20)     1898 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/oci-template.nix
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110395 batou_ext-2.4.7/src/batou_ext/resources/php/
--rw-r--r--   0 zagy       (501) staff       (20)      588 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/php/php-fpm.conf
--rw-r--r--   0 zagy       (501) staff       (20)      296 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/php/php-fpm.sh
--rw-r--r--   0 zagy       (501) staff       (20)    71038 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/php/php.ini
--rw-r--r--   0 zagy       (501) staff       (20)      576 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/python.nix
--rw-r--r--   0 zagy       (501) staff       (20)      118 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/rediscleanup.sh
--rw-r--r--   0 zagy       (501) staff       (20)      560 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/setupEnv.sh
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110582 batou_ext-2.4.7/src/batou_ext/resources/ssl/
--rw-r--r--   0 zagy       (501) staff       (20)      597 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/ssl/local_certificate_check.sh
--rw-r--r--   0 zagy       (501) staff       (20)      178 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/systemd.service
--rw-r--r--   0 zagy       (501) staff       (20)      617 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/userenv.nix
--rw-r--r--   0 zagy       (501) staff       (20)     6869 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/watchdog-wrapper.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110991 batou_ext-2.4.7/src/batou_ext/roundcube/
--rw-r--r--   0 zagy       (501) staff       (20)     3456 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/roundcube/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     4181 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/roundcube/config.inc.php
--rw-r--r--   0 zagy       (501) staff       (20)      623 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/roundcube/postgres.py
--rw-r--r--   0 zagy       (501) staff       (20)     1525 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/run.py
--rw-r--r--   0 zagy       (501) staff       (20)     4745 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/s3.py
--rw-r--r--   0 zagy       (501) staff       (20)     9400 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/s3_bootstrap.py
--rw-r--r--   0 zagy       (501) staff       (20)     3572 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/ssh.py
--rw-r--r--   0 zagy       (501) staff       (20)    11133 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/ssl.py
--rw-r--r--   0 zagy       (501) staff       (20)     5258 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/versions.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.111173 batou_ext-2.4.7/src/batou_ext.egg-info/
--rw-r--r--   0 zagy       (501) staff       (20)     4474 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/PKG-INFO
--rw-r--r--   0 zagy       (501) staff       (20)     2695 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/SOURCES.txt
--rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/dependency_links.txt
--rw-r--r--   0 zagy       (501) staff       (20)      171 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/entry_points.txt
--rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/not-zip-safe
--rw-r--r--   0 zagy       (501) staff       (20)      153 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/requires.txt
--rw-r--r--   0 zagy       (501) staff       (20)       10 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/top_level.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.975054 batou_ext-2.4.8/
+-rw-r--r--   0 zagy       (501) staff       (20)     2930 2024-05-08 12:04:49.000000 batou_ext-2.4.8/CHANGES.md
+-rw-r--r--   0 zagy       (501) staff       (20)     1608 2024-05-08 12:04:49.000000 batou_ext-2.4.8/LICENSE.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      144 2024-05-08 12:04:49.000000 batou_ext-2.4.8/MANIFEST.in
+-rw-r--r--   0 zagy       (501) staff       (20)     5160 2024-05-08 12:04:49.974959 batou_ext-2.4.8/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     1163 2024-05-08 12:04:49.000000 batou_ext-2.4.8/README.md
+-rw-r--r--   0 zagy       (501) staff       (20)      121 2024-05-08 12:04:49.000000 batou_ext-2.4.8/pyproject.toml
+-rw-r--r--   0 zagy       (501) staff       (20)      491 2024-05-08 12:04:49.975369 batou_ext-2.4.8/setup.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)     1737 2024-05-08 12:04:49.000000 batou_ext-2.4.8/setup.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.961970 batou_ext-2.4.8/src/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.968169 batou_ext-2.4.8/src/batou_ext/
+-rw-r--r--   0 zagy       (501) staff       (20)       23 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1213 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/acl.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1080 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/archive.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3560 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/config.py
+-rw-r--r--   0 zagy       (501) staff       (20)     7494 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/cron.py
+-rw-r--r--   0 zagy       (501) staff       (20)    10472 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/fcio.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5087 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/file.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1498 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/geoip.py
+-rw-r--r--   0 zagy       (501) staff       (20)     8165 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/git.py
+-rw-r--r--   0 zagy       (501) staff       (20)      616 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/htpasswd.py
+-rw-r--r--   0 zagy       (501) staff       (20)     9614 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/http.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4162 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/jenkins.py
+-rw-r--r--   0 zagy       (501) staff       (20)      714 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/journalbeat.py
+-rw-r--r--   0 zagy       (501) staff       (20)      831 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/keypair.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5641 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/mail.py
+-rw-r--r--   0 zagy       (501) staff       (20)      245 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/mailhog.py
+-rw-r--r--   0 zagy       (501) staff       (20)      972 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/memcached.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3325 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/mirror.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1512 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/mysql.py
+-rw-r--r--   0 zagy       (501) staff       (20)      617 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/nfs.py
+-rw-r--r--   0 zagy       (501) staff       (20)    24116 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/nix.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2214 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/nixos.py
+-rw-r--r--   0 zagy       (501) staff       (20)     7737 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/oci.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3923 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/php.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.969736 batou_ext-2.4.8/src/batou_ext/postfixadmin/
+-rw-r--r--   0 zagy       (501) staff       (20)     1997 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/__init__.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.970010 batou_ext-2.4.8/src/batou_ext/postfixadmin/dovecot/
+-rw-r--r--   0 zagy       (501) staff       (20)      751 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/dovecot/database.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      447 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/dovecot/local.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      584 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/dovecot.py
+-rw-r--r--   0 zagy       (501) staff       (20)      576 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/goceptnet.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.970737 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix/
+-rw-r--r--   0 zagy       (501) staff       (20)      668 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix/local.cf
+-rw-r--r--   0 zagy       (501) staff       (20)      369 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
+-rw-r--r--   0 zagy       (501) staff       (20)      371 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
+-rw-r--r--   0 zagy       (501) staff       (20)      376 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
+-rw-r--r--   0 zagy       (501) staff       (20)      457 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
+-rw-r--r--   0 zagy       (501) staff       (20)     1541 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.970878 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfixadmin/
+-rw-r--r--   0 zagy       (501) staff       (20)      864 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postfixadmin/config.local.php
+-rw-r--r--   0 zagy       (501) staff       (20)      607 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postfixadmin/postgres.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5294 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/postgres.py
+-rw-r--r--   0 zagy       (501) staff       (20)     8391 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/python.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5691 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/rabbitmq.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1268 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/redis.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.972925 batou_ext-2.4.8/src/batou_ext/resources/
+-rw-r--r--   0 zagy       (501) staff       (20)      541 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/cert.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      388 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/check_systemd_unit.py
+-rw-r--r--   0 zagy       (501) staff       (20)      117 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/cron-wrapper.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      200 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/geoip-update.sh
+-rw-r--r--   0 zagy       (501) staff       (20)     1552 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/http-watchdog.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      203 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/journalbeat.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      955 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/loader.c
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.973058 batou_ext-2.4.8/src/batou_ext/resources/mailhog/
+-rw-r--r--   0 zagy       (501) staff       (20)     1371 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/mailhog/mailhog.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      946 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/mirror.conf
+-rw-r--r--   0 zagy       (501) staff       (20)     1898 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/oci-template.nix
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.973418 batou_ext-2.4.8/src/batou_ext/resources/php/
+-rw-r--r--   0 zagy       (501) staff       (20)      588 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/php/php-fpm.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      296 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/php/php-fpm.sh
+-rw-r--r--   0 zagy       (501) staff       (20)    71038 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/php/php.ini
+-rw-r--r--   0 zagy       (501) staff       (20)      576 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/python.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      118 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/rediscleanup.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      560 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/setupEnv.sh
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.973584 batou_ext-2.4.8/src/batou_ext/resources/ssl/
+-rw-r--r--   0 zagy       (501) staff       (20)      597 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/ssl/local_certificate_check.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      178 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/systemd.service
+-rw-r--r--   0 zagy       (501) staff       (20)      617 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/userenv.nix
+-rw-r--r--   0 zagy       (501) staff       (20)     6869 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/resources/watchdog-wrapper.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.973952 batou_ext-2.4.8/src/batou_ext/roundcube/
+-rw-r--r--   0 zagy       (501) staff       (20)     3456 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/roundcube/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4181 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/roundcube/config.inc.php
+-rw-r--r--   0 zagy       (501) staff       (20)      623 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/roundcube/postgres.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1525 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/run.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4745 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/s3.py
+-rw-r--r--   0 zagy       (501) staff       (20)     9400 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/s3_bootstrap.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3572 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/ssh.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11133 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/ssl.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5258 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext/versions.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-05-08 12:04:49.974131 batou_ext-2.4.8/src/batou_ext.egg-info/
+-rw-r--r--   0 zagy       (501) staff       (20)     5160 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext.egg-info/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     2695 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      171 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext.egg-info/entry_points.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext.egg-info/not-zip-safe
+-rw-r--r--   0 zagy       (501) staff       (20)      153 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext.egg-info/requires.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       10 2024-05-08 12:04:49.000000 batou_ext-2.4.8/src/batou_ext.egg-info/top_level.txt
```

### Comparing `batou_ext-2.4.7/CHANGES.md` & `batou_ext-2.4.8/CHANGES.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,23 @@
 
+## 2.4.8 (2024-05-08)
+
+
+- systemd timers: add an option to enable persistence
+  breaking change: systemd timers are now non-persistent by default.
+  The previous default behaviour was a problem for cronjobs that should
+  not be started immediately following a reboot / downtime
+
+* Added a component `batou_ext.python.FixELFRunPath` which modifies `DT_RUNPATH` & `DT_RPATH` of `.so`-files in a venv to load the correct libraries (from either a Nix env or other Python libraries). Please read the docstring carefully before using it.
+
+- OCI: cache validation result during deployment.
+
+  Caching results speeds up deployments where multiple containers with the same image are deployed.
+
+
 ## 2.4.7 (2024-04-29)
 
 
 * Added component `batou_ext.http.HTTPServiceWatchdog` that adds a check to a systemd unit
   whether a given URL is reachable (e.g. a `/health` endpoint). If the URL cannot be reached within
   a certain interval, the service will be restarted. Further details are documented in the
   docstring.
```

### Comparing `batou_ext-2.4.7/LICENSE.txt` & `batou_ext-2.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/PKG-INFO` & `batou_ext-2.4.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou_ext
-Version: 2.4.7
+Version: 2.4.8
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
@@ -66,14 +66,29 @@
 creating an [S3 bucket](https://wiki.flyingcircus.io/S3) and - if needed -
 an access keypair and lifecycle rules.
 
 On an activated virtualenv this can be tested with `python -m batou_ext.s3_bootstrap`.
 
 
 
+## 2.4.8 (2024-05-08)
+
+
+- systemd timers: add an option to enable persistence
+  breaking change: systemd timers are now non-persistent by default.
+  The previous default behaviour was a problem for cronjobs that should
+  not be started immediately following a reboot / downtime
+
+* Added a component `batou_ext.python.FixELFRunPath` which modifies `DT_RUNPATH` & `DT_RPATH` of `.so`-files in a venv to load the correct libraries (from either a Nix env or other Python libraries). Please read the docstring carefully before using it.
+
+- OCI: cache validation result during deployment.
+
+  Caching results speeds up deployments where multiple containers with the same image are deployed.
+
+
 ## 2.4.7 (2024-04-29)
 
 
 * Added component `batou_ext.http.HTTPServiceWatchdog` that adds a check to a systemd unit
   whether a given URL is reachable (e.g. a `/health` endpoint). If the URL cannot be reached within
   a certain interval, the service will be restarted. Further details are documented in the
   docstring.
```

### Comparing `batou_ext-2.4.7/README.md` & `batou_ext-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/setup.py` & `batou_ext-2.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def project_path(*names):
     return os.path.join(*names)
 
 
 setup(
     name="batou_ext",
-    version="2.4.7",
+    version="2.4.8",
     install_requires=[
         "batou >= 2.3b4",
         "pyaml",
         "setuptools",
         "six",
         "InquirerPy",
     ],
```

### Comparing `batou_ext-2.4.7/src/batou_ext/acl.py` & `batou_ext-2.4.8/src/batou_ext/acl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/archive.py` & `batou_ext-2.4.8/src/batou_ext/archive.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/config.py` & `batou_ext-2.4.8/src/batou_ext/config.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/cron.py` & `batou_ext-2.4.8/src/batou_ext/cron.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,21 +122,30 @@
             command="bin/cleanup some stuff",
             onCalendar="*:0/5",
             timeout="3m")
 
     See https://www.freedesktop.org/software/systemd/man/systemd.time.html
     for details about the `onCalendar` timer settings.
 
+    If `persistent` is set to True, the time when the service unit was last
+    triggered is stored on disk.
+    When the timer is activated, the service unit is triggered immediately
+    if it would have been triggered at least once during the time when
+    the timer was inactive.
+
+    For deployments, this usually means that the unit is started immediately
+    after, without waiting for the next scheduled activation.
     """
 
     _required_params_ = {"command": "/bin/true", "onCalendar": "02:00:00"}
 
     namevar = "tag"
     command = batou.component.Attribute(str)
     onCalendar = batou.component.Attribute(str)
+    persistent = batou.component.Attribute("literal", False)
     timeout = "1h"
     description = None
     additional_service_config = None
     run_as = batou.component.Attribute(
         str,
         default=batou.component.ConfigString(
             "{{component.environment.service_user}}"
@@ -162,25 +171,30 @@
 
             """
             )
             + self.command,
         )
         self.wrapped_command = self._.path
 
+        if isinstance(self.persistent, bool) and self.persistent:
+            self.persistent_timer_config = "true"
+        else:
+            self.persistent_timer_config = "false"
+
         self += batou.lib.file.File(
             f"/etc/local/nixos/timer-{self.tag}.nix",
             content=dedent(
                 """\
               { ... }:
               {
                 systemd.timers."{{component.tag}}" = {
                   wantedBy = [ "timers.target" ];
                   timerConfig = {
                     OnCalendar = "{{component.onCalendar}}";
-                    Persistent = true;
+                    Persistent = {{component.persistent_timer_config}};
                   };
                 };
 
                 systemd.services."{{component.tag}}" = {
                   description = "{{component.description}}";
                   serviceConfig = {
                     Type = "oneshot";
```

### Comparing `batou_ext-2.4.7/src/batou_ext/fcio.py` & `batou_ext-2.4.8/src/batou_ext/fcio.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/file.py` & `batou_ext-2.4.8/src/batou_ext/file.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/geoip.py` & `batou_ext-2.4.8/src/batou_ext/geoip.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/git.py` & `batou_ext-2.4.8/src/batou_ext/git.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/htpasswd.py` & `batou_ext-2.4.8/src/batou_ext/htpasswd.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/http.py` & `batou_ext-2.4.8/src/batou_ext/http.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/jenkins.py` & `batou_ext-2.4.8/src/batou_ext/jenkins.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/journalbeat.py` & `batou_ext-2.4.8/src/batou_ext/journalbeat.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/keypair.py` & `batou_ext-2.4.8/src/batou_ext/keypair.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/mail.py` & `batou_ext-2.4.8/src/batou_ext/mail.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/memcached.py` & `batou_ext-2.4.8/src/batou_ext/memcached.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/mirror.py` & `batou_ext-2.4.8/src/batou_ext/mirror.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/mysql.py` & `batou_ext-2.4.8/src/batou_ext/mysql.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/nfs.py` & `batou_ext-2.4.8/src/batou_ext/nfs.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/nix.py` & `batou_ext-2.4.8/src/batou_ext/nix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/nixos.py` & `batou_ext-2.4.8/src/batou_ext/nixos.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/oci.py` & `batou_ext-2.4.8/src/batou_ext/oci.py`

 * *Files 23% similar despite different names*

```diff
@@ -79,14 +79,17 @@
     registry_user = Attribute(Optional[str], None)
     registry_password = Attribute(Optional[str], None)
 
     _required_params_ = {
         "image": "mysql",
     }
 
+    # cache spanning multiple components deploying the same container
+    _remote_manifest_cache = {}
+
     def configure(self):
         if (
             self.registry_user or self.registry_password
         ) and not self.registry_address:
             self.log(
                 "WARN: you might want to specify the registry explicitly"
                 " unless you really intend to log into the default"
@@ -132,59 +135,92 @@
             ),
         )
 
     def verify(self):
         self.assert_no_changes()
         self.envfile.assert_no_changes()
 
-        if self.registry_address:
-            logintxt, _ = self.cmd(
-                self.expand(
-                    dedent(
-                        """\
-        docker login \\
-            {%- if component.registry_user and component.registry_password %}
-            -u {{component.registry_user}} \\
-            -p {{component.registry_password}} \\
-            {%- endif %}
-            {{component.registry_address}}
-        """
-                    )
-                )
-            )
+        valid = False
 
-        local_digest, stderr = self.cmd(
+        container_image_id, stderr = self.cmd(
+            dedent(
+                """\
+            docker container insepct {{component.container_name}} \
+                | jq -r '.[0].Image'
+                """
+            )
+        )
+        local_image_id, stderr = self.cmd(
             dedent(
                 """\
             docker image inspect {{component.image}}:{{component.version}} \
-                | jq -r 'first | .RepoDigests | first | split("@") | last' \
+                | jq -r '.[0].Id' \
                 || echo image not available locally
                 """
             )
         )
-        try:
-            self.cmd(
-                "docker manifest inspect"
-                f" {self.image}:{self.version}@{local_digest}"
-            )
-        except CmdExecutionError as e:
-            valid = False
-            error = e.stderr
-            if error.startswith("unsupported manifest format"):  # gitlab
-                batou.output.annotate(error, debug=True)
-                error = error[:50]
-        else:
-            valid = True
-
-        # `docker manifest inspect` silently raises an error, returns code 0
-        # when unathorized
-        if stderr == "unauthorized":
-            raise RuntimeError(
-                "Wrong credentials for remote container registry"
+        if local_image_id != container_image_id:
+            # If the container is not running the image we expect, we need to
+            # restart it. If its the same, we need to dig further
+            error = (
+                "Container is running different image. "
+                "({container_image_id} vs. {local_image_id})"
+            )
+            local_digest, stderr = self.cmd(
+                dedent(
+                    """\
+                docker image inspect {{component.image}}:{{component.version}} \
+                    | jq -r 'first | .RepoDigests | first | split("@") | last' \
+                    || echo image not available locally
+                    """
+                )
             )
 
+            image_ident = f"{self.image}:{self.version}@{local_digest}"
+            try:
+                valid = self._remote_manifest_cache[image_ident]
+                error = "(cached)"
+            except KeyError:
+                if self.registry_address:
+                    logintxt, _ = self.cmd(
+                        self.expand(
+                            dedent(
+                                """\
+                docker login \\
+                    {%- if component.registry_user and component.registry_password %}
+                    -u {{component.registry_user}} \\
+                    -p {{component.registry_password}} \\
+                    {%- endif %}
+                    {{component.registry_address}}
+                """
+                            )
+                        )
+                    )
+
+                try:
+                    stdout, stderr = self.cmd(
+                        f"docker manifest inspect {image_ident}"
+                    )
+                except CmdExecutionError as e:
+                    valid = False
+                    error = e.stderr
+                    if error.startswith(
+                        "unsupported manifest format"
+                    ):  # gitlab
+                        batou.output.annotate(error, debug=True)
+                        error = error[:50]
+                else:
+                    # `docker manifest inspect` silently raises an error,
+                    # returns code 0 when unathorized
+                    if stderr == "unauthorized":
+                        raise RuntimeError(
+                            "Wrong credentials for remote container registry"
+                        )
+                    valid = True
+                self._remote_manifest_cache[image_ident] = valid
+
         if not valid:
             self.log("Update due digest verification error: %r", error)
             raise UpdateNeeded()
 
     def update(self):
         self.cmd(f"sudo systemctl restart docker-{self.container_name}")
```

### Comparing `batou_ext-2.4.7/src/batou_ext/php.py` & `batou_ext-2.4.8/src/batou_ext/php.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/__init__.py` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/database.conf` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/dovecot/database.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot.py` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/dovecot.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/goceptnet.py` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/local.cf` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix/local.cf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix.py` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/postfix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/postfixadmin/config.local.php` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/postfixadmin/config.local.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postfixadmin/postgres.py` & `batou_ext-2.4.8/src/batou_ext/postfixadmin/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/postgres.py` & `batou_ext-2.4.8/src/batou_ext/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/python.py` & `batou_ext-2.4.8/src/batou_ext/roundcube/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,112 @@
-import os.path
+import os
 
-import batou.component
-import batou.lib.python
+from batou import UpdateNeeded
+from batou.component import Attribute, Component, ConfigString
+from batou.lib.archive import Extract
+from batou.lib.download import Download
+from batou.lib.file import Directory, File, SyncDirectory
+from batou.utils import Address
 
+from batou_ext.php import FPM
 
-class Pipenv(batou.component.Component):
-    """Sync pipenv
 
-    Usage:
-
-    * Checkout project to workdir, expecting Pipfile/Pipfile.lock there
-    * self += Pipenv()`
-    * Run services via `pipenv.executable` (points ot virualenv'ed python)
-
-    Notes:
-
-    * The Python version *is* specified in the Pipfile. So there is no need to
-      pass.
-    * `pipenv` is epxected to be there already. I.e. coming from the system.
-    * For NixOS you can `nix-env -iA nixos.pipenv`. You will also need
-      `nixos.which` and the python version the Pipfile specifies.
+class Roundcube(Component):
+    """Configure Roundcube with database connection.
 
+    Roundcube is installed with php/fastcgi. A basic configuration for the
+    frontend is created but it is up to the user to fine-tune that
+    configuration.
     """
 
-    target = None
+    release = "1.1.4"
+    checksum = "sha256:9bfe88255d4ffc288f5776de1cead78352469b1766d5ebaebe6e28043affe181"  # noqa: E501 line too long
 
-    def configure(self):
-        if self.target is None:
-            self.target = self.workdir
-        self.venv = os.path.join(self.workdir, self.target, ".venv")
-        self.executable = os.path.join(self.venv, "bin/python")
+    address = Attribute(Address, ConfigString("127.0.0.1:9000"))
+    skin = "larry"
+    support_url = "http://localhost"
 
-    def verify(self):
-        with self.chdir(self.target):
-            self.assert_file_is_current(
-                self.executable, ["Pipfile", "Pipfile.lock"]
-            )
-            # Is this Python (still) functional 'enough'
-            # from a setuptools/distribute perspective?
-            self.assert_cmd(
-                '{{component.executable}} -c "import pkg_resources"'
-            )
-
-    def update(self):
-        with self.chdir(self.target):
-            self.cmd("rm -rf .venv")
-            self.cmd("pipenv sync", env={"PIPENV_VENV_IN_PROJECT": "1"})
+    smtp_user = "%u"
+    smtp_pass = "%p"
 
+    config = os.path.join(os.path.dirname(__file__), "config.inc.php")
 
-class VirtualEnvRequirements(batou.component.Component):
-    """
-    Installs a Python VirtualEnv with a given requirements.txt
-
-    Usage::
-        self += VirtualEnvRequirements(
-            version='2.7',
-            requirements_path='/path/to/my/requirements.txt')
-    """
-
-    version = batou.component.Attribute(str, default="2.7")
-    requirements_path = batou.component.Attribute(
-        str, batou.component.ConfigString("requirements.txt")
-    )
+    def configure(self):
+        self.db = self.require_one("roundcube::database")
+        postfix = self.require_one("postfix")
 
-    # Shell script to be sourced before creating VirtualEnv and pip
-    pre_run_script_path = None
+        self.imap_host = postfix.connect.host
+        self.smtp_server = postfix.connect.host
+        self.smtp_port = postfix.connect.port
+
+        self.basedir = self.map("roundcube")
+        self.provide("roundcube", self)
+
+        self += Directory("download")
+        download = Download(
+            "http://downloads.sourceforge.net/project/roundcubemail/"
+            "roundcubemail/{}/roundcubemail-{}-complete.tar.gz".format(
+                self.release, self.release
+            ),
+            target="download/roundcube-{}.tar.gz".format(self.release),
+            checksum=self.checksum,
+        )
+        self += download
+
+        self += Extract(download.target, target="roundcube.orig")
+        self += SyncDirectory(
+            self.basedir,
+            source=self.map(
+                "roundcube.orig/roundcubemail-{}".format(self.release)
+            ),
+        )
+
+        self.db_dsnw = "{}://{}:{}@{}/{}".format(
+            self.db.dbms,
+            self.db.username,
+            self.db.password,
+            self.db.address.connect.host,
+            self.db.database,
+        )
+
+        self += File(
+            self.basedir + "/config/config.inc.php", source=self.config
+        )
+
+        self.fpm = FPM("roundcube")
+        self += self.fpm
 
-    # Passing environmental variables to batou's cmd
-    env = None
+        self += RoundcubeInit(self)
 
-    # May pass pre-fabricated virtualenv
-    venv = None
 
-    def configure(self):
+class RoundcubeInit(Component):
 
-        if isinstance(self.requirements_path, str):
-            self.requirements_paths = [self.requirements_path]
-        elif isinstance(self.requirements_path, list):
-            self.requirements_paths = self.requirements_path
-        else:
-            raise RuntimeError("Needs to be either string or list")
-
-        if self.venv is None:
-            self.venv = batou.lib.python.VirtualEnv(self.version)
-        self += self.venv
+    namevar = "roundcube"
 
     def verify(self):
-        self.assert_no_changes()
-        self.parent.assert_no_changes()
+        os.environ["PGPASSWORD"] = self.roundcube.db.password
+        host = self.roundcube.db.address.connect.host
+        db = self.roundcube.db
+        try:
+
+            result = self.cmd(
+                f"psql -h {host} -U {db.username} -d {db.database} -c "
+                '"SELECT * FROM information_schema.tables '
+                "WHERE table_schema='public' "
+                "AND table_catalog='roundcube';\""
+            )
+            if "contact" not in result[0]:
+                raise UpdateNeeded()
+        finally:
+            del os.environ["PGPASSWORD"]
 
     def update(self):
-        for req in self.requirements_paths:
-            if self.pre_run_script_path:
-                self.cmd(
-                    (
-                        "source {} && {} " "-m pip install --upgrade -r {}"
-                    ).format(self.pre_run_script_path, self.venv.python, req),
-                    env=self.env,
-                )
-            else:
-                self.cmd(
-                    "{} -m pip install --upgrade -r {}".format(
-                        self.venv.python, req
-                    ),
-                    env=self.env,
-                )
+        os.environ["PGPASSWORD"] = self.roundcube.db.password
+        self.cmd(
+            "psql -h {} -d {} -U {} -f {}/SQL/postgres.initial.sql".format(
+                self.roundcube.db.address.connect.host,
+                self.roundcube.db.database,
+                self.roundcube.db.username,
+                self.roundcube.basedir,
+            )
+        )
+        del os.environ["PGPASSWORD"]
```

### Comparing `batou_ext-2.4.7/src/batou_ext/rabbitmq.py` & `batou_ext-2.4.8/src/batou_ext/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/redis.py` & `batou_ext-2.4.8/src/batou_ext/redis.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/cert.sh` & `batou_ext-2.4.8/src/batou_ext/resources/cert.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/http-watchdog.nix` & `batou_ext-2.4.8/src/batou_ext/resources/http-watchdog.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/loader.c` & `batou_ext-2.4.8/src/batou_ext/resources/loader.c`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/mailhog/mailhog.nix` & `batou_ext-2.4.8/src/batou_ext/resources/mailhog/mailhog.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/mirror.conf` & `batou_ext-2.4.8/src/batou_ext/resources/mirror.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/oci-template.nix` & `batou_ext-2.4.8/src/batou_ext/resources/oci-template.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/php/php-fpm.conf` & `batou_ext-2.4.8/src/batou_ext/resources/php/php-fpm.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/php/php.ini` & `batou_ext-2.4.8/src/batou_ext/resources/php/php.ini`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/python.nix` & `batou_ext-2.4.8/src/batou_ext/resources/python.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/setupEnv.sh` & `batou_ext-2.4.8/src/batou_ext/resources/setupEnv.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/ssl/local_certificate_check.sh` & `batou_ext-2.4.8/src/batou_ext/resources/ssl/local_certificate_check.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/userenv.nix` & `batou_ext-2.4.8/src/batou_ext/resources/userenv.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/resources/watchdog-wrapper.py` & `batou_ext-2.4.8/src/batou_ext/resources/watchdog-wrapper.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/roundcube/config.inc.php` & `batou_ext-2.4.8/src/batou_ext/roundcube/config.inc.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/roundcube/postgres.py` & `batou_ext-2.4.8/src/batou_ext/roundcube/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/run.py` & `batou_ext-2.4.8/src/batou_ext/run.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/s3.py` & `batou_ext-2.4.8/src/batou_ext/s3.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/s3_bootstrap.py` & `batou_ext-2.4.8/src/batou_ext/s3_bootstrap.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/ssh.py` & `batou_ext-2.4.8/src/batou_ext/ssh.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/ssl.py` & `batou_ext-2.4.8/src/batou_ext/ssl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext/versions.py` & `batou_ext-2.4.8/src/batou_ext/versions.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.7/src/batou_ext.egg-info/PKG-INFO` & `batou_ext-2.4.8/src/batou_ext.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou_ext
-Version: 2.4.7
+Version: 2.4.8
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
@@ -66,14 +66,29 @@
 creating an [S3 bucket](https://wiki.flyingcircus.io/S3) and - if needed -
 an access keypair and lifecycle rules.
 
 On an activated virtualenv this can be tested with `python -m batou_ext.s3_bootstrap`.
 
 
 
+## 2.4.8 (2024-05-08)
+
+
+- systemd timers: add an option to enable persistence
+  breaking change: systemd timers are now non-persistent by default.
+  The previous default behaviour was a problem for cronjobs that should
+  not be started immediately following a reboot / downtime
+
+* Added a component `batou_ext.python.FixELFRunPath` which modifies `DT_RUNPATH` & `DT_RPATH` of `.so`-files in a venv to load the correct libraries (from either a Nix env or other Python libraries). Please read the docstring carefully before using it.
+
+- OCI: cache validation result during deployment.
+
+  Caching results speeds up deployments where multiple containers with the same image are deployed.
+
+
 ## 2.4.7 (2024-04-29)
 
 
 * Added component `batou_ext.http.HTTPServiceWatchdog` that adds a check to a systemd unit
   whether a given URL is reachable (e.g. a `/health` endpoint). If the URL cannot be reached within
   a certain interval, the service will be restarted. Further details are documented in the
   docstring.
```

### Comparing `batou_ext-2.4.7/src/batou_ext.egg-info/SOURCES.txt` & `batou_ext-2.4.8/src/batou_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*


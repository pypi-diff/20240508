# Comparing `tmp/py4web-1.20240428.2.tar.gz` & `tmp/py4web-1.20240507.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20240428.2.tar", last modified: Sun Apr 28 20:11:14 2024, max compression
+gzip compressed data, was "py4web-1.20240507.1.tar", last modified: Wed May  8 05:54:16 2024, max compression
```

## Comparing `py4web-1.20240428.2.tar` & `py4web-1.20240507.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 20:11:14.747056 py4web-1.20240428.2/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240428.2/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-28 20:11:14.747056 py4web-1.20240428.2/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-28 19:36:37.000000 py4web-1.20240428.2/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 20:11:14.710386 py4web-1.20240428.2/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      764 2024-04-28 19:45:42.000000 py4web-1.20240428.2/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 20:11:14.730388 py4web-1.20240428.2/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-04-28 20:11:06.000000 py4web-1.20240428.2/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-04-28 20:11:06.000000 py4web-1.20240428.2/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-04-28 20:11:06.000000 py4web-1.20240428.2/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-04-28 20:11:06.000000 py4web-1.20240428.2/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-04-28 20:11:06.000000 py4web-1.20240428.2/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392768 2024-04-28 20:11:07.000000 py4web-1.20240428.2/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68426 2024-04-28 19:44:28.000000 py4web-1.20240428.2/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 20:11:14.737055 py4web-1.20240428.2/py4web/utils/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240428.2/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72891 2024-04-28 20:10:23.000000 py4web-1.20240428.2/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 20:11:14.743722 py4web-1.20240428.2/py4web/utils/auth_plugins/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240428.2/py4web/utils/cors.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2102 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/downloader.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35880 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69730 2024-04-28 19:43:29.000000 py4web-1.20240428.2/py4web/utils/grid.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/mailer.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/misc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240428.2/py4web/utils/param.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/populate.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/publisher.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/recaptcha.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/security.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-28 19:36:37.000000 py4web-1.20240428.2/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 20:11:14.713720 py4web-1.20240428.2/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-28 20:11:14.000000 py4web-1.20240428.2/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-04-28 20:11:14.000000 py4web-1.20240428.2/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-28 20:11:14.000000 py4web-1.20240428.2/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-04-28 20:11:14.000000 py4web-1.20240428.2/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-04-28 20:11:14.000000 py4web-1.20240428.2/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-04-28 20:11:14.000000 py4web-1.20240428.2/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-04-28 19:45:29.000000 py4web-1.20240428.2/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-28 20:10:23.000000 py4web-1.20240428.2/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-04-28 20:11:14.747056 py4web-1.20240428.2/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 20:11:14.747056 py4web-1.20240428.2/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240428.2/tests/test_action.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8104 2024-04-28 20:10:23.000000 py4web-1.20240428.2/tests/test_auth.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_cache.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_fixture.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_json.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_main.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_session.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240428.2/tests/test_template.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240428.2/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.814381 py4web-1.20240507.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240507.1/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-08 05:54:16.814381 py4web-1.20240507.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-28 19:36:37.000000 py4web-1.20240507.1/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.771046 py4web-1.20240507.1/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      764 2024-05-08 05:52:53.000000 py4web-1.20240507.1/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.797714 py4web-1.20240507.1/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-08 05:54:09.000000 py4web-1.20240507.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392764 2024-05-08 05:54:09.000000 py4web-1.20240507.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68805 2024-05-08 05:51:19.000000 py4web-1.20240507.1/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.804381 py4web-1.20240507.1/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72777 2024-05-08 05:42:38.000000 py4web-1.20240507.1/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.811048 py4web-1.20240507.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240507.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35921 2024-05-02 06:57:14.000000 py4web-1.20240507.1/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69667 2024-05-02 06:57:02.000000 py4web-1.20240507.1/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.774379 py4web-1.20240507.1/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-05-08 05:52:21.000000 py4web-1.20240507.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-28 20:10:23.000000 py4web-1.20240507.1/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-08 05:54:16.814381 py4web-1.20240507.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.814381 py4web-1.20240507.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240507.1/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8104 2024-04-28 20:10:23.000000 py4web-1.20240507.1/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240507.1/tests/test_url.py
```

### Comparing `py4web-1.20240428.2/LICENSE.md` & `py4web-1.20240507.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/PKG-INFO` & `py4web-1.20240507.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240428.2
+Version: 1.20240507.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240428.2/README.rst` & `py4web-1.20240507.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/__init__.py` & `py4web-1.20240507.1/py4web/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20240428.2"
+__version__ = "1.20240507.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20240428.2/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240507.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/assets/py4web.app._default.zip` & `py4web-1.20240507.1/py4web/assets/py4web.app._default.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240507.1/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240507.1/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240507.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240507.1/py4web/assets/py4web.app.showcase.zip`

 * *Files 0% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1392768 bytes, number of entries: 143
+Zip file size: 1392764 bytes, number of entries: 143
 -rw-r--r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
 -rw-r--r--  3.0 unx     4206 tx defN 24-Apr-28 19:36 __init__.py
 -rw-r--r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
 -rwxr--r--  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
 -rw-r--r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
 -rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
 -rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
@@ -24,15 +24,15 @@
 -rw-r--r--  3.0 unx     4809 tx defN 23-May-08 00:39 examples/common.py
 -rw-r--r--  3.0 unx      171 tx defN 23-May-08 00:39 examples/page_with_template.py
 -rw-r--r--  3.0 unx      378 tx defN 23-May-08 00:39 examples/auth_form.py
 -rw-r--r--  3.0 unx      456 tx defN 23-May-08 00:39 examples/create_form.py
 -rw-r--r--  3.0 unx      272 tx defN 23-May-08 00:39 examples/ws.py
 -rw-r--r--  3.0 unx      255 tx defN 23-May-08 00:39 examples/show_a_button.py
 -rw-r--r--  3.0 unx      106 tx defN 23-May-08 00:39 examples/page_without_template.py
--rw-r--r--  3.0 unx     1470 tx defN 23-May-08 00:39 examples/settings.py
+-rw-r--r--  3.0 unx     1467 tx defN 24-May-08 05:06 examples/settings.py
 -rw-r--r--  3.0 unx      420 tx defN 23-May-08 00:39 examples/page_with_postback.py
 -rw-r--r--  3.0 unx      465 tx defN 23-May-08 00:39 examples/update_form.py
 -rw-r--r--  3.0 unx     1966 tx defN 23-May-08 00:39 examples/example_multiple_forms.py
 -rw-r--r--  3.0 unx      870 tx defN 23-May-08 00:39 examples/component_loader.py
 -rw-r--r--  3.0 unx      130 tx defN 23-May-08 00:39 examples/hello.py
 -rw-r--r--  3.0 unx      375 tx defN 23-May-08 00:39 examples/tagsinput_form.py
 -rw-r--r--  3.0 unx      236 tx defN 23-May-08 00:39 examples/example_helpers.py
@@ -138,8 +138,8 @@
 -rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/forms.html
 -rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/html_grid.html
 -rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/component_loader.html
 -rw-r--r--  3.0 unx      228 tx defN 23-May-08 00:39 templates/examples/generic.html
 -rw-r--r--  3.0 unx      193 tx defN 23-May-08 00:39 templates/examples/auth_form.html
 -rw-r--r--  3.0 unx     2778 tx defN 23-May-08 00:39 templates/layout.html
 -rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
-143 files, 9348902 bytes uncompressed, 1365612 bytes compressed:  85.4%
+143 files, 9348899 bytes uncompressed, 1365608 bytes compressed:  85.4%
```

#### examples/settings.py

```diff
@@ -5,15 +5,15 @@
 - i18n settings
 This file is provided as an example:
 """
 import os
 
 MODE = os.environ.get("PY4WEB_DASHBOARD_MODE", "none")
 # db settings
-APP_FOLDER = os.path.join(os.path.dirname(__file__), "..")
+APP_FOLDER = os.path.dirname(os.path.dirname(__file__))
 APP_NAME = os.path.split(APP_FOLDER)[-1]
 # DB_FOLDER:    Sets the place where migration files will be created
 #               and is the store location for SQLite databases
 DB_FOLDER = os.path.join(APP_FOLDER, "databases")
 DB_URI = "sqlite://storage.db"
 DB_POOL_SIZE = 1
 DB_MIGRATE = MODE == "full"
```

### Comparing `py4web-1.20240428.2/py4web/core.py` & `py4web-1.20240507.1/py4web/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -943,19 +943,26 @@
         def wrapper(*func_args, **func_kwargs):
             try:
                 request.app_name = app_name
                 ret = func(*func_args, **func_kwargs)
                 if isinstance(ret, (list, dict)):
                     response.headers["Content-Type"] = "application/json"
                     ret = dumps(ret)
+                elif ret is None:
+                    ret = ""
+                elif isinstance(ret, yatl.helpers.TAGGER):
+                    res = str(ret)
+                elif not hasattr(ret, "__iter__"):
+                    raise RuntimeError(f"Cannot return type {ret.__class__.__name__}")
                 return ret
             except HTTP as http:
                 response.status = http.status
                 response.headers.update(http.headers)
-                return http.body
+                body = http.body
+                return dumps(body) if isinstance(body, (list, dict)) else str(body)
             except bottle.HTTPResponse:
                 raise
             except Exception:
                 snapshot = get_error_snapshot()
                 logging.error(snapshot["traceback"])
                 ticket_uuid = error_logger.log(request.app_name, snapshot) or "unknown"
                 response.status = 500
```

### Comparing `py4web-1.20240428.2/py4web/server_adapters.py` & `py4web-1.20240507.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth.py` & `py4web-1.20240507.1/py4web/utils/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,23 +65,21 @@
         self.auth = auth
         self.condition = condition
 
     def on_success(self, context):
         self.auth.on_success(context)
 
     def abort_or_redirect(self, page, message=""):
-        """Return HTTP 403 if 'application/json' in HTTP_ACCEPT
-        and HTTP_JSON_REDIRECTS flag is not set in the request to 'on'.
-        Else redirects to page
+        """
+        Return HTTP 403 if 'text/htmp' not in HTTP_ACCEPT
+        else redirects to specified page
         """
 
-        if re.search(REGEX_APPJSON, request.headers.get("accept", "")) and (
-            request.headers.get("json-redirects", "") != "on"
-        ):
-            raise HTTP(403)
+        if "text/html" not in request.headers.get("accept", ""):
+            raise HTTP(403, body={"message": message})
         redirect_next = request.fullpath
         if request.query_string:
             redirect_next = redirect_next + "?{}".format(request.query_string)
         self.auth.flash.set(message)
         redirect(
             URL(
                 self.auth.route,
```

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240507.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/cors.py` & `py4web-1.20240507.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/dbstore.py` & `py4web-1.20240507.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/downloader.py` & `py4web-1.20240507.1/py4web/utils/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 
     except (AttributeError, KeyError):
         raise HTTP(404)
     try:
         (original_name, stream) = field.retrieve(filename, path, nameonly=True)
         fullpath = os.path.join(path, filename)
         if not os.path.exists(fullpath) and hasattr(stream, "read"):
-            with open(fullpath, "wb") as fp:
-                shutil.copyfile(fp, stream)
+            return stream.read()
     except NotAuthorizedException:
         raise HTTP(403)
     except NotFoundException:
         raise HTTP(404)
     except IOError:
         raise HTTP(404)
     if not request.query.get("attachment"):
```

### Comparing `py4web-1.20240428.2/py4web/utils/factories.py` & `py4web-1.20240507.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/form.py` & `py4web-1.20240507.1/py4web/utils/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -846,14 +846,15 @@
                             if value is not None:
                                 validated_vars[field.name] = value
                         self.accepted = True
                         self.vars.update(validated_vars)
                         if dbio:
                             self.update_or_insert(validated_vars)
                 elif dbio:
+                    self.accepted = True
                     self.deleted = True
                     self.record.delete_record()
             elif self.record:
                 # This form should not be processed.  We return the same as for GET.
                 self.vars = self._read_vars_from_record(table)
         if self.csrf_protection:
             self._sign_form()
```

### Comparing `py4web-1.20240428.2/py4web/utils/grid.py` & `py4web-1.20240507.1/py4web/utils/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,15 +757,14 @@
                 if self.param.edit_submit_value:
                     self.form.param.submit_value = self.param.edit_submit_value
 
             # redirect to the referrer
             if (
                 self.form.accepted
                 or (readonly and request.method == "POST")
-                or (self.form.deletable and self.form.deleted)
             ):
                 referrer = request.query.get("_referrer")
                 if referrer:
                     redirect(base64.b16decode(referrer.encode("utf8")).decode("utf8"))
                 else:
                     redirect(self.endpoint)
```

### Comparing `py4web-1.20240428.2/py4web/utils/jsonrpc.py` & `py4web-1.20240507.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/mailer.py` & `py4web-1.20240507.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/misc.py` & `py4web-1.20240507.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/populate.py` & `py4web-1.20240507.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/publisher.py` & `py4web-1.20240507.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/recaptcha.py` & `py4web-1.20240507.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/security.py` & `py4web-1.20240507.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web/utils/url_signer.py` & `py4web-1.20240507.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/py4web.egg-info/PKG-INFO` & `py4web-1.20240507.1/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240428.2
+Version: 1.20240507.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240428.2/py4web.egg-info/SOURCES.txt` & `py4web-1.20240507.1/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/pyproject.toml` & `py4web-1.20240507.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py4web"
-version = "1.20240428.2"
+version = "1.20240507.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20240428.2/tests/test_action.py` & `py4web-1.20240507.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_auth.py` & `py4web-1.20240507.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_cache.py` & `py4web-1.20240507.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_fixture.py` & `py4web-1.20240507.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_form.py` & `py4web-1.20240507.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_get_error_snapshot.py` & `py4web-1.20240507.1/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_json.py` & `py4web-1.20240507.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_main.py` & `py4web-1.20240507.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_session.py` & `py4web-1.20240507.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240428.2/tests/test_tags.py` & `py4web-1.20240507.1/tests/test_tags.py`

 * *Files identical despite different names*


# Comparing `tmp/pyslth-0.2.9.tar.gz` & `tmp/pyslth-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.2.9.tar", last modified: Wed May  8 08:47:03 2024, max compression
+gzip compressed data, was "pyslth-0.3.1.tar", last modified: Wed May  8 14:19:33 2024, max compression
```

## Comparing `pyslth-0.2.9.tar` & `pyslth-0.3.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.724033 pyslth-0.2.9/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.9/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 08:47:03.723832 pyslth-0.2.9/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.687834 pyslth-0.2.9/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.9/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-08 08:47:03.724099 pyslth-0.2.9/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-08 08:46:46.000000 pyslth-0.2.9/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.694731 pyslth-0.2.9/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-05-05 12:13:46.000000 pyslth-0.2.9/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     7036 2024-05-06 09:18:10.000000 pyslth-0.2.9/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.695345 pyslth-0.2.9/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.9/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.9/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    22579 2024-05-07 13:01:04.000000 pyslth-0.2.9/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.2.9/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    22178 2024-05-05 11:07:40.000000 pyslth-0.2.9/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.695661 pyslth-0.2.9/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.696332 pyslth-0.2.9/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.9/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.9/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.699267 pyslth-0.2.9/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.9/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.9/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6529 2024-05-06 02:38:49.000000 pyslth-0.2.9/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.9/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.2.9/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19474 2024-05-05 01:08:32.000000 pyslth-0.2.9/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.9/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.699744 pyslth-0.2.9/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.9/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.9/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14274 2024-05-05 11:25:25.000000 pyslth-0.2.9/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.700063 pyslth-0.2.9/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.701946 pyslth-0.2.9/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.9/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.706217 pyslth-0.2.9/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.9/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.9/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.9/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.9/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1670 2024-05-06 02:58:09.000000 pyslth-0.2.9/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.9/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.2.9/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.708573 pyslth-0.2.9/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.9/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.9/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.9/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.2.9/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.9/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.722880 pyslth-0.2.9/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-08 08:46:42.000000 pyslth-0.2.9/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.2.9/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-08 08:46:42.000000 pyslth-0.2.9/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)    90388 2024-05-08 08:46:42.000000 pyslth-0.2.9/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.723526 pyslth-0.2.9/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3138 2024-05-07 11:57:05.000000 pyslth-0.2.9/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.9/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.9/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.9/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.9/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.151298 pyslth-0.3.1/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.1/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 14:19:33.151091 pyslth-0.3.1/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.115587 pyslth-0.3.1/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 14:19:33.000000 pyslth-0.3.1/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-08 14:19:33.000000 pyslth-0.3.1/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-08 14:19:33.000000 pyslth-0.3.1/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-08 14:19:33.000000 pyslth-0.3.1/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-08 14:19:33.000000 pyslth-0.3.1/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.1/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-08 14:19:33.151358 pyslth-0.3.1/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-08 14:19:12.000000 pyslth-0.3.1/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.126194 pyslth-0.3.1/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-05-05 12:13:46.000000 pyslth-0.3.1/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     7036 2024-05-06 09:18:10.000000 pyslth-0.3.1/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.126769 pyslth-0.3.1/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.1/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.3.1/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    22625 2024-05-08 13:37:06.000000 pyslth-0.3.1/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.1/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.3.1/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    22178 2024-05-05 11:07:40.000000 pyslth-0.3.1/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.127177 pyslth-0.3.1/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.1/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.127876 pyslth-0.3.1/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.1/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.1/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.1/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.130844 pyslth-0.3.1/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.1/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.1/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.1/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.1/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.1/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.1/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6529 2024-05-06 02:38:49.000000 pyslth-0.3.1/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.3.1/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.1/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.3.1/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19474 2024-05-05 01:08:32.000000 pyslth-0.3.1/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.1/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.131361 pyslth-0.3.1/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.1/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.1/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14274 2024-05-05 11:25:25.000000 pyslth-0.3.1/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.131723 pyslth-0.3.1/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.133512 pyslth-0.3.1/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.1/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.137456 pyslth-0.3.1/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.1/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.1/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.1/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.1/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1670 2024-05-06 02:58:09.000000 pyslth-0.3.1/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.1/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.1/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.139765 pyslth-0.3.1/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.1/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.1/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.1/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.1/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.1/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.150221 pyslth-0.3.1/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-08 14:17:25.000000 pyslth-0.3.1/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.1/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117685 2024-05-08 13:45:30.000000 pyslth-0.3.1/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-08 14:17:25.000000 pyslth-0.3.1/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    91237 2024-05-08 14:17:25.000000 pyslth-0.3.1/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.3.1/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 14:19:33.150810 pyslth-0.3.1/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3138 2024-05-08 14:13:35.000000 pyslth-0.3.1/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.3.1/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.1/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.1/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.3.1/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.1/slth/views.py
```

### Comparing `pyslth-0.2.9/PKG-INFO` & `pyslth-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.9
+Version: 0.3.1
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.9/pyslth.egg-info/PKG-INFO` & `pyslth-0.3.1/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.9
+Version: 0.3.1
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.9/pyslth.egg-info/SOURCES.txt` & `pyslth-0.3.1/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/setup.py` & `pyslth-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.2.9',
+    version='0.3.1',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.2.9/slth/__init__.py` & `pyslth-0.3.1/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/components.py` & `pyslth-0.3.1/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/db/models.py` & `pyslth-0.3.1/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/endpoints.py` & `pyslth-0.3.1/slth/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,14 +402,17 @@
 class Icons(PublicEndpoint):
     class Meta:
         modal = True
         verbose_name = 'Icons'
 
     def get(self):
         return IconSet()
+    
+    def check_permission(self):
+        return settings.DEBUG
 
 
 class Search(Endpoint):
     def get(self):
         key = '_options_'
         options = self.cache.get(key, [])
         term = self.request.GET.get('term')
@@ -436,15 +439,15 @@
         modal = False
         verbose_name = 'Usuários'
 
     def get(self):
         return (
             super().get().search('username', 'email')
             .filters('is_superuser', 'is_active')
-            .fields('username', 'email', 'is_superuser', 'get_roles')
+            .fields('username', 'email', 'get_roles')
             .actions('add', 'view', 'edit', 'delete', 'sendpushnotification', 'changepassword')
         )
     
 class ChangePassword(ChildInstanceEndpoint):
     password = forms.CharField(label='Senha', required=False)
 
     class Meta:
@@ -565,15 +568,15 @@
 
     def get(self):
         return dict(
             {
                 "name": APPLICATON['title'],
                 "short_name": APPLICATON['title'],
                 "lang": 'pt-BR',
-                "start_url": build_url(self.request, "/app/dashboard/"),
+                "start_url": build_url(self.request, "/app/home/"),
                 "scope": build_url(self.request, "/app/"),
                 "display": "standalone",
                 "icons": [{
                     "src": build_url(self.request, APPLICATON['logo']),
                     "sizes": "192x192",
                     "type": "image/png"
                 }]
```

### Comparing `pyslth-0.2.9/slth/factory.py` & `pyslth-0.3.1/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/forms.py` & `pyslth-0.3.1/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/management/commands/integration_test.py` & `pyslth-0.3.1/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/management/commands/sync.py` & `pyslth-0.3.1/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/migrations/0001_initial.py` & `pyslth-0.3.1/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.3.1/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.3.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/migrations/0006_user.py` & `pyslth-0.3.1/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/models.py` & `pyslth-0.3.1/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/oauth.py` & `pyslth-0.3.1/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/permissions.py` & `pyslth-0.3.1/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/queryset.py` & `pyslth-0.3.1/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/roles.py` & `pyslth-0.3.1/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/selenium/__init__.py` & `pyslth-0.3.1/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/selenium/browser.py` & `pyslth-0.3.1/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/serializer.py` & `pyslth-0.3.1/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/.DS_Store` & `pyslth-0.3.1/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/fontawesome.min.css` & `pyslth-0.3.1/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/fonts/.DS_Store` & `pyslth-0.3.1/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.3.1/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.3.1/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.3.1/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.3.1/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/slth.css` & `pyslth-0.3.1/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/css/solid.min.css` & `pyslth-0.3.1/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/images/logo.png` & `pyslth-0.3.1/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/images/logo.svg` & `pyslth-0.3.1/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/images/user.png` & `pyslth-0.3.1/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/echarts.min.js` & `pyslth-0.3.1/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/index.min.js` & `pyslth-0.3.1/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/ios-splash.min.js` & `pyslth-0.3.1/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/peerjs.min.js` & `pyslth-0.3.1/slth/static/js/peerjs.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3322,10 +3322,8 @@
             n ? this._initialize(n) : this._api.retrieveId().then(e => this._initialize(e)).catch(e => this._abort(E.ServerError, e))
         }
     }
     e1.DEFAULT_KEY = "peerjs", window.peerjs = {
         Peer: e1,
         util: eM
     }, /** @deprecated Should use peerjs namespace */ window.Peer = e1
-})(); //# sourceMappingURL=peerjs.min.js.map
-
-//# sourceMappingURL=peerjs.min.js.map
+})(); //# sourceMappingURL=peerjs.min.js.map
```

### Comparing `pyslth-0.2.9/slth/static/js/qrcode.min.js` & `pyslth-0.3.1/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/react-trigger-change.js` & `pyslth-0.3.1/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/react.min.js` & `pyslth-0.3.1/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/slth.min.js` & `pyslth-0.3.1/slth/static/js/slth.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     j as t,
-    c as H,
+    c as F,
     r as I,
     R as Be
 } from "./react.min.js";
-const C = {
+const S = {
     colors: {
         primary: "var(--primary-color)",
         success: "var(--success-color)",
         warning: "var(--warning-color)",
         info: "var(--info-color)",
         danger: "var(--danger-color)",
         highlight: "var(--highlight-color)",
@@ -72,94 +72,94 @@
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function S(e) {
+function j(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
 
-function he(e) {
+function fe(e) {
     function n() {
         const a = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: e.display || "block"
         };
-        return e.primary && (a.backgroundColor = C.colors.primary, a.color = "white"), e.default && (a.color = C.colors.primary, a.border = "solid 1px " + C.colors.primary), t.jsx("a", {
+        return e.primary && (a.backgroundColor = S.colors.primary, a.color = "white"), e.default && (a.color = S.colors.primary, a.border = "solid 1px " + S.colors.primary), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(S, {
+            children: t.jsx(j, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
 const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
 function Re(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
-            backgroundColor: e.isError ? "#e52207" : C.colors.primary,
+            backgroundColor: e.isError ? "#e52207" : S.colors.primary,
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(S, {
+            children: [t.jsx(j, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
 function te(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(Re, {
+    a.classList.add("message"), F.createRoot(document.body.appendChild(a)).render(t.jsx(Re, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function xe() {
+function oe() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
-function oe(e) {
+function de(e) {
     function n() {
         const a = {
-            color: C.colors.info,
-            backgroundColor: C.background.info,
+            color: S.colors.info,
+            backgroundColor: S.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
@@ -171,65 +171,65 @@
             })]
         })
     }
     return n()
 }
 
 function Ne(e) {
-    return ve(e.data)
+    return pe(e.data)
 }
 
 function q(e) {
     return e.replace("/app/", "/api/")
 }
 
 function U(e) {
     return e.replace("/api/", "/app/")
 }
 
 function B(e, n, a, r) {
-    const d = localStorage.getItem("token");
+    const o = localStorage.getItem("token");
     var i = {
         Accept: "application/json"
     };
-    d && (i.Authorization = "Token " + d);
+    o && (i.Authorization = "Token " + o);
     const l = q(n);
     var s = {
         method: e,
         headers: new Headers(i),
         ajax: 1
     };
     r && (s.body = r);
     var c = null,
         u = null;
-    fetch(l, s).then(function(o) {
-        if (c = o, u = c.headers.get("Content-Type"), u == "application/json") return o.text();
-        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
-        o.text()
-    }).then(o => {
+    fetch(l, s).then(function(d) {
+        if (c = d, u = c.headers.get("Content-Type"), u == "application/json") return d.text();
+        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return d.arrayBuffer();
+        d.text()
+    }).then(d => {
         if (u == "application/json") {
-            var h = JSON.parse(o || "{}");
+            var h = JSON.parse(d || "{}");
             typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, c)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var f = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
+            var f = window.URL.createObjectURL(new Blob([new Uint8Array(d)], {
                     type: u
                 })),
                 w = document.createElement("a");
             w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, c)
-        } else a && a(o, c)
+        } else a && a(d, c)
     })
 }
 
-function ve(e) {
+function pe(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
     }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = U(e.redirect)) : e.message && te(e.message)
 }
 
-function z(e) {
+function H(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
         var n = e.toString().split(".");
         return n.length == 1 ? e.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".") : (n[0] = n[0].toString().replace(/\B(?=(\d{3})+(?!\d))/g, "."), n[1] = n[1].substring(0, 2), n[1].length == 1 && (n[1] = n[1] + "0"), n[0] + "," + n[1])
     }
@@ -250,50 +250,56 @@
     }
     return typeof e == "object" && e.type ? t.jsx(p, {
         data: e
     }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : t.jsx("ul", {
         style: {
             padding: 0
         },
-        children: e.map(function(d) {
+        children: e.map(function(o) {
             return t.jsx("li", {
-                children: d
+                children: o
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
-function pe() {
-    document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {}))
+function se() {
+    document.querySelector(".layer") == null && F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {}))
 }
 
 function be(e, n) {
-    xe(), pe(), window.reloader = n;
+    oe(), se(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
+    F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         url: q(e)
     }))
 }
 
 function Oe(e) {
-    xe(), pe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
+    oe(), se(), F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(He, {
         url: q(e)
     }))
 }
 
 function J(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
 function _e(e) {
+    oe(), se(), F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(We, {
+        actions: e
+    }))
+}
+
+function Fe(e) {
     const n = {
         backgroundColor: "black",
         bottom: 0,
         left: 0,
         position: "fixed",
         right: 0,
         top: 0,
@@ -305,23 +311,23 @@
         onClick: function() {
             J()
         },
         style: n
     })
 }
 
-function Fe(e) {
-    const [n, a] = I.useState(null), [r, d] = I.useState(0);
+function ze(e) {
+    const [n, a] = I.useState(null), [r, o] = I.useState(0);
     I.useEffect(() => {
         i(q(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function i(c) {
         B("GET", q(c), function(u) {
-            a(u), d(r + 1)
+            a(u), o(r + 1)
         })
     }
 
     function l() {
         const c = {
                 maxWidth: 800
             },
@@ -330,61 +336,63 @@
                 cursor: "pointer",
                 marginTop: -15
             };
         if (n) return t.jsxs("div", {
             style: c,
             children: [t.jsx("div", {
                 style: u,
-                children: t.jsx(S, {
+                children: t.jsx(j, {
                     icon: "x",
                     onClick: () => J()
                 })
             }), t.jsx(p, {
                 data: n
             })]
         })
     }
     const s = {
         minWidth: "50%",
         display: n ? "block" : "none",
-        maxWidth: "90%",
-        top: window.scrollY + 40
+        maxWidth: 800,
+        top: window.scrollY + 40,
+        border: 0
     };
     return t.jsx("dialog", {
         style: s,
         children: l()
     }, r)
 }
 
-function ze(e) {
+function He(e) {
     var n = Math.random();
     I.useEffect(() => {
         document.querySelector(".layer").style.display = "block";
         var r = document.getElementById(n);
         r.style.top = document.documentElement.scrollTop + 100
     }, []);
 
     function a() {
         const r = {
                 minWidth: "50%",
                 display: "block",
-                maxWidth: "90%",
-                top: window.scrollY + 40
+                maxWidth: 800,
+                top: window.scrollY + 40,
+                border: 0
             },
-            d = {
+            o = {
                 float: "right",
                 cursor: "pointer",
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
-                style: d,
-                children: t.jsx(S, {
+                style: o,
+                children: t.jsx(j, {
                     icon: "x",
                     onClick: () => J()
                 })
             }), t.jsx("iframe", {
                 src: q(e.url),
                 width: "100%",
                 height: 500,
@@ -393,31 +401,78 @@
                 }
             })]
         })
     }
     return a()
 }
 
+function We(e) {
+    const n = Math.random();
+    I.useEffect(() => {
+        document.querySelector(".layer").style.display = "block"
+    }, []);
+
+    function a() {
+        const i = {
+            width: "100%",
+            borderBottom: "solid 1px #DDDD",
+            padding: 20
+        };
+        return t.jsx("div", {
+            align: "center",
+            style: {},
+            children: e.actions.map(function(l) {
+                return t.jsx("div", {
+                    style: i,
+                    onClick: r,
+                    children: t.jsx(_, {
+                        data: l,
+                        strech: !0
+                    })
+                }, Math.random())
+            })
+        })
+    }
+
+    function r() {
+        const i = document.getElementById(n);
+        i.close(), i.classList.remove("opened"), i.remove(), document.querySelector(".layer").style.display = "none"
+    }
+    const o = {
+        width: "auto",
+        display: "block",
+        position: "fixed",
+        bottom: 0,
+        border: 0,
+        padding: 0
+    };
+    return t.jsx("dialog", {
+        id: n,
+        style: o,
+        children: a()
+    })
+}
+
 function T(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function _(e) {
     const n = e.id || Math.random(),
         [a, r] = I.useState(e.data.name);
 
-    function d(s) {
+    function o(s) {
         s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(U(e.data.url)) : be(e.data.url)
     }
 
     function i() {
-        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(S, {
+        return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(j, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(S, {
+            children: [t.jsx(j, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
@@ -425,20 +480,20 @@
     function l() {
         var s = {
             padding: 12,
             textDecoration: "none",
             borderRadius: 5,
             margin: 5
         };
-        return e.primary && (s.backgroundColor = C.colors.primary, s.color = "white"), e.default && (s.border = "solid 1px " + C.colors.primary, s.color = C.colors.primary), e.style && Object.keys(e.style).map(function(c) {
+        return e.primary && (s.backgroundColor = S.colors.primary, s.color = "white"), e.default && (s.border = "solid 1px " + S.colors.primary, s.color = S.colors.primary), e.style && Object.keys(e.style).map(function(c) {
             s[c] = e.style[c]
         }), t.jsx("a", {
             id: n,
             href: U(e.data.url) || "#",
-            onClick: d,
+            onClick: o,
             style: s,
             "data-label": T(e.data.name),
             children: i()
         })
     }
     return l()
 }
@@ -459,15 +514,15 @@
     }
 
     function r(i) {
         const l = n(i);
         l.style.display = "none"
     }
 
-    function d() {
+    function o() {
         const i = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
@@ -498,44 +553,44 @@
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
-    return d()
+    return o()
 }
 
 function N({
     id: e,
     href: n,
     modal: a,
     imodal: r,
-    children: d,
+    children: o,
     onClick: i,
     dataLabel: l,
     style: s
 }) {
     const c = n && n.indexOf("/media/") < 0 ? U(n) : n;
 
     function u(h) {
         c.indexOf("http") == 0 ? document.location.href = c : (h.preventDefault(), a ? be(c) : r ? Oe(c) : window.load(c))
     }
 
-    function o() {
+    function d() {
         return t.jsx("a", {
             id: e,
             onClick: i || u,
             href: c || "#",
             "data-label": T(l),
             style: s,
-            children: d
+            children: o
         })
     }
-    return o()
+    return d()
 }
 
 function G(e) {
     function n() {
         const r = {
             display: "grid",
             gridGap: 0,
@@ -548,36 +603,36 @@
         })
     }
     return n()
 }
 
 function Y(e) {
     function n() {
-        return e.data.url ? t.jsx(He, {
+        return e.data.url ? t.jsx(Pe, {
             data: e.data
         }) : t.jsx(we, {
             data: e.data
         })
     }
     return n()
 }
 
 function we(e) {
     function n() {
         return e.data.url ? t.jsx(N, {
             href: e.data.url,
             children: t.jsxs(t.Fragment, {
-                children: [z(e.data.value), t.jsx(S, {
+                children: [H(e.data.value), t.jsx(j, {
                     icon: "external-link",
                     style: {
                         marginLeft: 10
                     }
                 })]
             })
-        }) : z(e.data.value)
+        }) : H(e.data.value)
     }
 
     function a() {
         const r = {
             minWidth: e.width + "%",
             marginTop: 5,
             marginBottom: 5
@@ -588,26 +643,26 @@
                 children: e.data.label
             }), ":", t.jsx("br", {}), n()]
         })
     }
     return a()
 }
 
-function He(e) {
+function Pe(e) {
     const n = Math.random(),
         [a, r] = I.useState(e.data);
 
-    function d(l) {
+    function o(l) {
         B("GET", l, function(s) {
             r(s)
         })
     }
 
     function i() {
-        return window[n] = () => d(e.data.url), t.jsx("div", {
+        return window[n] = () => o(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
             children: t.jsx(we, {
                 data: a,
                 width: 100
             })
         })
@@ -653,15 +708,15 @@
                 })
             }, Math.random())
         })
     }
     return n()
 }
 
-function We(e) {
+function Ue(e) {
     function n() {
         const i = {
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsx("h3", {
             style: i,
@@ -677,29 +732,29 @@
 
     function r() {
         return t.jsx(je, {
             data: e.data.actions
         })
     }
 
-    function d() {
+    function o() {
         const i = {
             border: "solid 1px #DDD",
             padding: 10,
             borderStyle: "dashed"
         };
         return t.jsxs("div", {
             style: i,
             children: [n(), a(), r()]
         })
     }
-    return d()
+    return o()
 }
 
-function Pe(e) {
+function Ge(e) {
     function n() {
         const l = {
             paddingTop: 15,
             marginBottom: 10,
             color: "#1151b3"
         };
         return t.jsx("div", {
@@ -744,15 +799,15 @@
                 children: e.data.data[1].value
             }), t.jsx("div", {
                 style: c
             })]
         })
     }
 
-    function d() {
+    function o() {
         return t.jsx(je, {
             data: e.data.actions
         })
     }
 
     function i() {
         const l = {
@@ -766,26 +821,26 @@
             s = {
                 marginLeft: 20
             };
         return t.jsxs("div", {
             style: l,
             children: [r(), t.jsxs("div", {
                 style: s,
-                children: [n(), a(), d()]
+                children: [n(), a(), o()]
             })]
         })
     }
     return i()
 }
 
-function Ue(e) {
+function Ve(e) {
     const n = Math.random(),
         [a, r] = I.useState(e.data);
 
-    function d() {
+    function o() {
         return t.jsx(Se, {
             data: a
         })
     }
 
     function i() {
         const u = {
@@ -801,58 +856,58 @@
 
     function l() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
         }) : a.data.map(function(u) {
             return Array.isArray(u) ? t.jsx(G, {
                 width: 300,
-                children: u.map(o => t.jsx(Y, {
-                    data: o,
+                children: u.map(d => t.jsx(Y, {
+                    data: d,
                     width: 100 / u.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
                 children: t.jsx(Y, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
         }) : t.jsx(p, {
             data: a.data
         })
     }
 
     function s(u) {
-        B("GET", u, function(o) {
-            r(o)
+        B("GET", u, function(d) {
+            r(d)
         })
     }
 
     function c() {
         return e.data.url ? (window[n] = () => s(e.data.url), t.jsxs("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: [d(), i()]
+            children: [o(), i()]
         })) : t.jsxs("div", {
-            children: [d(), i()]
+            children: [o(), i()]
         })
     }
     return c()
 }
 
-function Ge(e) {
+function $e(e) {
     const n = Math.random(),
         [a, r] = I.useState(e.data.actions);
 
-    function d() {
+    function o() {
         const s = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + s + "only=actions"
     }
 
     function i() {
-        B("GET", d(), function(s) {
+        B("GET", o(), function(s) {
             r(s)
         })
     }
 
     function l() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
@@ -864,15 +919,15 @@
                 }, Math.random())
             })
         })
     }
     return l()
 }
 
-function Ve(e) {
+function Je(e) {
     function n() {
         const a = {
                 display: "flex",
                 justifyContent: "space-between",
                 alignItems: "baseline"
             },
             r = {
@@ -880,15 +935,15 @@
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h1", {
                 style: r,
                 "data-label": T(e.data.title),
                 children: e.data.title
-            }), t.jsx(Ge, {
+            }), t.jsx($e, {
                 data: e.data
             })]
         })
     }
     return n()
 }
 
@@ -906,63 +961,63 @@
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
                 "data-label": T(e.data.title),
                 children: e.data.title
             }), e.data.actions && e.data.actions.length > 0 && t.jsx("div", {
-                children: e.data.actions.map(function(d) {
+                children: e.data.actions.map(function(o) {
                     return t.jsx(_, {
-                        data: d,
+                        data: o,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
     return n()
 }
 
-function $e(e) {
+function Ye(e) {
     function n() {
-        return t.jsx(Ve, {
+        return t.jsx(Je, {
             data: e.data
         })
     }
 
     function a() {
-        return e.data.data.map(function(d, i) {
+        return e.data.data.map(function(o, i) {
             return t.jsx(p, {
-                data: d
+                data: o
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function Je(e) {
+function Qe(e) {
     function n() {
         return t.jsx(Se, {
             data: e.data
         })
     }
 
     function a() {
-        const d = {
+        const o = {
             backgroundColor: "white"
         };
         return e.data.data.map(function(i, l) {
             return t.jsx("div", {
-                style: d,
+                style: o,
                 children: t.jsx(p, {
                     data: i
                 }, Math.random())
             })
         })
     }
 
@@ -970,171 +1025,171 @@
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function Ye(e) {
+function Xe(e) {
     const [n, a] = I.useState(0);
 
     function r() {
         return t.jsx("div", {
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
-            children: e.data.map(function(d, i) {
+            children: e.data.map(function(o, i) {
                 return t.jsx(N, {
-                    href: d.url,
+                    href: o.url,
                     style: {
                         padding: 5,
                         fontWeight: n == i ? "bold" : "normal",
                         borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(l) {
-                        l.preventDefault(), a(i), e.loadContent(d.url)
+                        l.preventDefault(), a(i), e.loadContent(o.url)
                     },
-                    dataLabel: T(d.title),
-                    children: d.title
+                    dataLabel: T(o.title),
+                    children: o.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
-function Qe(e) {
+function Ke(e) {
     var n = Math.random();
     const [a, r] = I.useState(e.data.data[0]);
 
-    function d() {
+    function o() {
         return e.data.title != "Top" && t.jsx("h2", {
             "data-label": T(e.data.title),
             children: e.data.title
         })
     }
 
     function i() {
-        return t.jsx(Ye, {
+        return t.jsx(Xe, {
             data: e.data.data,
             loadContent: c
         })
     }
 
     function l() {
-        var o = {
+        var d = {
             ...a
         };
-        o.title = null;
+        d.title = null;
         const h = {
             padding: 0
         };
         return t.jsx("div", {
             style: h,
             children: t.jsx(p, {
-                data: o
+                data: d
             }, Math.random())
         })
     }
 
     function s() {
-        const o = {
+        const d = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: o
+            style: d
         })
     }
 
-    function c(o) {
-        B("GET", o, function(h) {
+    function c(d) {
+        B("GET", d, function(h) {
             r(h)
         })
     }
 
     function u() {
         return window[n] = () => c(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [d(), i(), l(), s()]
+            children: [o(), i(), l(), s()]
         })
     }
     return u()
 }
 
-function Xe() {
+function Ze() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
 function R({
     id: e,
     onClick: n,
     icon: a,
     label: r,
-    display: d,
+    display: o,
     primary: i,
     compact: l,
     spin: s
 }) {
     function c() {
-        return a ? l || !r ? t.jsx(S, {
+        return a ? l || !r ? t.jsx(j, {
             icon: a
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(Ae, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(S, {
+            }), t.jsx(j, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
-        const o = {
+        const d = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
-            display: d || "block",
+            display: o || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return i ? (o.backgroundColor = C.colors.primary, o.color = "white") : (o.border = "solid 1px " + C.colors.primary, o.color = C.colors.primary), t.jsx("a", {
+        return i ? (d.backgroundColor = S.colors.primary, d.color = "white") : (d.border = "solid 1px " + S.colors.primary, d.color = S.colors.primary), t.jsx("a", {
             id: e,
-            style: o,
+            style: d,
             "data-label": T(r || a),
             onClick: h => {
                 h.preventDefault(), a && s && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: c()
         })
     }
     return u()
 }
-const Ke = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
+const et = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
     Q = {
         padding: 15,
         border: "solid 1px #d9d9d9",
         borderRadius: 5
     };
 
 function ie(e) {
@@ -1144,118 +1199,118 @@
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
 function ee(e, n) {
     const a = e.closest("form"),
         r = new FormData(a),
-        d = n.indexOf("?") >= 0 ? "&" : "?";
-    n += d + new URLSearchParams(r).toString(), B("GET", n, Ce)
+        o = n.indexOf("?") >= 0 ? "&" : "?";
+    n += o + new URLSearchParams(r).toString(), B("GET", n, Ce)
 }
 
-function Ze(e) {
+function tt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
         a && (a.style.display = "none")
     }
 }
 
-function et(e) {
+function nt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "block");
         var a = document.querySelector(".form-group." + e);
         a && (a.style.display = "flex")
     }
 }
 
-function tt(e, n) {
+function at(e, n) {
     var a = document.querySelector(".form-group." + e),
         r = a.querySelector('*[name="' + e + '"]');
     if (r.tagName == "INPUT") r.value = n;
     else if (r.tagName == "SELECT") {
         if (r.style.display != "none") r.dispatchEvent(new CustomEvent("customchange", {
             detail: {
                 value: n
             }
         }));
         else
-            for (var d = 0; d < r.options.length; d++)
-                if (r.options[d].value == n) {
-                    r.selectedIndex = d;
+            for (var o = 0; o < r.options.length; o++)
+                if (r.options[o].value == n) {
+                    r.selectedIndex = o;
                     break
                 }
     }
 }
 
 function Ce(e) {
     if (e) {
-        for (var n = 0; n < e.hide.length; n++) Ze(e.hide[n]);
-        for (var n = 0; n < e.show.length; n++) et(e.show[n]);
-        for (var a in e.set) tt(a, e.set[a])
+        for (var n = 0; n < e.hide.length; n++) tt(e.hide[n]);
+        for (var n = 0; n < e.show.length; n++) nt(e.show[n]);
+        for (var a in e.set) at(a, e.set[a])
     }
 }
 
-function nt(e) {
+function rt(e) {
     function n() {
         const a = {
-            color: C.colors.info,
-            backgroundColor: C.background.info,
+            color: S.colors.info,
+            backgroundColor: S.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(S, {
+                children: [t.jsx(j, {
                     icon: "circle-check",
                     style: {
-                        color: C.colors.info,
+                        color: S.colors.info,
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function at(e) {
+function it(e) {
     function n() {
         const a = {
             color: "white",
             display: "none",
             backgroundColor: "#e52207",
             marginTop: 2,
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
             className: "error",
-            children: [t.jsx(S, {
+            children: [t.jsx(j, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
     return n()
 }
 
-function rt(e) {
+function lt(e) {
     function n() {
         const a = {
             marginTop: 2,
             marginBottom: 2,
             fontStyle: "italic"
         };
         return t.jsx("div", {
@@ -1288,77 +1343,77 @@
                     padding: 0
                 }
             })]
         })
     }
 
     function r() {
-        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Ke.indexOf(e.data.type) >= 0 ? t.jsx(me, {
+        return e.data.type == "datetime" && (e.data.type = "datetime-local"), et.indexOf(e.data.type) >= 0 ? t.jsx(ge, {
             data: e.data
-        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(fe, {
+        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ye, {
             data: e.data
         }) : t.jsx(le, {
             data: e.data
-        }) : t.jsx(ot, {
+        }) : t.jsx(st, {
             data: e.data
-        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(fe, {
+        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ye, {
             data: e.data
         }) : t.jsx(le, {
             data: e.data
         }) : t.jsx(Te, {
             data: e.data
-        }) : e.data.type == "decimal" ? t.jsx(me, {
+        }) : e.data.type == "decimal" ? t.jsx(ge, {
             data: e.data
-        }) : e.data.type == "boolean" ? t.jsx(lt, {
+        }) : e.data.type == "boolean" ? t.jsx(dt, {
             data: e.data
-        }) : e.data.type == "textarea" ? t.jsx(it, {
+        }) : e.data.type == "textarea" ? t.jsx(ot, {
             data: e.data
         }) : t.jsx("span", {
             children: e.data.name
         })
     }
 
-    function d() {
+    function o() {
         return t.jsx("div", {
-            children: t.jsx(at, {
+            children: t.jsx(it, {
                 id: e.data.name + "_error"
             })
         })
     }
 
     function i() {
-        return e.data.help_text && t.jsx(rt, {
+        return e.data.help_text && t.jsx(lt, {
             text: e.data.help_text
         })
     }
 
     function l() {
         const s = {
             display: e.data.type == "hidden" ? "none" : "flex",
             flexDirection: "column",
             padding: 5,
             width: "calc(100%-5px)"
         };
         return t.jsxs("div", {
             id: n,
             style: s,
-            children: [a(), r(), i(), d()]
+            children: [a(), r(), i(), o()]
         })
     }
     return l()
 }
 
-function me(e) {
+function ge(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), I.useEffect(() => {
-        function l(u, o, h) {
+        function l(u, d, h) {
             var f = h.target,
                 w = f.value.replace(/\D/g, ""),
-                M = f.value.length > o ? 1 : 0;
+                M = f.value.length > d ? 1 : 0;
             VMasker(f).unMask(), VMasker(f).maskPattern(u[M]), f.value = VMasker.toPattern(w, u[M])
         }
         if (e.data.mask) {
             var s = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(s).maskMoney({
                 precision: 2,
                 separator: ",",
@@ -1371,36 +1426,36 @@
         }
     }, []);
 
     function r(l) {
         ee(l.target, e.data.onchange)
     }
 
-    function d(l) {
+    function o(l) {
         if (e.data.type == "file" && l.target.files) {
             let c = l.target.files[0];
             var s = new FileReader;
             s.onload = function(u) {
                 if (ie(c.name)) {
                     const w = "display" + a;
-                    var o = document.createElement("img");
-                    o.id = l.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(M) {
-                        const D = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
+                    var d = document.createElement("img");
+                    d.id = l.target.id + "img", d.style.width = "200px", d.style.display = "block", d.style.margin = "auto", d.style.marginTop = "20px", d.onload = function(M) {
+                        const D = e.data.width > e.data.height ? e.data.width / d.width : e.data.height / d.height;
                         var y = document.createElement("canvas");
-                        const j = y.getContext("2d");
-                        y.height = y.width * (o.height / o.width);
+                        const k = y.getContext("2d");
+                        y.height = y.width * (d.height / d.width);
                         const x = document.createElement("canvas"),
                             L = x.getContext("2d");
-                        x.width = o.width * D, x.height = o.height * D, L.drawImage(o, 0, 0, x.width, x.height), j.drawImage(x, 0, 0, x.width * D, x.height * D, 0, 0, y.width, y.height), x.toBlob(function(m) {
+                        x.width = d.width * D, x.height = d.height * D, L.drawImage(d, 0, 0, x.width, x.height), k.drawImage(x, 0, 0, x.width * D, x.height * D, 0, 0, y.width, y.height), x.toBlob(function(m) {
                             const v = new DataTransfer;
                             v.items.add(new File([m], c.name)), l.target.files = v.files
                         });
                         var b = document.getElementById(w);
-                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), l.target.parentNode.appendChild(b)
-                    }, o.src = u.target.result
+                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(d), l.target.parentNode.appendChild(b)
+                    }, d.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
                 var f = c.size / 1024;
                 f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = c.name + " / " + f, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
             }, s.readAsDataURL(c)
         }
     }
@@ -1412,31 +1467,31 @@
                 alignContent: "center",
                 minHeight: 75,
                 padding: 5,
                 maxWidth: "100%",
                 margin: "auto"
             };
             var s = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (s = e.data.extensions.map(o => "." + o).join(", ")), t.jsxs(t.Fragment, {
+            return e.data.extensions && e.data.extensions.length > 0 && (s = e.data.extensions.map(d => "." + d).join(", ")), t.jsxs(t.Fragment, {
                 children: [t.jsxs("div", {
                     style: {
                         display: window.innerWidth < 800 ? "block" : "flex",
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10,
                         textAlign: "center"
                     },
                     children: [t.jsx("div", {
                         style: u,
-                        children: t.jsx(S, {
+                        children: t.jsx(j, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
-                                color: C.colors.primary
+                                color: S.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
                         children: [e.data.value && ie(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
@@ -1449,15 +1504,15 @@
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
-                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(o => "." + o).join(" ou "), "."]
+                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(d => "." + d).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
                         children: t.jsx(R, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
@@ -1467,15 +1522,15 @@
                     className: "form-control " + n,
                     type: l,
                     name: e.data.name,
                     id: a,
                     "data-label": T(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
-                    onChange: d,
+                    onChange: o,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
                     accept: s
                 })]
             })
@@ -1488,15 +1543,15 @@
                 type: l,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
                 "data-label": T(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
-                onChange: d,
+                onChange: o,
                 style: c
             })
         }
     }
     return i()
 }
 
@@ -1509,70 +1564,70 @@
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
-        d = Array.isArray(e.data.value),
+        o = Array.isArray(e.data.value),
         [i, l] = I.useState(!1),
         [s, c] = I.useState(null);
     var u = !1;
-    let o;
+    let d;
     I.useEffect(() => {
-        j(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
-            j(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+        k(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
+            k(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function h() {
         const b = document.getElementById(a);
-        if (d) {
+        if (o) {
             const m = {
                     padding: 5,
                     display: "inline"
                 },
                 v = {
                     cursor: "pointer",
                     marginRight: 5
                 },
                 g = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [b == null && n.map((k, E) => t.jsxs("div", {
+                children: [b == null && n.map((C, E) => t.jsxs("div", {
                     style: m,
                     children: [t.jsx("span", {
                         onClick: () => x(E),
                         style: v,
-                        children: t.jsx(S, {
+                        children: t.jsx(j, {
                             icon: "trash-can",
                             style: g
                         })
-                    }), k.value]
-                }, Math.random())), b != null && Array.from(b.options).map((k, E) => t.jsxs("div", {
+                    }), C.value]
+                }, Math.random())), b != null && Array.from(b.options).map((C, E) => t.jsxs("div", {
                     style: m,
                     children: [t.jsx("span", {
                         onClick: () => x(E),
                         style: v,
-                        children: t.jsx(S, {
+                        children: t.jsx(j, {
                             icon: "trash-can",
                             style: g
                         })
-                    }), k.innerHTML]
+                    }), C.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
     function f() {
         return t.jsx("select", {
             id: a,
             name: e.data.name,
-            multiple: d,
+            multiple: o,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
@@ -1590,34 +1645,34 @@
                 maxHeight: 150,
                 overflowY: "auto"
             };
         m.position = "absolute", m.backgroundColor = "white";
         const v = document.getElementById(r);
         if (e.data.icon && (b.paddingLeft = 30), v) {
             let A = null,
-                F = v,
+                z = v,
                 V = null;
-            for (; !V && (F = F.parentElement) instanceof HTMLElement;) F.matches("dialog") && (V = F);
+            for (; !V && (z = z.parentElement) instanceof HTMLElement;) z.matches("dialog") && (V = z);
             A = V;
             const P = v.getBoundingClientRect();
             var g = P.top + P.height,
-                k = P.left;
+                C = P.left;
             if (A) {
                 const $ = A.getBoundingClientRect();
-                g = g - $.top, k = k - $.left
-            } else g += window.scrollY, k += window.scrollX;
-            m.width = P.width, m.top = g, m.left = k
+                g = g - $.top, C = C - $.left
+            } else g += window.scrollY, C += window.scrollX;
+            m.width = P.width, m.top = g, m.left = C
         }
         const E = {
                 cursor: "pointer",
                 padding: 10
             },
-            ae = !d && n.length > 0 && n[0].value || "";
+            ae = !o && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
-            children: [e.data.icon && t.jsx(S, {
+            children: [e.data.icon && t.jsx(j, {
                 icon: e.data.icon,
                 style: {
                     position: "absolute",
                     margin: 13,
                     color: "#d9d9d9"
                 }
             }), t.jsx("input", {
@@ -1641,15 +1696,15 @@
                     u = !0
                 },
                 children: [s.length == 0 && t.jsx("li", {
                     style: E,
                     children: "Nenhuma opção encontrada."
                 }), s.map(A => t.jsx("li", {
                     onClick: () => {
-                        l(!1), e.onSelect ? e.onSelect(A) : j(A)
+                        l(!1), e.onSelect ? e.onSelect(A) : k(A)
                     },
                     style: E,
                     className: "autocomplete-item",
                     "data-label": T(A.value),
                     children: A.value
                 }, Math.random()))]
             })]
@@ -1662,31 +1717,31 @@
         }, 250)
     }
 
     function D(b) {
         const m = document.getElementById(a);
         if (m) {
             const v = document.getElementById(r);
-            d || m.options.length > 0 && v.value != m.options[0].innerHTML && (m.innerHTML = "", v.value = "", l(!1), e.data.onchange && ee(v, e.data.onchange)), b.target.tagName == "UL" ? l(!1) : u || l(!1)
+            o || m.options.length > 0 && v.value != m.options[0].innerHTML && (m.innerHTML = "", v.value = "", l(!1), e.data.onchange && ee(v, e.data.onchange)), b.target.tagName == "UL" ? l(!1) : u || l(!1)
         }
     }
 
     function y(b) {
-        clearTimeout(o), o = setTimeout(function() {
+        clearTimeout(d), d = setTimeout(function() {
             const m = e.data.choices.indexOf("?") < 0 ? "?" : "&";
             l(!0), B("GET", e.data.choices + m + "term=" + b.target.value, function(g) {
                 c(g)
             })
         }, 1e3)
     }
 
-    function j(b, m = !1) {
+    function k(b, m = !1) {
         const v = document.getElementById(a),
             g = document.getElementById(r);
-        v.innerHTML == null && (v.innerHTML = ""), Array.isArray(b) ? v.innerHTML = b.map(k => `<option selected value="${k.id}">${k.value}</option>`).join("") : d ? (v.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, g.value = "") : (v.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, g.value = b.value), e.data.onchange && !m && ee(g, e.data.onchange)
+        v.innerHTML == null && (v.innerHTML = ""), Array.isArray(b) ? v.innerHTML = b.map(C => `<option selected value="${C.id}">${C.value}</option>`).join("") : o ? (v.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, g.value = "") : (v.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, g.value = b.value), e.data.onchange && !m && ee(g, e.data.onchange)
     }
 
     function x(b) {
         const m = document.getElementById(a);
         var v = Array.from(m.options);
         m.innerHTML = v.slice(0, b).concat(v.slice(b + 1)).map(g => `<option selected value="${g.value}">${g.innerHTML}</option>`).join(""), c([])
     }
@@ -1695,15 +1750,15 @@
         return t.jsxs(t.Fragment, {
             children: [h(), f(), w()]
         })
     }
     return L()
 }
 
-function it(e) {
+function ot(e) {
     function n() {
         var a = {
             ...Q
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
@@ -1712,15 +1767,15 @@
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
 
-function lt(e) {
+function dt(e) {
     var n = e.data;
     return n.choices = [{
         id: !0,
         value: "Sim"
     }, {
         id: !1,
         value: "Não"
@@ -1733,15 +1788,15 @@
     var n = Math.random(),
         a = e.data;
 
     function r(s) {
         return a.value != null ? a.value == s.id ? !0 : a.value.id == s.id : !1
     }
 
-    function d(s) {
+    function o(s) {
         var c = document.getElementById(s);
         a.checked && (c.checked = !1), e.data.onchange && ee(c, e.data.onchange)
     }
 
     function i(s) {
         var c = document.getElementById(s);
         a.checked = c.checked
@@ -1760,15 +1815,15 @@
                     id: a.name + n + c,
                     type: "radio",
                     name: a.name,
                     defaultValue: s.id,
                     defaultChecked: r(s),
                     "data-label": T(s.value),
                     onClick: function() {
-                        d(a.name + n + c)
+                        o(a.name + n + c)
                     },
                     onMouseEnter: function() {
                         i(a.name + n + c)
                     }
                 }), t.jsx("label", {
                     htmlFor: a.name + n + c,
                     children: s.value
@@ -1777,29 +1832,29 @@
         }) : t.jsx("i", {
             children: "Nenhuma opção disponível para seleção."
         })
     }
     return l()
 }
 
-function fe(e) {
+function ye(e) {
     var n = Math.random(),
         a = e.data;
 
     function r(i) {
         var l = !1;
         if (a.value)
             for (var s = 0; s < a.value.length; s++) {
                 var c = a.value[s];
                 (c == i.id || c.id == i.id) && (l = !0)
             }
         return l
     }
 
-    function d() {
+    function o() {
         return a.choices.length > 0 ? t.jsx("div", {
             className: "checkbox-group",
             children: a.choices.map((i, l) => t.jsxs("div", {
                 style: {
                     paddingTop: 10,
                     display: "inline-block",
                     marginRight: 25
@@ -1816,18 +1871,18 @@
                     children: i.value
                 })]
             }, n + l))
         }) : t.jsx("i", {
             children: "Nenhuma opção disponível para seleção."
         })
     }
-    return d()
+    return o()
 }
 
-function ot(e) {
+function st(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
             "data-label": T(n.label),
@@ -1837,23 +1892,23 @@
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
     })
 }
 
-function dt(e) {
+function ct(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
-    function d() {
+    function o() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
-            children: t.jsxs(oe, {
+            children: t.jsxs(de, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => i(!0),
@@ -1868,30 +1923,30 @@
                 })]
             })
         })
     }
 
     function i(c) {
         const u = document.querySelector("input[name=" + r.name + "]"),
-            o = document.getElementById("inline-form-" + n),
+            d = document.getElementById("inline-form-" + n),
             h = document.getElementById("show-" + n),
             f = document.getElementById("hide-" + n);
-        o.style.display = c ? "block" : "none", h.style.display = c ? "none" : "inline", f.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+        d.style.display = c ? "block" : "none", h.style.display = c ? "none" : "inline", f.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
     function l() {
         const c = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (c.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
             className: "fieldset-inline-forms",
             style: c,
             id: "inline-form-" + n,
             children: e.data.value.map(function(u) {
-                return t.jsx(de, {
+                return t.jsx(ce, {
                     data: u
                 }, Math.random())
             })
         })
     }
 
     function s() {
@@ -1900,34 +1955,34 @@
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: c,
                 "data-label": T(e.data.label),
                 children: e.data.label
-            }), d(), l()]
+            }), o(), l()]
         })
     }
     return s()
 }
 
-function st(e) {
+function ut(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
-    function r(o, h) {
+    function r(d, h) {
         const f = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
             id: "form-" + f + "-" + a,
-            children: [t.jsx(de, {
-                data: o
+            children: [t.jsx(ce, {
+                data: d
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
                 children: [t.jsx(R, {
@@ -1942,58 +1997,58 @@
                     onClick: () => l(f),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
-    function d() {
-        const o = s(),
-            h = o.length > 0 ? "none" : "inline";
+    function o() {
+        const d = s(),
+            h = d.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = h;
         for (var f = 0; f < n; f++) {
             var w = document.getElementById("extra-add-" + f + "-");
             w.style.display = "none"
         }
-        if (o.length > 0) {
-            var w = document.getElementById("extra-add-" + o[o.length - 1] + "-");
+        if (d.length > 0) {
+            var w = document.getElementById("extra-add-" + d[d.length - 1] + "-");
             w.style.display = "inline"
         }
     }
 
     function i() {
-        d();
-        var o = JSON.parse(JSON.stringify(e.data.template));
-        o.fields ? (o.fields.map(function(h) {
+        o();
+        var d = JSON.parse(JSON.stringify(e.data.template));
+        d.fields ? (d.fields.map(function(h) {
             h.name = h.name.replace("__n__", "__" + n + "__")
-        }), o.fields[0].value = 0) : o.fieldsets.map(function(h) {
+        }), d.fields[0].value = 0) : d.fieldsets.map(function(h) {
             h.fields.map(function(f) {
                 f.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
                 }), f[0].value = 0
             })
-        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(d, 100)
+        }), F.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(d, "inline")), setTimeout(o, 100)
     }
 
-    function l(o) {
+    function l(d) {
         const h = e.data.template,
-            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
+            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + d + "__"),
             M = document.querySelector("input[name=" + w + "]");
-        parseInt(M.value) == 0 ? M.value = "" : M.value = -parseInt(M.value), document.getElementById("form-" + o + "-" + a).style.display = "none", d()
+        parseInt(M.value) == 0 ? M.value = "" : M.value = -parseInt(M.value), document.getElementById("form-" + d + "-" + a).style.display = "none", o()
     }
 
     function s() {
-        for (var o = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && o.push(h);
-        return o
+        for (var d = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && d.push(h);
+        return d
     }
 
     function c() {
         return t.jsx("div", {
             id: "info-" + a,
-            children: t.jsx(oe, {
+            children: t.jsx(de, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
                 children: t.jsx(R, {
                     primary: !0,
                     icon: "add",
                     onClick: () => i(),
@@ -2001,21 +2056,21 @@
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
         })
     }
 
     function u() {
-        const o = {
+        const d = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: o,
+                style: d,
                 "data-label": T(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
@@ -2024,23 +2079,23 @@
                 })]
             })]
         })
     }
     return u()
 }
 
-function de(e) {
+function ce(e) {
     I.useEffect(() => {
-        e.data.controls && (console.log(e.data.controls), Ce(e.data.controls))
+        e.data.controls && Ce(e.data.controls)
     }, []);
 
     function n(r) {
-        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(dt, {
+        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(ct, {
             data: r
-        }, Math.random()) : t.jsx(st, {
+        }, Math.random()) : t.jsx(ut, {
             data: r
         }, Math.random()) : t.jsx(K, {
             data: r
         }, Math.random())
     }
 
     function a() {
@@ -2052,65 +2107,65 @@
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
                     "data-label": T(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
-                }), r.fields.map(d => t.jsx("div", {
-                    children: d.map(i => t.jsx("div", {
+                }), r.fields.map(o => t.jsx("div", {
+                    children: o.map(i => t.jsx("div", {
                         className: "form-group " + i.name,
                         style: {
-                            width: 100 / d.length + "%",
+                            width: 100 / o.length + "%",
                             display: i.type == "hidden" ? "none" : "inline-block"
                         },
                         children: n(i)
                     }, Math.random()))
                 }, Math.random()))]
             })
         }, Math.random()))
     }
     return a()
 }
 
-function ct(e) {
+function ht(e) {
     const n = Math.random();
 
     function a() {
         const h = {
             margin: 0
         };
         return t.jsx("h1", {
             style: h,
             children: e.data.title
         })
     }
 
     function r() {
-        return e.data.info && t.jsx(nt, {
+        return e.data.info && t.jsx(rt, {
             data: {
                 text: e.data.info
             }
         })
     }
 
-    function d() {
+    function o() {
         if (e.data.display) return t.jsxs(t.Fragment, {
             children: [e.data.display.map(h => t.jsx(p, {
                 data: h
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
     }
 
     function i() {
-        return t.jsx(de, {
+        return t.jsx(ce, {
             data: e.data
         })
     }
 
     function l() {
         return t.jsxs("div", {
             style: {
@@ -2119,15 +2174,15 @@
             },
             children: [t.jsx(R, {
                 onClick: u,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
             }), t.jsx(R, {
-                onClick: o,
+                onClick: d,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
@@ -2151,58 +2206,58 @@
             method: e.data.method,
             children: [t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 style: {
                     padding: 5
                 },
-                children: [a(), r(), d(), i(), l(), s()]
+                children: [a(), r(), o(), i(), l(), s()]
             })]
         })
     }
 
     function u() {
         J()
     }
 
-    function o(h) {
+    function d(h) {
         h.preventDefault();
         var f = e.data.url,
             w = document.getElementById(n),
             M = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
             const D = f.indexOf("?") >= 0 ? "&" : "?";
             f = f + D + "form=" + e.data.title + "&" + new URLSearchParams(M).toString(), M = null
         }
         B(w.method.toUpperCase(), f, function(y) {
-            if (w.querySelectorAll(".error").forEach(x => x.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), y.type == "response") return J(), Xe(), ve(y);
+            if (w.querySelectorAll(".error").forEach(x => x.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), y.type == "response") return J(), Ze(), pe(y);
             if (y.type == "error") {
-                var j = y.text;
+                var k = y.text;
                 console.log(y), Object.keys(y.errors).map(function(x) {
-                    if (x == "__all__") j = y.errors[x];
+                    if (x == "__all__") k = y.errors[x];
                     else {
                         const L = w.querySelector("#" + x + "_error");
                         L.querySelector("span").innerHTML = y.errors[x], L.style.display = "block"
                     }
-                }), te(j, !0)
+                }), te(k, !0)
             } else {
                 const x = document.querySelector("#output");
-                x.innerHTML = "", H.createRoot(x.appendChild(document.createElement("div"))).render(t.jsx(p, {
+                x.innerHTML = "", F.createRoot(x.appendChild(document.createElement("div"))).render(t.jsx(p, {
                     data: y
                 }))
             }
         }, M)
     }
     return c()
 }
 
-function ut(e) {
+function mt(e) {
     function n() {
         const a = {
-            backgroundColor: C.colors.primary,
+            backgroundColor: S.colors.primary,
             color: "white",
             borderRadius: "50%",
             minWidth: 13,
             marginLeft: 2,
             padding: 4,
             fontSize: "70%",
             display: "inline-block",
@@ -2214,15 +2269,15 @@
             style: a,
             children: e.total
         })
     }
     return n()
 }
 
-function ht(e) {
+function ft(e) {
     e.data.id == null && (e.data.id = Math.random());
     const [n, a] = I.useState(e.data);
 
     function r() {
         const m = {
             margin: 0
         };
@@ -2233,15 +2288,15 @@
         }) : t.jsx("h1", {
             style: m,
             "data-label": T(n.title),
             children: n.title
         })
     }
 
-    function d() {
+    function o() {
         const m = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "center"
         };
         return t.jsxs("div", {
             style: m,
@@ -2277,63 +2332,63 @@
                         paddingLeft: 15,
                         paddingRight: 15,
                         fontWeight: g ? "bold" : "normal",
                         borderBottom: g ? "solid 3px #2670e8" : 0,
                         textDecoration: "none",
                         color: "#0c326f"
                     },
-                    onClick: function(k) {
-                        k.preventDefault(), s(m.name)
+                    onClick: function(C) {
+                        C.preventDefault(), s(m.name)
                     },
                     dataLabel: T(m.label),
-                    children: [m.label, " ", t.jsx(ut, {
+                    children: [m.label, " ", t.jsx(mt, {
                         total: m.count
                     })]
                 }, Math.random())
             })
         })
     }
 
     function s(m) {
         const v = document.getElementById("subset-" + e.data.id);
         v.value = m || "", x()
     }
 
     function c(m, v, g) {
-        const k = document.getElementById("form-" + e.data.id);
-        k.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", k.querySelector("input[name=" + n.calendar.field + "__month]").value = v || "", k.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", x()
+        const C = document.getElementById("form-" + e.data.id);
+        C.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", C.querySelector("input[name=" + n.calendar.field + "__month]").value = v || "", C.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", x()
     }
 
     function u() {
         if (n.calendar) {
             const E = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
                 ae = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
                 A = {
                     width: "100%",
                     borderSpacing: 0,
                     borderCollapse: "collapse",
                     marginTop: 15,
                     marginBottom: 15
                 },
-                F = {
+                z = {
                     marginLeft: "17",
                     textAlign: "right",
                     paddingRight: 2,
                     paddingTop: 2,
                     float: "right",
                     fontSize: "0.8rem"
                 },
                 V = {
                     verticalAlign: "top",
                     width: "14.2%",
                     height: 55,
                     border: "solid 1px #EEE"
                 },
                 P = {
-                    backgroundColor: C.colors.primary,
+                    backgroundColor: S.colors.primary,
                     borderRadius: "50%",
                     color: "white",
                     display: "block",
                     width: 30,
                     height: 30,
                     margin: "auto",
                     cursor: "pointer",
@@ -2345,62 +2400,62 @@
                 },
                 Ee = {
                     display: "flex",
                     justifyContent: "space-between",
                     alignItems: "baseline"
                 },
                 Ie = new Date,
-                ue = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
+                me = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
             for (var m = [
                     [],
                     [],
                     [],
                     [],
                     [],
                     []
                 ], v = n.calendar.month - 1, g = new Date(n.calendar.year, n.calendar.month - 1, 1); g.getDay() > 1;) g.setDate(g.getDate() - 1);
-            for (var k = 0;
-                (g.getMonth() <= v || m[k].length < 7) && (m[k].length == 7 && (k += 1), k != 5);) m[k].push({
+            for (var C = 0;
+                (g.getMonth() <= v || m[C].length < 7) && (m[C].length == 7 && (C += 1), C != 5);) m[C].push({
                 date: g.getDate(),
                 total: n.calendar.total[g.toLocaleDateString("pt-BR")],
                 today: g.getDate() === Ie.getDate(),
-                selected: ue ? g.getDate() == ue.getDate() : !1
+                selected: me ? g.getDate() == me.getDate() : !1
             }), g.setDate(g.getDate() + 1);
             return t.jsxs("div", {
                 className: "calendar",
                 children: [t.jsxs("div", {
                     style: Ee,
                     children: [t.jsx("div", {
-                        children: t.jsx(he, {
+                        children: t.jsx(fe, {
                             default: !0,
                             icon: "arrow-left",
                             onClick: () => c(null, n.calendar.previous.month, n.calendar.previous.year)
                         })
                     }), t.jsxs("div", {
                         children: [t.jsxs("h3", {
                             align: "center",
                             style: {
                                 margin: 0
                             },
                             children: [ae[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
-                            className: F,
-                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(S, {
+                            className: z,
+                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(j, {
                                 default: !0,
                                 icon: "x",
                                 onClick: () => c(null, n.calendar.month, n.calendar.year),
                                 style: {
                                     marginLeft: 10,
                                     cursor: "pointer"
                                 }
                             })]
                         })]
                     }), t.jsx("div", {
-                        children: t.jsx(he, {
+                        children: t.jsx(fe, {
                             default: !0,
                             icon: "arrow-right",
                             onClick: () => c(null, n.calendar.next.month, n.calendar.next.year)
                         })
                     })]
                 }), t.jsxs("table", {
                     style: A,
@@ -2411,15 +2466,15 @@
                             }, Math.random()))
                         })
                     }), t.jsx("tbody", {
                         children: m.map(re => t.jsx("tr", {
                             children: re.map(O => t.jsxs("td", {
                                 style: V,
                                 children: [t.jsx("div", {
-                                    style: F,
+                                    style: z,
                                     children: O.today ? t.jsx("span", {
                                         style: {
                                             textDecoration: "underline"
                                         },
                                         children: O.date
                                     }) : O.date + O.today
                                 }), O.total && t.jsx("div", {
@@ -2442,20 +2497,20 @@
                         }, Math.random()))
                     })]
                 })]
             })
         }
     }
 
-    function o(m) {
+    function d(m) {
         const v = {
             textAlign: "left",
             verticalAlign: "top",
             lineHeight: "3rem",
-            color: C.colors.primary,
+            color: S.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
             children: [m.map(function(g) {
                 return g.label != "ID" && t.jsx("th", {
                     style: v,
                     className: "bold",
@@ -2483,38 +2538,39 @@
                 children: m.title
             }, Math.random()), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: m.actions.map(function(k) {
-                        return t.jsx(_, {
-                            data: k,
-                            default: !0,
-                            compact: !0
-                        }, Math.random())
+                    children: t.jsx(j, {
+                        icon: "chevron-right",
+                        onClick: () => _e(m.actions),
+                        style: {
+                            cursor: "pointer",
+                            marginRight: 20
+                        }
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [m.data.map(function(k) {
-                return k.label != "ID" && t.jsx("td", {
+            children: [m.data.map(function(C) {
+                return C.label != "ID" && t.jsx("td", {
                     style: v,
-                    children: z(k.value)
+                    children: H(C.value)
                 }, Math.random())
             }), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: m.actions.map(function(k) {
+                    children: m.actions.map(function(C) {
                         return t.jsx(_, {
-                            data: k,
+                            data: C,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
@@ -2526,15 +2582,15 @@
                 marginBottom: 15
             },
             children: n.data.map(function(m) {
                 return m.type = n.renderer, t.jsx(p, {
                     data: m
                 }, Math.random())
             })
-        }) : w() : t.jsx(oe, {
+        }) : w() : t.jsx(de, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
@@ -2548,15 +2604,15 @@
                 borderSpacing: 0
             };
         return t.jsx("div", {
             style: m,
             children: t.jsxs("table", {
                 style: v,
                 children: [t.jsx("thead", {
-                    children: o(n.data[0].data)
+                    children: d(n.data[0].data)
                 }), t.jsx("tbody", {
                     children: n.data.map(function(g) {
                         return h(g)
                     })
                 })]
             })
         })
@@ -2579,29 +2635,29 @@
                 lineHeight: "4rem",
                 alignItems: "baseline"
             },
             g = {
                 display: "inline",
                 paddingRight: 10
             },
-            k = {
+            C = {
                 marginLeft: 10,
                 marginRight: 10,
                 height: "2.5rem",
                 paddingLeft: 5,
                 paddingRight: 5,
                 textAlign: "center"
             };
         return n.pagination.page.total > 1 && t.jsxs("div", {
             style: v,
             children: [t.jsxs("div", {
                 children: [t.jsxs("div", {
                     style: g,
                     children: ["Exibir", t.jsx("select", {
-                        style: k,
+                        style: C,
                         name: "page_size",
                         onChange: () => M(1),
                         value: n.pagination.page.size,
                         children: n.pagination.page.sizes.map(function(E) {
                             return t.jsx("option", {
                                 children: E
                             }, Math.random())
@@ -2664,38 +2720,38 @@
                     data: m,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
-    function j() {
+    function k() {
         const m = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
             v = n.search.length > 0,
             g = n.filters.length > 0;
         if ((n.bi || n.data.length >= 0) && (v || g)) {
-            const k = {
+            const C = {
                 name: "q",
                 value: "",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves"
             };
             return t.jsxs("div", {
                 style: m,
                 children: [t.jsxs(G, {
                     width: 250,
                     children: [v && t.jsx("div", {
                         children: t.jsx(K, {
-                            data: k
+                            data: C
                         })
                     }), g && n.filters.map(function(E) {
                         return E.type != "hidden" && t.jsx("div", {
                             children: t.jsx(K, {
                                 data: E
                             })
                         }, Math.random())
@@ -2725,29 +2781,29 @@
         e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + v : m = e.data.url + "?" + v, B("GET", m, function(g) {
             a(g), i(!1)
         })
     }
 
     function L() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [j(), n.bi.map(function(m) {
+            children: [k(), n.bi.map(function(m) {
                 return t.jsx(G, {
                     width: 300,
                     alignItems: "start",
                     children: m.map(function(v) {
                         return t.jsx("div", {
                             children: t.jsx(p, {
                                 data: v
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [y(), l(), j(), u(), f(), D()]
+            children: [y(), l(), k(), u(), f(), D()]
         })
     }
 
     function b() {
         window[e.data.id] = () => x();
         const m = {
             backgroundColor: "white",
@@ -2761,55 +2817,55 @@
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), d(), L()]
+                }), o(), L()]
             })
         })
     }
     return b()
 }
 
 function ne(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
         if (r) {
-            var d = echarts.init(r);
-            d.setOption(e.option)
+            var o = echarts.init(r);
+            o.setOption(e.option)
         } else setTimeout(a, 1e3)
     }
     return setTimeout(a, 1e3), t.jsx("div", {
         id: n,
         style: {
             width: "100%",
             height: 300
         }
     })
 }
 
-function se(e) {
+function ue(e) {
     var n = [
         ["70%", "78%"],
         ["60%", "68%"],
         ["50%", "58%"],
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
         ["10%", "18%"]
     ];
 
     function a() {
-        return e.headers ? e.headers.slice(1).map(function(d, i) {
+        return e.headers ? e.headers.slice(1).map(function(o, i) {
             return {
-                name: d,
+                name: o,
                 type: "pie",
                 radius: n[i],
                 emphasis: {
                     label: {
                         show: !0,
                         formatter: function(l) {
                             return l.value.toLocaleString("pt-BR")
@@ -2828,32 +2884,32 @@
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
             emphasis: {
                 label: {
                     show: !0,
-                    formatter: function(d) {
-                        return d.value.toLocaleString("pt-BR")
+                    formatter: function(o) {
+                        return o.value.toLocaleString("pt-BR")
                     },
                     fontWeight: "bold"
                 }
             },
             roseType: e.area ? "area" : null,
-            data: e.rows.map(function(d, i) {
+            data: e.rows.map(function(o, i) {
                 return {
-                    name: d[0],
-                    value: d[1]
+                    name: o[0],
+                    value: o[1]
                 }
             })
         }
     }
 
     function r() {
-        var d = {
+        var o = {
             tooltip: {
                 trigger: "item",
                 formatter: function(i) {
                     return `${i.name}: <b>${i.data.value.toLocaleString("pt-BR")}</b> (${i.percent.toLocaleString("pt-BR")}%)`
                 }
             },
             legend: {},
@@ -2862,41 +2918,41 @@
                 formatter(i) {
                     return i.name + " (" + i.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
         return t.jsx(ne, {
-            option: d
+            option: o
         })
     }
     return r()
 }
 
-function mt(e) {
-    return t.jsx(se, {
+function gt(e) {
+    return t.jsx(ue, {
         donut: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function ft(e) {
-    return t.jsx(se, {
+function yt(e) {
+    return t.jsx(ue, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function W(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
-        d = {
+        o = {
             type: "value"
         },
         i = {
             show: !0,
             feature: {
                 mark: {
                     show: !0
@@ -2910,42 +2966,42 @@
 
     function s() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
-            data: e.rows.map(function(o) {
-                return o[0]
+            data: e.rows.map(function(d) {
+                return d[0]
             })
         }
     }
 
     function c() {
-        return e.headers ? e.rows.map(function(o) {
+        return e.headers ? e.rows.map(function(d) {
             return {
-                name: o[0],
-                data: o.slice(1),
+                name: d[0],
+                data: d.slice(1),
                 type: a,
                 stack: r,
                 areaStyle: l
             }
         }) : [{
             name: null,
-            data: e.rows.map(function(o) {
-                return o[1]
+            data: e.rows.map(function(d) {
+                return d[1]
             }),
             type: a,
             stack: r,
             areaStyle: l
         }]
     }
 
     function u() {
-        var o = {
+        var d = {
             toolbox: i,
             tooltip: {
                 trigger: "axis",
                 axisPointer: {
                     type: "shadow"
                 },
                 formatter: function(h) {
@@ -2955,88 +3011,88 @@
             legend: {},
             label: {
                 show: !0,
                 formatter: function(h) {
                     return h.value.toLocaleString("pt-BR")
                 }
             },
-            xAxis: n ? d : s(),
-            yAxis: n ? s() : d,
+            xAxis: n ? o : s(),
+            yAxis: n ? s() : o,
             series: c()
         };
         return t.jsx(ne, {
-            option: o
+            option: d
         })
     }
     return u()
 }
 
-function gt(e) {
+function xt(e) {
     return t.jsx(W, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function yt(e) {
+function vt(e) {
     return t.jsx(W, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function xt(e) {
+function pt(e) {
     return t.jsx(W, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function vt(e) {
+function bt(e) {
     return t.jsx(W, {
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function pt(e) {
+function wt(e) {
     return t.jsx(W, {
         invert: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function bt(e) {
+function jt(e) {
     return t.jsx(W, {
         invert: !0,
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function wt(e) {
+function kt(e) {
     function n() {
         return e.headers ? [{
             type: "treemap",
             roam: "move",
             nodeClick: !0,
-            data: e.headers.slice(1).map(function(r, d) {
+            data: e.headers.slice(1).map(function(r, o) {
                 return {
                     name: r,
                     type: "pie",
                     children: e.rows.map(function(i) {
                         return {
                             name: i[0],
-                            value: i[d + 1]
+                            value: i[o + 1]
                         }
                     })
                 }
             })
         }] : [{
             type: "treemap",
             roam: "move",
@@ -3054,28 +3110,28 @@
         var r = {
             tooltip: {
                 trigger: "item"
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(d) {
-                    return d.name + " (" + d.value.toLocaleString("pt-BR") + ")"
+                formatter(o) {
+                    return o.name + " (" + o.value.toLocaleString("pt-BR") + ")"
                 }
             },
             series: n()
         };
         return t.jsx(ne, {
             option: r
         })
     }
     return a()
 }
 
-function jt(e) {
+function St(e) {
     function n() {
         var a = {
             series: [{
                 type: "gauge",
                 startAngle: 0,
                 endAngle: 360,
                 min: 0,
@@ -3116,69 +3172,69 @@
         return t.jsx(ne, {
             option: a
         })
     }
     return n()
 }
 
-function ge(e) {
+function xe(e) {
     function n() {
         switch (e.type) {
             case "pie":
-                return t.jsx(se, {
+                return t.jsx(ue, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "polar":
-                return t.jsx(ft, {
+                return t.jsx(yt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "donut":
-                return t.jsx(mt, {
+                return t.jsx(gt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "bar":
-                return t.jsx(gt, {
+                return t.jsx(xt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_bar":
-                return t.jsx(vt, {
+                return t.jsx(bt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "column":
-                return t.jsx(pt, {
+                return t.jsx(wt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_column":
-                return t.jsx(bt, {
+                return t.jsx(jt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "tree_map":
-                return t.jsx(wt, {
+                return t.jsx(kt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "line":
-                return t.jsx(yt, {
+                return t.jsx(vt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "area":
-                return t.jsx(xt, {
+                return t.jsx(pt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "progress":
-                return t.jsx(jt, {
+                return t.jsx(St, {
                     headers: e.headers,
                     rows: e.rows
                 });
             default:
                 return t.jsx(W, {
                     headers: e.headers,
                     rows: e.rows
@@ -3197,18 +3253,18 @@
                 children: e.title
             }), n()]
         })
     }
     return a()
 }
 
-function kt(e) {
+function Ct(e) {
     function n() {
-        for (var r = [], d = 0; d < e.data.series.length; d++) r.push([e.data.series[d][0], e.data.series[d][1]]);
-        return e.data.chart ? t.jsx(ge, {
+        for (var r = [], o = 0; o < e.data.series.length; o++) r.push([e.data.series[o][0], e.data.series[o][1]]);
+        return e.data.chart ? t.jsx(xe, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
                 "data-label": T(e.data.title),
@@ -3222,36 +3278,36 @@
                         children: i.map((l, s) => s == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left",
                                 lineHeight: "2rem"
                             },
                             children: l
                         }, Math.random()) : t.jsx("td", {
-                            children: z(l)
+                            children: H(l)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], d = [], i = Object.keys(e.data.series), l = [], s = 0; s < i.length; s++) {
+        for (var r = [], o = [], i = Object.keys(e.data.series), l = [], s = 0; s < i.length; s++) {
             s == 0 && r.push("");
-            for (var c = [i[s]], u = 0, o = 0; o < e.data.series[i[s]].length; o++) {
+            for (var c = [i[s]], u = 0, d = 0; d < e.data.series[i[s]].length; d++) {
                 var h = e.data.series[i[s]];
-                s == 0 && r.push(h[o][0]), c.push(h[o][1]), u += h[o][1], i.length > 1 && (s == 0 ? l.push(h[o][1]) : l[o] += h[o][1], o > 0 && o == e.data.series[i[s]].length - 1 && (s == 0 ? l.push(u) : l[o + 1] += u))
+                s == 0 && r.push(h[d][0]), c.push(h[d][1]), u += h[d][1], i.length > 1 && (s == 0 ? l.push(h[d][1]) : l[d] += h[d][1], d > 0 && d == e.data.series[i[s]].length - 1 && (s == 0 ? l.push(u) : l[d + 1] += u))
             }
-            c.length > 2 && (s == 0 && r.push("TOTAL"), c.push(u)), d.push(c)
+            c.length > 2 && (s == 0 && r.push("TOTAL"), c.push(u)), o.push(c)
         }
-        return e.data.chart ? t.jsx(ge, {
+        return e.data.chart ? t.jsx(xe, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
-            rows: d
+            rows: o
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
                 "data-label": T(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
@@ -3260,50 +3316,50 @@
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: r.map(f => t.jsx("th", {
                             children: f
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [d.map(f => t.jsx("tr", {
+                    children: [o.map(f => t.jsx("tr", {
                         children: f.map((w, M) => M == 0 ? t.jsx("th", {
                             children: w
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
                             style: {
                                 backgroundColor: M == f.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
                             },
-                            children: z(w)
+                            children: H(w)
                         }, Math.random()))
                     }, Math.random())), l.length > 0 && t.jsxs("tr", {
                         children: [t.jsx("th", {
                             children: "TOTAL"
                         }), l.map(f => t.jsxs("td", {
                             align: "center",
                             style: {
                                 backgroundColor: "var(--info-color)"
                             },
-                            children: [z(f), " "]
+                            children: [H(f), " "]
                         }, Math.random()))]
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
 }
 
-function St() {
+function Tt() {
     function e() {
         const i = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover",
-            backgroundColor: C.colors.primary
+            backgroundColor: S.colors.primary
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: i
@@ -3321,18 +3377,18 @@
         })
     }
 
     function n(i) {
         var l = i.target;
         const s = l.querySelector(":scope > ul, :scope > li");
         if (s) {
-            s.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(o) {
-                o.style.display = "block"
-            }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(o) {
-                o.style.display = "none"
+            s.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(d) {
+                d.style.display = "block"
+            }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(d) {
+                d.style.display = "none"
             });
             const c = l.querySelector(":scope > i.fa-solid.fa-chevron-right"),
                 u = l.querySelector(":scope > i.fa-solid.fa-chevron-up");
             return c && (c.classList.remove("fa-chevron-right"), c.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), i.preventDefault(), i.stopPropagation(), i.cancelBubble = !0, !1
         } else {
             const c = document.querySelector("aside");
             c.style.display = window.innerWidth < 800 ? "none" : "block"
@@ -3343,42 +3399,42 @@
         const s = {
                 display: l == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 5,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
-                color: C.colors.primary
+                color: S.colors.primary
             },
             c = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return i.url ? t.jsx("li", {
             style: s,
             onClick: n,
             children: t.jsxs(N, {
                 href: i.url,
                 dataLabel: T(i.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [l == 0 && t.jsx(S, {
+                children: [l == 0 && t.jsx(j, {
                     icon: i.icon || "dot-circle",
                     style: c
                 }), i.label]
             })
         }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: s,
             "data-label": T(i.label),
-            children: [l == 0 && t.jsx(S, {
+            children: [l == 0 && t.jsx(j, {
                 icon: i.icon || "dot-circle",
                 style: c
-            }), i.label, t.jsx(S, {
+            }), i.label, t.jsx(j, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
@@ -3400,37 +3456,37 @@
             style: i,
             children: window.application.menu.items.map(function(l) {
                 return a(l, 0)
             })
         })
     }
 
-    function d() {
+    function o() {
         const i = {
             padding: 25,
             height: "100%",
             borderRight: "solid 1px #EEE"
         };
         return t.jsxs("div", {
             style: i,
             children: [e(), r()]
         })
     }
-    return d()
+    return o()
 }
 
-function Ct(e) {
+function Mt(e) {
     var n;
 
     function a(i) {
         const l = "=".repeat((4 - i.length % 4) % 4),
             s = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
             c = window.atob(s),
             u = new Uint8Array(c.length);
-        for (let o = 0; o < c.length; ++o) u[o] = c.charCodeAt(o);
+        for (let d = 0; d < c.length; ++d) u[d] = c.charCodeAt(d);
         return u
     }
 
     function r() {
         "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(i) {
             if (i) {
                 const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
@@ -3453,36 +3509,36 @@
                 })
             } else console.log("No registered service worker.")
         }).catch(function(i) {
             alert("Erro"), console.error("Service Worker Error", i)
         }) : alert("Push messaging is not supported")
     }
 
-    function d() {
-        if (Notification.permission !== "granted") return t.jsx(S, {
+    function o() {
+        if (Notification.permission !== "granted") return t.jsx(j, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer",
-                color: C.colors.primary
+                color: S.colors.primary
             }
         })
     }
-    return d()
+    return o()
 }
 
-function Tt(e) {
+function Et(e) {
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
-                backgroundColor: C.colors.primary,
+                backgroundColor: S.colors.primary,
                 color: "white",
                 right: 10,
                 borderRadius: "50%",
                 cursor: "pointer"
             },
             r = {
                 paddingLeft: 14,
@@ -3492,74 +3548,74 @@
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 80
                 },
                 onClick: () => history.back(),
-                children: t.jsx(S, {
+                children: t.jsx(j, {
                     icon: "arrow-left",
                     style: r
                 })
             }), t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 20
                 },
                 onClick: () => window.scrollTo(0, 0),
-                children: t.jsx(S, {
+                children: t.jsx(j, {
                     icon: "arrow-up",
                     style: r
                 })
             })]
         })
     }
     return n()
 }
 
-function Mt(e) {
+function It(e) {
     const [n, a] = I.useState(e.data);
-    window.loaddata = d => a(d);
+    window.loaddata = o => a(o);
 
     function r() {
-        const d = {
+        const o = {
             minHeight: 400,
             margin: 20
         };
         return t.jsx("div", {
-            style: d,
+            style: o,
             id: "container",
             children: t.jsx(p, {
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
-function Et(e) {
+function Bt(e) {
     I.useEffect(() => {
-        const o = localStorage.getItem("message");
-        o && (localStorage.removeItem("message"), te(o)), window.addEventListener("resize", () => {
+        const d = localStorage.getItem("message");
+        d && (localStorage.removeItem("message"), te(d)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
         })
     }, []);
 
     function a() {
-        const o = document.querySelector("aside");
-        o.style.display = o.style.display == "none" ? "block" : "none"
+        const d = document.querySelector("aside");
+        d.style.display = d.style.display == "none" ? "block" : "none"
     }
 
-    function r(o) {
-        o.preventDefault(), window.load(o.target.href)
+    function r(d) {
+        d.preventDefault(), window.load(d.target.href)
     }
 
-    function d() {
-        const o = {
+    function o() {
+        const d = {
                 display: "flex",
                 width: "100%",
                 justifyContent: "space-between",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 overflowX: "hidden"
             },
             h = {
@@ -3569,20 +3625,20 @@
                 mask: null,
                 name: "search",
                 required: !1,
                 type: "choice",
                 icon: "search"
             };
         return e.data.navbar ? t.jsxs("div", {
-            style: o,
+            style: d,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [e.data.menu && t.jsx(S, {
+                children: [e.data.menu && t.jsx(j, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -3615,24 +3671,24 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(S, {
+                        children: t.jsx(j, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(Ct, {})
-                }), e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(f) {
+                    children: t.jsx(Mt, {})
+                }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(f) {
                     return f.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
                         children: t.jsx(_, {
                             data: f,
                             primary: !0
                         }, Math.random())
                     })
                 }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(f) {
@@ -3644,54 +3700,54 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(S, {
+                        children: t.jsx(j, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
-                        children: t.jsx(S, {
+                        children: t.jsx(j, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
                     children: t.jsx(Te, {
                         data: h,
                         style: {
                             padding: 10
                         },
                         onSelect: f => document.location.href = U(f.id)
                     })
-                }), e.data.navbar.usermenu.length > 0 && t.jsx("div", {
+                }), e.data.navbar.user && e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.usermenu,
                         position: {},
                         dataLabel: T(e.data.navbar.user),
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
                                 height: 30,
                                 borderRadius: "50%",
                                 objectFit: "cover",
-                                backgroundColor: C.colors.primary
+                                backgroundColor: S.colors.primary
                             }
                         })
                     })
                 })]
             })]
         }) : null
     }
@@ -3700,51 +3756,51 @@
         return window.application.menu && window.application.menu.items.length > 0 && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
-            children: t.jsx(St, {})
+            children: t.jsx(Tt, {})
         })
     }
 
     function l() {
-        const o = {
+        const d = {
                 margin: 15
             },
             h = {
-                color: C.colors.primary
+                color: S.colors.primary
             };
         return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
-            style: o,
+            style: d,
             children: [t.jsx(N, {
                 href: "/app/dashboard/",
                 style: {
                     marginRight: 10
                 },
-                children: t.jsx(S, {
+                children: t.jsx(j, {
                     icon: "home",
                     style: h
                 })
             }), "Área Administrativa"]
         })
     }
 
     function s() {
         return t.jsxs("main", {
             style: {
                 flexGrow: 6,
                 minWidth: "400px"
             },
-            children: [l(), t.jsx(Mt, {
+            children: [l(), t.jsx(It, {
                 data: e.data.content
             }), t.jsx("footer", {
                 children: c()
-            }), t.jsx(Tt, {})]
+            }), t.jsx(Et, {})]
         })
     }
 
     function c() {
         return e.data.footer ? t.jsxs("div", {
             align: "center",
             children: [t.jsx("div", {
@@ -3754,15 +3810,15 @@
             })]
         }) : null
     }
 
     function u() {
         return t.jsxs("div", {
             children: [t.jsx("header", {
-                children: d()
+                children: o()
             }), t.jsxs("div", {
                 style: {
                     overflowX: "hide",
                     width: "100%",
                     display: "flex",
                     overflow: "hidden",
                     minHeight: window.innerHeight - 70
@@ -3770,19 +3826,19 @@
                 children: [i(), s()]
             })]
         })
     }
     return u()
 }
 
-function It(e) {
+function Dt(e) {
     var n = null,
         a = null,
         r = null,
-        d = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
+        o = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
         i = {
             constraints: {
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
@@ -3790,94 +3846,94 @@
             },
             sdpTransform: y => y.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
     I.useEffect(() => {
         n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(y) {
             document.getElementById("callerid").innerHTML = e.data.caller
         }), n.on("call", function(y) {
-            d({
+            o({
                 video: {
                     width: {
                         exact: 320
                     },
                     height: {
                         exact: 240
                     }
                 },
                 audio: !0
-            }, function(j) {
-                a = j;
+            }, function(k) {
+                a = k;
                 var x = document.getElementById("video2");
                 x.addEventListener("loadedmetadata", function(L) {
                     x.style.width = this.videoWidth / 4 + "px", x.style.height = this.videoHeight / 4 + "px", x.style.marginLeft = -this.videoWidth / 4 + "px", x.style.visibility = "visible"
-                }, !1), x.srcObject = a, y.answer(j), y.on("stream", function(L) {
+                }, !1), x.srcObject = a, y.answer(k), y.on("stream", function(L) {
                     r = L, document.getElementById("video1").srcObject = r
                 }), y.on("close", function() {
                     c()
                 }), n.on("error", function(L) {
                     c()
                 })
-            }, function(j) {
-                console.log("Failed to get local stream", j)
+            }, function(k) {
+                console.log("Failed to get local stream", k)
             })
         }), n.on("error", function(y) {
             y.type == "browser-incompatible" ? alert("Navegador incompatível.") : y.type == "invalid-id" ? alert("Usuário inexistente.") : y.type == "network" ? alert("Problema na conexão do usuário.") : y.type == "peer-unavailable" && alert("Usuário indisponível.")
         })
     }, []);
 
     function l() {
-        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video")
+        d(a, "audio"), d(a, "video"), d(r, "audio"), d(r, "video")
     }
 
     function s() {
         h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video")
     }
 
     function c() {
         u(a, "audio"), u(a, "video"), u(r, "audio"), u(r, "video"), a = null, r = null, document.getElementById("video1").srcObject = null, document.getElementById("video2").srcObject = null, console.log("Stopped!")
     }
 
-    function u(y, j) {
+    function u(y, k) {
         y != null && y.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === j && x.stop()
+            x.readyState == "live" && x.kind === k && x.stop()
         })
     }
 
-    function o(y, j) {
+    function d(y, k) {
         y != null && y.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === j && (x.enabled = !1)
+            x.readyState == "live" && x.kind === k && (x.enabled = !1)
         })
     }
 
-    function h(y, j) {
+    function h(y, k) {
         y != null && y.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === j && (x.enabled = !0)
+            x.readyState == "live" && x.kind === k && (x.enabled = !0)
         })
     }
 
     function f() {
         var y = document.getElementById("video1");
         y.style.width == "" ? y.style.width = "400px" : y.style.width = ""
     }
 
     function w() {
         var y = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, i);
-        y.on("stream", function(j) {
-            r = j, document.getElementById("video1").srcObject = r
+        y.on("stream", function(k) {
+            r = k, document.getElementById("video1").srcObject = r
         }), y.on("close", function() {
             c()
-        }), n.on("error", function(j) {
+        }), n.on("error", function(k) {
             c()
         })
     }
 
     function M() {
         if (a != null && r == null) return w();
         if (a != null && r != null) return s();
-        d({
+        o({
             video: {
                 width: {
                     exact: 320
                 },
                 height: {
                     exact: 240
                 }
@@ -3890,29 +3946,29 @@
                 noiseSuppression: !1,
                 sampleRate: 48e3,
                 sampleSize: 16,
                 volume: 1
             }
         }, function(y) {
             a = y;
-            var j = document.getElementById("video2");
-            j.addEventListener("loadedmetadata", function(x) {
-                j.style.width = this.videoWidth / 4 + "px", j.style.height = this.videoHeight / 4 + "px", j.style.marginLeft = -this.videoWidth / 4 + "px", j.style.visibility = "visible"
-            }, !1), j.srcObject = a, w()
+            var k = document.getElementById("video2");
+            k.addEventListener("loadedmetadata", function(x) {
+                k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
+            }, !1), k.srcObject = a, w()
         }, function(y) {
             alert("Failed to get local stream.")
         })
     }
 
     function D() {
         var y = {
                 width: "fit-content",
                 margin: "auto"
             },
-            j = {
+            k = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
             x = {
                 color: "white",
                 backgroundColor: "black",
@@ -3929,60 +3985,60 @@
                 visibility: "hidden",
                 width: "0px"
             };
         return t.jsxs("div", {
             style: y,
             children: [t.jsx("div", {
                 id: "callerid",
-                style: j
+                style: k
             }), t.jsx("video", {
                 id: "video1",
                 style: b,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsx("video", {
                 id: "video2",
                 style: m,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsxs("div", {
                 style: L,
-                children: [t.jsx(S, {
+                children: [t.jsx(j, {
                     style: x,
                     onClick: M,
                     icon: "play"
-                }), t.jsx(S, {
+                }), t.jsx(j, {
                     style: x,
                     onClick: l,
                     icon: "pause"
-                }), t.jsx(S, {
+                }), t.jsx(j, {
                     style: x,
                     onClick: c,
                     icon: "stop"
-                }), t.jsx(S, {
+                }), t.jsx(j, {
                     style: x,
                     onClick: f,
                     icon: "maximize"
                 })]
             })]
         })
     }
     return D()
 }
 
-function Bt(e) {
+function Lt(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
         }
     })
 }
 
-function Dt(e) {
+function At(e) {
     const n = {
         width: "100%",
         textAlign: "center"
     };
     return t.jsx("div", {
         style: n,
         children: t.jsx("img", {
@@ -3992,30 +4048,30 @@
                 height: e.data.height,
                 borderRadius: e.data.round ? "50%" : 0
             }
         })
     })
 }
 
-function Lt(e) {
+function qt(e) {
     return t.jsx("iframe", {
         width: e.data.width || "100%",
         height: e.data.height || "400px",
         id: "gmap_canvas",
         src: "https://maps.google.com/maps?q=" + e.data.latitude + "," + e.data.longitude + "&t=&z=13&ie=UTF8&iwloc=&output=embed",
         frameBorder: "0",
         scrolling: "no",
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
-function At(e) {
+function Rt(e) {
     function n(i) {
-        return e.data.icon ? i.done ? t.jsx(S, {
+        return e.data.icon ? i.done ? t.jsx(j, {
             style: {
                 marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
@@ -4024,18 +4080,18 @@
             },
             children: i.number
         })
     }
 
     function a(i) {
         return {
-            border: "3px solid " + C.colors.primary,
+            border: "3px solid " + S.colors.primary,
             borderRadius: "50%",
-            background: i.done ? C.colors.primary : "white",
-            color: i.done ? "white" : C.colors.primary,
+            background: i.done ? S.colors.primary : "white",
+            color: i.done ? "white" : S.colors.primary,
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
@@ -4045,15 +4101,15 @@
             listStyleType: "none",
             display: "flex",
             justifyContent: "center",
             minWidth: i.length * 100
         }
     }
 
-    function d() {
+    function o() {
         const i = {
                 width: "100%",
                 margin: "auto",
                 overflowX: "auto",
                 "&::WebkitScrollbar": {
                     width: 0
                 }
@@ -4086,55 +4142,55 @@
                             children: c.name
                         })]
                     }, Math.random()))
                 })
             })
         })
     }
-    return d()
+    return o()
 }
 
-function qt(e) {
+function Nt(e) {
     function n() {
         const a = {
                 display: "inline-block",
                 width: "100%",
                 backgroundColor: "#DDD",
                 borderRadius: 5,
                 marginTop: 5
             },
             r = {
                 marginLeft: 10
             },
-            d = {
+            o = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: C.colors[e.data.style]
+                backgroundColor: S.colors[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
-                style: d,
+                style: o,
                 children: t.jsxs("span", {
                     style: r,
                     children: [e.data.value, "%"]
                 })
             })
         })
     }
     return n()
 }
 
-function Rt(e) {
+function Ot(e) {
     function n() {
-        return e.data.color = C.colors[e.data.style], t.jsx(Me, {
+        return e.data.color = S.colors[e.data.style], t.jsx(Me, {
             data: e.data
         })
     }
     return n()
 }
 
 function Me(e) {
@@ -4152,15 +4208,15 @@
             style: a,
             children: e.data.label
         })
     }
     return n()
 }
 
-function Nt(e) {
+function _t(e) {
     function n() {
         const a = {
                 padding: 20,
                 marginLeft: -20,
                 marginRight: -20,
                 textAlign: "center",
                 backgroundColor: "#f8f8f8"
@@ -4172,57 +4228,57 @@
                 width: 250,
                 height: 250,
                 backgroundColor: "white",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
-            d = {
+            o = {
                 marginTop: 30,
                 fontSize: "3rem",
-                color: C.colors.auxiliary
+                color: S.colors.auxiliary
             },
             i = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
-                color: C.colors.primary
+                color: S.colors.primary
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
                 "data-label": T(e.data.title),
                 style: {
-                    color: C.colors.primary
+                    color: S.colors.primary
                 },
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(l => t.jsxs(N, {
                     href: l.url,
                     style: r,
                     dataLabel: l.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(S, {
-                            style: d,
+                        children: t.jsx(j, {
+                            style: o,
                             icon: l.icon
                         })
                     }), t.jsx("div", {
                         style: i,
                         children: l.label
                     })]
                 }, Math.random()))
             })]
         }) : null
     }
     return n()
 }
 
-function Ot(e) {
+function Ft(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 backgroundColor: "black",
                 color: "white",
                 padding: "10px",
                 minHeight: "300px",
@@ -4234,44 +4290,44 @@
                 children: a
             }, Math.random()))
         })
     }
     return n()
 }
 
-function _t(e) {
+function zt(e) {
     function n() {
         return e.data.url ? t.jsx(N, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(S, {
+            children: e.data.icon ? t.jsx(j, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
 }
 
-function Ft(e) {
+function Ht(e) {
     function n() {
         return t.jsx("iframe", {
             src: e.data.url,
             width: "100%",
             height: 500,
             style: {
                 border: 0
             }
         })
     }
     return n()
 }
 
-function zt(e) {
+function Wt(e) {
     const n = Math.random();
     I.useEffect(() => {
         new QRCode(document.getElementById(n), {
             text: e.data.text,
             width: 128,
             height: 128,
             colorDark: "#333333",
@@ -4284,30 +4340,30 @@
         return t.jsx("div", {
             id: n
         })
     }
     return a()
 }
 
-function Ht(e) {
+function Pt(e) {
     function n() {
         const a = {
                 color: "white",
-                backgroundColor: C.colors.highlight,
+                backgroundColor: S.colors.highlight,
                 margin: -20,
                 textAlign: "center",
                 paddingTop: 20,
                 paddingBottom: 70
             },
             r = {
                 fontSize: "4rem",
                 fontWeight: "bold",
                 marginTop: 25
             },
-            d = {
+            o = {
                 fontSize: "1.2rem",
                 maxWidth: 200,
                 margin: "auto"
             };
         if (e.data) return t.jsxs("div", {
             className: "indicators",
             style: a,
@@ -4315,49 +4371,49 @@
                 "data-label": T(e.data.title),
                 children: e.data.title
             }), t.jsx(G, {
                 width: 300,
                 children: e.data.items.map(i => t.jsxs("div", {
                     children: [t.jsx("div", {
                         style: r,
-                        children: z(i.value)
+                        children: H(i.value)
                     }), t.jsx("div", {
-                        style: d,
+                        style: o,
                         children: i.name
                     })]
-                }))
+                }, Math.random()))
             }, Math.random()), t.jsx("div", {
                 className: "actions",
                 children: e.data.actions.map(i => t.jsx(N, {
                     href: q(i.url),
                     label: i.label,
                     modal: i.modal,
                     children: i.label
                 }, Math.random()))
             })]
         })
     }
     return n()
 }
 
-function Wt(e) {
+function Ut(e) {
     function n() {
         return t.jsx(G, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
                 children: t.jsx(p, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
 
-function Pt(e) {
+function Gt(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     fontSize: "12rem",
@@ -4366,89 +4422,89 @@
                 },
                 children: e.data.value
             })]
         })
     }
     return n()
 }
-var Z, ce = {};
-const Ut = "/api/application/",
-    ye = localStorage.getItem("application");
+var Z, he = {};
+const Vt = "/api/application/",
+    ve = localStorage.getItem("application");
 
 function p(e) {
-    const n = ce[e.data.type];
+    const n = he[e.data.type];
     return n ? Be.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
 p.register = function(e, n) {
-    ce[n.toLowerCase()] = e
+    he[n.toLowerCase()] = e
 };
 p.render = function(e) {
     Z = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-p.register(Pt, "Counter");
-p.register(ct, "Form");
-p.register(ht, "QuerySet");
-p.register(Ue, "Fieldset");
+p.register(Gt, "Counter");
+p.register(ht, "Form");
+p.register(ft, "QuerySet");
+p.register(Ve, "Fieldset");
 p.register(Y, "Field");
-p.register($e, "Object");
-p.register(Je, "Section");
-p.register(Qe, "Group");
-p.register(kt, "Statistics");
-p.register(Dt, "Image");
-p.register(Bt, "Banner");
-p.register(Lt, "Map");
-p.register(At, "Steps");
-p.register(zt, "QrCode");
+p.register(Ye, "Object");
+p.register(Qe, "Section");
+p.register(Ke, "Group");
+p.register(Ct, "Statistics");
+p.register(At, "Image");
+p.register(Lt, "Banner");
+p.register(qt, "Map");
+p.register(Rt, "Steps");
+p.register(Wt, "QrCode");
 p.register(Me, "Badge");
-p.register(Rt, "Status");
-p.register(qt, "Progress");
+p.register(Ot, "Status");
+p.register(Nt, "Progress");
 p.register(De, "Color");
-p.register(Nt, "Boxes");
-p.register(Ht, "Indicators");
-p.register(Ot, "Shell");
-p.register(_t, "FileLink");
-p.register(Ft, "FilePreview");
+p.register(_t, "Boxes");
+p.register(Pt, "Indicators");
+p.register(Ft, "Shell");
+p.register(zt, "FileLink");
+p.register(Ht, "FilePreview");
 p.register(Ne, "Response");
-p.register(Et, "Application");
+p.register(Bt, "Application");
 p.register(Le, "IconSet");
-p.register(Wt, "Grid");
-p.register(We, "Rows");
-p.register(Pe, "Timeline");
-p.register(It, "WebConf");
+p.register(Ut, "Grid");
+p.register(Ue, "Rows");
+p.register(Ge, "Timeline");
+p.register(Dt, "WebConf");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
-    ce[n] ? B("GET", q(e), function(a) {
+    he[n] ? B("GET", q(e), function(a) {
         Z.render(t.jsx(p, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), ye ? (window.application = JSON.parse(ye), B("GET", q(e), function(a) {
+    }, "", e), ve ? (window.application = JSON.parse(ve), B("GET", q(e), function(a) {
         window.application.content = a, Z.render(t.jsx(p, {
             data: window.application
         }, Math.random()))
-    })) : B("GET", Ut, function(r) {
-        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), B("GET", q(e), function(d) {
-            window.application.content = d, Z.render(t.jsx(p, {
+    })) : B("GET", Vt, function(r) {
+        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), B("GET", q(e), function(o) {
+            window.application.content = o, Z.render(t.jsx(p, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
     }, "", e), B("GET", q(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-p.render(H.createRoot(document.getElementById("root")));
+p.render(F.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.2.9/slth/static/js/vanilla-masker.js` & `pyslth-0.3.1/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/static/js/vanilla-masker.min.js` & `pyslth-0.3.1/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/statistics.py` & `pyslth-0.3.1/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/templates/index.html` & `pyslth-0.3.1/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/templates/service-worker.js` & `pyslth-0.3.1/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/tests.py` & `pyslth-0.3.1/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/urls.py` & `pyslth-0.3.1/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/utils.py` & `pyslth-0.3.1/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.9/slth/views.py` & `pyslth-0.3.1/slth/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from .exceptions import JsonResponseException
 from .serializer import serialize
 from .utils import build_url
 from slth import APPLICATON
 from django.shortcuts import render
+from django.views.decorators.cache import never_cache, cache_control
 
+@cache_control(max_age=0, no_cache=True, no_store=True, must_revalidate=True)
 def index(request, path=None):
     vite = not socket.socket(socket.AF_INET, socket.SOCK_STREAM).connect_ex(('127.0.0.1',5173))
     return render(request, 'index.html', dict(vite=vite, application=APPLICATON))
 
 def service_worker(request):
     return render(request, 'service-worker.js', content_type='text/javascript')
```


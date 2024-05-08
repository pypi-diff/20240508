# Comparing `tmp/pyslth-0.2.8.tar.gz` & `tmp/pyslth-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.2.8.tar", last modified: Tue May  7 21:06:28 2024, max compression
+gzip compressed data, was "pyslth-0.2.9.tar", last modified: Wed May  8 08:47:03 2024, max compression
```

## Comparing `pyslth-0.2.8.tar` & `pyslth-0.2.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.975819 pyslth-0.2.8/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.8/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-07 21:06:28.975603 pyslth-0.2.8/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.938287 pyslth-0.2.8/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.8/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-07 21:06:28.975880 pyslth-0.2.8/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-07 21:05:43.000000 pyslth-0.2.8/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.946053 pyslth-0.2.8/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-05-05 12:13:46.000000 pyslth-0.2.8/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     7036 2024-05-06 09:18:10.000000 pyslth-0.2.8/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.946682 pyslth-0.2.8/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.8/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.8/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    22579 2024-05-07 13:01:04.000000 pyslth-0.2.8/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.2.8/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    22178 2024-05-05 11:07:40.000000 pyslth-0.2.8/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.947035 pyslth-0.2.8/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.947708 pyslth-0.2.8/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.8/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.8/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.950459 pyslth-0.2.8/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.8/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.8/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6529 2024-05-06 02:38:49.000000 pyslth-0.2.8/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.8/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.2.8/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19474 2024-05-05 01:08:32.000000 pyslth-0.2.8/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.8/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.951035 pyslth-0.2.8/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.8/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.8/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14274 2024-05-05 11:25:25.000000 pyslth-0.2.8/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.951390 pyslth-0.2.8/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.953358 pyslth-0.2.8/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.8/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.961116 pyslth-0.2.8/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.8/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.8/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.8/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.8/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1670 2024-05-06 02:58:09.000000 pyslth-0.2.8/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.8/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.2.8/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.964487 pyslth-0.2.8/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.8/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.8/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.8/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.2.8/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.8/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.974278 pyslth-0.2.8/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-07 21:03:34.000000 pyslth-0.2.8/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.2.8/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-07 21:03:34.000000 pyslth-0.2.8/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)    90134 2024-05-07 21:03:34.000000 pyslth-0.2.8/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.975309 pyslth-0.2.8/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3138 2024-05-07 11:57:05.000000 pyslth-0.2.8/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.8/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.8/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.8/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.8/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.724033 pyslth-0.2.9/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.9/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 08:47:03.723832 pyslth-0.2.9/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.687834 pyslth-0.2.9/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-08 08:47:03.000000 pyslth-0.2.9/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.9/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-08 08:47:03.724099 pyslth-0.2.9/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-08 08:46:46.000000 pyslth-0.2.9/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.694731 pyslth-0.2.9/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-05-05 12:13:46.000000 pyslth-0.2.9/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     7036 2024-05-06 09:18:10.000000 pyslth-0.2.9/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.695345 pyslth-0.2.9/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.9/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.9/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    22579 2024-05-07 13:01:04.000000 pyslth-0.2.9/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.2.9/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    22178 2024-05-05 11:07:40.000000 pyslth-0.2.9/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.695661 pyslth-0.2.9/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.696332 pyslth-0.2.9/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.9/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.9/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.699267 pyslth-0.2.9/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.9/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.9/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.9/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6529 2024-05-06 02:38:49.000000 pyslth-0.2.9/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.9/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.2.9/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19474 2024-05-05 01:08:32.000000 pyslth-0.2.9/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.9/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.699744 pyslth-0.2.9/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.9/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.9/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14274 2024-05-05 11:25:25.000000 pyslth-0.2.9/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.700063 pyslth-0.2.9/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.701946 pyslth-0.2.9/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.9/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.706217 pyslth-0.2.9/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.9/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.9/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.9/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.9/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1670 2024-05-06 02:58:09.000000 pyslth-0.2.9/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.9/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.2.9/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.708573 pyslth-0.2.9/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.9/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.9/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.9/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.2.9/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.9/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.722880 pyslth-0.2.9/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-08 08:46:42.000000 pyslth-0.2.9/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.2.9/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-08 08:46:42.000000 pyslth-0.2.9/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    90388 2024-05-08 08:46:42.000000 pyslth-0.2.9/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.9/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 08:47:03.723526 pyslth-0.2.9/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3138 2024-05-07 11:57:05.000000 pyslth-0.2.9/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.9/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.9/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.9/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.9/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.9/slth/views.py
```

### Comparing `pyslth-0.2.8/PKG-INFO` & `pyslth-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.8
+Version: 0.2.9
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.8/pyslth.egg-info/PKG-INFO` & `pyslth-0.2.9/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.8
+Version: 0.2.9
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.8/pyslth.egg-info/SOURCES.txt` & `pyslth-0.2.9/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/setup.py` & `pyslth-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.2.8',
+    version='0.2.9',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.2.8/slth/__init__.py` & `pyslth-0.2.9/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/components.py` & `pyslth-0.2.9/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/db/models.py` & `pyslth-0.2.9/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/endpoints.py` & `pyslth-0.2.9/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/factory.py` & `pyslth-0.2.9/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/forms.py` & `pyslth-0.2.9/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/management/commands/integration_test.py` & `pyslth-0.2.9/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/management/commands/sync.py` & `pyslth-0.2.9/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/migrations/0001_initial.py` & `pyslth-0.2.9/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.2.9/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.2.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/migrations/0006_user.py` & `pyslth-0.2.9/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/models.py` & `pyslth-0.2.9/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/oauth.py` & `pyslth-0.2.9/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/permissions.py` & `pyslth-0.2.9/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/queryset.py` & `pyslth-0.2.9/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/roles.py` & `pyslth-0.2.9/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/selenium/__init__.py` & `pyslth-0.2.9/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/selenium/browser.py` & `pyslth-0.2.9/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/serializer.py` & `pyslth-0.2.9/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/.DS_Store` & `pyslth-0.2.9/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/fontawesome.min.css` & `pyslth-0.2.9/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/fonts/.DS_Store` & `pyslth-0.2.9/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.2.9/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.2.9/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.2.9/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.2.9/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/slth.css` & `pyslth-0.2.9/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/css/solid.min.css` & `pyslth-0.2.9/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/images/logo.png` & `pyslth-0.2.9/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/images/logo.svg` & `pyslth-0.2.9/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/images/user.png` & `pyslth-0.2.9/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/echarts.min.js` & `pyslth-0.2.9/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/index.min.js` & `pyslth-0.2.9/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/ios-splash.min.js` & `pyslth-0.2.9/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/peerjs.min.js` & `pyslth-0.2.9/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/qrcode.min.js` & `pyslth-0.2.9/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/react-trigger-change.js` & `pyslth-0.2.9/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/react.min.js` & `pyslth-0.2.9/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/slth.min.js` & `pyslth-0.2.9/slth/static/js/slth.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -141,15 +141,15 @@
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function ye() {
+function xe() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
 function oe(e) {
     function n() {
@@ -263,23 +263,23 @@
 }
 
 function pe() {
     document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {}))
 }
 
 function be(e, n) {
-    ye(), pe(), window.reloader = n;
+    xe(), pe(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
     H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
         url: q(e)
     }))
 }
 
 function Oe(e) {
-    ye(), pe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
+    xe(), pe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         url: q(e)
     }))
 }
 
 function J(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
@@ -446,17 +446,20 @@
 function X(e) {
     function n(i) {
         var l = i.target.parentNode.querySelector(".dropdown");
         return l == null && (l = i.target.parentNode.parentNode.querySelector(".dropdown")), l == null && (l = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), l
     }
 
     function a(i) {
-        const l = i.target.getBoundingClientRect(),
-            s = n(i);
-        document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), s.style.left = l.left - 150 + l.width + "px", s.style.display = "block"
+        const l = n(i);
+        if (l.style.display == "block") l.style.display = "none";
+        else {
+            const s = i.target.getBoundingClientRect();
+            document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), l.style.left = s.left - 150 + s.width + "px", l.style.display = "block"
+        }
     }
 
     function r(i) {
         const l = n(i);
         l.style.display = "none"
     }
 
@@ -1378,20 +1381,20 @@
             var s = new FileReader;
             s.onload = function(u) {
                 if (ie(c.name)) {
                     const w = "display" + a;
                     var o = document.createElement("img");
                     o.id = l.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(M) {
                         const D = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
-                        var x = document.createElement("canvas");
-                        const j = x.getContext("2d");
-                        x.height = x.width * (o.height / o.width);
-                        const y = document.createElement("canvas"),
-                            L = y.getContext("2d");
-                        y.width = o.width * D, y.height = o.height * D, L.drawImage(o, 0, 0, y.width, y.height), j.drawImage(y, 0, 0, y.width * D, y.height * D, 0, 0, x.width, x.height), y.toBlob(function(m) {
+                        var y = document.createElement("canvas");
+                        const j = y.getContext("2d");
+                        y.height = y.width * (o.height / o.width);
+                        const x = document.createElement("canvas"),
+                            L = x.getContext("2d");
+                        x.width = o.width * D, x.height = o.height * D, L.drawImage(o, 0, 0, x.width, x.height), j.drawImage(x, 0, 0, x.width * D, x.height * D, 0, 0, y.width, y.height), x.toBlob(function(m) {
                             const v = new DataTransfer;
                             v.items.add(new File([m], c.name)), l.target.files = v.files
                         });
                         var b = document.getElementById(w);
                         b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), l.target.parentNode.appendChild(b)
                     }, o.src = u.target.result
                 }
@@ -1535,25 +1538,25 @@
                 g = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
                 children: [b == null && n.map((k, E) => t.jsxs("div", {
                     style: m,
                     children: [t.jsx("span", {
-                        onClick: () => y(E),
+                        onClick: () => x(E),
                         style: v,
                         children: t.jsx(S, {
                             icon: "trash-can",
                             style: g
                         })
                     }), k.value]
                 }, Math.random())), b != null && Array.from(b.options).map((k, E) => t.jsxs("div", {
                     style: m,
                     children: [t.jsx("span", {
-                        onClick: () => y(E),
+                        onClick: () => x(E),
                         style: v,
                         children: t.jsx(S, {
                             icon: "trash-can",
                             style: g
                         })
                     }), k.innerHTML]
                 }, Math.random()))]
@@ -1619,17 +1622,17 @@
                 }
             }), t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
                 onFocus: A => {
-                    A.target.select(), x(A)
+                    A.target.select(), y(A)
                 },
-                onChange: x,
+                onChange: y,
                 onMouseLeave: M,
                 onBlur: M,
                 defaultValue: ae,
                 style: b,
                 "data-label": T(e.data.label)
             }), s && i && t.jsxs("ul", {
                 style: m,
@@ -1663,30 +1666,30 @@
         const m = document.getElementById(a);
         if (m) {
             const v = document.getElementById(r);
             d || m.options.length > 0 && v.value != m.options[0].innerHTML && (m.innerHTML = "", v.value = "", l(!1), e.data.onchange && ee(v, e.data.onchange)), b.target.tagName == "UL" ? l(!1) : u || l(!1)
         }
     }
 
-    function x(b) {
+    function y(b) {
         clearTimeout(o), o = setTimeout(function() {
             const m = e.data.choices.indexOf("?") < 0 ? "?" : "&";
             l(!0), B("GET", e.data.choices + m + "term=" + b.target.value, function(g) {
                 c(g)
             })
         }, 1e3)
     }
 
     function j(b, m = !1) {
         const v = document.getElementById(a),
             g = document.getElementById(r);
         v.innerHTML == null && (v.innerHTML = ""), Array.isArray(b) ? v.innerHTML = b.map(k => `<option selected value="${k.id}">${k.value}</option>`).join("") : d ? (v.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, g.value = "") : (v.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, g.value = b.value), e.data.onchange && !m && ee(g, e.data.onchange)
     }
 
-    function y(b) {
+    function x(b) {
         const m = document.getElementById(a);
         var v = Array.from(m.options);
         m.innerHTML = v.slice(0, b).concat(v.slice(b + 1)).map(g => `<option selected value="${g.value}">${g.innerHTML}</option>`).join(""), c([])
     }
 
     function L() {
         return t.jsxs(t.Fragment, {
@@ -2166,29 +2169,29 @@
         var f = e.data.url,
             w = document.getElementById(n),
             M = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
             const D = f.indexOf("?") >= 0 ? "&" : "?";
             f = f + D + "form=" + e.data.title + "&" + new URLSearchParams(M).toString(), M = null
         }
-        B(w.method.toUpperCase(), f, function(x) {
-            if (w.querySelectorAll(".error").forEach(y => y.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), x.type == "response") return J(), Xe(), ve(x);
-            if (x.type == "error") {
-                var j = x.text;
-                console.log(x), Object.keys(x.errors).map(function(y) {
-                    if (y == "__all__") j = x.errors[y];
+        B(w.method.toUpperCase(), f, function(y) {
+            if (w.querySelectorAll(".error").forEach(x => x.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), y.type == "response") return J(), Xe(), ve(y);
+            if (y.type == "error") {
+                var j = y.text;
+                console.log(y), Object.keys(y.errors).map(function(x) {
+                    if (x == "__all__") j = y.errors[x];
                     else {
-                        const L = w.querySelector("#" + y + "_error");
-                        L.querySelector("span").innerHTML = x.errors[y], L.style.display = "block"
+                        const L = w.querySelector("#" + x + "_error");
+                        L.querySelector("span").innerHTML = y.errors[x], L.style.display = "block"
                     }
                 }), te(j, !0)
             } else {
-                const y = document.querySelector("#output");
-                y.innerHTML = "", H.createRoot(y.appendChild(document.createElement("div"))).render(t.jsx(p, {
-                    data: x
+                const x = document.querySelector("#output");
+                x.innerHTML = "", H.createRoot(x.appendChild(document.createElement("div"))).render(t.jsx(p, {
+                    data: y
                 }))
             }
         }, M)
     }
     return c()
 }
 
@@ -2288,20 +2291,20 @@
                 }, Math.random())
             })
         })
     }
 
     function s(m) {
         const v = document.getElementById("subset-" + e.data.id);
-        v.value = m || "", y()
+        v.value = m || "", x()
     }
 
     function c(m, v, g) {
         const k = document.getElementById("form-" + e.data.id);
-        k.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", k.querySelector("input[name=" + n.calendar.field + "__month]").value = v || "", k.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", y()
+        k.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", k.querySelector("input[name=" + n.calendar.field + "__month]").value = v || "", k.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", x()
     }
 
     function u() {
         if (n.calendar) {
             const E = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
                 ae = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
                 A = {
@@ -2557,15 +2560,15 @@
                 })]
             })
         })
     }
 
     function M(m) {
         const g = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        g.value = m, y()
+        g.value = m, x()
     }
 
     function D() {
         const m = document.getElementById("form-" + e.data.id);
         if (m) {
             const E = m.querySelector("input[name=page]");
             E && (E.value = n.pagination.page.current)
@@ -2645,15 +2648,15 @@
                         onClick: () => M(n.pagination.page.next)
                     })]
                 })
             })]
         })
     }
 
-    function x() {
+    function y() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
             children: n.actions.map(function(m) {
@@ -2694,15 +2697,15 @@
                         return E.type != "hidden" && t.jsx("div", {
                             children: t.jsx(K, {
                                 data: E
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         children: t.jsx(R, {
-                            onClick: y,
+                            onClick: x,
                             label: "Filtrar",
                             icon: "filter",
                             primary: !0
                         })
                     })]
                 }), g && n.filters.map(function(E) {
                     return E.type == "hidden" && t.jsx("div", {
@@ -2711,15 +2714,15 @@
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function y() {
+    function x() {
         i(!0);
         var m;
         const v = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
         e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + v : m = e.data.url + "?" + v, B("GET", m, function(g) {
             a(g), i(!1)
         })
     }
@@ -2736,20 +2739,20 @@
                                 data: v
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [x(), l(), j(), u(), f(), D()]
+            children: [y(), l(), j(), u(), f(), D()]
         })
     }
 
     function b() {
-        window[e.data.id] = () => y();
+        window[e.data.id] = () => x();
         const m = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable",
             id: e.data.id,
@@ -2970,23 +2973,23 @@
 function gt(e) {
     return t.jsx(W, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function xt(e) {
+function yt(e) {
     return t.jsx(W, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function yt(e) {
+function xt(e) {
     return t.jsx(W, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
@@ -3157,20 +3160,20 @@
                 });
             case "tree_map":
                 return t.jsx(wt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "line":
-                return t.jsx(xt, {
+                return t.jsx(yt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "area":
-                return t.jsx(yt, {
+                return t.jsx(xt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "progress":
                 return t.jsx(jt, {
                     headers: e.headers,
                     rows: e.rows
@@ -3455,30 +3458,31 @@
     }
 
     function d() {
         if (Notification.permission !== "granted") return t.jsx(S, {
             onClick: r,
             icon: "bell",
             style: {
-                cursor: "pointer"
+                cursor: "pointer",
+                color: C.colors.primary
             }
         })
     }
     return d()
 }
 
 function Tt(e) {
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
-                backgroundColor: "#1151b3",
+                backgroundColor: C.colors.primary,
                 color: "white",
                 right: 10,
                 borderRadius: "50%",
                 cursor: "pointer"
             },
             r = {
                 paddingLeft: 14,
@@ -3672,15 +3676,24 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.usermenu,
                         position: {},
                         dataLabel: T(e.data.navbar.user),
-                        children: e.data.navbar.user
+                        children: t.jsx("img", {
+                            src: "/static/images/user.svg",
+                            style: {
+                                width: 30,
+                                height: 30,
+                                borderRadius: "50%",
+                                objectFit: "cover",
+                                backgroundColor: C.colors.primary
+                            }
+                        })
                     })
                 })]
             })]
         }) : null
     }
 
     function i() {
@@ -3771,47 +3784,47 @@
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
                 offerToReceiveVideo: 1
             },
-            sdpTransform: x => x.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
+            sdpTransform: y => y.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
     I.useEffect(() => {
-        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(x) {
+        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(y) {
             document.getElementById("callerid").innerHTML = e.data.caller
-        }), n.on("call", function(x) {
+        }), n.on("call", function(y) {
             d({
                 video: {
                     width: {
                         exact: 320
                     },
                     height: {
                         exact: 240
                     }
                 },
                 audio: !0
             }, function(j) {
                 a = j;
-                var y = document.getElementById("video2");
-                y.addEventListener("loadedmetadata", function(L) {
-                    y.style.width = this.videoWidth / 4 + "px", y.style.height = this.videoHeight / 4 + "px", y.style.marginLeft = -this.videoWidth / 4 + "px", y.style.visibility = "visible"
-                }, !1), y.srcObject = a, x.answer(j), x.on("stream", function(L) {
+                var x = document.getElementById("video2");
+                x.addEventListener("loadedmetadata", function(L) {
+                    x.style.width = this.videoWidth / 4 + "px", x.style.height = this.videoHeight / 4 + "px", x.style.marginLeft = -this.videoWidth / 4 + "px", x.style.visibility = "visible"
+                }, !1), x.srcObject = a, y.answer(j), y.on("stream", function(L) {
                     r = L, document.getElementById("video1").srcObject = r
-                }), x.on("close", function() {
+                }), y.on("close", function() {
                     c()
                 }), n.on("error", function(L) {
                     c()
                 })
             }, function(j) {
                 console.log("Failed to get local stream", j)
             })
-        }), n.on("error", function(x) {
-            x.type == "browser-incompatible" ? alert("Navegador incompatível.") : x.type == "invalid-id" ? alert("Usuário inexistente.") : x.type == "network" ? alert("Problema na conexão do usuário.") : x.type == "peer-unavailable" && alert("Usuário indisponível.")
+        }), n.on("error", function(y) {
+            y.type == "browser-incompatible" ? alert("Navegador incompatível.") : y.type == "invalid-id" ? alert("Usuário inexistente.") : y.type == "network" ? alert("Problema na conexão do usuário.") : y.type == "peer-unavailable" && alert("Usuário indisponível.")
         })
     }, []);
 
     function l() {
         o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video")
     }
 
@@ -3819,42 +3832,42 @@
         h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video")
     }
 
     function c() {
         u(a, "audio"), u(a, "video"), u(r, "audio"), u(r, "video"), a = null, r = null, document.getElementById("video1").srcObject = null, document.getElementById("video2").srcObject = null, console.log("Stopped!")
     }
 
-    function u(x, j) {
-        x != null && x.getTracks().forEach(y => {
-            y.readyState == "live" && y.kind === j && y.stop()
+    function u(y, j) {
+        y != null && y.getTracks().forEach(x => {
+            x.readyState == "live" && x.kind === j && x.stop()
         })
     }
 
-    function o(x, j) {
-        x != null && x.getTracks().forEach(y => {
-            y.readyState == "live" && y.kind === j && (y.enabled = !1)
+    function o(y, j) {
+        y != null && y.getTracks().forEach(x => {
+            x.readyState == "live" && x.kind === j && (x.enabled = !1)
         })
     }
 
-    function h(x, j) {
-        x != null && x.getTracks().forEach(y => {
-            y.readyState == "live" && y.kind === j && (y.enabled = !0)
+    function h(y, j) {
+        y != null && y.getTracks().forEach(x => {
+            x.readyState == "live" && x.kind === j && (x.enabled = !0)
         })
     }
 
     function f() {
-        var x = document.getElementById("video1");
-        x.style.width == "" ? x.style.width = "400px" : x.style.width = ""
+        var y = document.getElementById("video1");
+        y.style.width == "" ? y.style.width = "400px" : y.style.width = ""
     }
 
     function w() {
-        var x = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, i);
-        x.on("stream", function(j) {
+        var y = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, i);
+        y.on("stream", function(j) {
             r = j, document.getElementById("video1").srcObject = r
-        }), x.on("close", function() {
+        }), y.on("close", function() {
             c()
         }), n.on("error", function(j) {
             c()
         })
     }
 
     function M() {
@@ -3875,36 +3888,36 @@
                 echoCancellation: !1,
                 latency: 0,
                 noiseSuppression: !1,
                 sampleRate: 48e3,
                 sampleSize: 16,
                 volume: 1
             }
-        }, function(x) {
-            a = x;
+        }, function(y) {
+            a = y;
             var j = document.getElementById("video2");
-            j.addEventListener("loadedmetadata", function(y) {
+            j.addEventListener("loadedmetadata", function(x) {
                 j.style.width = this.videoWidth / 4 + "px", j.style.height = this.videoHeight / 4 + "px", j.style.marginLeft = -this.videoWidth / 4 + "px", j.style.visibility = "visible"
             }, !1), j.srcObject = a, w()
-        }, function(x) {
+        }, function(y) {
             alert("Failed to get local stream.")
         })
     }
 
     function D() {
-        var x = {
+        var y = {
                 width: "fit-content",
                 margin: "auto"
             },
             j = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
-            y = {
+            x = {
                 color: "white",
                 backgroundColor: "black",
                 padding: 2
             },
             L = {
                 position: "absolute",
                 marginTop: "-30px"
@@ -3913,15 +3926,15 @@
                 backgroundColor: "black"
             },
             m = {
                 visibility: "hidden",
                 width: "0px"
             };
         return t.jsxs("div", {
-            style: x,
+            style: y,
             children: [t.jsx("div", {
                 id: "callerid",
                 style: j
             }), t.jsx("video", {
                 id: "video1",
                 style: b,
                 playsInline: !0,
@@ -3930,27 +3943,27 @@
                 id: "video2",
                 style: m,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsxs("div", {
                 style: L,
                 children: [t.jsx(S, {
-                    style: y,
+                    style: x,
                     onClick: M,
                     icon: "play"
                 }), t.jsx(S, {
-                    style: y,
+                    style: x,
                     onClick: l,
                     icon: "pause"
                 }), t.jsx(S, {
-                    style: y,
+                    style: x,
                     onClick: c,
                     icon: "stop"
                 }), t.jsx(S, {
-                    style: y,
+                    style: x,
                     onClick: f,
                     icon: "maximize"
                 })]
             })]
         })
     }
     return D()
@@ -4170,20 +4183,23 @@
             },
             i = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
-                color: "#0c326f"
+                color: C.colors.primary
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
                 "data-label": T(e.data.title),
+                style: {
+                    color: C.colors.primary
+                },
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(l => t.jsxs(N, {
                     href: l.url,
                     style: r,
                     dataLabel: l.label,
                     children: [t.jsx("div", {
@@ -4352,15 +4368,15 @@
             })]
         })
     }
     return n()
 }
 var Z, ce = {};
 const Ut = "/api/application/",
-    xe = localStorage.getItem("application");
+    ye = localStorage.getItem("application");
 
 function p(e) {
     const n = ce[e.data.type];
     return n ? Be.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
@@ -4412,15 +4428,15 @@
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), xe ? (window.application = JSON.parse(xe), B("GET", q(e), function(a) {
+    }, "", e), ye ? (window.application = JSON.parse(ye), B("GET", q(e), function(a) {
         window.application.content = a, Z.render(t.jsx(p, {
             data: window.application
         }, Math.random()))
     })) : B("GET", Ut, function(r) {
         window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), B("GET", q(e), function(d) {
             window.application.content = d, Z.render(t.jsx(p, {
                 data: window.application
```

### Comparing `pyslth-0.2.8/slth/static/js/vanilla-masker.js` & `pyslth-0.2.9/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/static/js/vanilla-masker.min.js` & `pyslth-0.2.9/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/statistics.py` & `pyslth-0.2.9/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/templates/index.html` & `pyslth-0.2.9/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/templates/service-worker.js` & `pyslth-0.2.9/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/tests.py` & `pyslth-0.2.9/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/urls.py` & `pyslth-0.2.9/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/utils.py` & `pyslth-0.2.9/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.8/slth/views.py` & `pyslth-0.2.9/slth/views.py`

 * *Files identical despite different names*


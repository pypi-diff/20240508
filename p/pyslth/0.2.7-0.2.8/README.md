# Comparing `tmp/pyslth-0.2.7.tar.gz` & `tmp/pyslth-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.2.7.tar", last modified: Thu May  2 09:39:34 2024, max compression
+gzip compressed data, was "pyslth-0.2.8.tar", last modified: Tue May  7 21:06:28 2024, max compression
```

## Comparing `pyslth-0.2.7.tar` & `pyslth-0.2.8.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.496344 pyslth-0.2.7/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.7/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-02 09:39:34.495766 pyslth-0.2.7/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.427467 pyslth-0.2.7/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-02 09:39:34.000000 pyslth-0.2.7/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1791 2024-05-02 09:39:34.000000 pyslth-0.2.7/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-02 09:39:34.000000 pyslth-0.2.7/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-02 09:39:34.000000 pyslth-0.2.7/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-02 09:39:34.000000 pyslth-0.2.7/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.7/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-02 09:39:34.496564 pyslth-0.2.7/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-02 09:38:38.000000 pyslth-0.2.7/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.445482 pyslth-0.2.7/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.7/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6945 2024-04-30 16:46:55.000000 pyslth-0.2.7/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.446148 pyslth-0.2.7/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.7/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.7/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20556 2024-05-01 15:37:13.000000 pyslth-0.2.7/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.7/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2527 2024-05-01 13:30:46.000000 pyslth-0.2.7/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25571 2024-05-02 08:29:34.000000 pyslth-0.2.7/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.446502 pyslth-0.2.7/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.7/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.449249 pyslth-0.2.7/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.7/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.7/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.7/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.459428 pyslth-0.2.7/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.7/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.7/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.7/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.7/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.7/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.7/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6441 2024-05-01 14:04:01.000000 pyslth-0.2.7/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.7/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.7/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19351 2024-05-01 11:31:08.000000 pyslth-0.2.7/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.7/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.461527 pyslth-0.2.7/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.7/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.7/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14408 2024-05-01 13:49:16.000000 pyslth-0.2.7/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.462034 pyslth-0.2.7/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.465942 pyslth-0.2.7/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.7/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.473210 pyslth-0.2.7/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.7/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.7/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.7/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.7/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1574 2024-05-02 09:21:27.000000 pyslth-0.2.7/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.7/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.474943 pyslth-0.2.7/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.7/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.7/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.7/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.7/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.494516 pyslth-0.2.7/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-02 09:39:11.000000 pyslth-0.2.7/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.2.7/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-02 09:39:11.000000 pyslth-0.2.7/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)    87064 2024-05-02 09:39:11.000000 pyslth-0.2.7/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.7/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-02 09:39:34.495306 pyslth-0.2.7/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     2407 2024-05-02 09:31:38.000000 pyslth-0.2.7/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.7/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.7/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.7/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.7/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.7/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.975819 pyslth-0.2.8/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.8/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-07 21:06:28.975603 pyslth-0.2.8/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.938287 pyslth-0.2.8/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-07 21:06:28.000000 pyslth-0.2.8/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.8/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-07 21:06:28.975880 pyslth-0.2.8/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-07 21:05:43.000000 pyslth-0.2.8/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.946053 pyslth-0.2.8/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-05-05 12:13:46.000000 pyslth-0.2.8/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     7036 2024-05-06 09:18:10.000000 pyslth-0.2.8/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.946682 pyslth-0.2.8/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.8/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.8/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    22579 2024-05-07 13:01:04.000000 pyslth-0.2.8/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.2.8/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    22178 2024-05-05 11:07:40.000000 pyslth-0.2.8/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.947035 pyslth-0.2.8/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.947708 pyslth-0.2.8/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.8/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.8/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.950459 pyslth-0.2.8/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.8/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.8/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.8/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6529 2024-05-06 02:38:49.000000 pyslth-0.2.8/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.8/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.2.8/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19474 2024-05-05 01:08:32.000000 pyslth-0.2.8/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.8/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.951035 pyslth-0.2.8/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.8/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.8/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14274 2024-05-05 11:25:25.000000 pyslth-0.2.8/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.951390 pyslth-0.2.8/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.953358 pyslth-0.2.8/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.8/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.961116 pyslth-0.2.8/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.8/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.8/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.8/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.8/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1670 2024-05-06 02:58:09.000000 pyslth-0.2.8/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.8/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.2.8/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.964487 pyslth-0.2.8/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.8/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.8/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.8/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.2.8/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.8/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.974278 pyslth-0.2.8/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-07 21:03:34.000000 pyslth-0.2.8/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.2.8/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-07 21:03:34.000000 pyslth-0.2.8/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    90134 2024-05-07 21:03:34.000000 pyslth-0.2.8/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.8/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-07 21:06:28.975309 pyslth-0.2.8/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3138 2024-05-07 11:57:05.000000 pyslth-0.2.8/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.8/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.8/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.8/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.8/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.8/slth/views.py
```

### Comparing `pyslth-0.2.7/PKG-INFO` & `pyslth-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.7
+Version: 0.2.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.7/pyslth.egg-info/PKG-INFO` & `pyslth-0.2.8/pyslth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.7
+Version: 0.2.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.7/pyslth.egg-info/SOURCES.txt` & `pyslth-0.2.8/pyslth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 slth/components.py
 slth/endpoints.py
 slth/exceptions.py
 slth/factory.py
 slth/forms.py
 slth/models.py
 slth/notifications.py
+slth/oauth.py
 slth/permissions.py
 slth/queryset.py
 slth/roles.py
 slth/serializer.py
 slth/statistics.py
 slth/tests.py
 slth/urls.py
@@ -39,22 +40,24 @@
 slth/selenium/__init__.py
 slth/selenium/browser.py
 slth/static/index.html
 slth/static/css/.DS_Store
 slth/static/css/fontawesome.min.css
 slth/static/css/slth.css
 slth/static/css/solid.min.css
+slth/static/css/style.css
 slth/static/css/fonts/.DS_Store
 slth/static/css/fonts/fa-solid-900.woff2
 slth/static/css/fonts/rawline-400.woff
 slth/static/css/fonts/rawline-500i.woff
 slth/static/css/fonts/rawline-700.woff
 slth/static/images/logo.png
 slth/static/images/logo.svg
 slth/static/images/user.png
+slth/static/images/user.svg
 slth/static/js/echarts.min.js
 slth/static/js/index.min.js
 slth/static/js/ios-splash.min.js
 slth/static/js/peerjs.min.js
 slth/static/js/qrcode.min.js
 slth/static/js/react-trigger-change.js
 slth/static/js/react.min.js
```

### Comparing `pyslth-0.2.7/setup.py` & `pyslth-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.2.7',
+    version='0.2.8',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.2.7/slth/__init__.py` & `pyslth-0.2.8/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/components.py` & `pyslth-0.2.8/slth/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,37 +196,39 @@
         self['subtitle'] = subtitle
         self['logo'] = logo
         self['user'] = user
         self['usermenu'] = []
         self['adder'] = []
         self['tools'] = []
         self['settings'] = []
+        self['actions'] = []
 
-    def add_action(self, entrypoint, name, url, modal=True):
-        self[entrypoint].append(dict(name=name, url=url, modal=modal))
+    def add_action(self, entrypoint, name, url, modal=True, icon=None):
+        self[entrypoint].append(dict(name=name, url=url, modal=modal, icon=icon))
 
 class Menu(dict):
     def __init__(self, items, user=None, image=None):
         self['type'] = 'menu'
         self['items'] = items
         self['user'] = user
         self['image'] = image
 
 class Footer(dict):
     def __init__(self, version):
         self['type'] = 'navbar'
         self['version'] = version
 
 class Application(dict):
-    def __init__(self, icon=None, navbar=None, menu=None, footer=None):
+    def __init__(self, icon=None, navbar=None, menu=None, footer=None, oauth=()):
         self['type'] = 'application'
         self['icon'] = icon
         self['navbar'] = navbar
         self['menu'] = menu
         self['footer'] = footer
+        self['oauth'] = oauth
 
 class Response(dict):
 
     def __init__(self, message=None, redirect=None, store=None):
         self['type'] = 'response'
         self['message'] = message
         self['redirect'] = redirect
```

### Comparing `pyslth-0.2.7/slth/db/models.py` & `pyslth-0.2.8/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/endpoints.py` & `pyslth-0.2.8/slth/endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 
 import json
 import types
 import inspect
+from .models import Token
 from django.apps import apps
 from typing import TypeVar, Generic
 from django.core.cache import cache
 from django.conf import settings
 from django.utils.text import slugify
-from django.db import transaction, models
+from django.db import models
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from .factory import FormFactory
-from .forms import LoginForm, ModelForm, Form, SendPushNotificationForm, EditProfileForm, ChangePasswordForm
+from django.core.exceptions import ValidationError
+from slth import forms
+from django.contrib.auth import authenticate
+from .forms import ModelForm, Form
 from .serializer import serialize, Serializer
 from .components import Application as Application_, Navbar, Menu, Footer, Response, Boxes, IconSet
 from .exceptions import JsonResponseException
 from .utils import build_url, append_url
 from .models import PushSubscription, Profile, User
 from slth.queryset import QuerySet
+from .notifications import send_push_web_notification
 from slth import APPLICATON, ENDPOINTS
-
-
-import slth
+from . import oauth
 
 
 T = TypeVar("T")
 
 class ApiResponse(JsonResponse):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -73,14 +76,15 @@
 class Endpoint(metaclass=EnpointMetaclass):
     cache = cache
 
     def __init__(self):
         self.request = None
         self.source = None
         self.instantiator = None
+        self.cleaned_data = {}
         super().__init__()
 
     def configure(self, source, instantiator=None):
         self.source = source
         self.instantiator = instantiator
         return self
 
@@ -91,23 +95,15 @@
     def objects(self, model):
         return apps.get_model(model).objects
         
     def get(self):
         return {}
     
     def post(self):
-        data = self.get()
-        if isinstance(data, FormFactory):
-            data = data.form(self.request).post()
-        if isinstance(data, Form) or isinstance(data, ModelForm):
-            data = data.post()
-        return data
-    
-    def save(self, data):
-        pass
+        return Response(message='Ação realizada com sucesso')
     
     def check_permission(self):
         return self.request.user.is_superuser
     
     def check_role(self, *names, superuser=True):
         if self.request.user.is_superuser and superuser:
             return True
@@ -115,40 +111,46 @@
             if self.objects('slth.role').filter(username=self.request.user.username, name=name).exists():
                 return True
         return False
     
     def redirect(self, url):
         raise JsonResponseException(dict(type='redirect', url=url))
     
-    def getdata(self):
-        if self.request.method == 'GET':
-            data = self.get()
-        elif self.request.method == 'POST':
-            data = self.post()
-        else:
-            data = {}
-        title = self.get_metadata('verbose_name')
+    def getform(self, form):
+        return form
+    
+    def process(self):
+        data = self.get()
+        title = self.get_verbose_name()
         if isinstance(data, models.QuerySet):
             data = data.contextualize(self.request).settitle(title)
         elif isinstance(data, Serializer):
             data = data.contextualize(self.request).settitle(title)
         elif isinstance(data, FormFactory):
-            data = data.settitle(title).form(self.request)
+            form = self.getform(data.settitle(title).form(self))
+            if self.request.method == 'POST' or self.request.GET.get('form') == title:
+                try:
+                    self.cleaned_data = form.submit()
+                    return self.post()
+                except ValidationError as e:
+                    raise JsonResponseException(dict(type='error', text='\n'.join(e.messages), errors={}))
+            else:
+                data = form
         elif isinstance(data, Form) or isinstance(data, ModelForm):
             data = data.settitle(title)
-        return {} if data is None else data
+        return data
     
     def serialize(self):
-        return serialize(self.getdata())
+        return serialize(self.process())
     
     def to_response(self):
         return ApiResponse(self.serialize(), safe=False)
     
-    def formfactory(self, instance, delete=False) -> FormFactory:
-        return FormFactory(instance, delete=delete)
+    def formfactory(self, instance=None, method='POST') -> FormFactory:
+        return FormFactory(instance, method=method)
     
     def serializer(self, instance=None) -> Serializer:
         return Serializer(instance or self).contextualize(self.request)
     
     @classmethod
     def is_child(cls):
         return False
@@ -218,14 +220,17 @@
             value = getattr(metaclass, key, None)
         if value is None:
             if key == 'verbose_name':
                 value = cls.get_pretty_name()
             if key == 'modal':
                 value = issubclass(cls, EditEndpoint) or issubclass(cls, DeleteEndpoint) or issubclass(cls, Endpoint) or issubclass(cls, ChildEndpoint)
         return default if value is None else value
+    
+    def get_verbose_name(self):
+        return self.get_metadata('verbose_name')
 
 class PublicEndpoint(Endpoint):
     def check_permission(self):
         return True
 
 class ModelEndpoint(Endpoint):
     def __init__(self):
@@ -241,74 +246,66 @@
         return self.model.objects.all().actions(*actions)
     
 class ListEndpoint(Generic[T], ModelEndpoint):
     def get(self) -> QuerySet:
         return self.model.objects
 
 class AddEndpoint(Generic[T], ModelEndpoint):
+    def __init__(self):
+        super().__init__()
+        self.instance = self.model()
+
     def get(self) -> FormFactory:
         return self.model().formfactory()
+    
+    def get_instance(self):
+        return self.instance
 
 class ModelInstanceEndpoint(ModelEndpoint):
     def __init__(self, pk):
-        self.pk = pk
         super().__init__()
+        self.instance = self.model.objects.get(pk=pk)
 
     def get_instance(self):
-        return self.model.objects.get(pk=self.pk)
+        return self.instance
 
 class InstanceEndpoint(Generic[T], ModelInstanceEndpoint):
 
-    def formfactory(self, delete=False) -> FormFactory:
-        return FormFactory(self.get_instance(), delete=delete)
+    def formfactory(self) -> FormFactory:
+        return FormFactory(self.get_instance())
 
     def serializer(self) -> Serializer:
         return Serializer(self.get_instance()).contextualize(self.request)
     
 
 class ViewEndpoint(Generic[T], ModelInstanceEndpoint):
 
     class Meta:
         icon = 'eye'
         modal = False
         verbose_name = 'Visualizar'
 
     def get(self) -> Serializer:
         return self.get_instance().serializer().contextualize(self.request)
+    
+    def get_verbose_name(self):
+        return str(self.get_instance())
         
 class EditEndpoint(Generic[T], ModelInstanceEndpoint):
     def get(self) -> FormFactory:
         return self.get_instance().formfactory()
     
 class DeleteEndpoint(Generic[T], ModelInstanceEndpoint):
     def get(self) -> FormFactory:
-        return self.formfactory(self.get_instance(), delete=True)
-    
-
-class FormEndpoint(Generic[T], Endpoint):
-
-    def get_form_cls(self):
-        return self.__orig_bases__[0].__args__[0]
-
-    def get(self):
-        return self.get_form_cls()(request=self.request)
+        return self.formfactory(self.get_instance()).fields()
     
-class InstanceFormEndpoint(Generic[T], Endpoint):
-    def __init__(self, pk):
-        self.pk = pk
-        super().__init__()
-
-    def get_form_cls(self):
-        return self.__orig_bases__[0].__args__[0]
-
-    def get_instance(self):
-        return self.get_form_cls().Meta.model.objects.get(pk=self.pk)
+    def post(self):
+        self.get_instance().delete()
+        return super().post()
 
-    def get(self):
-        return self.get_form_cls()(self.get_instance(), request=self.request)
     
 class ChildEndpoint(Endpoint):
 
     @classmethod
     def is_child(cls):
         return True
     
@@ -327,44 +324,20 @@
     def __init__(self, instance):
         self.instance = instance
         super().__init__()
 
     def get_instance(self):
         return self.instance
     
-    def formfactory(self, delete=False) -> FormFactory:
-        return FormFactory(self.get_instance(), delete=delete)
+    def formfactory(self) -> FormFactory:
+        return FormFactory(self.get_instance())
     
     def serializer(self) -> Serializer:
         return Serializer(self.get_instance()).contextualize(self.request)
     
-class ChildFormEndpoint(Generic[T], Endpoint):
-
-    def get_form_cls(self):
-        return self.__orig_bases__[0].__args__[0]
-
-    def get(self):
-        return self.get_form_cls()(request=self.request, endpoint=self)
-    
-
-class ChildInstanceFormEndpoint(Generic[T], ChildEndpoint):
-
-    def __init__(self, source):
-        self.source = source
-        super().__init__()
-
-    def get_form_cls(self):
-        return self.__orig_bases__[0].__args__[0]
-    
-    def get_instance(self):
-        return self.source
-
-    def get(self):
-        return self.get_form_cls()(instance=self.get_instance(), request=self.request, endpoint=self)
-
 class View(ChildInstanceEndpoint):
     class Meta:
         icon = 'eye'
         modal = False
         verbose_name = 'Visualizar'
     
     def get(self) -> Serializer:
@@ -377,28 +350,58 @@
     def get(self) -> FormFactory:
         return self.get_instance().formfactory()
    
 class Delete(ChildInstanceEndpoint):
     class Meta:
         icon = 'trash'
         verbose_name = 'Excluir'
+    
     def get(self):
-        return self.formfactory(delete=True)
+        return self.formfactory().fields()
+    
+    def post(self):
+        self.get_instance().delete()
+        return super().post()
+
+class Login(PublicEndpoint):
+    username = forms.CharField(label='Username')
+    password = forms.CharField(label='Senha')
+
+    class Meta:
+        modal = False
+        icon = 'sign-in'
+        verbose_name = 'Login'
 
-class Login(Endpoint):
     def get(self):
-        return LoginForm(request=self.request)
+        code = self.request.GET.get('code')
+        if code:
+            user = oauth.authenticate(code)
+            if user:
+                token = Token.objects.create(user=user)
+                return Response(message='Bem-vindo!', redirect='/api/dashboard/', store=dict(token=token.key, application=None))
+        return self.formfactory().fields('username', 'password')
+    
+    def post(self):
+        user = authenticate(self.request, username=self.cleaned_data.get('username'), password=self.cleaned_data.get('password'))
+        if user:
+            token = Token.objects.create(user=user)
+            return Response(message='Bem-vindo!', redirect='/api/dashboard/', store=dict(token=token.key, application=None))
+        else:
+            raise ValidationError('Login e senha não conferem')
 
-class Logout(PublicEndpoint):
+class Logout(Endpoint):
     class Meta:
         modal = False
         verbose_name = 'Sair'
         
     def get(self):
-        return Response(message='Logout realizado com sucesso.', redirect='/api/login/', store=dict(token=None, application=None))
+        return Response(message='Logout realizado com sucesso.', redirect='/api/home/', store=dict(token=None, application=None))
+
+    def check_permission(self):
+        return self.request.user.is_authenticated
 
 class Icons(PublicEndpoint):
     class Meta:
         modal = True
         verbose_name = 'Icons'
 
     def get(self):
@@ -433,23 +436,42 @@
         modal = False
         verbose_name = 'Usuários'
 
     def get(self):
         return (
             super().get().search('username', 'email')
             .filters('is_superuser', 'is_active')
-            .fields('username', 'email', 'is_superuser')
+            .fields('username', 'email', 'is_superuser', 'get_roles')
             .actions('add', 'view', 'edit', 'delete', 'sendpushnotification', 'changepassword')
         )
     
-class ChangePassword(ChildInstanceFormEndpoint[ChangePasswordForm]):
+class ChangePassword(ChildInstanceEndpoint):
+    password = forms.CharField(label='Senha', required=False)
+
     class Meta:
         icon = 'user-lock'
         verbose_name = 'Alterar Senha'
 
+    def get(self):
+        return self.formfactory().fields('password')
+
+    def post(self):
+        self.instance.set_password(self.cleaned_data['password'])
+        self.instance.save()
+        return super().post()
+
+class Home(PublicEndpoint):
+    class Meta:
+        verbose_name = ''
+
+    def get(self):
+        cls = ENDPOINTS[APPLICATON['index']]
+        self.redirect(cls.get_api_url())
+
+
 class Dashboard(Endpoint):
     class Meta:
         verbose_name = ''
         
     def get(self):
         if self.request.user.is_authenticated:
             serializer = Serializer(request=self.request)
@@ -479,32 +501,36 @@
             self.redirect('/api/login/')
 
     def check_permission(self):
         return self.request.user.is_authenticated
     
 class Application(PublicEndpoint):
     def get(self):
+        user = None
         navbar = None
         menu = None
         icon = build_url(self.request, APPLICATON['logo'])
+        logo = build_url(self.request, APPLICATON['logo'])
         if self.request.user.is_authenticated:
-            logo = build_url(self.request, APPLICATON['logo'])
-            navbar = Navbar(
-                title=APPLICATON['title'], subtitle=APPLICATON['subtitle'],
-                logo=logo, user=self.request.user.username.split()[0].split('@')[0]
-            )
-            for entrypoint in ['usermenu', 'adder', 'settings', 'tools']:
-                if APPLICATON['dashboard'][entrypoint]:
-                    for endpoint in APPLICATON['dashboard'][entrypoint]:
-                        cls = ENDPOINTS[endpoint]
-                        if cls().instantiate(self.request, self).check_permission():
-                            label = cls.get_metadata('verbose_name')
-                            url = build_url(self.request, cls.get_api_url())
-                            modal = cls.get_metadata('modal', False)
-                            navbar.add_action(entrypoint, label, url, modal)
+            user = self.request.user.username.split()[0].split('@')[0]
+        navbar = Navbar(
+            title=APPLICATON['title'], subtitle=APPLICATON['subtitle'],
+            logo=logo, user=user
+        )
+        for entrypoint in ['actions', 'usermenu', 'adder', 'settings', 'tools']:
+            if APPLICATON['dashboard'][entrypoint]:
+                for endpoint in APPLICATON['dashboard'][entrypoint]:
+                    cls = ENDPOINTS[endpoint]
+                    if cls().instantiate(self.request, self).check_permission():
+                        label = cls.get_metadata('verbose_name')
+                        url = build_url(self.request, cls.get_api_url())
+                        modal = cls.get_metadata('modal', False)
+                        icon = cls.get_metadata('icon', None)
+                        navbar.add_action(entrypoint, label, url, modal, icon=icon)
+        if APPLICATON['menu']:
             items = []
             def get_item(k, v):
                 if isinstance(v, dict):
                     icon, label = k.split(':') if ':' in k else (None, k)
                     subitems = []
                     for k1, v1 in v.items():
                         subitem = get_item(k1, v1)
@@ -521,19 +547,20 @@
                             return dict(dict(label=label, url=url, icon=icon))
                     else:
                         print(v)
             for k, v in APPLICATON['menu'].items():
                 item = get_item(k, v)
                 if item:
                     items.append(item)
-            profile = Profile.objects.filter(user=self.request.user).first()
-            photo_url = profile.photo.url if profile and profile.photo else '/static/images/user.png'
-            menu = Menu(items, user=self.request.user.username, image=build_url(self.request, photo_url))
+            profile = Profile.objects.filter(user=self.request.user).first() if user else None
+            photo_url = profile.photo.url if profile and profile.photo else '/static/images/user.svg'
+            menu = Menu(items, user=user, image=build_url(self.request, photo_url))
+
         footer = Footer(APPLICATON['version'])
-        return Application_(icon=icon, navbar=navbar, menu=menu, footer=footer)
+        return Application_(icon=icon, navbar=navbar, menu=menu, footer=footer, oauth=oauth.providers())
     
 class Manifest(PublicEndpoint):
 
     class Meta:
         verbose_name = 'Manifest'
 
     def get(self):
@@ -574,23 +601,49 @@
     def check_permission(self):
         return True
     
 class PushSubscriptions(ListEndpoint[PushSubscription]):
     class Meta:
         verbose_name = 'Notificações'
 
-class SendPushNotification(ChildInstanceFormEndpoint[SendPushNotificationForm]):
+class SendPushNotification(ChildInstanceEndpoint):
+    message = forms.CharField(label='Texto', widget=forms.Textarea())
     class Meta:
         icon = 'mail-bulk'
         verbose_name = 'Enviar Notificação'
 
+    def get(self):
+        return self.formfactory().fields('message')
+
+    def post(self):
+        send_push_web_notification(self.instance, self.cleaned_data['message'])
+        return Response(message='Notificação enviada com sucesso.')
+
 class EditProfile(Endpoint):
+    password = forms.CharField(label='Senha', required=False)
+    password2 = forms.CharField(label='Confirmação', required=False)
+
     class Meta:
         verbose_name = 'Editar Perfil'
 
+    def __init__(self, *args, **kwargs):
+        self.instance = None
+        super().__init__(*args, **kwargs)
+       
     def get(self):
-        profile = Profile.objects.filter(user=self.request.user).first() or Profile(user=self.request.user)
-        return EditProfileForm(instance=profile, request=self.request)
+        self.instance = Profile.objects.filter(user=self.request.user).first() or Profile(user=self.request.user)
+        return (
+            self.formfactory(self.instance)
+            .fieldset('Dados Gerais', ('photo',))
+            .fieldset('Dados de Acesso', (('password', 'password2'),))
+        )
+    
+    def post(self):
+        self.instance.save()
+        if self.cleaned_data.get('password'):
+            self.instance.user.set_password(self.cleaned_data.get('password'))
+            self.instance.user.save()
+        return Response(message='Ação realizada com sucesso.', redirect='/api/dashboard/', store=dict(application=None))
 
     def check_permission(self):
         return self.request.user.is_authenticated
```

### Comparing `pyslth-0.2.7/slth/factory.py` & `pyslth-0.2.8/slth/factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,113 @@
+from django.db.models import Model
+from .serializer import Serializer
 class FormFactory:
-    def __init__(self, instance, delete=False):
+    def __init__(self, instance, endpoint=None, method='POST'):
         self._instance = instance
         self._fieldsets = {}
         self._values = {}
         self._fieldlist = []
-        self._serializer = None
+        self._display = {}
         self._title = None
         self._info = None
         self._actions = {}
-        self._delete = delete
+        self._initial = {}
+        self._choices = {}
         self._empty = False
+        self._method = method
+        self._hidden= []
+
+    def _append_field(self, field_name):
+        if ':' in field_name:
+            field_name, action_name = field_name.split(':')
+            self._actions[field_name] = action_name
+        self._fieldlist.append(field_name)
+        return field_name
 
     def fields(self, *names, **values) -> 'FormFactory':
         not_str = {name for name in names if not isinstance(name, str)}
         if not_str:
             self.fieldset('Dados Gerais', names)
         else:
-            self._fieldlist.extend(names)
+            for field_name in names:
+                self._append_field(field_name)
         for k in values:
-            self._fieldlist.append(k)
+            self._append_field(k)
             self.setvalue(**values)
         self._empty = not self._fieldlist
         return self
 
     def fieldset(self, title, fields) -> 'FormFactory':
-        self._fieldsets[title] = fields
+        self._fieldsets[title] = []
         for field in fields:
             if isinstance(field, str):
-                self._fieldlist.append(field)
+                self._fieldsets[title].append(self._append_field(field))
             else:
-                self._fieldlist.extend(field)
+                names = []
+                for field_name in field:
+                    names.append(self._append_field(field_name))
+                self._fieldsets[title].append(names)
         return self
     
-    def display(self, serializer) -> 'FormFactory':
-        self._serializer = serializer
+    def display(self, title, fields) -> 'FormFactory':
+        self._display[title] = fields
         return self
     
     def info(self, message) -> 'FormFactory':
         self._info = message
         return self
     
+    def initial(self, **kwargs) -> 'FormFactory':
+        self._initial.update(kwargs)
+        return self
+    
+    def choices(self, **kwargs) -> 'FormFactory':
+        self._choices.update(kwargs)
+        return self
+    
     def actions(self, **kwargs) -> 'FormFactory':
         self._actions.update(kwargs)
         return self
     
     def setvalue(self, **kwargs) -> 'FormFactory':
         self._values.update(kwargs)
         return self
     
     def settitle(self, title) -> 'FormFactory':
         self._title = title
         return self
-
-    def form(self, request):
-        from .forms import ModelForm, HiddenInput
-        class Form(ModelForm):
-            class Meta:
-                title = self._title or '{} {}'.format(
-                    'Excluir' if self._delete else ('Editar' if self._instance.pk else 'Cadastrar'),
-                    type(self._instance)._meta.verbose_name
-                )
-                model = type(self._instance)
-                fields = () if self._delete or self._empty else (self._fieldlist or '__all__')
     
-        form = Form(instance=self._instance, request=request, delete=self._delete)
+    def hidden(self, *names):
+        self._hidden.extend(names)
+        return self
+
+    def form(self, endpoint):
+        from .forms import ModelForm, Form
+        
+        if isinstance(self._instance, Model):
+            fieldlist = [field.name for field in type(self._instance)._meta.get_fields() if field.name in self._fieldlist]
+            class Form(ModelForm):
+                class Meta:
+                    model = type(self._instance)
+                    fields = () if self._empty else (fieldlist if self._fieldlist else '__all__')
+                
+        form = Form(instance=self._instance, endpoint=endpoint, initial=self._initial)
+        form._key = endpoint.get_api_name()
+        form._title = self._title
+        form._method = self._method
+        form._info = self._info
+        form._actions = self._actions
+        for name in self._fieldlist:
+            if name not in form.fields:
+                form.fields[name] = getattr(endpoint, name)
+        for name, queryset in self._choices.items():
+            form.fields[name].queryset = queryset
         form.fieldsets = self._fieldsets
-        if self._serializer:
-            form.display(self._serializer)
-        if self._info:
-            form.info(self._info)
-        if self._actions:
-            form.actions(**self._actions)
-        if self._values:
-            form.setvalue(**self._values)
+        form.setvalue(**self._values)
+        if self._display:
+            serializer = Serializer(self._instance, request=endpoint.request)
+            for title, fields in self._display.items():
+                serializer.fieldset(title, fields)
+            form._display = serializer
+        if self._hidden:
+            form.controller.hide(*self._hidden)
         return form
```

### Comparing `pyslth-0.2.7/slth/forms.py` & `pyslth-0.2.8/slth/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 
 import json
 from typing import Any
 import datetime
 from django.forms import *
 from django.utils.translation import gettext_lazy as _
-from django.contrib.auth import authenticate
-from django.contrib.auth.models import User
-from django.db.models.fields.files import FieldFile, ImageFieldFile
 from django.forms.models import ModelChoiceIterator, ModelMultipleChoiceField
 from django.db.models import Model, QuerySet, Manager
 from .models import Token, Profile
 from django.db import transaction
 from django.db.models import Manager
 from .exceptions import JsonResponseException
 from .utils import absolute_url, build_url
 from .serializer import Serializer
-from .components import Response
-from .notifications import send_push_web_notification
 from slth import ENDPOINTS
 
 
 DjangoModelForm = ModelForm
 DjangoForm = Form
 DjangoModelChoiceField = ModelChoiceField
 DjangoMultipleChoiceField = MultipleChoiceField
@@ -30,26 +25,93 @@
 
 MASKS = dict(
     cpf_cnpj='999.999.999-99|99.999.999/9999-99',
     cpf='999.999.999-99',
     cnpj='99.999.999/9999-99',
     telefone='(99) 99999-9999',
 )
+
+class FormController:
+
+    def __init__(self, form):
+        super().__init__()
+        self.form = form
+        self.controls = dict(hide=[], show=[], set={})
     
+    def hide(self, *names):
+        self.controls['hide'].extend(names)
+
+    def show(self, *names):
+        self.controls['show'].extend(names)
+
+    def set(self, **kwargs):
+        for k, v in kwargs.items():
+            if isinstance(v, Model):
+                v = dict(id=v.id, value=str(v))
+            elif isinstance(v, QuerySet) or isinstance(v, Manager):
+                v = [dict(id=v.id, value=str(v)) for v in v]
+            elif isinstance(v, bool):
+                v = str(v).lower()
+            elif isinstance(v, datetime.datetime):
+                v = v.strftime('%Y-%m-%d %H:%M')
+            elif isinstance(v, datetime.date):
+                v = v.strftime('%Y-%m-%d')
+            self.controls['set'][k] = v
+
+    def get(self, name, value, default=None):
+        if value is None:
+            return default
+        else:
+            try:
+                value = self.form.fields[name].to_python(value)
+            except KeyError:
+                pass
+            except ValidationError:
+                pass
+            return default if value is None else value
+        
+    def clear(self):
+        self.controls['show'].clear()
+        self.controls['hide'].clear()
+        self.controls['set'].clear()
+
+    def on_change(self, field_name):
+        self.clear()
+        getattr(self.form._endpoint, f'on_{field_name}_change')(self, self.values())
+        return self.controls
+    
+    def get_field_queryset(self, fname, qs):
+        method_attr = None
+        method_name = f'get_{fname}_queryset'
+        if hasattr(self.form._endpoint, method_name):
+            method_attr = getattr(self.form._endpoint, method_name)
+        elif hasattr(self.form, 'instance') and hasattr(self.form.instance, method_name):
+            method_attr = getattr(self.form.instance, method_name)
+
+        if method_attr:
+            qs = method_attr(qs, self.values())
+        return qs
+    
+    def values(self):
+        data = dict(**self.controls['set'])
+        for name in self.form.fields:
+            value = self.get(name, self.form.request.GET.get(name))
+            if value:
+                data[name] = value
+        return data
 
 class FormMixin:
 
     def fieldset(self, title, fields):
         self.fieldsets[title] = fields
         return self
 
     def parse_json(self):
         content_type = self.request.META.get('CONTENT_TYPE')
         method = self.request.method.lower()
-        # 'application/x-www-form-urlencoded'
         if content_type and content_type.lower() in 'application/json':
             if method == 'get' or method == 'post':
                 d1 = json.loads(self.request.body.decode()) if self.request.body else {}
                 d2 = self.request.GET if method == 'get' else self.request.POST
                 d2._mutable = True
                 d2.clear()
                 for k, v in d1.items():
@@ -68,53 +130,40 @@
                         d2[k] = v
                 d2._mutable = False
 
     @classmethod
     def get_metadata(cls, name, default=None):
         metaclass = getattr(cls, 'Meta', None)
         return getattr(metaclass, name, default) if metaclass else default
-    
-    def on_change(self, field_name):
-        self.controls['show'].clear()
-        self.controls['hide'].clear()
-        self.controls['set'].clear()
-        values = {}
-        for name2 in self.fields:
-            value2 = self.getdata(name2, self.request.POST.get(name2))
-            if value2:
-                values[name2] = value2
-        getattr(self, f'on_{field_name}_change')(values)
-        return self.controls
 
     def serialize(self):
         return self.to_dict()
-        # try:
-        #     return self.to_dict()
-        # except JsonResponseException as e:
-        #     return e.data
         
     def display(self, serializable):
-        self.display_data = serializable
+        self._display = serializable
         return self
 
     def to_dict(self, prefix=None):
+        field_name = self.request.GET.get('on_change')
+        if field_name:
+            raise JsonResponseException(self.controller.on_change(field_name))
+        
         data = dict(
-            type='form', title=self.get_metadata('title', self._title), icon=self.get_metadata('icon'),
+            type='form', key=self._key, method=self._method, title=self.get_metadata('title', self._title), icon=self.get_metadata('icon'),
             style=self.get_metadata('style'), url=absolute_url(self.request), info=self._info
         )
-        data.update(controls=self.controls, width=self.get_metadata('width', '100%'))
-        if self.display_data:
-            if isinstance(self.display_data, Serializer):
-                # self.display_data.request = self.request
-                data.update(display=self.display_data.serialize(forward_exception=True)['data'])
+        data.update(controls=self.controller.controls, width=self.get_metadata('width', '100%'))
+        if self._display:
+            if isinstance(self._display, Serializer):
+                # self._display.request = self.request
+                data.update(display=self._display.serialize(forward_exception=True)['data'])
         choices_field_name = self.request.GET.get('choices')
-        fieldsets = self.get_fieldsets()
-        if fieldsets:
+        if self.fieldsets:
             fieldsetlist = []
-            for title, names in fieldsets.items():
+            for title, names in self.fieldsets.items():
                 fields = []
                 if prefix:
                     value = self.instance.pk if isinstance(self, ModelForm) else ''
                     fields.append([dict(type='hidden', name=f'{prefix}__id', value=value, label='ID')])
                 for name in names:
                     if isinstance(name, str):
                         field = self.serialize_field(name, self.fields[name], prefix, choices_field_name)
@@ -146,20 +195,21 @@
             if isinstance(self, ModelForm):
                 if isinstance(field, OneToOneField):
                     instances.append(getattr(self.instance, name) if self.instance.id else None)
                 elif isinstance(field, OneToManyField):
                     instances.extend(getattr(self.instance, name).all() if self.instance.id else ())
             for i, instance in enumerate(instances):
                 prefix = name if is_one_to_one else f'{name}__{i}'
-                kwargs = dict(instance=instance, request=self.request) if isinstance(field, InlineModelField) else dict(request=self.request)
+                kwargs = dict(instance=instance, request=self.request) if isinstance(field, InlineModelField) else dict(endpoint=self._endpoint)
                 value.append(field.form(**kwargs).to_dict(prefix=prefix))
             if not is_one_to_one:
-                value.append(field.form(request=self.request).to_dict(prefix=f'{name}__n'))
+                value.append(field.form(endpoint=self._endpoint).to_dict(prefix=f'{name}__n'))
             required = getattr(field, 'required2', field.required)
-            data = dict(type='inline', min=field.min, max=field.max, name=name, count=len(instances), label=field.label, required=required, value=value)
+            label = field.label.title() if field.label else field.label
+            data = dict(type='inline', min=field.min, max=field.max, name=name, count=len(instances), label=label, required=required, value=value)
         else:
             extra = {}
             ftype = FIELD_TYPES.get(type(field).__name__, 'text')
             if name in self._values:
                 ftype = 'hidden'
                 value = self._values[name]
                 value = value.pk if isinstance(value, Model) else value
@@ -207,55 +257,35 @@
                 if name in self.request.GET:
                     data.update(type='hidden', value=self.request.GET[name])
                 else:
                     pick = getattr(field, 'pick', False)
                     if isinstance(field.choices, ModelChoiceIterator) and not pick:
                         if choices_field_name == fname:
                             qs = field.choices.queryset
-                            
-                            method_attr = None
-                            method_name = f'get_{fname}_queryset'
-                            if hasattr(self, method_name):
-                                method_attr = getattr(self, method_name)
-                            elif hasattr(self, 'instance') and hasattr(self.instance, method_name):
-                                method_attr = getattr(self.instance, method_name)
-
-                            if method_attr:
-                                values = dict(user=self.request.user)
-                                values.update(**self._values)
-                                for name2 in self.fields:
-                                    value2 = self.getdata(name2, self.request.GET.get(name2))
-                                    if value2:
-                                        values[name2] = value2
-                                qs = method_attr(qs, values)
-                            
+                            qs = self.controller.get_field_queryset(fname, qs)
                             if 'term' in self.request.GET:
                                 qs = qs.apply_search(self.request.GET['term'])
                             raise JsonResponseException([dict(id=obj.id, value=str(obj)) for obj in qs[0:10]])
                         else:
                             data['choices'] = absolute_url(self.request, f'choices={fname}')
                     else:
                         data['choices'] = [dict(id=str(k), value=v) for k, v in field.choices]
                     if pick:
                         data.update(pick=True)
                     
         attr_name = f'on_{name}_change'
-        if hasattr(self, attr_name):
+        if hasattr(self._endpoint, attr_name):
             data['onchange'] = absolute_url(self.request, f'on_change={name}')
         if name in self._actions:
             cls = ENDPOINTS[self._actions[name]]
             if cls.instantiate(self.request, self).check_permission():
                 data.update(action=cls.get_api_metadata(self.request, absolute_url(self.request)))
         return data
     
-    def post(self):
-        field_name = self.request.GET.get('on_change')
-        if field_name:
-            return self.on_change(field_name)
-
+    def submit(self):
         data = {}
         errors = {}
         inline_fields = {name: field for name, field in self.fields.items() if isinstance(field, InlineFormField) or isinstance(field, InlineModelField)}
         self.is_valid()
         errors.update(self.errors)
         for inline_field_name, inline_field in inline_fields.items():
             data[inline_field_name] = []
@@ -283,134 +313,97 @@
                             if isinstance(inline_form, DjangoModelForm):
                                 data[inline_field_name].append(inline_form.instance)
                             else:
                                 data[inline_field_name].append(inline_form.cleaned_data)
                         else:
                             errors.update({f'{prefix}__{name}': error for name, error in inline_form.errors.items()}) 
         if errors:
-            return dict(type='error', text='Please correct the errors.', errors=errors)
+            raise JsonResponseException(dict(type='error', text='Por favor, corrija os erros.', errors=errors))
         else:
             data.update({field_name: self.cleaned_data.get(field_name) for field_name in self.fields if field_name not in inline_fields})
             with transaction.atomic():
                 self.cleaned_data = data
                 if isinstance(self, DjangoModelForm):
                     for inline_field_name in inline_fields:
                         for obj in self.cleaned_data[inline_field_name]:
                             obj.save()
                             # set one-to-one
                             if hasattr(self.instance, f'{inline_field_name}_id'):
                                 if hasattr(obj, 'deleting'):
                                     setattr(self.instance, inline_field_name, None)
                                 else:
                                     setattr(self.instance, inline_field_name, obj)
-                    response = self.submit()
+                    self.save()
                     for inline_field_name in inline_fields:
                         for obj in self.cleaned_data[inline_field_name]:
                             if hasattr(obj, 'deleting'):
                                 obj.delete()
-                else:
-                    response = self.submit()
-            return response
-                
-    def hide(self, *names):
-        self.controls['hide'].extend(names)
-
-    def show(self, *names):
-        self.controls['show'].extend(names)
-
-    def setdata(self, **kwargs):
-        for k, v in kwargs.items():
-            if isinstance(v, Model):
-                v = dict(id=v.id, value=str(v))
-            elif isinstance(v, QuerySet) or isinstance(v, Manager):
-                v = [dict(id=v.id, value=str(v)) for v in v]
-            elif isinstance(v, bool):
-                v = str(v).lower()
-            elif isinstance(v, datetime.datetime):
-                v = v.strftime('%Y-%m-%d %H:%M')
-            elif isinstance(v, datetime.date):
-                v = v.strftime('%Y-%m-%d')
-            self.controls['set'][k] = v
-
-    def getdata(self, name, value, default=None):
-        if value is None:
-            return default
-        else:
-            try:
-                value = self.fields[name].to_python(value)
-            except KeyError:
-                pass
-            except ValidationError:
-                pass
-            return default if value is None else value
+                return self.cleaned_data
 
     def settitle(self, title):
         self._title = title 
         return self
     
     def setvalue(self, **kwargs):
         self._values.update(**kwargs)
+        return self
+    
+    def actions(self, **kwargs):
+        self._actions.update(kwargs)
+        return self
     
 
 class Form(DjangoForm, FormMixin):
     
-    def __init__(self, *args, request=None, endpoint=None, **kwargs):
-        self.fieldsets = {}
-        self.fields = dict(self.fieldsets)
-        self.display_data = []
-        self.controls = dict(hide=[], show=[], set={})
-        self.instance = kwargs.pop('instance', None)
-        self.endpoint = endpoint
-        self.request = request
+    def __init__(self, *args, endpoint=None, **kwargs):
+        self._display = []
+        self._endpoint = endpoint
         self._info = None
         self._values = {}
         self._title = type(self).__name__
         self._actions = {}
+        self._method = 'POST'
+        self._key = self._title.lower()
+
+        self.fieldsets = {}
+        self.fields = {}
+        self.request = endpoint.request
+        self.controller = FormController(self)
+        self.instance = kwargs.pop('instance', None)
+
         self.parse_json()
         if 'data' not in kwargs:
             if self.request.method.upper() == 'GET':
                 data = self.request.GET or None
             elif self.request.method.upper() == 'POST':
                 data = self.request.POST or {}
         else:
             data = kwargs['data']
         kwargs.update(data=data)
         if self.request:
             kwargs.update(files=self.request.FILES or None)
         super().__init__(*args, **kwargs)
 
-    def submit(self):
-        pass
-
-    def get_fieldsets(self):
-        return self.fieldsets
-    
-    def info(self, message):
-        self._info = message
-        return self
-    
-    def actions(self, **kwargs):
-        self._actions.update(kwargs)
-        return self
-
 
 class ModelForm(DjangoModelForm, FormMixin):
 
-    def __init__(self, instance=None, request=None, endpoint=None, delete=False, **kwargs):
-        self.fieldsets = {}
-        self.display_data = []
-        self.controls = dict(hide=[], show=[], set={})
-        self.request = request
-        self.endpoint = endpoint
-        self.endpoint = kwargs.pop('endpoint', None)
-        self.delete = delete
+    def __init__(self, instance=None, endpoint=None, **kwargs):
+        self._display = []
+        self._endpoint = endpoint
         self._info = None
         self._values = {}
         self._title = type(self).__name__
         self._actions = {}
+        self._method = 'POST'
+        self._key = self._title.lower()
+
+        self.fieldsets = {}
+        self.request = endpoint.request
+        self.controller = FormController(self)
+        
         self.parse_json()
         if 'data' not in kwargs:
             if self.request.method.upper() == 'GET':
                 data = self.request.GET or None
             elif self.request.method.upper() == 'POST':
                 data = self.request.POST or {}
             else:
@@ -418,29 +411,14 @@
         else:
             data = kwargs['data']
         kwargs.update(data=data)
         if self.request:
             kwargs.update(files=self.request.FILES or None)
         super().__init__(instance=instance, **kwargs)
 
-    def submit(self):
-        self.instance.delete() if self.delete else self.save()
-        return Response(message='Ação realizada com sucesso')
-
-    def get_fieldsets(self):
-        return self.fieldsets
-    
-    def info(self, message):
-        self._info = message
-        return self
-    
-    def actions(self, **kwargs):
-        self._actions.update(kwargs)
-        return self
-
 class InlineFormField(Field):
     def __init__(self, *args, form=None, min=1, max=3, **kwargs):
         self.form = form
         self.max = max
         self.min = min
         super().__init__(*args,  **kwargs)
         self.required = False
@@ -454,15 +432,15 @@
             field_names = []
             for field_name in fields:
                 if isinstance(field_name, str):
                     field_names.append(field_names)
                 else:
                     field_names.extend(field_name)
             self.form = modelform_factory(model, form=ModelForm, fields=field_names, exclude=exclude)
-            self.form.get_fieldsets = lambda _self: {None: fields}
+            self.form.fieldsets = {None: fields}
         self.max = max
         self.min = min
         super().__init__(*args,  **kwargs)
         self.required = False
 
 
 class OneToManyField(InlineModelField):
@@ -517,86 +495,15 @@
         super().__init__(*args, **kwargs)
 
 class ModelMultipleChoiceField(ModelMultipleChoiceField):
     
     def __init__(self, *args, **kwargs):
         self.pick = kwargs.pop('pick', False)
         super().__init__(*args, **kwargs)
-
-class LoginForm(Form):
-    username = CharField(label=_('Username'))
-    password = CharField(label=_('Password'))
-
-    class Meta:
-        title = 'Acesso ao Sistema'
-        width = 350
-
-    def __init__(self, *args, **kwargs):
-        self.token = None
-        super().__init__(*args, **kwargs)
-
-    def clean(self):
-        cleaned_data = super().clean()
-        user = authenticate(self.request, username=cleaned_data.get('username'), password=cleaned_data.get('password'))
-        if user is None:
-            raise ValidationError(_('Username or password are incorect'))
-        else:
-            self.token = Token.objects.create(user=user)
-            return cleaned_data
         
-    def submit(self):
-        return Response(message='Bem-vindo!', redirect='/api/dashboard/', store=dict(token=self.token.key, application=None))
-
-class ChangePasswordForm(ModelForm):
-    password = CharField(label=_('Senha'), required=False)
-    class Meta:
-        title = 'Alterar Senha'
-        model = User
-        fields = ()
-
-    def submit(self):
-        self.instance.set_password(self.cleaned_data['password'])
-        return super().submit()
-
-
-class EditProfileForm(ModelForm):
-    password = CharField(label=_('Senha'), required=False)
-    password2 = CharField(label=_('Confirmação'), required=False)
-
-    class Meta:
-        title = 'Editar Perfil'
-        model = Profile
-        fields = 'photo',
-
-    def get_fieldsets(self):
-        return {
-            'Dados Gerais': ('photo',),
-            'Dados de Acesso': (('password', 'password2'),)
-        }
-
-    def clean_password(self):
-        password = self.data.get('password')
-        password2 = self.data.get('password2')
-        if password and password != password2:
-            raise ValidationError('As senhas devem ser iguais.')
-        return password
-        
-    def submit(self):
-        self.save()
-        self.instance.user.set_password(self.cleaned_data.get('password'))
-        self.instance.user.save()
-        return Response(message='Ação realizada com sucesso.', redirect='/api/dashboard/', store=dict(application=None))
-
-class SendPushNotificationForm(Form):
-    message = CharField(label='Text', widget=Textarea())
-
-    def submit(self):
-        send_push_web_notification(self.instance, self.cleaned_data['message'])
-        return Response(message='Notificação enviada com sucesso.')
-
 
 FIELD_TYPES = {
     'CharField': 'text',
     'EmailField': 'email',
     'DecimalField': 'decimal',
     'BooleanField': 'boolean',
     'DateTimeField': 'datetime',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyslth-0.2.7/slth/management/commands/integration_test.py` & `pyslth-0.2.8/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/management/commands/sync.py` & `pyslth-0.2.8/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/migrations/0001_initial.py` & `pyslth-0.2.8/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.2.8/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.2.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/migrations/0006_user.py` & `pyslth-0.2.8/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/models.py` & `pyslth-0.2.8/slth/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,25 +165,27 @@
         verbose_name = 'Usuário'
         verbose_name_plural = 'Usuários'
 
     def formfactory(self):
         return (
             super().formfactory()
             .fieldset('Dados Gerais', (('first_name', 'last_name'), 'email'))
-            .fieldset('Dados de Acesso', (('is_superuser', 'is_active'),))
+            .fieldset('Dados de Acesso', ('username', ('is_superuser', 'is_active'),))
         )
     
     def serializer(self):
         return (
             super().serializer()
             .fieldset('Dados Gerais', (('first_name', 'last_name'), 'email'))
-            .fieldset('Dados de Acesso', (('is_superuser', 'is_active'),))
+            .fieldset('Dados de Acesso', ('username', ('is_superuser', 'is_active'),))
             .queryset('Notificação', 'get_push_subscriptions')
             .queryset('Papéis', 'get_roles')
         )
     
+    @meta('Inscrições de Notificação')
     def get_push_subscriptions(self):
         return self.pushsubscription_set.fields('device')
     
+    @meta('Papéis')
     def get_roles(self):
         return Role.objects.filter(username=self.username).fields('get_description')
```

### Comparing `pyslth-0.2.7/slth/permissions.py` & `pyslth-0.2.8/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/queryset.py` & `pyslth-0.2.8/slth/queryset.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,16 @@
         template = None
         calendar = None
 
         instance_actions = []
         queryset_actions = []
 
         base_url = append_url(build_url(self.request), 'only={}'.format(attrname) if attrname else '')
+        if self.request.GET.urlencode():
+            base_url = append_url(base_url, self.request.GET.urlencode())
 
         for qualified_name in self.metadata.get('actions', ()):
             cls = slth.ENDPOINTS[qualified_name]
             if cls.has_args():
                 instance_actions.append(cls)
             else:
                 queryset_actions.append(cls)
@@ -419,15 +421,15 @@
                 field_type = 'choice'
                 choices = append_url(base_url, f'choices={name}')
             if getattr(field, 'choices'):
                 field_type = 'choice'
                 choices = [{'id': '', 'value':''}]
                 choices.extend([{'id': k, 'value': v} for k, v in field.choices])
                 choices.append({'id': 'null', 'value':'Nulo'})
-            data = dict(name=name, type=field_type, value=value, label=str(field.verbose_name), required=False, mask=None)
+            data = dict(name=name, type=field_type, value=value, label=str(field.verbose_name).title(), required=False, mask=None)
             if choices:
                 data.update(choices=choices)
             return data
         return None
 
     def to_calendar(self, attr_name):
         today = date.today()
```

### Comparing `pyslth-0.2.7/slth/roles.py` & `pyslth-0.2.8/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/selenium/__init__.py` & `pyslth-0.2.8/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/selenium/browser.py` & `pyslth-0.2.8/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/serializer.py` & `pyslth-0.2.8/slth/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,45 +47,42 @@
         return str(obj)
     elif hasattr(obj, 'serialize'):
         return obj.serialize()
     return str(obj)
 
 def getfield(obj, name_or_names, request=None):
     if isinstance(name_or_names, str):
+        if ':' in name_or_names:
+            name_or_names, action_name = name_or_names.split(':')
+        else:
+            name_or_names, action_name = name_or_names, None
         attr = getattr(obj, name_or_names)
         if type(attr) == types.MethodType:
             value = attr()
             label = getattr(attr, 'verbose_name', name_or_names.replace('get_', ''))
         elif name_or_names.startswith('get_') and name_or_names.endswith('_display'):
             value = attr()
             label = getattr(type(obj), name_or_names[4:-8]).field.verbose_name
         else:
             value = attr
             label = getattr(type(obj), name_or_names).field.verbose_name
         label = label.title().replace('_', ' ') if label and label.islower() else label
         field = dict(type='field', name=name_or_names, label=label, value=serialize(value, primitive=True, request=request))
-        return field
-    elif isinstance(name_or_names, LinkField):
-        value = getattr(obj, name_or_names.name) if obj else None
-        field = dict(type='field', name=name_or_names.name, value=serialize(value, primitive=True))
-        if value:
-            if name_or_names.endpoint(value.id).contextualize(request).check_permission():
-                field.update(url=name_or_names.endpoint.get_api_url(value.id))
+        if action_name:
+            cls = slth.ENDPOINTS[action_name]
+            endpoint = cls.instantiate(request, obj)
+            if endpoint.check_permission():
+                field.update(url=endpoint.get_api_url(obj.id))
         return field
     else:
         fields = []
         for name in name_or_names:
             fields.append(getfield(obj, name, request))
         return fields
 
-class LinkField:
-    def __init__(self, name, endpoint):
-        self.name = name
-        self.endpoint = endpoint
-
 
 class Serializer:
     def __init__(self, obj=None, request=None, serializer=None, type='object', title=None):
         self.path = serializer.path.copy() if serializer else []
         self.obj = obj
         self.lazy = False
         self.ignore_only = False
@@ -263,15 +260,15 @@
                     cls = item['cls']
                     wrap = item['wrap']
                     if not only or key in only:
                         returned = {}
                         endpoint = cls.instantiate(self.request, self.obj)
                         if endpoint.check_permission():
                             if not lazy:
-                                returned = endpoint.getdata()
+                                returned = endpoint.process()
                             path = self.path + [key]
                             if wrap:
                                 data = dict(type='fieldset', key=key, title=title, url=None, data=serialize(returned))
                             else:
                                 data = serialize(returned)
                                 data['title'] = title
                             if isinstance(data, dict):
```

### Comparing `pyslth-0.2.7/slth/static/css/.DS_Store` & `pyslth-0.2.8/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/css/fontawesome.min.css` & `pyslth-0.2.8/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/css/fonts/.DS_Store` & `pyslth-0.2.8/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.2.8/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.2.8/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.2.8/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.2.8/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/css/slth.css` & `pyslth-0.2.8/slth/static/css/slth.css`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,23 @@
   }
   input[type="checkbox"]::before, input[type="radio"]::before {
     content: "";
     width: 0.65em;
     height: 0.65em;
     transform: scale(0);
     transition: 120ms transform ease-in-out;
-    box-shadow: inset 1em 1em #383838;
+    box-shadow: inset 1em 1em var(--primary-color);
   }
   input[type="checkbox"]:checked::before {
     transform: scale(1);
   }
   input[type="radio"]:checked::before {
     transform: scale(1);
     border-radius: 50%;
   }
+
+  form.login {
+    width: 350px;
+  }
+  form.login h1{
+    text-align: center;
+  }
```

### Comparing `pyslth-0.2.7/slth/static/css/solid.min.css` & `pyslth-0.2.8/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/images/logo.png` & `pyslth-0.2.8/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/images/logo.svg` & `pyslth-0.2.8/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/images/user.png` & `pyslth-0.2.8/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/echarts.min.js` & `pyslth-0.2.8/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/index.min.js` & `pyslth-0.2.8/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/ios-splash.min.js` & `pyslth-0.2.8/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/peerjs.min.js` & `pyslth-0.2.8/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/qrcode.min.js` & `pyslth-0.2.8/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/react-trigger-change.js` & `pyslth-0.2.8/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/react.min.js` & `pyslth-0.2.8/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/slth.min.js` & `pyslth-0.2.8/slth/static/js/slth.min.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,132 +1,165 @@
 import {
     j as t,
-    c as P,
-    r as M,
-    R as Ie
+    c as H,
+    r as I,
+    R as Be
 } from "./react.min.js";
+const C = {
+    colors: {
+        primary: "var(--primary-color)",
+        success: "var(--success-color)",
+        warning: "var(--warning-color)",
+        info: "var(--info-color)",
+        danger: "var(--danger-color)",
+        highlight: "var(--highlight-color)",
+        seconday: "var(--seconday-color)",
+        auxiliary: "var(--auxiliary-color)"
+    },
+    border: {
+        radius: "var(--border-radius)"
+    },
+    background: {
+        info: "var(--info-background)"
+    }
+};
+
+function De(e) {
+    function n() {
+        const a = {
+            width: 30,
+            height: 30,
+            borderRadius: "50%",
+            backgroundColor: e.data.value
+        };
+        return t.jsx("div", {
+            style: a
+        })
+    }
+    return n()
+}
 
-function Be(e) {
+function Le(e) {
     function n(r) {
-        navigator.clipboard.writeText(r), ee('Icon "' + r + '" copied to clipboard!')
+        navigator.clipboard.writeText(r), te('Icon "' + r + '" copied to clipboard!')
     }
     const a = {
         display: "inline-block",
         width: 150,
         textAlign: "center",
         cursor: "pointer"
     };
     return t.jsx("div", {
         style: {
             marginTop: 30
         },
-        children: Le.map(r => t.jsxs("div", {
+        children: qe.map(r => t.jsxs("div", {
             className: "icon-box",
             onClick: () => n(r),
             style: a,
             children: [t.jsx("i", {
                 className: "fa-solid fa-fw fa-" + r
             }), t.jsx("div", {
                 className: "icon-text",
                 children: r
             })]
         }, Math.random()))
     })
 }
 
-function De(e) {
+function Ae(e) {
     function n() {
         return t.jsx("i", {
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function k(e) {
+function S(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
 
-function ue(e) {
+function he(e) {
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
-        return e.primary && (a.backgroundColor = "#1351b4", a.color = "white"), e.default && (a.color = "#1351b4", a.border = "solid 1px #1351b4"), t.jsx("a", {
+        return e.primary && (a.backgroundColor = C.colors.primary, a.color = "white"), e.default && (a.color = C.colors.primary, a.border = "solid 1px " + C.colors.primary), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(k, {
+            children: t.jsx(S, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
-const Le = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
+const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
-function Ae(e) {
+function Re(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
-            backgroundColor: e.isError ? "#e52207" : "#1151b3",
+            backgroundColor: e.isError ? "#e52207" : C.colors.primary,
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(k, {
+            children: [t.jsx(S, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
-function ee(e, n = !1) {
+function te(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), P.createRoot(document.body.appendChild(a)).render(t.jsx(Ae, {
+    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(Re, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function xe() {
+function ye() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
-function le(e) {
+function oe(e) {
     function n() {
         const a = {
-            color: "#155bcb",
-            backgroundColor: "#d4e5ff",
+            color: C.colors.info,
+            backgroundColor: C.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
@@ -137,66 +170,66 @@
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function qe(e) {
-    return ye(e.data)
+function Ne(e) {
+    return ve(e.data)
 }
 
 function q(e) {
     return e.replace("/app/", "/api/")
 }
 
-function H(e) {
+function U(e) {
     return e.replace("/api/", "/app/")
 }
 
-function I(e, n, a, r) {
+function B(e, n, a, r) {
     const d = localStorage.getItem("token");
     var i = {
         Accept: "application/json"
     };
     d && (i.Authorization = "Token " + d);
-    const o = q(n);
+    const l = q(n);
     var s = {
         method: e,
         headers: new Headers(i),
         ajax: 1
     };
     r && (s.body = r);
     var c = null,
         u = null;
-    fetch(o, s).then(function(l) {
-        if (c = l, u = c.headers.get("Content-Type"), u == "application/json") return l.text();
-        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return l.arrayBuffer();
-        l.text()
-    }).then(l => {
+    fetch(l, s).then(function(o) {
+        if (c = o, u = c.headers.get("Content-Type"), u == "application/json") return o.text();
+        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
+        o.text()
+    }).then(o => {
         if (u == "application/json") {
-            var m = JSON.parse(l || "{}");
-            typeof m == "object" && m.type == "redirect" ? document.location.href = H(m.url) : a && a(m, c)
+            var h = JSON.parse(o || "{}");
+            typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, c)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var x = window.URL.createObjectURL(new Blob([new Uint8Array(l)], {
+            var f = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
                     type: u
                 })),
                 w = document.createElement("a");
-            w.href = x, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, c)
-        } else a && a(l, c)
+            w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, c)
+        } else a && a(o, c)
     })
 }
 
-function ye(e) {
+function ve(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
-    }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = H(e.redirect)) : e.message && ee(e.message)
+    }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = U(e.redirect)) : e.message && te(e.message)
 }
 
-function U(e) {
+function z(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
         var n = e.toString().split(".");
         return n.length == 1 ? e.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".") : (n[0] = n[0].toString().replace(/\B(?=(\d{3})+(?!\d))/g, "."), n[1] = n[1].substring(0, 2), n[1].length == 1 && (n[1] = n[1] + "0"), n[0] + "," + n[1])
     }
@@ -226,108 +259,109 @@
                 children: d
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function pe() {
-    document.querySelector(".layer") == null && P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Re, {}))
+    document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {}))
 }
 
-function ve(e, n) {
-    xe(), pe(), window.reloader = n;
+function be(e, n) {
+    ye(), pe(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ne, {
+    H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
         url: q(e)
     }))
 }
 
 function Oe(e) {
-    xe(), pe(), P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
+    ye(), pe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         url: q(e)
     }))
 }
 
-function V(e) {
+function J(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
-function Re(e) {
+function _e(e) {
     const n = {
         backgroundColor: "black",
         bottom: 0,
         left: 0,
         position: "fixed",
         right: 0,
         top: 0,
         opacity: .7,
         display: "none"
     };
     return t.jsx("div", {
         className: "layer",
         onClick: function() {
-            V()
+            J()
         },
         style: n
     })
 }
 
-function Ne(e) {
-    const [n, a] = M.useState(null), [r, d] = M.useState(0);
-    M.useEffect(() => {
+function Fe(e) {
+    const [n, a] = I.useState(null), [r, d] = I.useState(0);
+    I.useEffect(() => {
         i(q(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function i(c) {
-        I("GET", q(c), function(u) {
+        B("GET", q(c), function(u) {
             a(u), d(r + 1)
         })
     }
 
-    function o() {
+    function l() {
         const c = {
                 maxWidth: 800
             },
             u = {
                 textAlign: "right",
-                cursor: "pointer"
+                cursor: "pointer",
+                marginTop: -15
             };
         if (n) return t.jsxs("div", {
             style: c,
             children: [t.jsx("div", {
                 style: u,
-                children: t.jsx(k, {
+                children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => V()
+                    onClick: () => J()
                 })
             }), t.jsx(p, {
                 data: n
             })]
         })
     }
     const s = {
         minWidth: "50%",
         display: n ? "block" : "none",
         maxWidth: "90%",
         top: window.scrollY + 40
     };
     return t.jsx("dialog", {
         style: s,
-        children: o()
+        children: l()
     }, r)
 }
 
-function _e(e) {
+function ze(e) {
     var n = Math.random();
-    M.useEffect(() => {
+    I.useEffect(() => {
         document.querySelector(".layer").style.display = "block";
         var r = document.getElementById(n);
         r.style.top = document.documentElement.scrollTop + 100
     }, []);
 
     function a() {
         const r = {
@@ -342,166 +376,166 @@
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
                 style: d,
-                children: t.jsx(k, {
+                children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => V()
+                    onClick: () => J()
                 })
             }), t.jsx("iframe", {
                 src: q(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
     }
     return a()
 }
 
-function C(e) {
+function T(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
-function N(e) {
+function _(e) {
     const n = e.id || Math.random(),
-        [a, r] = M.useState(e.data.name);
+        [a, r] = I.useState(e.data.name);
 
     function d(s) {
-        s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(H(e.data.url)) : ve(e.data.url)
+        s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(U(e.data.url)) : be(e.data.url)
     }
 
     function i() {
-        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(k, {
+        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(S, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(k, {
+            children: [t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
 
-    function o() {
+    function l() {
         var s = {
             padding: 12,
             textDecoration: "none",
             borderRadius: 5,
             margin: 5
         };
-        return e.primary && (s.backgroundColor = "#1351b4", s.color = "white"), e.default && (s.border = "solid 1px #1351b4", s.color = "#1351b4"), e.style && Object.keys(e.style).map(function(c) {
+        return e.primary && (s.backgroundColor = C.colors.primary, s.color = "white"), e.default && (s.border = "solid 1px " + C.colors.primary, s.color = C.colors.primary), e.style && Object.keys(e.style).map(function(c) {
             s[c] = e.style[c]
         }), t.jsx("a", {
             id: n,
-            href: H(e.data.url) || "#",
+            href: U(e.data.url) || "#",
             onClick: d,
             style: s,
-            "data-label": C(e.data.name),
+            "data-label": T(e.data.name),
             children: i()
         })
     }
-    return o()
+    return l()
 }
 
 function X(e) {
     function n(i) {
-        var o = i.target.parentNode.querySelector(".dropdown");
-        return o == null && (o = i.target.parentNode.parentNode.querySelector(".dropdown")), o == null && (o = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), o
+        var l = i.target.parentNode.querySelector(".dropdown");
+        return l == null && (l = i.target.parentNode.parentNode.querySelector(".dropdown")), l == null && (l = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), l
     }
 
     function a(i) {
-        const o = i.target.getBoundingClientRect(),
+        const l = i.target.getBoundingClientRect(),
             s = n(i);
-        document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), s.style.left = o.left - 150 + o.width + "px", s.style.display = "block"
+        document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), s.style.left = l.left - 150 + l.width + "px", s.style.display = "block"
     }
 
     function r(i) {
-        const o = n(i);
-        o.style.display = "none"
+        const l = n(i);
+        l.style.display = "none"
     }
 
     function d() {
         const i = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
                 boxShadow: "15px 15px 10px -15px #DDD",
                 display: "none"
             },
-            o = {
+            l = {
                 listStyleType: "none",
                 padding: 10
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
-                "data-label": C(e.dataLabel),
+                "data-label": T(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: i,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(s => t.jsx("li", {
-                    style: o,
-                    children: t.jsx(N, {
+                    style: l,
+                    children: t.jsx(_, {
                         data: s,
                         style: {
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
     return d()
 }
 
-function W({
+function N({
     id: e,
     href: n,
     modal: a,
     imodal: r,
     children: d,
     onClick: i,
-    dataLabel: o,
+    dataLabel: l,
     style: s
 }) {
-    const c = n && n.indexOf("/media/") < 0 ? H(n) : n;
+    const c = n && n.indexOf("/media/") < 0 ? U(n) : n;
 
-    function u(m) {
-        m.preventDefault(), a ? ve(c) : r ? Oe(c) : window.load(c)
+    function u(h) {
+        c.indexOf("http") == 0 ? document.location.href = c : (h.preventDefault(), a ? be(c) : r ? Oe(c) : window.load(c))
     }
 
-    function l() {
+    function o() {
         return t.jsx("a", {
             id: e,
             onClick: i || u,
             href: c || "#",
-            "data-label": C(o),
+            "data-label": T(l),
             style: s,
             children: d
         })
     }
-    return l()
+    return o()
 }
 
-function $(e) {
+function G(e) {
     function n() {
         const r = {
             display: "grid",
             gridGap: 0,
             gridTemplateColumns: "repeat(auto-fit, minmax(" + (e.width || 200) + "px, 1fr))",
             alignItems: e.alignItems || "end"
         };
@@ -509,127 +543,141 @@
             style: r,
             children: e.children
         })
     }
     return n()
 }
 
-function J(e) {
+function Y(e) {
     function n() {
-        return e.data.url ? t.jsx(Fe, {
+        return e.data.url ? t.jsx(He, {
             data: e.data
-        }) : t.jsx(be, {
+        }) : t.jsx(we, {
             data: e.data
         })
     }
     return n()
 }
 
-function be(e) {
+function we(e) {
     function n() {
-        const a = {
+        return e.data.url ? t.jsx(N, {
+            href: e.data.url,
+            children: t.jsxs(t.Fragment, {
+                children: [z(e.data.value), t.jsx(S, {
+                    icon: "external-link",
+                    style: {
+                        marginLeft: 10
+                    }
+                })]
+            })
+        }) : z(e.data.value)
+    }
+
+    function a() {
+        const r = {
             minWidth: e.width + "%",
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsxs("div", {
-            style: a,
+            style: r,
             children: [t.jsx("strong", {
                 children: e.data.label
-            }), ":", t.jsx("br", {}), U(e.data.value)]
+            }), ":", t.jsx("br", {}), n()]
         })
     }
-    return n()
+    return a()
 }
 
-function Fe(e) {
+function He(e) {
     const n = Math.random(),
-        [a, r] = M.useState(e.data);
+        [a, r] = I.useState(e.data);
 
-    function d(o) {
-        I("GET", o, function(s) {
+    function d(l) {
+        B("GET", l, function(s) {
             r(s)
         })
     }
 
     function i() {
         return window[n] = () => d(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: t.jsx(be, {
+            children: t.jsx(we, {
                 data: a,
                 width: 100
             })
         })
     }
     return i()
 }
 
-function we(e) {
+function je(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 verticalAlign: "center",
                 textAlign: "right",
                 lineHeight: "3rem"
             },
             children: e.data.map(function(a) {
-                return t.jsx(N, {
+                return t.jsx(_, {
                     data: a,
                     default: !0,
                     compact: !0
                 }, Math.random())
             })
         })
     }
     return n()
 }
 
-function je(e) {
+function ke(e) {
     function n() {
         return e.data.map(function(a) {
-            if (Array.isArray(a)) return t.jsx($, {
+            if (Array.isArray(a)) return t.jsx(G, {
                 width: 300,
                 alignItems: "start",
-                children: a.map(r => t.jsx(J, {
+                children: a.map(r => t.jsx(Y, {
                     data: r,
                     width: 100 / a.length
                 }, Math.random()))
             }, Math.random());
             if (a.label != "ID" && a.label != e.exclude) return t.jsx("div", {
-                children: t.jsx(J, {
+                children: t.jsx(Y, {
                     data: a,
                     width: 100
                 })
             }, Math.random())
         })
     }
     return n()
 }
 
-function ze(e) {
+function We(e) {
     function n() {
         const i = {
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsx("h3", {
             style: i,
             children: e.data.title
         })
     }
 
     function a() {
-        return t.jsx(je, {
+        return t.jsx(ke, {
             data: e.data.data
         })
     }
 
     function r() {
-        return t.jsx(we, {
+        return t.jsx(je, {
             data: e.data.actions
         })
     }
 
     function d() {
         const i = {
             border: "solid 1px #DDD",
@@ -640,38 +688,38 @@
             style: i,
             children: [n(), a(), r()]
         })
     }
     return d()
 }
 
-function He(e) {
+function Pe(e) {
     function n() {
-        const o = {
+        const l = {
             paddingTop: 15,
             marginBottom: 10,
             color: "#1151b3"
         };
         return t.jsx("div", {
-            style: o,
+            style: l,
             children: t.jsx("strong", {
                 children: e.data.title
             })
         })
     }
 
     function a() {
-        return t.jsx(je, {
+        return t.jsx(ke, {
             data: e.data.data,
             exclude: e.data.data[1].label
         })
     }
 
     function r() {
-        const o = {
+        const l = {
                 position: "absolute",
                 width: 140,
                 marginLeft: -128,
                 display: "flex",
                 justifyContent: "space-between",
                 marginTop: 10,
                 alignItems: "flex-end"
@@ -683,99 +731,99 @@
                 width: 20,
                 height: 20,
                 border: "3px solid #1151b3",
                 backgroundColor: "white",
                 borderRadius: "50%"
             };
         return t.jsxs("div", {
-            style: o,
+            style: l,
             children: [t.jsx("div", {
                 style: s,
                 children: e.data.data[1].value
             }), t.jsx("div", {
                 style: c
             })]
         })
     }
 
     function d() {
-        return t.jsx(we, {
+        return t.jsx(je, {
             data: e.data.actions
         })
     }
 
     function i() {
-        const o = {
+        const l = {
                 borderBottom: "solid 1px #DDD",
                 padding: 0,
                 borderBottomStyle: "dashed",
                 marginLeft: 140,
                 borderLeft: "3px solid #1151b3",
                 marginBottom: -10
             },
             s = {
                 marginLeft: 20
             };
         return t.jsxs("div", {
-            style: o,
+            style: l,
             children: [r(), t.jsxs("div", {
                 style: s,
                 children: [n(), a(), d()]
             })]
         })
     }
     return i()
 }
 
-function We(e) {
+function Ue(e) {
     const n = Math.random(),
-        [a, r] = M.useState(e.data);
+        [a, r] = I.useState(e.data);
 
     function d() {
-        return t.jsx(ke, {
+        return t.jsx(Se, {
             data: a
         })
     }
 
     function i() {
         const u = {
             backgroundColor: "white",
             padding: 15,
             marginBottom: 15
         };
         return t.jsx("div", {
             style: u,
-            children: o()
+            children: l()
         })
     }
 
-    function o() {
+    function l() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
         }) : a.data.map(function(u) {
-            return Array.isArray(u) ? t.jsx($, {
+            return Array.isArray(u) ? t.jsx(G, {
                 width: 300,
-                children: u.map(l => t.jsx(J, {
-                    data: l,
+                children: u.map(o => t.jsx(Y, {
+                    data: o,
                     width: 100 / u.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
-                children: t.jsx(J, {
+                children: t.jsx(Y, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
         }) : t.jsx(p, {
             data: a.data
         })
     }
 
     function s(u) {
-        I("GET", u, function(l) {
-            r(l)
+        B("GET", u, function(o) {
+            r(o)
         })
     }
 
     function c() {
         return e.data.url ? (window[n] = () => s(e.data.url), t.jsxs("div", {
             className: e.data.url && "reloadable",
             id: n,
@@ -783,101 +831,101 @@
         })) : t.jsxs("div", {
             children: [d(), i()]
         })
     }
     return c()
 }
 
-function Pe(e) {
+function Ge(e) {
     const n = Math.random(),
-        [a, r] = M.useState(e.data.actions);
+        [a, r] = I.useState(e.data.actions);
 
     function d() {
         const s = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + s + "only=actions"
     }
 
     function i() {
-        I("GET", d(), function(s) {
+        B("GET", d(), function(s) {
             r(s)
         })
     }
 
-    function o() {
+    function l() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
             id: n,
             children: a.map(function(s) {
-                return t.jsx(N, {
+                return t.jsx(_, {
                     data: s,
                     default: !0
                 }, Math.random())
             })
         })
     }
-    return o()
+    return l()
 }
 
-function Ge(e) {
+function Ve(e) {
     function n() {
         const a = {
                 display: "flex",
                 justifyContent: "space-between",
                 alignItems: "baseline"
             },
             r = {
                 margin: 0
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h1", {
                 style: r,
-                "data-label": C(e.data.title),
+                "data-label": T(e.data.title),
                 children: e.data.title
-            }), t.jsx(Pe, {
+            }), t.jsx(Ge, {
                 data: e.data
             })]
         })
     }
     return n()
 }
 
-function ke(e) {
+function Se(e) {
     function n() {
         const a = {
                 display: "flex",
                 justifyContent: "space-between",
                 alignItems: "baseline"
             },
             r = {
                 marginBottom: 0,
                 marginTop: 15
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
-                "data-label": C(e.data.title),
+                "data-label": T(e.data.title),
                 children: e.data.title
-            }), e.data.actions.length > 0 && t.jsx("div", {
+            }), e.data.actions && e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(d) {
-                    return t.jsx(N, {
+                    return t.jsx(_, {
                         data: d,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
     return n()
 }
 
-function Ue(e) {
+function $e(e) {
     function n() {
-        return t.jsx(Ge, {
+        return t.jsx(Ve, {
             data: e.data
         })
     }
 
     function a() {
         return e.data.data.map(function(d, i) {
             return t.jsx(p, {
@@ -890,26 +938,26 @@
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function Ve(e) {
+function Je(e) {
     function n() {
-        return t.jsx(ke, {
+        return t.jsx(Se, {
             data: e.data
         })
     }
 
     function a() {
         const d = {
             backgroundColor: "white"
         };
-        return e.data.data.map(function(i, o) {
+        return e.data.data.map(function(i, l) {
             return t.jsx("div", {
                 style: d,
                 children: t.jsx(p, {
                     data: i
                 }, Math.random())
             })
         })
@@ -919,209 +967,211 @@
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function $e(e) {
-    const [n, a] = M.useState(0);
+function Ye(e) {
+    const [n, a] = I.useState(0);
 
     function r() {
         return t.jsx("div", {
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
             children: e.data.map(function(d, i) {
-                return t.jsx(W, {
+                return t.jsx(N, {
                     href: d.url,
                     style: {
                         padding: 5,
                         fontWeight: n == i ? "bold" : "normal",
                         borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
-                    onClick: function(o) {
-                        o.preventDefault(), a(i), e.loadContent(d.url)
+                    onClick: function(l) {
+                        l.preventDefault(), a(i), e.loadContent(d.url)
                     },
-                    dataLabel: C(d.title),
+                    dataLabel: T(d.title),
                     children: d.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
-function Je(e) {
+function Qe(e) {
     var n = Math.random();
-    const [a, r] = M.useState(e.data.data[0]);
+    const [a, r] = I.useState(e.data.data[0]);
 
     function d() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": C(e.data.title),
+            "data-label": T(e.data.title),
             children: e.data.title
         })
     }
 
     function i() {
-        return t.jsx($e, {
+        return t.jsx(Ye, {
             data: e.data.data,
             loadContent: c
         })
     }
 
-    function o() {
-        var l = {
+    function l() {
+        var o = {
             ...a
         };
-        l.title = null;
-        const m = {
+        o.title = null;
+        const h = {
             padding: 0
         };
         return t.jsx("div", {
-            style: m,
+            style: h,
             children: t.jsx(p, {
-                data: l
+                data: o
             }, Math.random())
         })
     }
 
     function s() {
-        const l = {
+        const o = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: l
+            style: o
         })
     }
 
-    function c(l) {
-        I("GET", l, function(m) {
-            r(m)
+    function c(o) {
+        B("GET", o, function(h) {
+            r(h)
         })
     }
 
     function u() {
         return window[n] = () => c(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [d(), i(), o(), s()]
+            children: [d(), i(), l(), s()]
         })
     }
     return u()
 }
 
-function Ye() {
+function Xe() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
-function A({
+function R({
     id: e,
     onClick: n,
     icon: a,
     label: r,
     display: d,
     primary: i,
-    compact: o,
+    compact: l,
     spin: s
 }) {
     function c() {
-        return a ? o || !r ? t.jsx(k, {
+        return a ? l || !r ? t.jsx(S, {
             icon: a
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(De, {
+            children: [t.jsx(Ae, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(k, {
+            }), t.jsx(S, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
-        const l = {
+        const o = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: d || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return i ? (l.backgroundColor = "#1351b4", l.color = "white") : (l.border = "solid 1px #1351b4", l.color = "#1351b4"), t.jsx("a", {
+        return i ? (o.backgroundColor = C.colors.primary, o.color = "white") : (o.border = "solid 1px " + C.colors.primary, o.color = C.colors.primary), t.jsx("a", {
             id: e,
-            style: l,
-            "data-label": C(r || a),
-            onClick: m => {
-                m.preventDefault(), a && s && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
+            style: o,
+            "data-label": T(r || a),
+            onClick: h => {
+                h.preventDefault(), a && s && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: c()
         })
     }
     return u()
 }
-const Qe = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
-    Y = {
+const Ke = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
+    Q = {
         padding: 15,
         border: "solid 1px #d9d9d9",
         borderRadius: 5
     };
 
-function re(e) {
+function ie(e) {
     if (e) {
         const a = [".png", ".jpeg", ".jpeg", ".gif"];
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
-function Se(e, n) {
-    var a = new FormData(e);
-    I("POST", n, et, a)
+function ee(e, n) {
+    const a = e.closest("form"),
+        r = new FormData(a),
+        d = n.indexOf("?") >= 0 ? "&" : "?";
+    n += d + new URLSearchParams(r).toString(), B("GET", n, Ce)
 }
 
-function Xe(e) {
+function Ze(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
         a && (a.style.display = "none")
     }
 }
 
-function Ke(e) {
+function et(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "block");
         var a = document.querySelector(".form-group." + e);
-        a && (a.style.display = "inline-block")
+        a && (a.style.display = "flex")
     }
 }
 
-function Ze(e, n) {
+function tt(e, n) {
     var a = document.querySelector(".form-group." + e),
         r = a.querySelector('*[name="' + e + '"]');
     if (r.tagName == "INPUT") r.value = n;
     else if (r.tagName == "SELECT") {
         if (r.style.display != "none") r.dispatchEvent(new CustomEvent("customchange", {
             detail: {
                 value: n
@@ -1132,76 +1182,77 @@
                 if (r.options[d].value == n) {
                     r.selectedIndex = d;
                     break
                 }
     }
 }
 
-function et(e) {
+function Ce(e) {
     if (e) {
-        for (var n = 0; n < e.hide.length; n++) Xe(e.hide[n]);
-        for (var n = 0; n < e.show.length; n++) Ke(e.show[n]);
-        for (var a in e.set) Ze(a, e.set[a])
+        for (var n = 0; n < e.hide.length; n++) Ze(e.hide[n]);
+        for (var n = 0; n < e.show.length; n++) et(e.show[n]);
+        for (var a in e.set) tt(a, e.set[a])
     }
 }
 
-function tt(e) {
+function nt(e) {
     function n() {
         const a = {
-            color: "#155bcb",
-            backgroundColor: "#d4e5ff",
+            color: C.colors.info,
+            backgroundColor: C.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(k, {
+                children: [t.jsx(S, {
                     icon: "circle-check",
                     style: {
-                        color: "#155bcb",
+                        color: C.colors.info,
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
 
-function nt(e) {
+function at(e) {
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
-            children: [t.jsx(k, {
+            className: "error",
+            children: [t.jsx(S, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
     return n()
 }
 
-function at(e) {
+function rt(e) {
     function n() {
         const a = {
             marginTop: 2,
             marginBottom: 2,
             fontStyle: "italic"
         };
         return t.jsx("div", {
@@ -1219,494 +1270,500 @@
 
     function a() {
         const s = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
-        return e.data.action && (e.data.action.modal = !0), t.jsxs("div", {
+        return e.data.action && (e.data.action.icon = null, e.data.action.modal = !0), t.jsxs("div", {
             style: s,
             children: [t.jsx("label", {
                 className: e.data.required ? "bold" : "",
                 children: e.data.label
-            }), e.data.action && t.jsx(N, {
+            }), e.data.action && t.jsx(_, {
                 data: e.data.action,
                 style: {
                     padding: 0
                 }
             })]
         })
     }
 
     function r() {
-        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Qe.indexOf(e.data.type) >= 0 ? t.jsx(he, {
+        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Ke.indexOf(e.data.type) >= 0 ? t.jsx(me, {
             data: e.data
-        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(me, {
+        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(fe, {
             data: e.data
-        }) : t.jsx(ie, {
+        }) : t.jsx(le, {
             data: e.data
-        }) : t.jsx(lt, {
+        }) : t.jsx(ot, {
             data: e.data
-        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(me, {
+        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(fe, {
             data: e.data
-        }) : t.jsx(ie, {
+        }) : t.jsx(le, {
             data: e.data
-        }) : t.jsx(Ce, {
+        }) : t.jsx(Te, {
             data: e.data
-        }) : e.data.type == "decimal" ? t.jsx(he, {
+        }) : e.data.type == "decimal" ? t.jsx(me, {
             data: e.data
-        }) : e.data.type == "boolean" ? t.jsx(it, {
+        }) : e.data.type == "boolean" ? t.jsx(lt, {
             data: e.data
-        }) : e.data.type == "textarea" ? t.jsx(rt, {
+        }) : e.data.type == "textarea" ? t.jsx(it, {
             data: e.data
         }) : t.jsx("span", {
             children: e.data.name
         })
     }
 
     function d() {
         return t.jsx("div", {
-            children: t.jsx(nt, {
+            children: t.jsx(at, {
                 id: e.data.name + "_error"
             })
         })
     }
 
     function i() {
-        return e.data.help_text && t.jsx(at, {
+        return e.data.help_text && t.jsx(rt, {
             text: e.data.help_text
         })
     }
 
-    function o() {
+    function l() {
         const s = {
             display: e.data.type == "hidden" ? "none" : "flex",
             flexDirection: "column",
-            padding: 5
+            padding: 5,
+            width: "calc(100%-5px)"
         };
         return t.jsxs("div", {
             id: n,
-            className: "form-group " + e.data.name,
             style: s,
             children: [a(), r(), i(), d()]
         })
     }
-    return o()
+    return l()
 }
 
-function he(e) {
+function me(e) {
     var n = "";
     const a = e.data.name + Math.random();
-    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), M.useEffect(() => {
-        function o(u, l, m) {
-            var x = m.target,
-                w = x.value.replace(/\D/g, ""),
-                S = x.value.length > l ? 1 : 0;
-            VMasker(x).unMask(), VMasker(x).maskPattern(u[S]), x.value = VMasker.toPattern(w, u[S])
+    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), I.useEffect(() => {
+        function l(u, o, h) {
+            var f = h.target,
+                w = f.value.replace(/\D/g, ""),
+                M = f.value.length > o ? 1 : 0;
+            VMasker(f).unMask(), VMasker(f).maskPattern(u[M]), f.value = VMasker.toPattern(w, u[M])
         }
         if (e.data.mask) {
             var s = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(s).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
             });
             else if (e.data.mask.indexOf("|") > 0) {
                 var c = e.data.mask.split("|");
-                VMasker(s).maskPattern(c[0]), s.addEventListener("input", o.bind(void 0, c, 14), !1)
+                VMasker(s).maskPattern(c[0]), s.addEventListener("input", l.bind(void 0, c, 14), !1)
             } else VMasker(s).maskPattern(e.data.mask)
         }
     }, []);
 
-    function r(o) {
-        Se(o.target.closest("form"), e.data.onchange)
+    function r(l) {
+        ee(l.target, e.data.onchange)
     }
 
-    function d(o) {
-        if (e.data.type == "file" && o.target.files) {
-            let c = o.target.files[0];
+    function d(l) {
+        if (e.data.type == "file" && l.target.files) {
+            let c = l.target.files[0];
             var s = new FileReader;
             s.onload = function(u) {
-                if (re(c.name)) {
+                if (ie(c.name)) {
                     const w = "display" + a;
-                    var l = document.createElement("img");
-                    l.id = o.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(S) {
-                        const B = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
-                        var y = document.createElement("canvas");
-                        const j = y.getContext("2d");
-                        y.height = y.width * (l.height / l.width);
-                        const v = document.createElement("canvas"),
-                            L = v.getContext("2d");
-                        v.width = l.width * B, v.height = l.height * B, L.drawImage(l, 0, 0, v.width, v.height), j.drawImage(v, 0, 0, v.width * B, v.height * B, 0, 0, y.width, y.height), v.toBlob(function(h) {
-                            const f = new DataTransfer;
-                            f.items.add(new File([h], c.name)), o.target.files = f.files
+                    var o = document.createElement("img");
+                    o.id = l.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(M) {
+                        const D = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
+                        var x = document.createElement("canvas");
+                        const j = x.getContext("2d");
+                        x.height = x.width * (o.height / o.width);
+                        const y = document.createElement("canvas"),
+                            L = y.getContext("2d");
+                        y.width = o.width * D, y.height = o.height * D, L.drawImage(o, 0, 0, y.width, y.height), j.drawImage(y, 0, 0, y.width * D, y.height * D, 0, 0, x.width, x.height), y.toBlob(function(m) {
+                            const v = new DataTransfer;
+                            v.items.add(new File([m], c.name)), l.target.files = v.files
                         });
-                        var D = document.getElementById(w);
-                        D == null ? (D = document.createElement("div"), D.id = w) : D.removeChild(D.childNodes[0]), D.appendChild(l), o.target.parentNode.appendChild(D)
-                    }, l.src = u.target.result
+                        var b = document.getElementById(w);
+                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), l.target.parentNode.appendChild(b)
+                    }, o.src = u.target.result
                 }
-                const m = document.getElementById("fileinfo" + a);
-                var x = c.size / 1024;
-                x < 1024 ? x = parseInt(x) + " Kb" : x = (x / 1024).toFixed(2) + " Mb", m.innerHTML = c.name + " / " + x, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + x + ". Por favor, adicione um arquivo menor.")
+                const h = document.getElementById("fileinfo" + a);
+                var f = c.size / 1024;
+                f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = c.name + " / " + f, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
             }, s.readAsDataURL(c)
         }
     }
 
     function i() {
-        var o = e.data.type;
-        if (o == "datetime" && (o = "datetime-regional"), o == "decimal" && (o = "text"), o == "file") {
+        var l = e.data.type;
+        if (l == "datetime" && (l = "datetime-regional"), l == "decimal" && (l = "text"), l == "file") {
             const u = {
                 alignContent: "center",
-                height: 75,
+                minHeight: 75,
                 padding: 5,
                 maxWidth: "100%",
                 margin: "auto"
             };
             var s = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (s = e.data.extensions.map(l => "." + l).join(", ")), t.jsxs(t.Fragment, {
+            return e.data.extensions && e.data.extensions.length > 0 && (s = e.data.extensions.map(o => "." + o).join(", ")), t.jsxs(t.Fragment, {
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
-                        children: t.jsx(k, {
+                        children: t.jsx(S, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
-                                color: "#1351b4"
+                                color: C.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
-                        children: [e.data.value && re(e.data.value) && t.jsx("div", {
+                        children: [e.data.value && ie(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: t.jsx("img", {
                                 src: e.data.value,
                                 height: 50
                             })
-                        }), e.data.value && !re(e.data.value) && t.jsx("div", {
+                        }), e.data.value && !ie(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
-                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(l => "." + l).join(" ou "), "."]
+                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(o => "." + o).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
-                        children: t.jsx(A, {
+                        children: t.jsx(R, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
-                    type: o,
+                    type: l,
                     name: e.data.name,
                     id: a,
-                    "data-label": C(e.data.label),
+                    "data-label": T(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
                     onChange: d,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
                     accept: s
                 })]
             })
         } else {
-            var c = Y;
-            return o == "color" && (c = {
-                ...Y
+            var c = Q;
+            return l == "color" && (c = {
+                ...Q
             }, c.width = "100%", c.backgroundColor = "white", c.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
-                type: o,
+                type: l,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": C(e.data.label),
+                "data-label": T(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
                 onChange: d,
                 style: c
             })
         }
     }
     return i()
 }
 
-function Ce(e) {
+function Te(e) {
     var n = [];
-    Array.isArray(e.data.value) ? e.data.value.forEach(function(h, f) {
+    Array.isArray(e.data.value) ? e.data.value.forEach(function(b, m) {
         n.push({
-            id: h.id,
-            value: h.label
+            id: b.id,
+            value: b.label
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
         d = Array.isArray(e.data.value),
-        [i, o] = M.useState(!1),
-        [s, c] = M.useState(null);
+        [i, l] = I.useState(!1),
+        [s, c] = I.useState(null);
     var u = !1;
-    let l;
-    M.useEffect(() => {
-        v(n), document.getElementById(a).addEventListener("customchange", function(h) {
-            v(h.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+    let o;
+    I.useEffect(() => {
+        j(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
+            j(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
-    function m() {
-        const h = document.getElementById(a);
+    function h() {
+        const b = document.getElementById(a);
         if (d) {
-            const f = {
+            const m = {
                     padding: 5,
                     display: "inline"
                 },
-                g = {
+                v = {
                     cursor: "pointer",
                     marginRight: 5
                 },
-                b = {
+                g = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [h == null && n.map((T, R) => t.jsxs("div", {
-                    style: f,
+                children: [b == null && n.map((k, E) => t.jsxs("div", {
+                    style: m,
                     children: [t.jsx("span", {
-                        onClick: () => L(R),
-                        style: g,
-                        children: t.jsx(k, {
+                        onClick: () => y(E),
+                        style: v,
+                        children: t.jsx(S, {
                             icon: "trash-can",
-                            style: b
+                            style: g
                         })
-                    }), T.value]
-                }, Math.random())), h != null && Array.from(h.options).map((T, R) => t.jsxs("div", {
-                    style: f,
+                    }), k.value]
+                }, Math.random())), b != null && Array.from(b.options).map((k, E) => t.jsxs("div", {
+                    style: m,
                     children: [t.jsx("span", {
-                        onClick: () => L(R),
-                        style: g,
-                        children: t.jsx(k, {
+                        onClick: () => y(E),
+                        style: v,
+                        children: t.jsx(S, {
                             icon: "trash-can",
-                            style: b
+                            style: g
                         })
-                    }), T.innerHTML]
+                    }), k.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
-    function x(h) {
-        c([])
-    }
-
-    function w() {
+    function f() {
         return t.jsx("select", {
-            onChange: x,
             id: a,
             name: e.data.name,
             multiple: d,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
-    function S() {
-        const h = {
-                ...Y,
+    function w() {
+        const b = {
+                ...Q,
                 ...e.style || {}
             },
-            f = {
+            m = {
                 padding: 0,
                 margin: 0,
                 border: "solid 1px #d9d9d9",
                 marginTop: -1,
                 borderRadius: 5,
                 maxHeight: 150,
                 overflowY: "auto"
             };
-        f.position = "absolute", f.backgroundColor = "white";
-        const g = document.getElementById(r);
-        if (g) {
-            let E = null,
-                z = g,
-                G = null;
-            for (; !G && (z = z.parentElement) instanceof HTMLElement;) z.matches("dialog") && (G = z);
-            E = G;
-            const _ = g.getBoundingClientRect();
-            var b = _.top + _.height,
-                T = _.left;
-            if (E) {
-                const Q = E.getBoundingClientRect();
-                b = b - Q.top, T = T - Q.left
-            } else b += window.scrollY, T += window.scrollX;
-            f.width = _.width, f.top = b, f.left = T
+        m.position = "absolute", m.backgroundColor = "white";
+        const v = document.getElementById(r);
+        if (e.data.icon && (b.paddingLeft = 30), v) {
+            let A = null,
+                F = v,
+                V = null;
+            for (; !V && (F = F.parentElement) instanceof HTMLElement;) F.matches("dialog") && (V = F);
+            A = V;
+            const P = v.getBoundingClientRect();
+            var g = P.top + P.height,
+                k = P.left;
+            if (A) {
+                const $ = A.getBoundingClientRect();
+                g = g - $.top, k = k - $.left
+            } else g += window.scrollY, k += window.scrollX;
+            m.width = P.width, m.top = g, m.left = k
         }
-        const R = {
+        const E = {
                 cursor: "pointer",
                 padding: 10
             },
-            ne = !d && n.length > 0 && n[0].value || "";
+            ae = !d && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
-            children: [t.jsx("input", {
+            children: [e.data.icon && t.jsx(S, {
+                icon: e.data.icon,
+                style: {
+                    position: "absolute",
+                    margin: 13,
+                    color: "#d9d9d9"
+                }
+            }), t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
-                onFocus: E => {
-                    E.target.select(), j(E)
+                onFocus: A => {
+                    A.target.select(), x(A)
                 },
-                onChange: j,
-                onMouseLeave: B,
-                onBlur: B,
-                defaultValue: ne,
-                style: h,
-                "data-label": C(e.data.label)
+                onChange: x,
+                onMouseLeave: M,
+                onBlur: M,
+                defaultValue: ae,
+                style: b,
+                "data-label": T(e.data.label)
             }), s && i && t.jsxs("ul", {
-                style: f,
-                onMouseLeave: y,
-                onMouseEnter: function(E) {
+                style: m,
+                onMouseLeave: D,
+                onMouseEnter: function(A) {
                     u = !0
                 },
                 children: [s.length == 0 && t.jsx("li", {
-                    style: R,
+                    style: E,
                     children: "Nenhuma opção encontrada."
-                }), s.map(E => t.jsx("li", {
+                }), s.map(A => t.jsx("li", {
                     onClick: () => {
-                        o(!1), e.onSelect ? e.onSelect(E) : v(E)
+                        l(!1), e.onSelect ? e.onSelect(A) : j(A)
                     },
-                    style: R,
+                    style: E,
                     className: "autocomplete-item",
-                    "data-label": C(E.value),
-                    children: E.value
+                    "data-label": T(A.value),
+                    children: A.value
                 }, Math.random()))]
             })]
         })
     }
 
-    function B(h) {
+    function M(b) {
         u = !1, setTimeout(function() {
-            y(h)
+            u || D(b)
         }, 250)
     }
 
-    function y(h) {
-        const f = document.getElementById(a),
-            g = document.getElementById(r);
-        d || f.options.length > 0 && g.value != f.options[0].innerHTML && (f.innerHTML = "", g.value = "", o(!1)), h.target.tagName == "UL" ? o(!1) : u || o(!1)
+    function D(b) {
+        const m = document.getElementById(a);
+        if (m) {
+            const v = document.getElementById(r);
+            d || m.options.length > 0 && v.value != m.options[0].innerHTML && (m.innerHTML = "", v.value = "", l(!1), e.data.onchange && ee(v, e.data.onchange)), b.target.tagName == "UL" ? l(!1) : u || l(!1)
+        }
     }
 
-    function j(h) {
-        clearTimeout(l), l = setTimeout(function() {
-            const f = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            o(!0), I("GET", e.data.choices + f + "term=" + h.target.value, function(b) {
-                c(b)
+    function x(b) {
+        clearTimeout(o), o = setTimeout(function() {
+            const m = e.data.choices.indexOf("?") < 0 ? "?" : "&";
+            l(!0), B("GET", e.data.choices + m + "term=" + b.target.value, function(g) {
+                c(g)
             })
         }, 1e3)
     }
 
-    function v(h) {
-        const f = document.getElementById(a),
+    function j(b, m = !1) {
+        const v = document.getElementById(a),
             g = document.getElementById(r);
-        f.innerHTML == null && (f.innerHTML = ""), Array.isArray(h) ? f.innerHTML = h.map(b => `<option selected value="${b.id}">${b.value}</option>`).join("") : d ? (f.innerHTML += `<option selected value="${h.id}">${h.value}</option>`, g.value = "") : (f.innerHTML = `<option selected value="${h.id}">${h.value}</option>`, g.value = h.value), e.data.onchange && Se(g.closest("form"), e.data.onchange)
+        v.innerHTML == null && (v.innerHTML = ""), Array.isArray(b) ? v.innerHTML = b.map(k => `<option selected value="${k.id}">${k.value}</option>`).join("") : d ? (v.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, g.value = "") : (v.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, g.value = b.value), e.data.onchange && !m && ee(g, e.data.onchange)
     }
 
-    function L(h) {
-        const f = document.getElementById(a);
-        var g = Array.from(f.options);
-        f.innerHTML = g.slice(0, h).concat(g.slice(h + 1)).map(b => `<option selected value="${b.value}">${b.innerHTML}</option>`).join(""), c([])
+    function y(b) {
+        const m = document.getElementById(a);
+        var v = Array.from(m.options);
+        m.innerHTML = v.slice(0, b).concat(v.slice(b + 1)).map(g => `<option selected value="${g.value}">${g.innerHTML}</option>`).join(""), c([])
     }
 
-    function D() {
+    function L() {
         return t.jsxs(t.Fragment, {
-            children: [m(), w(), S()]
+            children: [h(), f(), w()]
         })
     }
-    return D()
+    return L()
 }
 
-function rt(e) {
+function it(e) {
     function n() {
         var a = {
-            ...Y
+            ...Q
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": C(e.data.label),
+            "data-label": T(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
 
-function it(e) {
+function lt(e) {
     var n = e.data;
     return n.choices = [{
         id: !0,
         value: "Sim"
     }, {
         id: !1,
         value: "Não"
-    }], t.jsx(ie, {
+    }], t.jsx(le, {
         data: n
     })
 }
 
-function ie(e) {
+function le(e) {
     var n = Math.random(),
         a = e.data;
 
     function r(s) {
         return a.value != null ? a.value == s.id ? !0 : a.value.id == s.id : !1
     }
 
     function d(s) {
         var c = document.getElementById(s);
-        a.checked && (c.checked = !1)
+        a.checked && (c.checked = !1), e.data.onchange && ee(c, e.data.onchange)
     }
 
     function i(s) {
         var c = document.getElementById(s);
         a.checked = c.checked
     }
 
-    function o() {
+    function l() {
         return a.choices.length > 0 ? t.jsx("div", {
             className: "radio-group",
-            children: a.choices.map((s, c) => t.jsxs("div", {
+            children: a.choices.map((s, c) => s.id && t.jsxs("div", {
                 style: {
-                    paddingTop: 10
+                    paddingTop: 10,
+                    display: "inline-block",
+                    marginRight: 25
                 },
                 children: [t.jsx("input", {
                     id: a.name + n + c,
                     type: "radio",
                     name: a.name,
                     defaultValue: s.id,
                     defaultChecked: r(s),
-                    "data-label": C(s.value),
+                    "data-label": T(s.value),
                     onClick: function() {
                         d(a.name + n + c)
                     },
                     onMouseEnter: function() {
                         i(a.name + n + c)
                     }
                 }), t.jsx("label", {
@@ -1714,413 +1771,435 @@
                     children: s.value
                 })]
             }, n + c))
         }) : t.jsx("i", {
             children: "Nenhuma opção disponível para seleção."
         })
     }
-    return o()
+    return l()
 }
 
-function me(e) {
+function fe(e) {
     var n = Math.random(),
         a = e.data;
 
     function r(i) {
-        var o = !1;
+        var l = !1;
         if (a.value)
             for (var s = 0; s < a.value.length; s++) {
                 var c = a.value[s];
-                (c == i.id || c.id == i.id) && (o = !0)
+                (c == i.id || c.id == i.id) && (l = !0)
             }
-        return o
+        return l
     }
 
     function d() {
         return a.choices.length > 0 ? t.jsx("div", {
             className: "checkbox-group",
-            children: a.choices.map((i, o) => t.jsxs("div", {
+            children: a.choices.map((i, l) => t.jsxs("div", {
                 style: {
-                    paddingTop: 10
+                    paddingTop: 10,
+                    display: "inline-block",
+                    marginRight: 25
                 },
                 children: [t.jsx("input", {
-                    id: a.name + n + o,
+                    id: a.name + n + l,
                     type: "checkbox",
                     name: a.name,
                     defaultValue: i.id,
                     defaultChecked: r(i),
-                    "data-label": C(i.value)
+                    "data-label": T(i.value)
                 }), t.jsx("label", {
-                    htmlFor: a.name + n + o,
+                    htmlFor: a.name + n + l,
                     children: i.value
                 })]
-            }, n + o))
+            }, n + l))
         }) : t.jsx("i", {
             children: "Nenhuma opção disponível para seleção."
         })
     }
     return d()
 }
 
-function lt(e) {
+function ot(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": C(n.label),
+            "data-label": T(n.label),
             defaultValue: n.value,
-            style: Y,
+            style: Q,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
     })
 }
 
-function ot(e) {
+function dt(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
     function d() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
-            children: t.jsxs(le, {
+            children: t.jsxs(oe, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
-                children: [t.jsx(A, {
+                children: [t.jsx(R, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => i(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
-                }), t.jsx(A, {
+                }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => i(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
         })
     }
 
     function i(c) {
         const u = document.querySelector("input[name=" + r.name + "]"),
-            l = document.getElementById("inline-form-" + n),
-            m = document.getElementById("show-" + n),
-            x = document.getElementById("hide-" + n);
-        l.style.display = c ? "block" : "none", m.style.display = c ? "none" : "inline", x.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+            o = document.getElementById("inline-form-" + n),
+            h = document.getElementById("show-" + n),
+            f = document.getElementById("hide-" + n);
+        o.style.display = c ? "block" : "none", h.style.display = c ? "none" : "inline", f.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
-    function o() {
+    function l() {
         const c = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (c.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
             className: "fieldset-inline-forms",
             style: c,
             id: "inline-form-" + n,
             children: e.data.value.map(function(u) {
-                return t.jsx(oe, {
+                return t.jsx(de, {
                     data: u
                 }, Math.random())
             })
         })
     }
 
     function s() {
         const c = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: c,
-                "data-label": C(e.data.label),
+                "data-label": T(e.data.label),
                 children: e.data.label
-            }), d(), o()]
+            }), d(), l()]
         })
     }
     return s()
 }
 
-function dt(e) {
+function st(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
-    function r(l, m) {
-        const x = n;
+    function r(o, h) {
+        const f = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
-            id: "form-" + x + "-" + a,
-            children: [t.jsx(oe, {
-                data: l
+            id: "form-" + f + "-" + a,
+            children: [t.jsx(de, {
+                data: o
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
-                children: [t.jsx(A, {
+                children: [t.jsx(R, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => i(),
-                    id: "extra-add-" + x + "-",
-                    display: m
-                }), t.jsx(A, {
+                    id: "extra-add-" + f + "-",
+                    display: h
+                }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => o(x),
+                    onClick: () => l(f),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
     function d() {
-        const l = s(),
-            m = l.length > 0 ? "none" : "inline";
-        document.getElementById("add-" + a).style.display = m;
-        for (var x = 0; x < n; x++) {
-            var w = document.getElementById("extra-add-" + x + "-");
+        const o = s(),
+            h = o.length > 0 ? "none" : "inline";
+        document.getElementById("add-" + a).style.display = h;
+        for (var f = 0; f < n; f++) {
+            var w = document.getElementById("extra-add-" + f + "-");
             w.style.display = "none"
         }
-        if (l.length > 0) {
-            var w = document.getElementById("extra-add-" + l[l.length - 1] + "-");
+        if (o.length > 0) {
+            var w = document.getElementById("extra-add-" + o[o.length - 1] + "-");
             w.style.display = "inline"
         }
     }
 
     function i() {
         d();
-        var l = JSON.parse(JSON.stringify(e.data.template));
-        l.fields ? (l.fields.map(function(m) {
-            m.name = m.name.replace("__n__", "__" + n + "__")
-        }), l.fields[0].value = 0) : l.fieldsets.map(function(m) {
-            m.fields.map(function(x) {
-                x.map(function(w) {
+        var o = JSON.parse(JSON.stringify(e.data.template));
+        o.fields ? (o.fields.map(function(h) {
+            h.name = h.name.replace("__n__", "__" + n + "__")
+        }), o.fields[0].value = 0) : o.fieldsets.map(function(h) {
+            h.fields.map(function(f) {
+                f.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
-                }), x[0].value = 0
+                }), f[0].value = 0
             })
-        }), P.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(d, 100)
+        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(d, 100)
     }
 
-    function o(l) {
-        const m = e.data.template,
-            w = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + l + "__"),
-            S = document.querySelector("input[name=" + w + "]");
-        parseInt(S.value) == 0 ? S.value = "" : S.value = -parseInt(S.value), document.getElementById("form-" + l + "-" + a).style.display = "none", d()
+    function l(o) {
+        const h = e.data.template,
+            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
+            M = document.querySelector("input[name=" + w + "]");
+        parseInt(M.value) == 0 ? M.value = "" : M.value = -parseInt(M.value), document.getElementById("form-" + o + "-" + a).style.display = "none", d()
     }
 
     function s() {
-        for (var l = [], m = 0; m < n; m++) document.getElementById("form-" + m + "-" + a).style.display == "block" && l.push(m);
-        return l
+        for (var o = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && o.push(h);
+        return o
     }
 
     function c() {
         return t.jsx("div", {
             id: "info-" + a,
-            children: t.jsx(le, {
+            children: t.jsx(oe, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
-                children: t.jsx(A, {
+                children: t.jsx(R, {
                     primary: !0,
                     icon: "add",
                     onClick: () => i(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
         })
     }
 
     function u() {
-        const l = {
+        const o = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: l,
-                "data-label": C(e.data.label),
+                style: o,
+                "data-label": T(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
-                children: [c(), e.data.value.map(function(m, x) {
-                    return r(m, x == e.data.value.length - 1 ? "inline" : "none")
+                children: [c(), e.data.value.map(function(h, f) {
+                    return r(h, f == e.data.value.length - 1 ? "inline" : "none")
                 })]
             })]
         })
     }
     return u()
 }
 
-function oe(e) {
+function de(e) {
+    I.useEffect(() => {
+        e.data.controls && (console.log(e.data.controls), Ce(e.data.controls))
+    }, []);
+
     function n(r) {
-        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(ot, {
+        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(dt, {
             data: r
-        }, Math.random()) : t.jsx(dt, {
+        }, Math.random()) : t.jsx(st, {
             data: r
         }, Math.random()) : t.jsx(K, {
             data: r
         }, Math.random())
     }
 
     function a() {
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": C(r.title),
+                    "data-label": T(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
-                }), t.jsx("div", {
-                    className: "fieldset-fields",
-                    children: r.fields.map(d => t.jsx("div", {
-                        children: d.map(i => t.jsx("div", {
-                            style: {
-                                width: 100 / d.length + "%",
-                                display: i.type == "hidden" ? "none" : "inline-block"
-                            },
-                            children: n(i)
-                        }, Math.random()))
+                }), r.fields.map(d => t.jsx("div", {
+                    children: d.map(i => t.jsx("div", {
+                        className: "form-group " + i.name,
+                        style: {
+                            width: 100 / d.length + "%",
+                            display: i.type == "hidden" ? "none" : "inline-block"
+                        },
+                        children: n(i)
                     }, Math.random()))
-                })]
+                }, Math.random()))]
             })
         }, Math.random()))
     }
     return a()
 }
 
-function st(e) {
+function ct(e) {
     const n = Math.random();
 
     function a() {
-        const l = {
-            margin: 0,
-            textAlign: "left"
+        const h = {
+            margin: 0
         };
         return t.jsx("h1", {
-            style: l,
+            style: h,
             children: e.data.title
         })
     }
 
     function r() {
-        return e.data.info && t.jsx(tt, {
+        return e.data.info && t.jsx(nt, {
             data: {
                 text: e.data.info
             }
         })
     }
 
     function d() {
         if (e.data.display) return t.jsxs(t.Fragment, {
-            children: [e.data.display.map(l => t.jsx(p, {
-                data: l
+            children: [e.data.display.map(h => t.jsx(p, {
+                data: h
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
     }
 
     function i() {
-        return t.jsx(oe, {
+        return t.jsx(de, {
             data: e.data
         })
     }
 
-    function o() {
+    function l() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
-            children: [t.jsx(A, {
-                onClick: c,
+            children: [t.jsx(R, {
+                onClick: u,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
-            }), t.jsx(A, {
-                onClick: u,
+            }), t.jsx(R, {
+                onClick: o,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
     }
 
     function s() {
+        return t.jsx("div", {
+            id: "output"
+        })
+    }
+
+    function c() {
         return t.jsxs("form", {
             id: n,
+            className: e.data.key,
             action: e.data.url,
             style: {
                 margin: "auto",
-                width: e.data.width,
                 backgroundColor: "white"
             },
+            method: e.data.method,
             children: [t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 style: {
                     padding: 5
                 },
-                children: [a(), r(), d(), i(), o()]
+                children: [a(), r(), d(), i(), l(), s()]
             })]
         })
     }
 
-    function c() {
-        V()
+    function u() {
+        J()
     }
 
-    function u(l) {
-        l.preventDefault();
-        var m = document.getElementById(n),
-            x = new FormData(m);
-        I("POST", e.data.url, function(S) {
-            if (l.target.dataset.spinning && (l.target.querySelector("i.fa-spin").style.display = "none", l.target.querySelector("i.fa-" + l.target.dataset.spinning).style.display = "inline-block"), S.type == "response") return V(), Ye(), ye(S);
-            var B = S.text;
-            console.log(S), Object.keys(S.errors).map(function(y) {
-                if (y == "__all__") B = S.errors[y];
-                else {
-                    const j = m.querySelector("#" + y + "_error");
-                    j.querySelector("span").innerHTML = S.errors[y], j.style.display = "block"
-                }
-            }), ee(B, !0)
-        }, x)
+    function o(h) {
+        h.preventDefault();
+        var f = e.data.url,
+            w = document.getElementById(n),
+            M = new FormData(w);
+        if (w.method.toUpperCase() == "GET") {
+            const D = f.indexOf("?") >= 0 ? "&" : "?";
+            f = f + D + "form=" + e.data.title + "&" + new URLSearchParams(M).toString(), M = null
+        }
+        B(w.method.toUpperCase(), f, function(x) {
+            if (w.querySelectorAll(".error").forEach(y => y.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), x.type == "response") return J(), Xe(), ve(x);
+            if (x.type == "error") {
+                var j = x.text;
+                console.log(x), Object.keys(x.errors).map(function(y) {
+                    if (y == "__all__") j = x.errors[y];
+                    else {
+                        const L = w.querySelector("#" + y + "_error");
+                        L.querySelector("span").innerHTML = x.errors[y], L.style.display = "block"
+                    }
+                }), te(j, !0)
+            } else {
+                const y = document.querySelector("#output");
+                y.innerHTML = "", H.createRoot(y.appendChild(document.createElement("div"))).render(t.jsx(p, {
+                    data: x
+                }))
+            }
+        }, M)
     }
-    return s()
+    return c()
 }
 
-function ct(e) {
+function ut(e) {
     function n() {
         const a = {
-            backgroundColor: "#1351b4",
+            backgroundColor: C.colors.primary,
             color: "white",
             borderRadius: "50%",
             minWidth: 13,
             marginLeft: 2,
             padding: 4,
             fontSize: "70%",
             display: "inline-block",
@@ -2132,400 +2211,400 @@
             style: a,
             children: e.total
         })
     }
     return n()
 }
 
-function ut(e) {
+function ht(e) {
     e.data.id == null && (e.data.id = Math.random());
-    const [n, a] = M.useState(e.data);
+    const [n, a] = I.useState(e.data);
 
     function r() {
-        const h = {
+        const m = {
             margin: 0
         };
         return n.attrname ? t.jsx("h2", {
-            style: h,
-            "data-label": C(n.title),
+            style: m,
+            "data-label": T(n.title),
             children: n.title
         }) : t.jsx("h1", {
-            style: h,
-            "data-label": C(n.title),
+            style: m,
+            "data-label": T(n.title),
             children: n.title
         })
     }
 
     function d() {
-        const h = {
+        const m = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "center"
         };
         return t.jsxs("div", {
-            style: h,
+            style: m,
             children: [r(), t.jsx("i", {
                 id: "loader-" + e.data.id,
                 style: {
                     display: "none"
                 },
                 className: "fa-solid fa-circle-notch fa-spin fa-1x"
             })]
         })
     }
 
-    function i(h) {
-        document.getElementById("loader-" + e.data.id).style.display = h ? "block" : "none"
+    function i(m) {
+        document.getElementById("loader-" + e.data.id).style.display = m ? "block" : "none"
     }
 
-    function o() {
+    function l() {
         return n.subsets && t.jsx("div", {
             style: {
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 paddingBottom: 20,
                 lineHeight: "2.5rem"
             },
-            children: n.subsets.map(function(h, f) {
-                var g = n.subset === h.name || !n.subset && f == 0;
-                return t.jsxs(W, {
+            children: n.subsets.map(function(m, v) {
+                var g = n.subset === m.name || !n.subset && v == 0;
+                return t.jsxs(N, {
                     href: "#",
                     style: {
                         paddingBottom: 5,
                         paddingLeft: 15,
                         paddingRight: 15,
                         fontWeight: g ? "bold" : "normal",
                         borderBottom: g ? "solid 3px #2670e8" : 0,
                         textDecoration: "none",
                         color: "#0c326f"
                     },
-                    onClick: function(b) {
-                        b.preventDefault(), s(h.name)
+                    onClick: function(k) {
+                        k.preventDefault(), s(m.name)
                     },
-                    dataLabel: C(h.label),
-                    children: [h.label, " ", t.jsx(ct, {
-                        total: h.count
+                    dataLabel: T(m.label),
+                    children: [m.label, " ", t.jsx(ut, {
+                        total: m.count
                     })]
                 }, Math.random())
             })
         })
     }
 
-    function s(h) {
-        const f = document.getElementById("subset-" + e.data.id);
-        f.value = h || "", v()
+    function s(m) {
+        const v = document.getElementById("subset-" + e.data.id);
+        v.value = m || "", y()
     }
 
-    function c(h, f, g) {
-        const b = document.getElementById("form-" + e.data.id);
-        b.querySelector("input[name=" + n.calendar.field + "__day]").value = h || "", b.querySelector("input[name=" + n.calendar.field + "__month]").value = f || "", b.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", v()
+    function c(m, v, g) {
+        const k = document.getElementById("form-" + e.data.id);
+        k.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", k.querySelector("input[name=" + n.calendar.field + "__month]").value = v || "", k.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", y()
     }
 
     function u() {
         if (n.calendar) {
-            const T = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
-                R = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
-                ne = {
+            const E = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
+                ae = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
+                A = {
                     width: "100%",
                     borderSpacing: 0,
                     borderCollapse: "collapse",
                     marginTop: 15,
                     marginBottom: 15
                 },
-                E = {
+                F = {
                     marginLeft: "17",
                     textAlign: "right",
                     paddingRight: 2,
                     paddingTop: 2,
                     float: "right",
                     fontSize: "0.8rem"
                 },
-                z = {
+                V = {
                     verticalAlign: "top",
                     width: "14.2%",
                     height: 55,
                     border: "solid 1px #EEE"
                 },
-                G = {
-                    backgroundColor: "#1351b4",
+                P = {
+                    backgroundColor: C.colors.primary,
                     borderRadius: "50%",
                     color: "white",
                     display: "block",
                     width: 30,
                     height: 30,
                     margin: "auto",
                     cursor: "pointer",
                     lineHeight: "2rem"
                 },
-                _ = {
+                $ = {
                     padding: 10,
                     textAlign: "center"
                 },
-                Q = {
+                Ee = {
                     display: "flex",
                     justifyContent: "space-between",
                     alignItems: "baseline"
                 },
-                Ee = new Date,
-                ce = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
-            for (var h = [
+                Ie = new Date,
+                ue = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
+            for (var m = [
                     [],
                     [],
                     [],
                     [],
                     [],
                     []
-                ], f = n.calendar.month - 1, g = new Date(n.calendar.year, n.calendar.month - 1, 1); g.getDay() > 1;) g.setDate(g.getDate() - 1);
-            for (var b = 0;
-                (g.getMonth() <= f || h[b].length < 7) && (h[b].length == 7 && (b += 1), b != 5);) h[b].push({
+                ], v = n.calendar.month - 1, g = new Date(n.calendar.year, n.calendar.month - 1, 1); g.getDay() > 1;) g.setDate(g.getDate() - 1);
+            for (var k = 0;
+                (g.getMonth() <= v || m[k].length < 7) && (m[k].length == 7 && (k += 1), k != 5);) m[k].push({
                 date: g.getDate(),
                 total: n.calendar.total[g.toLocaleDateString("pt-BR")],
-                today: g.getDate() === Ee.getDate(),
-                selected: ce ? g.getDate() == ce.getDate() : !1
+                today: g.getDate() === Ie.getDate(),
+                selected: ue ? g.getDate() == ue.getDate() : !1
             }), g.setDate(g.getDate() + 1);
             return t.jsxs("div", {
                 className: "calendar",
                 children: [t.jsxs("div", {
-                    style: Q,
+                    style: Ee,
                     children: [t.jsx("div", {
-                        children: t.jsx(ue, {
+                        children: t.jsx(he, {
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
-                            children: [R[n.calendar.month - 1], " ", n.calendar.year]
+                            children: [ae[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
-                            className: E,
-                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(k, {
+                            className: F,
+                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(S, {
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
-                        children: t.jsx(ue, {
+                        children: t.jsx(he, {
                             default: !0,
                             icon: "arrow-right",
                             onClick: () => c(null, n.calendar.next.month, n.calendar.next.year)
                         })
                     })]
                 }), t.jsxs("table", {
-                    style: ne,
+                    style: A,
                     children: [t.jsx("thead", {
                         children: t.jsx("tr", {
-                            children: T.map(ae => t.jsx("th", {
-                                children: ae
+                            children: E.map(re => t.jsx("th", {
+                                children: re
                             }, Math.random()))
                         })
                     }), t.jsx("tbody", {
-                        children: h.map(ae => t.jsx("tr", {
-                            children: ae.map(O => t.jsxs("td", {
-                                style: z,
+                        children: m.map(re => t.jsx("tr", {
+                            children: re.map(O => t.jsxs("td", {
+                                style: V,
                                 children: [t.jsx("div", {
-                                    style: E,
+                                    style: F,
                                     children: O.today ? t.jsx("span", {
                                         style: {
                                             textDecoration: "underline"
                                         },
                                         children: O.date
                                     }) : O.date + O.today
                                 }), O.total && t.jsx("div", {
-                                    style: _,
+                                    style: $,
                                     onClick: () => c(O.date, n.calendar.month, n.calendar.year),
                                     children: t.jsx("div", {
-                                        style: G,
+                                        style: P,
                                         children: t.jsx("span", {
                                             style: {
                                                 textDecoration: O.selected ? "underline" : "normal"
                                             },
                                             children: O.total
                                         })
                                     })
                                 }), !O.total && t.jsx("div", {
-                                    style: _,
+                                    style: $,
                                     children: " "
                                 })]
                             }, Math.random()))
                         }, Math.random()))
                     })]
                 })]
             })
         }
     }
 
-    function l(h) {
-        const f = {
+    function o(m) {
+        const v = {
             textAlign: "left",
             verticalAlign: "top",
-            backgroundColor: "#f0f0f0",
             lineHeight: "3rem",
-            color: "#1351b4",
+            color: C.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
-            children: [h.map(function(g) {
+            children: [m.map(function(g) {
                 return g.label != "ID" && t.jsx("th", {
-                    style: f,
+                    style: v,
+                    className: "bold",
                     children: g.label
                 }, Math.random())
             }), t.jsx("th", {
-                style: f
+                style: v
             })]
         })
     }
 
-    function m(h) {
-        const f = {
+    function h(m) {
+        const v = {
                 borderBottom: "solid 1px #DDD",
                 padding: 5
             },
             g = {
                 borderBottom: "solid 1px #DDD",
                 lineHeight: "3rem",
                 textAlign: "right"
             };
         return window.innerWidth < 800 ? t.jsxs("tr", {
             children: [t.jsx("td", {
-                style: f,
-                children: h.title
+                style: v,
+                children: m.title
             }, Math.random()), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: h.actions.map(function(b) {
-                        return t.jsx(N, {
-                            data: b,
+                    children: m.actions.map(function(k) {
+                        return t.jsx(_, {
+                            data: k,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [h.data.map(function(b) {
-                return b.label != "ID" && t.jsx("td", {
-                    style: f,
-                    children: U(b.value)
+            children: [m.data.map(function(k) {
+                return k.label != "ID" && t.jsx("td", {
+                    style: v,
+                    children: z(k.value)
                 }, Math.random())
             }), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: h.actions.map(function(b) {
-                        return t.jsx(N, {
-                            data: b,
+                    children: m.actions.map(function(k) {
+                        return t.jsx(_, {
+                            data: k,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
     }
 
-    function x() {
+    function f() {
         return n.data.length > 0 ? n.renderer ? t.jsx("div", {
             style: {
                 marginBottom: 15
             },
-            children: n.data.map(function(h) {
-                return h.type = n.renderer, t.jsx(p, {
-                    data: h
+            children: n.data.map(function(m) {
+                return m.type = n.renderer, t.jsx(p, {
+                    data: m
                 }, Math.random())
             })
-        }) : w() : t.jsx(le, {
+        }) : w() : t.jsx(oe, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
-        const h = {
+        const m = {
                 width: "100%",
                 overflowX: "auto"
             },
-            f = {
+            v = {
                 width: "100%",
                 lineHeight: "2rem",
                 borderSpacing: 0
             };
         return t.jsx("div", {
-            style: h,
+            style: m,
             children: t.jsxs("table", {
-                style: f,
+                style: v,
                 children: [t.jsx("thead", {
-                    children: l(n.data[0].data)
+                    children: o(n.data[0].data)
                 }), t.jsx("tbody", {
                     children: n.data.map(function(g) {
-                        return m(g)
+                        return h(g)
                     })
                 })]
             })
         })
     }
 
-    function S(h) {
+    function M(m) {
         const g = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        g.value = h, v()
+        g.value = m, y()
     }
 
-    function B() {
-        const h = document.getElementById("form-" + e.data.id);
-        if (h) {
-            const T = h.querySelector("input[name=page]");
-            T && (T.value = n.pagination.page.current)
+    function D() {
+        const m = document.getElementById("form-" + e.data.id);
+        if (m) {
+            const E = m.querySelector("input[name=page]");
+            E && (E.value = n.pagination.page.current)
         }
-        const f = {
+        const v = {
                 display: "flex",
                 justifyContent: "space-between",
                 lineHeight: "4rem",
                 alignItems: "baseline"
             },
             g = {
                 display: "inline",
                 paddingRight: 10
             },
-            b = {
+            k = {
                 marginLeft: 10,
                 marginRight: 10,
                 height: "2.5rem",
                 paddingLeft: 5,
                 paddingRight: 5,
                 textAlign: "center"
             };
         return n.pagination.page.total > 1 && t.jsxs("div", {
-            style: f,
+            style: v,
             children: [t.jsxs("div", {
                 children: [t.jsxs("div", {
                     style: g,
                     children: ["Exibir", t.jsx("select", {
-                        style: b,
+                        style: k,
                         name: "page_size",
-                        onChange: () => S(1),
+                        onChange: () => M(1),
                         value: n.pagination.page.size,
-                        children: n.pagination.page.sizes.map(function(T) {
+                        children: n.pagination.page.sizes.map(function(E) {
                             return t.jsx("option", {
-                                children: T
+                                children: E
                             }, Math.random())
                         })
                     })]
                 }), t.jsx("div", {
                     style: g,
                     children: "|"
                 }), t.jsxs("div", {
@@ -2544,157 +2623,157 @@
                         style: {
                             width: 30,
                             marginLeft: 10,
                             marginRight: 10,
                             height: "2rem",
                             textAlign: "center"
                         },
-                        onKeyDown: function(T) {
-                            T.key == "Enter" && (T.preventDefault(), S(T.target.value < 0 ? 1 : Math.min(T.target.value, n.pagination.page.total)))
+                        onKeyDown: function(E) {
+                            E.key == "Enter" && (E.preventDefault(), M(E.target.value < 0 ? 1 : Math.min(E.target.value, n.pagination.page.total)))
                         }
                     }), t.jsx("div", {
                         style: g,
                         children: "|"
-                    }), n.pagination.page.previous && t.jsx(A, {
+                    }), n.pagination.page.previous && t.jsx(R, {
                         icon: "chevron-left",
                         default: !0,
                         display: "inline",
-                        onClick: () => S(n.pagination.page.previous)
-                    }), n.pagination.page.next && t.jsx(A, {
+                        onClick: () => M(n.pagination.page.previous)
+                    }), n.pagination.page.next && t.jsx(R, {
                         icon: "chevron-right",
                         default: !0,
                         display: "inline",
-                        onClick: () => S(n.pagination.page.next)
+                        onClick: () => M(n.pagination.page.next)
                     })]
                 })
             })]
         })
     }
 
-    function y() {
+    function x() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
-            children: n.actions.map(function(h) {
-                return t.jsx(N, {
-                    data: h,
+            children: n.actions.map(function(m) {
+                return t.jsx(_, {
+                    data: m,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
     function j() {
-        const h = {
+        const m = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
-            f = n.search.length > 0,
+            v = n.search.length > 0,
             g = n.filters.length > 0;
-        if ((n.bi || n.data.length > 0) && (f || g)) {
-            const b = {
+        if ((n.bi || n.data.length >= 0) && (v || g)) {
+            const k = {
                 name: "q",
                 value: "",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves"
             };
             return t.jsxs("div", {
-                style: h,
-                children: [t.jsxs($, {
+                style: m,
+                children: [t.jsxs(G, {
                     width: 250,
-                    children: [f && t.jsx("div", {
+                    children: [v && t.jsx("div", {
                         children: t.jsx(K, {
-                            data: b
+                            data: k
                         })
-                    }), g && n.filters.map(function(T) {
-                        return T.type != "hidden" && t.jsx("div", {
+                    }), g && n.filters.map(function(E) {
+                        return E.type != "hidden" && t.jsx("div", {
                             children: t.jsx(K, {
-                                data: T
+                                data: E
                             })
                         }, Math.random())
                     }), t.jsx("div", {
-                        children: t.jsx(A, {
-                            onClick: v,
+                        children: t.jsx(R, {
+                            onClick: y,
                             label: "Filtrar",
                             icon: "filter",
                             primary: !0
                         })
                     })]
-                }), g && n.filters.map(function(T) {
-                    return T.type == "hidden" && t.jsx("div", {
+                }), g && n.filters.map(function(E) {
+                    return E.type == "hidden" && t.jsx("div", {
                         children: t.jsx(K, {
-                            data: T
+                            data: E
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function v() {
+    function y() {
         i(!0);
-        var h;
-        const f = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? h = e.data.url + "&" + f : h = e.data.url + "?" + f, I("GET", h, function(g) {
+        var m;
+        const v = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
+        e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + v : m = e.data.url + "?" + v, B("GET", m, function(g) {
             a(g), i(!1)
         })
     }
 
     function L() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [j(), n.bi.map(function(h) {
-                return t.jsx($, {
+            children: [j(), n.bi.map(function(m) {
+                return t.jsx(G, {
                     width: 300,
                     alignItems: "start",
-                    children: h.map(function(f) {
+                    children: m.map(function(v) {
                         return t.jsx("div", {
                             children: t.jsx(p, {
-                                data: f
+                                data: v
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [y(), o(), j(), u(), x(), B()]
+            children: [x(), l(), j(), u(), f(), D()]
         })
     }
 
-    function D() {
-        window[e.data.id] = () => v();
-        const h = {
+    function b() {
+        window[e.data.id] = () => y();
+        const m = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable",
             id: e.data.id,
-            sytle: h,
+            sytle: m,
             children: t.jsxs("form", {
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
                 }), d(), L()]
             })
         })
     }
-    return D()
+    return b()
 }
 
-function te(e) {
+function ne(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
         if (r) {
             var d = echarts.init(r);
             d.setOption(e.option)
@@ -2705,15 +2784,15 @@
         style: {
             width: "100%",
             height: 300
         }
     })
 }
 
-function de(e) {
+function se(e) {
     var n = [
         ["70%", "78%"],
         ["60%", "68%"],
         ["50%", "58%"],
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
@@ -2725,25 +2804,25 @@
             return {
                 name: d,
                 type: "pie",
                 radius: n[i],
                 emphasis: {
                     label: {
                         show: !0,
-                        formatter: function(o) {
-                            return o.value.toLocaleString("pt-BR")
+                        formatter: function(l) {
+                            return l.value.toLocaleString("pt-BR")
                         },
                         fontWeight: "bold"
                     }
                 },
                 roseType: null,
-                data: e.rows.map(function(o) {
+                data: e.rows.map(function(l) {
                     return {
-                        name: o[0],
-                        value: o[i + 1]
+                        name: l[0],
+                        value: l[i + 1]
                     }
                 })
             }
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
@@ -2779,38 +2858,38 @@
                 show: !0,
                 formatter(i) {
                     return i.name + " (" + i.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
-        return t.jsx(te, {
+        return t.jsx(ne, {
             option: d
         })
     }
     return r()
 }
 
-function ht(e) {
-    return t.jsx(de, {
+function mt(e) {
+    return t.jsx(se, {
         donut: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function mt(e) {
-    return t.jsx(de, {
+function ft(e) {
+    return t.jsx(se, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function F(e) {
+function W(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
         d = {
             type: "value"
         },
         i = {
@@ -2820,128 +2899,128 @@
                     show: !0
                 },
                 saveAsImage: {
                     show: !0
                 }
             }
         },
-        o = e.area ? {} : null;
+        l = e.area ? {} : null;
 
     function s() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
-            data: e.rows.map(function(l) {
-                return l[0]
+            data: e.rows.map(function(o) {
+                return o[0]
             })
         }
     }
 
     function c() {
-        return e.headers ? e.rows.map(function(l) {
+        return e.headers ? e.rows.map(function(o) {
             return {
-                name: l[0],
-                data: l.slice(1),
+                name: o[0],
+                data: o.slice(1),
                 type: a,
                 stack: r,
-                areaStyle: o
+                areaStyle: l
             }
         }) : [{
             name: null,
-            data: e.rows.map(function(l) {
-                return l[1]
+            data: e.rows.map(function(o) {
+                return o[1]
             }),
             type: a,
             stack: r,
-            areaStyle: o
+            areaStyle: l
         }]
     }
 
     function u() {
-        var l = {
+        var o = {
             toolbox: i,
             tooltip: {
                 trigger: "axis",
                 axisPointer: {
                     type: "shadow"
                 },
-                formatter: function(m) {
-                    return `${m[0].name}: <b>${m[0].value.toLocaleString("pt-BR")}</b>`
+                formatter: function(h) {
+                    return `${h[0].name}: <b>${h[0].value.toLocaleString("pt-BR")}</b>`
                 }
             },
             legend: {},
             label: {
                 show: !0,
-                formatter: function(m) {
-                    return m.value.toLocaleString("pt-BR")
+                formatter: function(h) {
+                    return h.value.toLocaleString("pt-BR")
                 }
             },
             xAxis: n ? d : s(),
             yAxis: n ? s() : d,
             series: c()
         };
-        return t.jsx(te, {
-            option: l
+        return t.jsx(ne, {
+            option: o
         })
     }
     return u()
 }
 
-function ft(e) {
-    return t.jsx(F, {
+function gt(e) {
+    return t.jsx(W, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function gt(e) {
-    return t.jsx(F, {
+function xt(e) {
+    return t.jsx(W, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function xt(e) {
-    return t.jsx(F, {
+function yt(e) {
+    return t.jsx(W, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function yt(e) {
-    return t.jsx(F, {
+function vt(e) {
+    return t.jsx(W, {
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function pt(e) {
-    return t.jsx(F, {
+    return t.jsx(W, {
         invert: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function vt(e) {
-    return t.jsx(F, {
+function bt(e) {
+    return t.jsx(W, {
         invert: !0,
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function bt(e) {
+function wt(e) {
     function n() {
         return e.headers ? [{
             type: "treemap",
             roam: "move",
             nodeClick: !0,
             data: e.headers.slice(1).map(function(r, d) {
                 return {
@@ -2978,22 +3057,22 @@
                 show: !0,
                 formatter(d) {
                     return d.name + " (" + d.value.toLocaleString("pt-BR") + ")"
                 }
             },
             series: n()
         };
-        return t.jsx(te, {
+        return t.jsx(ne, {
             option: r
         })
     }
     return a()
 }
 
-function wt(e) {
+function jt(e) {
     function n() {
         var a = {
             series: [{
                 type: "gauge",
                 startAngle: 0,
                 endAngle: 360,
                 min: 0,
@@ -3027,81 +3106,81 @@
                     }
                 },
                 data: [{
                     value: e.value
                 }]
             }]
         };
-        return t.jsx(te, {
+        return t.jsx(ne, {
             option: a
         })
     }
     return n()
 }
 
-function fe(e) {
+function ge(e) {
     function n() {
         switch (e.type) {
             case "pie":
-                return t.jsx(de, {
+                return t.jsx(se, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "polar":
-                return t.jsx(mt, {
+                return t.jsx(ft, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "donut":
-                return t.jsx(ht, {
+                return t.jsx(mt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "bar":
-                return t.jsx(ft, {
+                return t.jsx(gt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_bar":
-                return t.jsx(yt, {
+                return t.jsx(vt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "column":
                 return t.jsx(pt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_column":
-                return t.jsx(vt, {
+                return t.jsx(bt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "tree_map":
-                return t.jsx(bt, {
+                return t.jsx(wt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "line":
-                return t.jsx(gt, {
+                return t.jsx(xt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "area":
-                return t.jsx(xt, {
+                return t.jsx(yt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "progress":
-                return t.jsx(wt, {
+                return t.jsx(jt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             default:
-                return t.jsx(F, {
+                return t.jsx(W, {
                     headers: e.headers,
                     rows: e.rows
                 })
         }
     }
 
     function a() {
@@ -3115,234 +3194,213 @@
                 children: e.title
             }), n()]
         })
     }
     return a()
 }
 
-function jt(e) {
+function kt(e) {
     function n() {
         for (var r = [], d = 0; d < e.data.series.length; d++) r.push([e.data.series[d][0], e.data.series[d][1]]);
-        return e.data.chart ? t.jsx(fe, {
+        return e.data.chart ? t.jsx(ge, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": C(e.data.title),
+                "data-label": T(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%"
                 },
                 children: t.jsx("tbody", {
                     children: r.map(i => t.jsx("tr", {
-                        children: i.map((o, s) => s == 0 ? t.jsx("th", {
+                        children: i.map((l, s) => s == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left",
                                 lineHeight: "2rem"
                             },
-                            children: o
+                            children: l
                         }, Math.random()) : t.jsx("td", {
-                            children: U(o)
+                            children: z(l)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], d = [], i = Object.keys(e.data.series), o = [], s = 0; s < i.length; s++) {
+        for (var r = [], d = [], i = Object.keys(e.data.series), l = [], s = 0; s < i.length; s++) {
             s == 0 && r.push("");
-            for (var c = [i[s]], u = 0, l = 0; l < e.data.series[i[s]].length; l++) {
-                var m = e.data.series[i[s]];
-                s == 0 && r.push(m[l][0]), c.push(m[l][1]), u += m[l][1], i.length > 1 && (s == 0 ? o.push(m[l][1]) : o[l] += m[l][1], l > 0 && l == e.data.series[i[s]].length - 1 && (s == 0 ? o.push(u) : o[l + 1] += u))
+            for (var c = [i[s]], u = 0, o = 0; o < e.data.series[i[s]].length; o++) {
+                var h = e.data.series[i[s]];
+                s == 0 && r.push(h[o][0]), c.push(h[o][1]), u += h[o][1], i.length > 1 && (s == 0 ? l.push(h[o][1]) : l[o] += h[o][1], o > 0 && o == e.data.series[i[s]].length - 1 && (s == 0 ? l.push(u) : l[o + 1] += u))
             }
             c.length > 2 && (s == 0 && r.push("TOTAL"), c.push(u)), d.push(c)
         }
-        return e.data.chart ? t.jsx(fe, {
+        return e.data.chart ? t.jsx(ge, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
             rows: d
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": C(e.data.title),
+                "data-label": T(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%"
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: r.map(x => t.jsx("th", {
-                            children: x
+                        children: r.map(f => t.jsx("th", {
+                            children: f
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [d.map(x => t.jsx("tr", {
-                        children: x.map((w, S) => S == 0 ? t.jsx("th", {
+                    children: [d.map(f => t.jsx("tr", {
+                        children: f.map((w, M) => M == 0 ? t.jsx("th", {
                             children: w
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
                             style: {
-                                backgroundColor: S == x.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
+                                backgroundColor: M == f.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
                             },
-                            children: U(w)
+                            children: z(w)
                         }, Math.random()))
-                    }, Math.random())), o.length > 0 && t.jsxs("tr", {
+                    }, Math.random())), l.length > 0 && t.jsxs("tr", {
                         children: [t.jsx("th", {
                             children: "TOTAL"
-                        }), o.map(x => t.jsxs("td", {
+                        }), l.map(f => t.jsxs("td", {
                             align: "center",
                             style: {
                                 backgroundColor: "var(--info-color)"
                             },
-                            children: [U(x), " "]
+                            children: [z(f), " "]
                         }, Math.random()))]
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
 }
-const Te = {
-    primary: "#1351b4",
-    success: "green",
-    warning: "orange",
-    info: "blue",
-    danger: "red"
-};
-
-function kt(e) {
-    function n() {
-        const a = {
-            width: 30,
-            height: 30,
-            borderRadius: "50%",
-            backgroundColor: e.data.value
-        };
-        return t.jsx("div", {
-            style: a
-        })
-    }
-    return n()
-}
 
 function St() {
     function e() {
         const i = {
             width: 150,
             height: 150,
             borderRadius: "50%",
-            objectFit: "cover"
+            objectFit: "cover",
+            backgroundColor: C.colors.primary
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: i
                 })
             }), t.jsx("div", {
-                children: t.jsx(W, {
+                children: t.jsx(N, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
             })]
         })
     }
 
     function n(i) {
-        var o = i.target;
-        const s = o.querySelector(":scope > ul, :scope > li");
+        var l = i.target;
+        const s = l.querySelector(":scope > ul, :scope > li");
         if (s) {
-            s.offsetParent === null ? o.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(l) {
-                l.style.display = "block"
-            }) : o.querySelectorAll(":scope > ul, :scope > li").forEach(function(l) {
-                l.style.display = "none"
+            s.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(o) {
+                o.style.display = "block"
+            }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(o) {
+                o.style.display = "none"
             });
-            const c = o.querySelector(":scope > i.fa-solid.fa-chevron-right"),
-                u = o.querySelector(":scope > i.fa-solid.fa-chevron-up");
+            const c = l.querySelector(":scope > i.fa-solid.fa-chevron-right"),
+                u = l.querySelector(":scope > i.fa-solid.fa-chevron-up");
             return c && (c.classList.remove("fa-chevron-right"), c.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), i.preventDefault(), i.stopPropagation(), i.cancelBubble = !0, !1
         } else {
             const c = document.querySelector("aside");
             c.style.display = window.innerWidth < 800 ? "none" : "block"
         }
     }
 
-    function a(i, o) {
+    function a(i, l) {
         const s = {
-                display: o == 0 ? "block" : "none",
+                display: l == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 5,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
-                color: "#1351b4"
+                color: C.colors.primary
             },
             c = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return i.url ? t.jsx("li", {
             style: s,
             onClick: n,
-            children: t.jsxs(W, {
+            children: t.jsxs(N, {
                 href: i.url,
-                dataLabel: C(i.label),
+                dataLabel: T(i.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [o == 0 && t.jsx(k, {
+                children: [l == 0 && t.jsx(S, {
                     icon: i.icon || "dot-circle",
                     style: c
                 }), i.label]
             })
         }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: s,
-            "data-label": C(i.label),
-            children: [o == 0 && t.jsx(k, {
+            "data-label": T(i.label),
+            children: [l == 0 && t.jsx(S, {
                 icon: i.icon || "dot-circle",
                 style: c
-            }), i.label, t.jsx(k, {
+            }), i.label, t.jsx(S, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
                     display: "none",
                     paddingLeft: 15
                 },
                 children: i.items.map(function(u) {
-                    return a(u, o + 1)
+                    return a(u, l + 1)
                 })
             })]
         }, Math.random())
     }
 
     function r() {
         const i = {
             padding: 0
         };
         return window.application.menu.items.length > 0 && t.jsx("ul", {
             style: i,
-            children: window.application.menu.items.map(function(o) {
-                return a(o, 0)
+            children: window.application.menu.items.map(function(l) {
+                return a(l, 0)
             })
         })
     }
 
     function d() {
         const i = {
             padding: 25,
@@ -3357,34 +3415,34 @@
     return d()
 }
 
 function Ct(e) {
     var n;
 
     function a(i) {
-        const o = "=".repeat((4 - i.length % 4) % 4),
-            s = (i + o).replace(/\-/g, "+").replace(/_/g, "/"),
+        const l = "=".repeat((4 - i.length % 4) % 4),
+            s = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
             c = window.atob(s),
             u = new Uint8Array(c.length);
-        for (let l = 0; l < c.length; ++l) u[l] = c.charCodeAt(l);
+        for (let o = 0; o < c.length; ++o) u[o] = c.charCodeAt(o);
         return u
     }
 
     function r() {
         "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(i) {
             if (i) {
-                const o = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
+                const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
                 i.pushManager.subscribe({
                     userVisibleOnly: !0,
-                    applicationServerKey: o
+                    applicationServerKey: l
                 }).then(function(s) {
                     if (console.log(s), n = JSON.stringify(s), console.log(n), s) {
                         alert("Notificação ativada com sucesso.");
                         var c = new FormData;
-                        c.append("subscription", n), I("POST", "/api/pushsubscribe/", function(u) {
+                        c.append("subscription", n), B("POST", "/api/pushsubscribe/", function(u) {
                             console.log(u)
                         }, c)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
                 }).catch(function(s) {
@@ -3393,15 +3451,15 @@
             } else console.log("No registered service worker.")
         }).catch(function(i) {
             alert("Erro"), console.error("Service Worker Error", i)
         }) : alert("Push messaging is not supported")
     }
 
     function d() {
-        return t.jsx(k, {
+        if (Notification.permission !== "granted") return t.jsx(S, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer"
             }
         })
     }
@@ -3430,36 +3488,36 @@
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 80
                 },
                 onClick: () => history.back(),
-                children: t.jsx(k, {
+                children: t.jsx(S, {
                     icon: "arrow-left",
                     style: r
                 })
             }), t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 20
                 },
                 onClick: () => window.scrollTo(0, 0),
-                children: t.jsx(k, {
+                children: t.jsx(S, {
                     icon: "arrow-up",
                     style: r
                 })
             })]
         })
     }
     return n()
 }
 
 function Mt(e) {
-    const [n, a] = M.useState(e.data);
+    const [n, a] = I.useState(e.data);
     window.loaddata = d => a(d);
 
     function r() {
         const d = {
             minHeight: 400,
             margin: 20
         };
@@ -3471,176 +3529,205 @@
             }, Math.random())
         })
     }
     return r()
 }
 
 function Et(e) {
-    M.useEffect(() => {
-        const l = localStorage.getItem("message");
-        l && (localStorage.removeItem("message"), ee(l)), window.addEventListener("resize", () => {
-            const m = document.querySelector("aside");
-            m.style.display = window.innerWidth < 800 ? "none" : "block"
+    I.useEffect(() => {
+        const o = localStorage.getItem("message");
+        o && (localStorage.removeItem("message"), te(o)), window.addEventListener("resize", () => {
+            const h = document.querySelector("aside");
+            h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
         })
     }, []);
 
     function a() {
-        const l = document.querySelector("aside");
-        l.style.display = l.style.display == "none" ? "block" : "none"
+        const o = document.querySelector("aside");
+        o.style.display = o.style.display == "none" ? "block" : "none"
     }
 
-    function r(l) {
-        l.preventDefault(), window.load(l.target.href)
+    function r(o) {
+        o.preventDefault(), window.load(o.target.href)
     }
 
     function d() {
-        const l = {
+        const o = {
                 display: "flex",
                 width: "100%",
                 justifyContent: "space-between",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 overflowX: "hidden"
             },
-            m = {
+            h = {
                 choices: "/api/search/",
                 help_text: null,
                 label: null,
                 mask: null,
                 name: "search",
                 required: !1,
-                type: "choice"
+                type: "choice",
+                icon: "search"
             };
         return e.data.navbar ? t.jsxs("div", {
-            style: l,
+            style: o,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [t.jsx(k, {
+                children: [e.data.menu && t.jsx(S, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
                 }), t.jsxs("a", {
-                    href: "/app/dashboard/",
+                    className: "brand",
+                    href: "/app/home/",
                     onClick: r,
                     style: {
                         fontSize: "1.5rem",
                         textDecoration: "none"
                     },
                     children: [e.data.navbar.logo && t.jsx("img", {
                         src: e.data.navbar.logo,
-                        height: 20
-                    }), e.data.navbar.title]
+                        height: 20,
+                        style: {
+                            marginRight: 10
+                        }
+                    }), t.jsx("span", {
+                        children: e.data.navbar.title
+                    })]
+                }), t.jsx("div", {
+                    children: e.data.navbar.subtitle
                 })]
             }), t.jsxs("div", {
                 style: {
                     display: "flex",
                     alignItems: "center"
                 },
                 children: [e.data.navbar.adder.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(k, {
+                        children: t.jsx(S, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Ct, {})
+                }), e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(f) {
+                    return f.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
+                        children: t.jsx(_, {
+                            data: f,
+                            primary: !0
+                        }, Math.random())
+                    })
+                }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(f) {
+                    return t.jsx(N, {
+                        href: f.url,
+                        children: f.label
+                    })
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(k, {
+                        children: t.jsx(S, {
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
-                        children: t.jsx(k, {
+                        children: t.jsx(S, {
                             icon: "gear"
                         })
                     })
-                }), window.innerWidth > 800 && t.jsx(Ce, {
-                    data: m,
-                    style: {
-                        padding: 10
-                    },
-                    onSelect: x => document.location.href = H(x.id)
+                }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
+                    children: t.jsx(Te, {
+                        data: h,
+                        style: {
+                            padding: 10
+                        },
+                        onSelect: f => document.location.href = U(f.id)
+                    })
                 }), e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: C(e.data.navbar.user),
+                        dataLabel: T(e.data.navbar.user),
                         children: e.data.navbar.user
                     })
                 })]
             })]
         }) : null
     }
 
     function i() {
-        return window.application.menu && t.jsx("aside", {
+        return window.application.menu && window.application.menu.items.length > 0 && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
             children: t.jsx(St, {})
         })
     }
 
-    function o() {
-        const l = {
+    function l() {
+        const o = {
                 margin: 15
             },
-            m = {
-                color: "#1351b4"
+            h = {
+                color: C.colors.primary
             };
-        return e.data.navbar && t.jsxs("div", {
-            style: l,
-            children: [t.jsx(k, {
-                icon: "home",
-                style: m
-            }), " Área Administrativa"]
+        return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
+            style: o,
+            children: [t.jsx(N, {
+                href: "/app/dashboard/",
+                style: {
+                    marginRight: 10
+                },
+                children: t.jsx(S, {
+                    icon: "home",
+                    style: h
+                })
+            }), "Área Administrativa"]
         })
     }
 
     function s() {
         return t.jsxs("main", {
             style: {
                 flexGrow: 6,
                 minWidth: "400px"
             },
-            children: [o(), t.jsx(Mt, {
+            children: [l(), t.jsx(Mt, {
                 data: e.data.content
             }), t.jsx("footer", {
                 children: c()
             }), t.jsx(Tt, {})]
         })
     }
 
@@ -3684,97 +3771,97 @@
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
                 offerToReceiveVideo: 1
             },
-            sdpTransform: y => y.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
+            sdpTransform: x => x.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
-    M.useEffect(() => {
-        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(y) {
+    I.useEffect(() => {
+        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(x) {
             document.getElementById("callerid").innerHTML = e.data.caller
-        }), n.on("call", function(y) {
+        }), n.on("call", function(x) {
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
-                var v = document.getElementById("video2");
-                v.addEventListener("loadedmetadata", function(L) {
-                    v.style.width = this.videoWidth / 4 + "px", v.style.height = this.videoHeight / 4 + "px", v.style.marginLeft = -this.videoWidth / 4 + "px", v.style.visibility = "visible"
-                }, !1), v.srcObject = a, y.answer(j), y.on("stream", function(L) {
+                var y = document.getElementById("video2");
+                y.addEventListener("loadedmetadata", function(L) {
+                    y.style.width = this.videoWidth / 4 + "px", y.style.height = this.videoHeight / 4 + "px", y.style.marginLeft = -this.videoWidth / 4 + "px", y.style.visibility = "visible"
+                }, !1), y.srcObject = a, x.answer(j), x.on("stream", function(L) {
                     r = L, document.getElementById("video1").srcObject = r
-                }), y.on("close", function() {
+                }), x.on("close", function() {
                     c()
                 }), n.on("error", function(L) {
                     c()
                 })
             }, function(j) {
                 console.log("Failed to get local stream", j)
             })
-        }), n.on("error", function(y) {
-            y.type == "browser-incompatible" ? alert("Navegador incompatível.") : y.type == "invalid-id" ? alert("Usuário inexistente.") : y.type == "network" ? alert("Problema na conexão do usuário.") : y.type == "peer-unavailable" && alert("Usuário indisponível.")
+        }), n.on("error", function(x) {
+            x.type == "browser-incompatible" ? alert("Navegador incompatível.") : x.type == "invalid-id" ? alert("Usuário inexistente.") : x.type == "network" ? alert("Problema na conexão do usuário.") : x.type == "peer-unavailable" && alert("Usuário indisponível.")
         })
     }, []);
 
-    function o() {
-        l(a, "audio"), l(a, "video"), l(r, "audio"), l(r, "video")
+    function l() {
+        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video")
     }
 
     function s() {
-        m(a, "audio"), m(a, "video"), m(r, "audio"), m(r, "video")
+        h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video")
     }
 
     function c() {
         u(a, "audio"), u(a, "video"), u(r, "audio"), u(r, "video"), a = null, r = null, document.getElementById("video1").srcObject = null, document.getElementById("video2").srcObject = null, console.log("Stopped!")
     }
 
-    function u(y, j) {
-        y != null && y.getTracks().forEach(v => {
-            v.readyState == "live" && v.kind === j && v.stop()
+    function u(x, j) {
+        x != null && x.getTracks().forEach(y => {
+            y.readyState == "live" && y.kind === j && y.stop()
         })
     }
 
-    function l(y, j) {
-        y != null && y.getTracks().forEach(v => {
-            v.readyState == "live" && v.kind === j && (v.enabled = !1)
+    function o(x, j) {
+        x != null && x.getTracks().forEach(y => {
+            y.readyState == "live" && y.kind === j && (y.enabled = !1)
         })
     }
 
-    function m(y, j) {
-        y != null && y.getTracks().forEach(v => {
-            v.readyState == "live" && v.kind === j && (v.enabled = !0)
+    function h(x, j) {
+        x != null && x.getTracks().forEach(y => {
+            y.readyState == "live" && y.kind === j && (y.enabled = !0)
         })
     }
 
-    function x() {
-        var y = document.getElementById("video1");
-        y.style.width == "" ? y.style.width = "400px" : y.style.width = ""
+    function f() {
+        var x = document.getElementById("video1");
+        x.style.width == "" ? x.style.width = "400px" : x.style.width = ""
     }
 
     function w() {
-        var y = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, i);
-        y.on("stream", function(j) {
+        var x = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, i);
+        x.on("stream", function(j) {
             r = j, document.getElementById("video1").srcObject = r
-        }), y.on("close", function() {
+        }), x.on("close", function() {
             c()
         }), n.on("error", function(j) {
             c()
         })
     }
 
-    function S() {
+    function M() {
         if (a != null && r == null) return w();
         if (a != null && r != null) return s();
         d({
             video: {
                 width: {
                     exact: 320
                 },
@@ -3788,89 +3875,89 @@
                 echoCancellation: !1,
                 latency: 0,
                 noiseSuppression: !1,
                 sampleRate: 48e3,
                 sampleSize: 16,
                 volume: 1
             }
-        }, function(y) {
-            a = y;
+        }, function(x) {
+            a = x;
             var j = document.getElementById("video2");
-            j.addEventListener("loadedmetadata", function(v) {
+            j.addEventListener("loadedmetadata", function(y) {
                 j.style.width = this.videoWidth / 4 + "px", j.style.height = this.videoHeight / 4 + "px", j.style.marginLeft = -this.videoWidth / 4 + "px", j.style.visibility = "visible"
             }, !1), j.srcObject = a, w()
-        }, function(y) {
+        }, function(x) {
             alert("Failed to get local stream.")
         })
     }
 
-    function B() {
-        var y = {
+    function D() {
+        var x = {
                 width: "fit-content",
                 margin: "auto"
             },
             j = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
-            v = {
+            y = {
                 color: "white",
                 backgroundColor: "black",
                 padding: 2
             },
             L = {
                 position: "absolute",
                 marginTop: "-30px"
             },
-            D = {
+            b = {
                 backgroundColor: "black"
             },
-            h = {
+            m = {
                 visibility: "hidden",
                 width: "0px"
             };
         return t.jsxs("div", {
-            style: y,
+            style: x,
             children: [t.jsx("div", {
                 id: "callerid",
                 style: j
             }), t.jsx("video", {
                 id: "video1",
-                style: D,
+                style: b,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsx("video", {
                 id: "video2",
-                style: h,
+                style: m,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsxs("div", {
                 style: L,
-                children: [t.jsx(k, {
-                    style: v,
-                    onClick: S,
+                children: [t.jsx(S, {
+                    style: y,
+                    onClick: M,
                     icon: "play"
-                }), t.jsx(k, {
-                    style: v,
-                    onClick: o,
+                }), t.jsx(S, {
+                    style: y,
+                    onClick: l,
                     icon: "pause"
-                }), t.jsx(k, {
-                    style: v,
+                }), t.jsx(S, {
+                    style: y,
                     onClick: c,
                     icon: "stop"
-                }), t.jsx(k, {
-                    style: v,
-                    onClick: x,
+                }), t.jsx(S, {
+                    style: y,
+                    onClick: f,
                     icon: "maximize"
                 })]
             })]
         })
     }
-    return B()
+    return D()
 }
 
 function Bt(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
@@ -3907,15 +3994,15 @@
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
 function At(e) {
     function n(i) {
-        return e.data.icon ? i.done ? t.jsx(k, {
+        return e.data.icon ? i.done ? t.jsx(S, {
             style: {
                 marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
@@ -3924,18 +4011,18 @@
             },
             children: i.number
         })
     }
 
     function a(i) {
         return {
-            border: "3px solid " + (i.done ? "#1351b4" : "#1151b3"),
+            border: "3px solid " + C.colors.primary,
             borderRadius: "50%",
-            background: i.done ? "#1351b4" : "white",
-            color: i.done ? "white" : "#1151b3",
+            background: i.done ? C.colors.primary : "white",
+            color: i.done ? "white" : C.colors.primary,
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
@@ -3954,15 +4041,15 @@
                 width: "100%",
                 margin: "auto",
                 overflowX: "auto",
                 "&::WebkitScrollbar": {
                     width: 0
                 }
             },
-            o = {
+            l = {
                 width: 100,
                 marginWidth: 100,
                 textAlign: "center"
             },
             s = {
                 position: "relative",
                 borderBottom: "2px solid #1151b3",
@@ -3972,15 +4059,15 @@
             };
         return t.jsx("div", {
             children: t.jsx("div", {
                 style: i,
                 children: t.jsx("ul", {
                     style: r(e.data.steps),
                     children: e.data.steps.map((c, u) => t.jsxs("li", {
-                        style: o,
+                        style: l,
                         children: [t.jsx("div", {
                             style: a(c),
                             children: n(c)
                         }), u < e.data.steps.length - 1 && t.jsx("div", {
                             style: s
                         }), t.jsx("div", {
                             children: c.name
@@ -4008,15 +4095,15 @@
             d = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: Te[e.data.style]
+                backgroundColor: C.colors[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
                 style: d,
                 children: t.jsxs("span", {
                     style: r,
@@ -4024,17 +4111,17 @@
                 })
             })
         })
     }
     return n()
 }
 
-function Ot(e) {
+function Rt(e) {
     function n() {
-        return e.data.color = Te[e.data.style], t.jsx(Me, {
+        return e.data.color = C.colors[e.data.style], t.jsx(Me, {
             data: e.data
         })
     }
     return n()
 }
 
 function Me(e) {
@@ -4052,15 +4139,15 @@
             style: a,
             children: e.data.label
         })
     }
     return n()
 }
 
-function Rt(e) {
+function Nt(e) {
     function n() {
         const a = {
                 padding: 20,
                 marginLeft: -20,
                 marginRight: -20,
                 textAlign: "center",
                 backgroundColor: "#f8f8f8"
@@ -4075,51 +4162,51 @@
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
             d = {
                 marginTop: 30,
                 fontSize: "3rem",
-                color: "#2670e8"
+                color: C.colors.auxiliary
             },
             i = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
                 color: "#0c326f"
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
-                "data-label": C(e.data.title),
+                "data-label": T(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
-                children: e.data.items.map(o => t.jsxs(W, {
-                    href: o.url,
+                children: e.data.items.map(l => t.jsxs(N, {
+                    href: l.url,
                     style: r,
-                    dataLabel: o.label,
+                    dataLabel: l.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(k, {
+                        children: t.jsx(S, {
                             style: d,
-                            icon: o.icon
+                            icon: l.icon
                         })
                     }), t.jsx("div", {
                         style: i,
-                        children: o.label
+                        children: l.label
                     })]
                 }, Math.random()))
             })]
         }) : null
     }
     return n()
 }
 
-function Nt(e) {
+function Ot(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 backgroundColor: "black",
                 color: "white",
                 padding: "10px",
                 minHeight: "300px",
@@ -4133,18 +4220,18 @@
         })
     }
     return n()
 }
 
 function _t(e) {
     function n() {
-        return e.data.url ? t.jsx(W, {
+        return e.data.url ? t.jsx(N, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(k, {
+            children: e.data.icon ? t.jsx(S, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
@@ -4162,15 +4249,15 @@
         })
     }
     return n()
 }
 
 function zt(e) {
     const n = Math.random();
-    M.useEffect(() => {
+    I.useEffect(() => {
         new QRCode(document.getElementById(n), {
             text: e.data.text,
             width: 128,
             height: 128,
             colorDark: "#333333",
             colorLight: "#ffffff",
             correctLevel: QRCode.CorrectLevel.H
@@ -4183,27 +4270,78 @@
         })
     }
     return a()
 }
 
 function Ht(e) {
     function n() {
-        return t.jsx($, {
+        const a = {
+                color: "white",
+                backgroundColor: C.colors.highlight,
+                margin: -20,
+                textAlign: "center",
+                paddingTop: 20,
+                paddingBottom: 70
+            },
+            r = {
+                fontSize: "4rem",
+                fontWeight: "bold",
+                marginTop: 25
+            },
+            d = {
+                fontSize: "1.2rem",
+                maxWidth: 200,
+                margin: "auto"
+            };
+        if (e.data) return t.jsxs("div", {
+            className: "indicators",
+            style: a,
+            children: [t.jsx("h1", {
+                "data-label": T(e.data.title),
+                children: e.data.title
+            }), t.jsx(G, {
+                width: 300,
+                children: e.data.items.map(i => t.jsxs("div", {
+                    children: [t.jsx("div", {
+                        style: r,
+                        children: z(i.value)
+                    }), t.jsx("div", {
+                        style: d,
+                        children: i.name
+                    })]
+                }))
+            }, Math.random()), t.jsx("div", {
+                className: "actions",
+                children: e.data.actions.map(i => t.jsx(N, {
+                    href: q(i.url),
+                    label: i.label,
+                    modal: i.modal,
+                    children: i.label
+                }, Math.random()))
+            })]
+        })
+    }
+    return n()
+}
+
+function Wt(e) {
+    function n() {
+        return t.jsx(G, {
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
 
-function Wt(e) {
+function Pt(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     fontSize: "12rem",
@@ -4212,88 +4350,89 @@
                 },
                 children: e.data.value
             })]
         })
     }
     return n()
 }
-var Z, se = {};
-const Pt = "/api/application/",
-    ge = localStorage.getItem("application");
+var Z, ce = {};
+const Ut = "/api/application/",
+    xe = localStorage.getItem("application");
 
 function p(e) {
-    const n = se[e.data.type];
-    return n ? Ie.createElement(n, {
+    const n = ce[e.data.type];
+    return n ? Be.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
 p.register = function(e, n) {
-    se[n.toLowerCase()] = e
+    ce[n.toLowerCase()] = e
 };
 p.render = function(e) {
-    Z = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
+    Z = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-p.register(Wt, "Counter");
-p.register(st, "Form");
-p.register(ut, "QuerySet");
-p.register(We, "Fieldset");
-p.register(J, "Field");
-p.register(Ue, "Object");
-p.register(Ve, "Section");
-p.register(Je, "Group");
-p.register(jt, "Statistics");
+p.register(Pt, "Counter");
+p.register(ct, "Form");
+p.register(ht, "QuerySet");
+p.register(Ue, "Fieldset");
+p.register(Y, "Field");
+p.register($e, "Object");
+p.register(Je, "Section");
+p.register(Qe, "Group");
+p.register(kt, "Statistics");
 p.register(Dt, "Image");
 p.register(Bt, "Banner");
 p.register(Lt, "Map");
 p.register(At, "Steps");
 p.register(zt, "QrCode");
 p.register(Me, "Badge");
-p.register(Ot, "Status");
+p.register(Rt, "Status");
 p.register(qt, "Progress");
-p.register(kt, "Color");
-p.register(Rt, "Boxes");
-p.register(Nt, "Shell");
+p.register(De, "Color");
+p.register(Nt, "Boxes");
+p.register(Ht, "Indicators");
+p.register(Ot, "Shell");
 p.register(_t, "FileLink");
 p.register(Ft, "FilePreview");
-p.register(qe, "Response");
+p.register(Ne, "Response");
 p.register(Et, "Application");
-p.register(Be, "IconSet");
-p.register(Ht, "Grid");
-p.register(ze, "Rows");
-p.register(He, "Timeline");
+p.register(Le, "IconSet");
+p.register(Wt, "Grid");
+p.register(We, "Rows");
+p.register(Pe, "Timeline");
 p.register(It, "WebConf");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
-    se[n] ? I("GET", q(e), function(a) {
+    ce[n] ? B("GET", q(e), function(a) {
         Z.render(t.jsx(p, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), ge ? (window.application = JSON.parse(ge), I("GET", q(e), function(a) {
+    }, "", e), xe ? (window.application = JSON.parse(xe), B("GET", q(e), function(a) {
         window.application.content = a, Z.render(t.jsx(p, {
             data: window.application
         }, Math.random()))
-    })) : I("GET", Pt, function(r) {
-        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), I("GET", q(e), function(d) {
+    })) : B("GET", Ut, function(r) {
+        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), B("GET", q(e), function(d) {
             window.application.content = d, Z.render(t.jsx(p, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), I("GET", q(e), function(n) {
+    }, "", e), B("GET", q(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-p.render(P.createRoot(document.getElementById("root")));
+p.render(H.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.2.7/slth/static/js/vanilla-masker.js` & `pyslth-0.2.8/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/static/js/vanilla-masker.min.js` & `pyslth-0.2.8/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/statistics.py` & `pyslth-0.2.8/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/templates/index.html` & `pyslth-0.2.8/slth/templates/index.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <!DOCTYPE html>
 <html lang="pt">
 
 <head>
   <meta charset="UTF-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
   <title>{{ application.version }} {{ application.title }}</title>
+  <link rel="stylesheet" href="/static/css/style.css">
   <link rel="stylesheet" href="/static/css/slth.css">
   <link rel="stylesheet" href="/static/css/fontawesome.min.css">
   <link rel="stylesheet" href="/static/css/solid.min.css">
   <script type="module" src="/static/js/vanilla-masker.min.js"></script>
   <script type="module" src="/static/js/react-trigger-change.js"></script>
   <!-- <script type="module" src="/static/js/qrcode.min.js"></script> -->
   <script type="module" src="/static/js/peerjs.min.js"></script>
@@ -44,14 +45,30 @@
       RefreshRuntime.injectIntoGlobalHook(window)
       window.$RefreshReg$ = () => { }
       window.$RefreshSig$ = () => (type) => type
       window.__vite_plugin_react_preamble_installed__ = true
     }
   </script>
   {% endif %}
+
+  <style>
+    :root{
+      --primary-color: {{ application.theme.colors.primary }};
+      --secondary-color: {{ application.theme.colors.secondary }};
+      --auxiliary-color: {{ application.theme.colors.auxiliary }};
+      --highlight-color: {{ application.theme.colors.highlight }};
+      --info-color: {{ application.theme.colors.info }};
+      --success-color: {{ application.theme.colors.success }};
+      --warning-color: {{ application.theme.colors.warning }};
+      --danger-color: {{ application.theme.colors.danger }};
+      --border-radius: {{ application.theme.border.radius }};
+      --info-background: {{ application.theme.background.info }};
+    }
+  </style>
+
 </head>
 
 <body>
   <div id="root"></div>
 </body>
 
 {% if vite %}
```

### Comparing `pyslth-0.2.7/slth/templates/service-worker.js` & `pyslth-0.2.8/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/tests.py` & `pyslth-0.2.8/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/urls.py` & `pyslth-0.2.8/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/utils.py` & `pyslth-0.2.8/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.7/slth/views.py` & `pyslth-0.2.8/slth/views.py`

 * *Files identical despite different names*


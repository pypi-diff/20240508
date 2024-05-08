# Comparing `tmp/mercury-2.3.9.tar.gz` & `tmp/mercury-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-2.3.9.tar", last modified: Wed Mar 20 14:23:28 2024, max compression
+gzip compressed data, was "mercury-2.4.0.tar", last modified: Wed May  8 11:27:05 2024, max compression
```

## Comparing `mercury-2.3.9.tar` & `mercury-2.4.0.tar`

### file list

```diff
@@ -1,194 +1,228 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    34575 2023-07-14 08:51:02.000000 mercury-2.3.9/LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.3.9/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8682 2024-03-20 14:23:28.748715 mercury-2.3.9/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8038 2023-06-19 11:13:10.000000 mercury-2.3.9/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.740715 mercury-2.3.9/mercury/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2024-03-20 14:22:42.000000 mercury-2.3.9/mercury/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.740715 mercury-2.3.9/mercury/apps/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.740715 mercury-2.3.9/mercury/apps/accounts/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.9/mercury/apps/accounts/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.3.9/mercury/apps/accounts/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.3.9/mercury/apps/accounts/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.3.9/mercury/apps/accounts/fields.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.740715 mercury-2.3.9/mercury/apps/accounts/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/accounts/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.9/mercury/apps/accounts/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.3.9/mercury/apps/accounts/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.3.9/mercury/apps/accounts/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.3.9/mercury/apps/accounts/tasks.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.740715 mercury-2.3.9/mercury/apps/accounts/templatetags/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2024-01-10 11:48:55.000000 mercury-2.3.9/mercury/apps/accounts/templatetags/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      293 2024-01-10 11:51:23.000000 mercury-2.3.9/mercury/apps/accounts/templatetags/replace.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.740715 mercury-2.3.9/mercury/apps/accounts/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.3.9/mercury/apps/accounts/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/accounts/tests/test_accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.3.9/mercury/apps/accounts/tests/test_invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.3.9/mercury/apps/accounts/tests/test_secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-06-22 08:59:21.000000 mercury-2.3.9/mercury/apps/accounts/tests/test_sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/accounts/tests/test_subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2024-01-10 11:49:35.000000 mercury-2.3.9/mercury/apps/accounts/urls.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/accounts/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.3.9/mercury/apps/accounts/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1979 2024-03-08 14:49:21.000000 mercury-2.3.9/mercury/apps/accounts/views/accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.3.9/mercury/apps/accounts/views/invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.3.9/mercury/apps/accounts/views/permissions.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.3.9/mercury/apps/accounts/views/secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7505 2023-08-10 13:34:52.000000 mercury-2.3.9/mercury/apps/accounts/views/sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4176 2024-03-08 14:45:37.000000 mercury-2.3.9/mercury/apps/accounts/views/subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      892 2023-08-10 13:34:52.000000 mercury-2.3.9/mercury/apps/accounts/views/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/nb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/nb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.3.9/mercury/apps/nb/exporter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4523 2023-08-10 13:34:52.000000 mercury-2.3.9/mercury/apps/nb/nbrun.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/nb/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.3.9/mercury/apps/nb/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1252 2023-07-18 10:35:22.000000 mercury-2.3.9/mercury/apps/nb/tests/test_nbrun.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.3.9/mercury/apps/nb/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/nb/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/nbworker/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/nbworker/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1705 2024-03-05 10:43:40.000000 mercury-2.3.9/mercury/apps/nbworker/__main__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17644 2024-03-08 14:08:13.000000 mercury-2.3.9/mercury/apps/nbworker/nb.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2024-03-08 14:46:57.000000 mercury-2.3.9/mercury/apps/nbworker/rest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4898 2023-06-28 11:59:58.000000 mercury-2.3.9/mercury/apps/nbworker/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/nbworker/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2858 2024-03-05 09:51:03.000000 mercury-2.3.9/mercury/apps/nbworker/ws.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/notebooks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/notebooks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/notebooks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/notebooks/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/notebooks/management/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/notebooks/management/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/notebooks/management/commands/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/notebooks/management/commands/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.3.9/mercury/apps/notebooks/management/commands/add.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.3.9/mercury/apps/notebooks/management/commands/delete.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.3.9/mercury/apps/notebooks/management/commands/list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/notebooks/management/commands/watch.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/notebooks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/notebooks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/notebooks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.3.9/mercury/apps/notebooks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.3.9/mercury/apps/notebooks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.3.9/mercury/apps/notebooks/slides_themes.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11759 2024-03-18 07:18:56.000000 mercury-2.3.9/mercury/apps/notebooks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.3.9/mercury/apps/notebooks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.3.9/mercury/apps/notebooks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2023-04-27 15:18:53.000000 mercury-2.3.9/mercury/apps/notebooks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/storage/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/storage/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/storage/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/storage/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/storage/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/storage/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.3.9/mercury/apps/storage/migrations/0002_useruploadedfile.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/storage/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/storage/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.3.9/mercury/apps/storage/s3utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.3.9/mercury/apps/storage/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11214 2024-03-08 14:48:27.000000 mercury-2.3.9/mercury/apps/storage/storage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.3.9/mercury/apps/storage/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2602 2024-02-19 11:05:39.000000 mercury-2.3.9/mercury/apps/storage/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      902 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/apps/storage/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/storage/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.3.9/mercury/apps/storage/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6773 2024-02-19 11:25:22.000000 mercury-2.3.9/mercury/apps/storage/views/dashboardfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.3.9/mercury/apps/storage/views/notebookfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3496 2023-08-10 13:34:52.000000 mercury-2.3.9/mercury/apps/storage/views/stylefiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.3.9/mercury/apps/storage/views/workerfiles.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.744715 mercury-2.3.9/mercury/apps/tasks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/tasks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/tasks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/tasks/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.3.9/mercury/apps/tasks/clean_service.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4018 2023-06-22 08:55:52.000000 mercury-2.3.9/mercury/apps/tasks/export_pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.3.9/mercury/apps/tasks/export_png.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/mercury/apps/tasks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/tasks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/apps/tasks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.3.9/mercury/apps/tasks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/tasks/notify.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.3.9/mercury/apps/tasks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.3.9/mercury/apps/tasks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1335 2023-05-23 13:34:07.000000 mercury-2.3.9/mercury/apps/tasks/tasks_export.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/tasks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1431 2023-04-25 12:37:36.000000 mercury-2.3.9/mercury/apps/tasks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8684 2024-03-08 14:49:09.000000 mercury-2.3.9/mercury/apps/tasks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/mercury/apps/workers/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/workers/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/workers/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/workers/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      532 2023-07-18 10:35:22.000000 mercury-2.3.9/mercury/apps/workers/constants.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/mercury/apps/workers/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.3.9/mercury/apps/workers/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-06-20 12:58:36.000000 mercury-2.3.9/mercury/apps/workers/migrations/0002_machine.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-06-22 09:33:58.000000 mercury-2.3.9/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/workers/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1832 2023-06-28 12:00:54.000000 mercury-2.3.9/mercury/apps/workers/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/workers/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6117 2024-03-08 14:49:03.000000 mercury-2.3.9/mercury/apps/workers/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1360 2023-08-02 15:55:58.000000 mercury-2.3.9/mercury/apps/workers/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      468 2024-03-05 09:51:03.000000 mercury-2.3.9/mercury/apps/workers/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6845 2023-08-10 13:34:52.000000 mercury-2.3.9/mercury/apps/workers/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/mercury/apps/ws/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/ws/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/ws/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6689 2024-03-05 10:50:03.000000 mercury-2.3.9/mercury/apps/ws/client.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.3.9/mercury/apps/ws/middleware.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/mercury/apps/ws/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/apps/ws/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.3.9/mercury/apps/ws/routing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3114 2024-03-08 15:03:14.000000 mercury-2.3.9/mercury/apps/ws/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-06-21 07:54:00.000000 mercury-2.3.9/mercury/apps/ws/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5839 2024-03-08 14:48:55.000000 mercury-2.3.9/mercury/apps/ws/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2470 2024-03-05 10:39:26.000000 mercury-2.3.9/mercury/apps/ws/worker.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.3.9/mercury/demo.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/manage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9993 2024-03-20 14:17:46.000000 mercury-2.3.9/mercury/mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      563 2024-03-20 14:17:46.000000 mercury-2.3.9/mercury/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/mercury/server/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.3.9/mercury/server/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-08-31 09:59:17.000000 mercury-2.3.9/mercury/server/asgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3376 2023-09-19 13:56:49.000000 mercury-2.3.9/mercury/server/celery.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10336 2024-03-05 10:38:07.000000 mercury-2.3.9/mercury/server/settings.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.3.9/mercury/server/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.3.9/mercury/server/views.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.3.9/mercury/server/wsgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2461 2023-06-21 11:57:21.000000 mercury-2.3.9/mercury/start_instance.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.748715 mercury-2.3.9/mercury/widgets/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.9/mercury/widgets/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5787 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/app.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4062 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/button.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.3.9/mercury/widgets/chat.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4557 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/checkbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.3.9/mercury/widgets/confetti.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5514 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/file.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      851 2023-08-29 14:20:20.000000 mercury-2.3.9/mercury/widgets/in_mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.3.9/mercury/widgets/json.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7046 2024-03-18 07:33:46.000000 mercury-2.3.9/mercury/widgets/manager.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.3.9/mercury/widgets/md.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6209 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/multiselect.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2228 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/note.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3145 2023-08-29 14:20:20.000000 mercury-2.3.9/mercury/widgets/numberbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6115 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/numeric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.3.9/mercury/widgets/outputdir.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      463 2023-08-29 14:20:20.000000 mercury-2.3.9/mercury/widgets/pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5753 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/range.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6482 2024-03-05 08:37:14.000000 mercury-2.3.9/mercury/widgets/select.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6475 2024-01-10 11:15:09.000000 mercury-2.3.9/mercury/widgets/slider.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.3.9/mercury/widgets/stop.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2024-03-20 14:17:46.000000 mercury-2.3.9/mercury/widgets/table.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4742 2024-03-18 07:26:24.000000 mercury-2.3.9/mercury/widgets/text.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      814 2023-08-29 14:20:20.000000 mercury-2.3.9/mercury/widgets/user.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-20 14:23:28.740715 mercury-2.3.9/mercury.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8682 2024-03-20 14:23:28.000000 mercury-2.3.9/mercury.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5359 2024-03-20 14:23:28.000000 mercury-2.3.9/mercury.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-03-20 14:23:28.000000 mercury-2.3.9/mercury.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       49 2024-03-20 14:23:28.000000 mercury-2.3.9/mercury.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      508 2024-03-20 14:23:28.000000 mercury-2.3.9/mercury.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2024-03-20 14:23:28.000000 mercury-2.3.9/mercury.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.3.9/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-03-20 14:23:28.748715 mercury-2.3.9/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1386 2024-03-20 14:22:31.000000 mercury-2.3.9/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.402736 mercury-2.4.0/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    34575 2023-07-14 08:51:02.000000 mercury-2.4.0/LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.4.0/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8683 2024-05-08 11:27:05.402736 mercury-2.4.0/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8039 2024-05-07 13:52:16.000000 mercury-2.4.0/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.386736 mercury-2.4.0/mercury/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2024-05-08 11:25:21.000000 mercury-2.4.0/mercury/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.386736 mercury-2.4.0/mercury/apps/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.386736 mercury-2.4.0/mercury/apps/accounts/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.4.0/mercury/apps/accounts/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.4.0/mercury/apps/accounts/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.4.0/mercury/apps/accounts/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.4.0/mercury/apps/accounts/fields.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.386736 mercury-2.4.0/mercury/apps/accounts/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.4.0/mercury/apps/accounts/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.4.0/mercury/apps/accounts/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.4.0/mercury/apps/accounts/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.4.0/mercury/apps/accounts/tasks.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/accounts/templatetags/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2024-01-10 11:48:55.000000 mercury-2.4.0/mercury/apps/accounts/templatetags/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      293 2024-01-10 11:51:23.000000 mercury-2.4.0/mercury/apps/accounts/templatetags/replace.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/accounts/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.4.0/mercury/apps/accounts/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/accounts/tests/test_accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.4.0/mercury/apps/accounts/tests/test_invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.4.0/mercury/apps/accounts/tests/test_secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-06-22 08:59:21.000000 mercury-2.4.0/mercury/apps/accounts/tests/test_sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/accounts/tests/test_subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2024-01-10 11:49:35.000000 mercury-2.4.0/mercury/apps/accounts/urls.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/accounts/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.4.0/mercury/apps/accounts/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1979 2024-03-08 14:49:21.000000 mercury-2.4.0/mercury/apps/accounts/views/accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.4.0/mercury/apps/accounts/views/invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.4.0/mercury/apps/accounts/views/permissions.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.4.0/mercury/apps/accounts/views/secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7505 2023-08-10 13:34:52.000000 mercury-2.4.0/mercury/apps/accounts/views/sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4176 2024-03-08 14:45:37.000000 mercury-2.4.0/mercury/apps/accounts/views/subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      892 2023-08-10 13:34:52.000000 mercury-2.4.0/mercury/apps/accounts/views/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/nb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/nb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.4.0/mercury/apps/nb/exporter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4523 2023-08-10 13:34:52.000000 mercury-2.4.0/mercury/apps/nb/nbrun.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/nb/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.4.0/mercury/apps/nb/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1252 2023-07-18 10:35:22.000000 mercury-2.4.0/mercury/apps/nb/tests/test_nbrun.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.4.0/mercury/apps/nb/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/nb/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/nbworker/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/nbworker/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1786 2024-05-06 12:35:47.000000 mercury-2.4.0/mercury/apps/nbworker/__main__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    19411 2024-05-07 11:02:27.000000 mercury-2.4.0/mercury/apps/nbworker/nb.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9765 2024-05-07 08:10:41.000000 mercury-2.4.0/mercury/apps/nbworker/rest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4898 2023-06-28 11:59:58.000000 mercury-2.4.0/mercury/apps/nbworker/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/nbworker/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2858 2024-03-05 09:51:03.000000 mercury-2.4.0/mercury/apps/nbworker/ws.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/notebooks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/notebooks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/notebooks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/notebooks/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/notebooks/management/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/notebooks/management/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/notebooks/management/commands/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/notebooks/management/commands/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.4.0/mercury/apps/notebooks/management/commands/add.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.4.0/mercury/apps/notebooks/management/commands/delete.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.4.0/mercury/apps/notebooks/management/commands/list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/notebooks/management/commands/watch.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/notebooks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/notebooks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/notebooks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.4.0/mercury/apps/notebooks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.4.0/mercury/apps/notebooks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.4.0/mercury/apps/notebooks/slides_themes.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11759 2024-03-18 07:18:56.000000 mercury-2.4.0/mercury/apps/notebooks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.4.0/mercury/apps/notebooks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.4.0/mercury/apps/notebooks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2024-04-12 10:17:00.000000 mercury-2.4.0/mercury/apps/notebooks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/storage/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/storage/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/storage/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/storage/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/storage/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/storage/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.4.0/mercury/apps/storage/migrations/0002_useruploadedfile.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/storage/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/storage/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.4.0/mercury/apps/storage/s3utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.4.0/mercury/apps/storage/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11511 2024-05-07 08:14:32.000000 mercury-2.4.0/mercury/apps/storage/storage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.4.0/mercury/apps/storage/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2602 2024-02-19 11:05:39.000000 mercury-2.4.0/mercury/apps/storage/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      902 2024-01-10 11:15:09.000000 mercury-2.4.0/mercury/apps/storage/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.390736 mercury-2.4.0/mercury/apps/storage/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.4.0/mercury/apps/storage/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6773 2024-02-19 11:25:22.000000 mercury-2.4.0/mercury/apps/storage/views/dashboardfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.4.0/mercury/apps/storage/views/notebookfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3496 2023-08-10 13:34:52.000000 mercury-2.4.0/mercury/apps/storage/views/stylefiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.4.0/mercury/apps/storage/views/workerfiles.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/apps/tasks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/tasks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/tasks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/tasks/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.4.0/mercury/apps/tasks/clean_service.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4018 2023-06-22 08:55:52.000000 mercury-2.4.0/mercury/apps/tasks/export_pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.4.0/mercury/apps/tasks/export_png.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/apps/tasks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2121 2024-05-07 08:11:51.000000 mercury-2.4.0/mercury/apps/tasks/migrations/0002_restapitask.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/apps/tasks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1735 2024-05-07 08:07:52.000000 mercury-2.4.0/mercury/apps/tasks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/tasks/notify.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.4.0/mercury/apps/tasks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.4.0/mercury/apps/tasks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1335 2023-05-23 13:34:07.000000 mercury-2.4.0/mercury/apps/tasks/tasks_export.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/tasks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1594 2024-05-07 11:42:50.000000 mercury-2.4.0/mercury/apps/tasks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10906 2024-05-07 12:34:09.000000 mercury-2.4.0/mercury/apps/tasks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/apps/workers/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/workers/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/workers/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/workers/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      532 2023-07-18 10:35:22.000000 mercury-2.4.0/mercury/apps/workers/constants.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/apps/workers/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.4.0/mercury/apps/workers/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-06-20 12:58:36.000000 mercury-2.4.0/mercury/apps/workers/migrations/0002_machine.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-06-22 09:33:58.000000 mercury-2.4.0/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/workers/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1832 2024-04-12 09:41:31.000000 mercury-2.4.0/mercury/apps/workers/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/workers/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8697 2024-04-12 10:16:03.000000 mercury-2.4.0/mercury/apps/workers/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1612 2024-05-07 08:04:54.000000 mercury-2.4.0/mercury/apps/workers/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      468 2024-03-05 09:51:03.000000 mercury-2.4.0/mercury/apps/workers/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11279 2024-05-07 11:04:20.000000 mercury-2.4.0/mercury/apps/workers/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/apps/ws/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/ws/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/ws/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6689 2024-05-06 11:03:38.000000 mercury-2.4.0/mercury/apps/ws/client.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.4.0/mercury/apps/ws/middleware.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/apps/ws/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/apps/ws/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.4.0/mercury/apps/ws/routing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3114 2024-03-08 15:03:14.000000 mercury-2.4.0/mercury/apps/ws/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-06-21 07:54:00.000000 mercury-2.4.0/mercury/apps/ws/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5839 2024-03-08 14:48:55.000000 mercury-2.4.0/mercury/apps/ws/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2470 2024-03-05 10:39:26.000000 mercury-2.4.0/mercury/apps/ws/worker.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.4.0/mercury/demo.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/frontend-dist/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/asset-manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/favicon-old.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/favicon.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/index.html
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/jupyter-additional.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/jupyter-syntax.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   580392 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/jupyter-theme-light.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/mercury_black_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/mercury_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2024-05-08 11:26:49.000000 mercury-2.4.0/mercury/frontend-dist/robots.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.386736 mercury-2.4.0/mercury/frontend-dist/static/
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.394736 mercury-2.4.0/mercury/frontend-dist/static/css/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3071 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5632 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.402736 mercury-2.4.0/mercury/frontend-dist/static/js/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/js/2.81b1917f.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  4972959 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    96124 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/js/main.51571475.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   286726 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/js/main.51571475.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.402736 mercury-2.4.0/mercury/frontend-dist/static/media/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2024-05-08 11:27:04.000000 mercury-2.4.0/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/manage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10038 2024-05-07 09:50:27.000000 mercury-2.4.0/mercury/mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      563 2024-04-12 08:02:38.000000 mercury-2.4.0/mercury/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.402736 mercury-2.4.0/mercury/server/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.4.0/mercury/server/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-08-31 09:59:17.000000 mercury-2.4.0/mercury/server/asgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3376 2023-09-19 13:56:49.000000 mercury-2.4.0/mercury/server/celery.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10336 2024-03-05 10:38:07.000000 mercury-2.4.0/mercury/server/settings.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.4.0/mercury/server/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.4.0/mercury/server/views.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.4.0/mercury/server/wsgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2461 2023-06-21 11:57:21.000000 mercury-2.4.0/mercury/start_instance.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.402736 mercury-2.4.0/mercury/widgets/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.0/mercury/widgets/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1475 2024-05-07 10:14:58.000000 mercury-2.4.0/mercury/widgets/apiresponse.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5787 2024-01-10 11:15:09.000000 mercury-2.4.0/mercury/widgets/app.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4062 2024-01-10 11:15:09.000000 mercury-2.4.0/mercury/widgets/button.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.4.0/mercury/widgets/chat.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4599 2024-05-07 10:40:08.000000 mercury-2.4.0/mercury/widgets/checkbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.4.0/mercury/widgets/confetti.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5514 2024-01-10 11:15:09.000000 mercury-2.4.0/mercury/widgets/file.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      851 2023-08-29 14:20:20.000000 mercury-2.4.0/mercury/widgets/in_mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.4.0/mercury/widgets/json.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7486 2024-05-07 10:39:24.000000 mercury-2.4.0/mercury/widgets/manager.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.4.0/mercury/widgets/md.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6251 2024-05-07 10:40:18.000000 mercury-2.4.0/mercury/widgets/multiselect.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2228 2024-01-10 11:15:09.000000 mercury-2.4.0/mercury/widgets/note.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3145 2023-08-29 14:20:20.000000 mercury-2.4.0/mercury/widgets/numberbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6115 2024-01-10 11:15:09.000000 mercury-2.4.0/mercury/widgets/numeric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.4.0/mercury/widgets/outputdir.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      463 2023-08-29 14:20:20.000000 mercury-2.4.0/mercury/widgets/pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6524 2024-05-08 09:08:28.000000 mercury-2.4.0/mercury/widgets/range.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6524 2024-05-07 10:40:44.000000 mercury-2.4.0/mercury/widgets/select.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6517 2024-05-07 10:40:49.000000 mercury-2.4.0/mercury/widgets/slider.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.4.0/mercury/widgets/stop.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2024-03-20 14:17:46.000000 mercury-2.4.0/mercury/widgets/table.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4784 2024-05-07 10:41:39.000000 mercury-2.4.0/mercury/widgets/text.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      814 2023-08-29 14:20:20.000000 mercury-2.4.0/mercury/widgets/user.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:27:05.386736 mercury-2.4.0/mercury.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8683 2024-05-08 11:27:05.000000 mercury-2.4.0/mercury.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6849 2024-05-08 11:27:05.000000 mercury-2.4.0/mercury.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-05-08 11:27:05.000000 mercury-2.4.0/mercury.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       49 2024-05-08 11:27:05.000000 mercury-2.4.0/mercury.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      508 2024-05-08 11:27:05.000000 mercury-2.4.0/mercury.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2024-05-08 11:27:05.000000 mercury-2.4.0/mercury.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.4.0/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-05-08 11:27:05.402736 mercury-2.4.0/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1386 2024-05-08 11:25:08.000000 mercury-2.4.0/setup.py
```

### Comparing `mercury-2.3.9/LICENSE.txt` & `mercury-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/PKG-INFO` & `mercury-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.3.9
+Version: 2.4.0
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Author: MLJAR Sp. z o.o.
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
-
 <p align="center">
   <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/main.png#gh-light-mode-only" width="100%" />  
 </p>
 <p align="center">
   <img 
@@ -30,15 +29,15 @@
 </p>
 
 [![Tests](https://github.com/mljar/mercury/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mercury/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mercury.svg)](https://badge.fury.io/py/mercury)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mercury.svg)](https://pypi.python.org/pypi/mercury/)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-mercury/badges/license.svg)](https://anaconda.org/conda-forge/mljar-mercury)
 
-# Build Web Apps in Jupyter Notebook
+# Convert Jupyter Notebook to Web App
 
 Mercury allows you to add interactive widgets in Python notebooks, so you can share notebooks as web applications. Forget about rewriting notebooks to web frameworks just to share your results. Mercury offers a set of widgets with simple re-execution of cells.
 
 You can build with Mercury:
 - Turn your notebook into beautiful [Web Apps](https://runmercury.com/tutorials/web-app-python-jupyter-notebook/),
 - Create interactive [Presentations](https://runmercury.com/tutorials/presentation-python-jupyter-notebook/) with widgets, you can recompute slides during the show,
 - Share notebooks as static [Websites](https://runmercury.com/tutorials/website-python-jupyter-notebook/),
@@ -76,14 +75,15 @@
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets3.png#gh-light-mode-only" width="100%" />  
 </p>
  <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets_black.png#gh-dark-mode-only" width="100%" />  
 </p>
+
 ## Integrations
  
 Mercury works with virtually every Python package!
 Among the most important are machine learning libraries such as Scikit-Learn, Pandas, and Seaborn or visualization libraries: Plotly, matplotlib, Vega-Altair, and Ipyvizzu.
  <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/Integrations.png#gh-light-mode-only" width="100%" />
```

### Comparing `mercury-2.3.9/README.md` & `mercury-2.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-
 <p align="center">
   <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/main.png#gh-light-mode-only" width="100%" />  
 </p>
 <p align="center">
   <img 
@@ -12,15 +11,15 @@
 </p>
 
 [![Tests](https://github.com/mljar/mercury/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mercury/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mercury.svg)](https://badge.fury.io/py/mercury)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mercury.svg)](https://pypi.python.org/pypi/mercury/)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-mercury/badges/license.svg)](https://anaconda.org/conda-forge/mljar-mercury)
 
-# Build Web Apps in Jupyter Notebook
+# Convert Jupyter Notebook to Web App
 
 Mercury allows you to add interactive widgets in Python notebooks, so you can share notebooks as web applications. Forget about rewriting notebooks to web frameworks just to share your results. Mercury offers a set of widgets with simple re-execution of cells.
 
 You can build with Mercury:
 - Turn your notebook into beautiful [Web Apps](https://runmercury.com/tutorials/web-app-python-jupyter-notebook/),
 - Create interactive [Presentations](https://runmercury.com/tutorials/presentation-python-jupyter-notebook/) with widgets, you can recompute slides during the show,
 - Share notebooks as static [Websites](https://runmercury.com/tutorials/website-python-jupyter-notebook/),
@@ -58,14 +57,15 @@
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets3.png#gh-light-mode-only" width="100%" />  
 </p>
  <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets_black.png#gh-dark-mode-only" width="100%" />  
 </p>
+
 ## Integrations
  
 Mercury works with virtually every Python package!
 Among the most important are machine learning libraries such as Scikit-Learn, Pandas, and Seaborn or visualization libraries: Plotly, matplotlib, Vega-Altair, and Ipyvizzu.
  <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/Integrations.png#gh-light-mode-only" width="100%" />
```

### Comparing `mercury-2.3.9/mercury/apps/accounts/fields.py` & `mercury-2.4.0/mercury/apps/accounts/fields.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/migrations/0001_initial.py` & `mercury-2.4.0/mercury/apps/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/models.py` & `mercury-2.4.0/mercury/apps/accounts/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/serializers.py` & `mercury-2.4.0/mercury/apps/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/tasks.py` & `mercury-2.4.0/mercury/apps/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/tests/test_accounts.py` & `mercury-2.4.0/mercury/apps/accounts/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/tests/test_invitations.py` & `mercury-2.4.0/mercury/apps/accounts/tests/test_invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/tests/test_secrets.py` & `mercury-2.4.0/mercury/apps/accounts/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/tests/test_sites.py` & `mercury-2.4.0/mercury/apps/accounts/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/tests/test_subscription.py` & `mercury-2.4.0/mercury/apps/accounts/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/urls.py` & `mercury-2.4.0/mercury/apps/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/views/accounts.py` & `mercury-2.4.0/mercury/apps/accounts/views/accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/views/invitations.py` & `mercury-2.4.0/mercury/apps/accounts/views/invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/views/permissions.py` & `mercury-2.4.0/mercury/apps/accounts/views/permissions.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/views/secrets.py` & `mercury-2.4.0/mercury/apps/accounts/views/secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/views/sites.py` & `mercury-2.4.0/mercury/apps/accounts/views/sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/views/subscription.py` & `mercury-2.4.0/mercury/apps/accounts/views/subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/accounts/views/utils.py` & `mercury-2.4.0/mercury/apps/accounts/views/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/nb/exporter.py` & `mercury-2.4.0/mercury/apps/nb/exporter.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/nb/nbrun.py` & `mercury-2.4.0/mercury/apps/nb/nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/nb/tests/test_nbrun.py` & `mercury-2.4.0/mercury/apps/nb/tests/test_nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/nb/tests.py` & `mercury-2.4.0/mercury/apps/nb/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/nbworker/__main__.py` & `mercury-2.4.0/mercury/apps/nbworker/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import logging
 
 CURRENT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 BACKEND_DIR = os.path.join(CURRENT_DIR, "..")
 sys.path.insert(0, BACKEND_DIR)
 
 LOG_LEVEL = (
-    logging.ERROR if os.environ.get("DJANGO_LOG_LEVEL", "ERROR") == "ERROR" else logging.INFO
+    logging.ERROR
+    if os.environ.get("DJANGO_LOG_LEVEL", "ERROR") == "ERROR"
+    else logging.INFO
 )
 
 logging.basicConfig(
     # filename="nbworker.log", filemode="w",
     format="NB %(asctime)s %(message)s",
     level=LOG_LEVEL,
 )
@@ -60,8 +62,11 @@
     for _ in range(CONNECT_MAX_TRIES):
         nb_worker = NBWorker(
             f"{server_url}/ws/worker/{notebook_id}/{session_id}/{worker_id}/",
             notebook_id,
             session_id,
             worker_id,
         )
-        time.sleep(RECONNECT_WAIT_TIME)
+        if nb_worker.is_task_mode():
+            break
+        else:
+            time.sleep(RECONNECT_WAIT_TIME)
```

### Comparing `mercury-2.3.9/mercury/apps/nbworker/nb.py` & `mercury-2.4.0/mercury/apps/nbworker/nb.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,29 @@
 
         # monitor notebook file updates if running locally
         if (
             "127.0.0.1" in ws_address
             and os.environ.get("MERCURY_DISABLE_AUTO_RELOAD", "NO") != "YES"
         ):
             threading.Thread(target=self.nb_file_watch, daemon=True).start()
-        threading.Thread(target=self.process_msgs, daemon=True).start()
-        self.ws.run_forever(ping_interval=10, ping_timeout=5)
+
+        if self.is_task_mode():
+            log.info(f"Worker processing task {self.notebook.task_id}")
+            self.init_notebook()
+        else:
+            log.info("Starting worker processing thread")
+            threading.Thread(target=self.process_msgs, daemon=True).start()
+            self.ws.run_forever(ping_interval=10, ping_timeout=5)
+
+    def is_task_mode(self):
+        log.info("is task mode")
+        log.info(self.notebook)
+        if self.notebook.task_id != "":
+            return True
+        return False
 
     @staticmethod
     def md5(fname):
         hash_md5 = hashlib.md5()
         with open(fname, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
@@ -293,120 +306,110 @@
         secrets = self.list_secrets()
         if secrets:
             cmd = "import os\n"
             for s in secrets:
                 name = s.get("name", "")
                 secret = s.get("secret", "")
                 cmd += f'os.environ["{name}"] = "{secret}"'
-                cmd += "\n" # add new line between secrets
+                cmd += "\n"  # add new line between secrets
             log.info("Set secrets")
             self.nbrun.run_code(cmd)
 
     def init_notebook(self):
         log.info(f"Init notebook, show_code={self.show_code()}")
 
+        if self.notebook.task_id != "":
+            log.info(
+                f"Task available {self.notebook.task_id}, params {self.notebook.params}"
+            )
+            try:
+                if hasattr(self.notebook, "task_params"):
+                    task_params = self.notebook.task_params
+                    if task_params != "":
+                        task_params = json.loads(task_params)
+                        for k in task_params:
+                            if k != "":
+                                WidgetsManager.set_preset_value(url_key=k, value=task_params[k])
+            except Exception as e:
+                log.error(f"Error when initialize notebook, {str(e)}")
+                self.update_rest_api_task(state="ERROR", response="Error parsing input data")
+                return
+
         self.sm.provision_uploaded_files()
 
         self.prev_nb = None
         self.prev_widgets = {}
         self.prev_body = ""
 
-        self.update_worker_state(WorkerState.Busy)
+        if not self.is_task_mode():
+            self.update_worker_state(WorkerState.Busy)
 
         self.nbrun = NbRun(
             show_code=self.show_code(),
             show_prompt=self.show_prompt(),
             is_presentation=self.is_presentation(),
             reveal_theme=self.reveal_theme(),
             stop_on_error=self.stop_on_error(),
             user_info=self.get_user_info(),
         )
-        
+
         self.provision_secrets()
         self.install_new_packages()
 
         # we need to initialize the output dir always
         # even if there is no OutputDir in the notebook
         self.initialize_outputdir()
 
         self.nb_original = read_nb(self.notebook.path)
 
         self.nbrun.run_notebook(self.nb_original)
 
-        self.sm.sync_output_dir()
+        if self.is_task_mode():
+            log.info("Task mode, update response")
+            self.nb = copy.deepcopy(self.nb_original)
+            self.save_nb_task_to_html()
+        else:
+            log.info("Websocket mode, update db and send reponse")
 
-        # TODO: update params in db if needed"
-        params = {}
-        parse_params(nb2dict(self.nb_original), params)
-
-        # update database ...
-
-        log.info(f"Executed params {json.dumps(params, indent=4)}")
-        update_database = self.update_notebook(params)
-
-        # update_database = False
-        # if params.get("title", "") != "" and self.notebook.title != params.get(
-        #     "title", ""
-        # ):
-        #     self.notebook.title = params.get("title", "")
-        #     update_database = True
-
-        # nb_params = json.loads(self.notebook.params)
-        # for property in [
-        #     "show-code",
-        #     "show-prompt",
-        #     "continuous_update",
-        #     "static_notebook",
-        #     "description",
-        #     "show_sidebar",
-        #     "full_screen",
-        #     "allow_download",
-        # ]:
-        #     if params.get(property) is not None and nb_params.get(
-        #         property
-        #     ) != params.get(property):
-        #         nb_params[property] = params.get(property)
-        #         update_database = True
-        # # save widgets params
-        # if json.dumps(nb_params.get("params", {})) != json.dumps(
-        #     params.get("params", {})
-        # ):
-        #     nb_params["params"] = params["params"]
-        #     update_database = True
-
-        # if update_database:
-        #     self.notebook.params = json.dumps(nb_params)
-        #     self.notebook.save()
+            self.sm.sync_output_dir()
+            
+            # TODO: update params in db if needed"
+            params = {}
+            parse_params(nb2dict(self.nb_original), params)
+
+            # update database ...
+            log.info(f"Executed params {json.dumps(params, indent=4)}")
+            update_database = self.update_notebook(params)
 
-        nb_params = json.loads(self.notebook.params)
+            nb_params = json.loads(self.notebook.params)
 
-        self.nbrun.set_show_code_and_prompt(
-            nb_params.get("show-code", False), nb_params.get("show-prompt", True)
-        )
-        self.nbrun.set_is_presentation(nb_params.get("output", "app") == "slides")
-        self.nbrun.set_stop_on_error(nb_params.get("stop_on_error", False))
+            self.nbrun.set_show_code_and_prompt(
+                nb_params.get("show-code", False), nb_params.get("show-prompt", True)
+            )
+            self.nbrun.set_is_presentation(nb_params.get("output", "app") == "slides")
+            self.nbrun.set_stop_on_error(nb_params.get("stop_on_error", False))
 
-        log.info(params)
-        log.info(f"Exporter show_code {self.nbrun.exporter.show_code}")
+            log.info(params)
+            log.info(f"Exporter show_code {self.nbrun.exporter.show_code}")
 
-        self.nb = copy.deepcopy(self.nb_original)
+            self.nb = copy.deepcopy(self.nb_original)
 
-        if self.is_presentation():
-            body = self.nbrun.export_html(self.nb, full_header=True)
-        else:
-            body = self.nbrun.export_html(self.nb, full_header=False)
+            if self.is_presentation():
+                body = self.nbrun.export_html(self.nb, full_header=True)
+            else:
+                body = self.nbrun.export_html(self.nb, full_header=False)
 
-        msg = {"purpose": Purpose.ExecutedNotebook, "body": body}
-        if update_database:
-            msg["reloadNotebook"] = True
-        self.ws.send(json.dumps(msg))
-        self.prev_body = copy.deepcopy(body)
+            msg = {"purpose": Purpose.ExecutedNotebook, "body": body}
+            if update_database:
+                msg["reloadNotebook"] = True
+            self.ws.send(json.dumps(msg))
+            self.prev_body = copy.deepcopy(body)
 
-        self.send_widgets(self.nb, expected_widgets_keys=[], init_widgets=True)
-        self.update_worker_state(WorkerState.Running)
+            self.send_widgets(self.nb, expected_widgets_keys=[], init_widgets=True)
+            self.update_worker_state(WorkerState.Running)
 
     # def save_notebook(self):
     #     log.info(f"Save notebook")
     #     # save nb in HTML
     #     if self.is_presentation():
     #         nb_body = self.nbrun.export_html(self.nb, full_header=True)
     #     else:
@@ -428,14 +431,49 @@
 
     #     # send notice that nb saved
     #     self.ws.send(json.dumps({"purpose": Purpose.SavedNotebook}))
 
     def display_notebook(self, json_params):
         log.info(f"Display notebook ({json_params})")
 
+    
+        
+    def get_task_api_response(self):
+        log.info("Get task APIResponse")
+        try:
+            for cell in self.nb.cells:
+                for output in cell.get("outputs", []):
+
+                    if "data" in output:
+                        if "application/mercury+json" in output["data"]:
+                            w = output["data"]["application/mercury+json"]
+                            log.info(w)
+                            w = json.loads(w)
+                            if w["widget"] == "APIResponse":
+                                return json.dumps(w["value"])
+        except Exception as e:
+            log.error(f"Problem when parsing task APIResponse, {str(e)}")
+            return ""
+        return ""
+
+    def save_nb_task_to_html(self):
+        log.info(f"Save notebook task to HTML")
+        # save nb in HTML with full header
+        if self.is_presentation():
+            nb_body = self.nbrun.export_html(self.nb, full_header=True)
+        else:
+            nb_body = self.nbrun.export_html(self.nb, full_header=True)
+
+        html_path, _ = self.sm.save_nb_html(nb_body, get_download_link=False, output_dir="rest-api-notebooks")
+
+        response = self.get_task_api_response()
+        # save nb_path in task
+        self.update_rest_api_task(state="DONE", response=response, html_path = html_path)
+
+
     def download_html(self):
         log.info(f"Download HTML")
         # save nb in HTML with full header
         if self.is_presentation():
             nb_body = self.nbrun.export_html(self.nb, full_header=True)
         else:
             nb_body = self.nbrun.export_html(self.nb, full_header=True)
```

### Comparing `mercury-2.3.9/mercury/apps/nbworker/rest.py` & `mercury-2.4.0/mercury/apps/nbworker/rest.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,29 +27,30 @@
         self.load_owner_and_user()
 
     def load_notebook(self):
         try:
             log.info(f"Load notebook id={self.notebook_id}")
             response = requests.get(
                 f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/nb",
-                timeout=5
+                timeout=5,
             )
+            log.info(response.json())
             if response.status_code != 200:
                 raise Exception("Cant load notebook")
             self.notebook = SimpleNamespace(**response.json())
         except Exception:
             log.exception("Exception when notebook load, quit")
             sys.exit(0)
 
     def load_owner_and_user(self):
         try:
             log.info("Load owner and user")
             response = requests.get(
                 f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/owner-and-user",
-                timeout=5
+                timeout=5,
             )
             if response.status_code != 200:
                 raise Exception("Cant load onwer and user information")
             owner = response.json().get("owner", {})
             user = response.json().get("user", {})
             if owner:
                 self.owner = SimpleNamespace(**owner)
@@ -100,15 +101,15 @@
 
         if update_database:
             try:
                 log.info(f"Update notebook id={self.notebook_id}")
                 response = requests.post(
                     f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/update-nb",
                     {"title": self.notebook.title, "params": json.dumps(nb_params)},
-                    timeout=5
+                    timeout=5,
                 )
                 if response.status_code != 200:
                     raise Exception(f"Cant update notebook {response}")
                 self.notebook = SimpleNamespace(**response.json())
             except Exception:
                 log.exception("Exception when updating notebook")
 
@@ -171,15 +172,15 @@
             self.state = new_state
             # set worker machine id
             # to control number of workers
             # in the single machine
             response = requests.post(
                 f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/set-worker-state",
                 {"state": new_state, "machine_id": machine_uuid()},
-                timeout=5
+                timeout=5,
             )
             if response.status_code != 200:
                 raise Exception(f"Problem when set worker state {response}")
             self.worker = SimpleNamespace(**response.json())
         except Exception:
             log.exception("Exception when set worker state")
 
@@ -187,15 +188,15 @@
     def delete_worker_in_db(session_id, worker_id, notebook_id):
         try:
             log.info(f"Delete worker id={worker_id}")
             server_url = os.environ.get("MERCURY_SERVER_URL", "http://127.0.0.1:8000")
 
             response = requests.post(
                 f"{server_url}/api/v1/worker/{session_id}/{worker_id}/{notebook_id}/delete-worker",
-                timeout=5
+                timeout=5,
             )
             if response.status_code != 204:
                 raise Exception(f"Problem when delete worker {response}")
 
         except Exception:
             pass
             # log.exception(f"Exception when delete worker")
@@ -207,28 +208,28 @@
 
     def worker_exists(self):
         try:
             log.info(f"Worker id={self.worker_id} exists")
 
             response = requests.get(
                 f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/worker",
-                timeout=5
+                timeout=5,
             )
             self.worker = SimpleNamespace(**response.json())
 
         except Exception as e:
             # log.exception(f"Worker id={self.worker_id} does not exists, quit")
             sys.exit(1)
         return True
 
     def is_worker_stale(self):
         try:
             response = requests.get(
                 f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/is-worker-stale",
-                timeout=5
+                timeout=5,
             )
             if response.status_code == 200:
                 is_stale = response.json().get("is_stale", True)
                 log.info(f"Check worker id={self.worker_id} is stale {is_stale}")
                 return is_stale
             return True
 
@@ -238,14 +239,28 @@
             )
         return True
 
     def list_secrets(self):
         try:
             response = requests.get(
                 f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/worker-secrets",
-                timeout=5
+                timeout=5,
             )
             if response.status_code == 200:
                 return response.json()
         except Exception:
             log.exception(f"Exception when list worker id={self.worker_id} secrets")
         return []
+
+
+    def update_rest_api_task(self, state="", response="", html_path=""):
+        try:
+            log.info("Update Rest API Task")
+            response = requests.post(
+                f"{self.server_url}/api/v1/update-rest-task/{self.session_id}",
+                {"state": state, "response": response, "html_path": html_path},
+                timeout=5,
+            )
+            if response.status_code != 200:
+                raise Exception(f"Problem when update rest api task {response}")
+        except Exception:
+            log.exception("Exception when update rest api task")
```

### Comparing `mercury-2.3.9/mercury/apps/nbworker/tests.py` & `mercury-2.4.0/mercury/apps/nbworker/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/nbworker/utils.py` & `mercury-2.4.0/mercury/apps/nbworker/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/nbworker/ws.py` & `mercury-2.4.0/mercury/apps/nbworker/ws.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/management/commands/add.py` & `mercury-2.4.0/mercury/apps/notebooks/management/commands/add.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/management/commands/delete.py` & `mercury-2.4.0/mercury/apps/notebooks/management/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/management/commands/list.py` & `mercury-2.4.0/mercury/apps/notebooks/management/commands/list.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/management/commands/watch.py` & `mercury-2.4.0/mercury/apps/notebooks/management/commands/watch.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/migrations/0001_initial.py` & `mercury-2.4.0/mercury/apps/notebooks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/models.py` & `mercury-2.4.0/mercury/apps/notebooks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/serializers.py` & `mercury-2.4.0/mercury/apps/notebooks/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/slides_themes.py` & `mercury-2.4.0/mercury/apps/notebooks/slides_themes.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/tasks.py` & `mercury-2.4.0/mercury/apps/notebooks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/urls.py` & `mercury-2.4.0/mercury/apps/notebooks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/notebooks/views.py` & `mercury-2.4.0/mercury/apps/notebooks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/migrations/0001_initial.py` & `mercury-2.4.0/mercury/apps/storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/migrations/0002_useruploadedfile.py` & `mercury-2.4.0/mercury/apps/storage/migrations/0002_useruploadedfile.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/models.py` & `mercury-2.4.0/mercury/apps/storage/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/s3utils.py` & `mercury-2.4.0/mercury/apps/storage/s3utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/storage.py` & `mercury-2.4.0/mercury/apps/storage/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 import requests
 
 from apps.nbworker.utils import stop_event
 from apps.storage.utils import get_worker_bucket_key
 from apps.tasks.export_pdf import to_pdf
 from apps.storage.utils import STORAGE, STORAGE_MEDIA, STORAGE_S3, MEDIA_ROOT, MEDIA_URL
+from apps.storage.utils import (
+    get_worker_bucket_key,
+)
 
 
 log = logging.getLogger(__name__)
 
 
 class StorageManager:
     def __init__(self, session_id, worker_id, notebook_id):
@@ -155,43 +158,48 @@
     #     if settings.STORAGE == settings.STORAGE_MEDIA:
     #         fpath = os.path.join(
     #             self.worker_output_dir(), f"nb-{self.some_hash()}.ipynb"
     #         )
     #         write_nb(nb, fpath)
     #     return fpath
 
-    def save_nb_html(self, nb_html_body):
-        html_path, url = None, None
+    def save_nb_html(self, nb_html_body, get_download_link=True, output_dir = "downdload-html"):
+        html_path, html_url, url = None, None, None
         fname = f"download-notebook-{self.some_hash()}.html"
 
         if STORAGE == STORAGE_MEDIA:
             html_path = os.path.join(self.worker_output_dir(), fname)
             with open(html_path, "w", encoding="utf-8", errors="ignore") as fout:
                 fout.write(nb_html_body)
             html_url = f"{MEDIA_URL}/{self.session_id}/output_{self.worker_id}/{fname}"
         elif STORAGE == STORAGE_S3:
             # 1.
             # get upload link
             action = "put_object"
-            output_dir = "downdload-html"
             url = f"{self.server_url}/api/v1/worker/presigned-url/{action}/{self.session_id}/{self.worker_id}/{self.notebook_id}/{output_dir}/{fname}"
             response = requests.get(url, timeout=15)
             upload_url = response.json().get("url")
             # 2.
             # upload file
             response = requests.put(upload_url, nb_html_body.encode("utf-8"), timeout=15)
             if response.status_code != 200:
                 raise Exception(f"Notebook not uploaded {response}")
-            # 3.
-            # get download link
-            action = "get_object"
-            output_dir = "downdload-html"
-            url = f"{self.server_url}/api/v1/worker/presigned-url/{action}/{self.session_id}/{self.worker_id}/{self.notebook_id}/{output_dir}/{fname}"
-            response = requests.get(url, timeout=15)
-            html_url = response.json().get("url")
+            
+            html_path = get_worker_bucket_key(
+                self.session_id, output_dir, fname.replace(" ", "-")
+            )
+
+            if get_download_link:
+                # 3.
+                # get download link
+                action = "get_object"
+                output_dir = "downdload-html"
+                url = f"{self.server_url}/api/v1/worker/presigned-url/{action}/{self.session_id}/{self.worker_id}/{self.notebook_id}/{output_dir}/{fname}"
+                response = requests.get(url, timeout=15)
+                html_url = response.json().get("url")
 
         return html_path, html_url
 
     def save_nb_pdf(self, nb_html_body, is_presentation):
         pdf_path, pdf_url = None, None
         fname = f"download-notebook-{self.some_hash()}.pdf"
         if STORAGE == STORAGE_MEDIA:
```

### Comparing `mercury-2.3.9/mercury/apps/storage/tests.py` & `mercury-2.4.0/mercury/apps/storage/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/urls.py` & `mercury-2.4.0/mercury/apps/storage/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/utils.py` & `mercury-2.4.0/mercury/apps/storage/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/views/dashboardfiles.py` & `mercury-2.4.0/mercury/apps/storage/views/dashboardfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/views/notebookfiles.py` & `mercury-2.4.0/mercury/apps/storage/views/notebookfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/views/stylefiles.py` & `mercury-2.4.0/mercury/apps/storage/views/stylefiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/storage/views/workerfiles.py` & `mercury-2.4.0/mercury/apps/storage/views/workerfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/export_pdf.py` & `mercury-2.4.0/mercury/apps/tasks/export_pdf.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/export_png.py` & `mercury-2.4.0/mercury/apps/tasks/export_png.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/migrations/0001_initial.py` & `mercury-2.4.0/mercury/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/models.py` & `mercury-2.4.0/mercury/apps/tasks/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.db import models
 
 from apps.notebooks.models import Notebook
-
+from django.contrib.auth.models import User
+from apps.accounts.fields import AutoLastModifiedField
 
 class Task(models.Model):
     # task id from Celery
     task_id = models.CharField(max_length=128, blank=True)
     # web browser session id
     session_id = models.CharField(max_length=128)
     # notebook
@@ -17,7 +18,30 @@
     # state of execution, can be: CREATED, RECEIVED, DONE, ERROR
     state = models.CharField(max_length=128, blank=True)
     # input params for task
     params = models.TextField(blank=True)
     # result of execution, should contain
     # the path with HTML notebook
     result = models.TextField(blank=True)
+
+class RestAPITask(models.Model):
+    # web browser session id
+    session_id = models.CharField(max_length=128)
+    # notebook
+    notebook = models.ForeignKey(
+        Notebook,
+        on_delete=models.CASCADE,
+    )
+    created_at = models.DateTimeField(auto_now_add=True)
+    updated_at = AutoLastModifiedField()
+    created_by = models.ForeignKey(User, on_delete=models.SET_NULL, null=True, blank=True)
+    # state of execution, can be: CREATED, RECEIVED, DONE, ERROR
+    state = models.CharField(max_length=128, blank=True)
+    # input params for task
+    params = models.TextField(blank=True)
+    # result of execution, should contain
+    # the path with HTML notebook
+    nb_html_path = models.TextField(blank=True)
+    # PDF path
+    nb_pdf_path = models.TextField(blank=True)
+    # JSON response
+    response = models.TextField(blank=True)
```

### Comparing `mercury-2.3.9/mercury/apps/tasks/notify.py` & `mercury-2.4.0/mercury/apps/tasks/notify.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/tasks.py` & `mercury-2.4.0/mercury/apps/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/tasks_export.py` & `mercury-2.4.0/mercury/apps/tasks/tasks_export.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/tests.py` & `mercury-2.4.0/mercury/apps/tasks/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/tasks/urls.py` & `mercury-2.4.0/mercury/apps/tasks/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ExportPDF,
     GetLastTaskView,
     GetPDFAddress,
     GetRestAPITask,
     ListOutputFilesView,
     ListWorkerOutputFilesView,
     TaskCreateView,
+    ListRestAPITasks
 )
 
 tasks_urlpatterns = [
     re_path("api/v1/execute/(?P<notebook_id>.+)", TaskCreateView.as_view()),
     re_path(
         "api/v1/latest_task/(?P<notebook_id>.+)/(?P<session_id>.+)",
         GetLastTaskView.as_view(),
@@ -28,17 +29,20 @@
         "api/v1/worker-output-files/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)",
         ListWorkerOutputFilesView.as_view(),
     ),
     re_path(
         "api/v1/clear_tasks/(?P<notebook_id>.+)/(?P<session_id>.+)",
         ClearTasksView.as_view(),
     ),
-    # used by notebook as REST API
-    re_path("run/(?P<notebook_slug>.+)", CreateRestAPITask.as_view()),
-    re_path("get/(?P<session_id>.+)", GetRestAPITask.as_view()),
+    # 
     re_path("export_pdf", ExportPDF.as_view()),
     re_path("get_pdf/(?P<job_id>.+)", GetPDFAddress.as_view()),
     re_path(
         "api/v1/execution_history/(?P<notebook_id>.+)/(?P<session_id>.+)",
         ExecutionHistoryView.as_view(),
     ),
+
+    # used by notebook as REST API
+    re_path("api/v1/(?P<site_id>.+)/run/(?P<notebook_slug>.+)", CreateRestAPITask.as_view()),
+    re_path("api/v1/get/(?P<task_id>.+)", GetRestAPITask.as_view()),
+    re_path("api/v1/(?P<site_id>.+)/(?P<notebook_id>.+)/list-rest-tasks", ListRestAPITasks.as_view()),
 ]
```

### Comparing `mercury-2.3.9/mercury/apps/tasks/views.py` & `mercury-2.4.0/mercury/apps/tasks/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 from apps.storage.s3utils import S3
 from apps.storage.storage import StorageManager
 from apps.tasks.models import Task
 from apps.tasks.serializers import TaskSerializer
 from apps.tasks.tasks import task_execute
 from apps.tasks.tasks_export import export_to_pdf
 
+from apps.workers.models import Worker
+from apps.ws.tasks import task_start_websocket_worker
+
+from apps.tasks.models import RestAPITask
+
+from rest_framework import permissions
+from apps.accounts.views.permissions import HasEditRights
+
 
 class TaskCreateView(CreateAPIView):
     serializer_class = TaskSerializer
     queryset = Task.objects.all()
 
     def perform_create(self, serializer):
         notebook = get_object_or_404(
@@ -135,67 +143,14 @@
                 f"Trying to clear tasks for notebook_id {notebook_id} and session_id {session_id}"
             )
             print("Exception occured", str(e))
 
         return Response(status=status.HTTP_204_NO_CONTENT)
 
 
-class CreateRestAPITask(APIView):
-    def post(self, request, notebook_slug):
-        try:
-            notebook = (
-                notebooks_queryset(request).filter(slug=notebook_slug).latest("id")
-            )
-        except Notebook.DoesNotExist:
-            raise Http404()
-        try:
-            with transaction.atomic():
-                task = Task(
-                    session_id=uuid.uuid4().hex,
-                    state="CREATED",
-                    notebook=notebook,
-                    params=json.dumps(request.data),
-                )
-                task.save()
-                job_params = {"db_id": task.id}
-                transaction.on_commit(lambda: task_execute.delay(job_params))
-            return Response({"id": task.session_id}, status=status.HTTP_201_CREATED)
-        except Exception as e:
-            raise APIException(str(e))
-
-
-class GetRestAPITask(APIView):
-    def get(self, requset, session_id):
-        try:
-            task = Task.objects.filter(
-                session_id=session_id,
-            ).latest("id")
-
-            if task.state == "DONE":
-                response = {}
-                try:
-                    fname = os.path.join(
-                        settings.MEDIA_ROOT, task.session_id, "response.json"
-                    )
-                    if os.path.exists(fname):
-                        with open(fname) as fin:
-                            response = json.loads(fin.read())
-                except Exception as e:
-                    return Response(
-                        str(e), status=status.HTTP_500_INTERNAL_SERVER_ERROR
-                    )
-                return Response(response, status=status.HTTP_200_OK)
-            if task.state == "ERROR":
-                return Response(
-                    task.result, status=status.HTTP_500_INTERNAL_SERVER_ERROR
-                )
-            return Response({"state": "running"}, status=status.HTTP_202_ACCEPTED)
-        except Task.DoesNotExist:
-            raise Http404()
-
 
 class ExportPDF(APIView):
     def post(self, request):
         try:
             # check if user can access the notebook
             notebook = notebooks_queryset(request, request.data.get("site_id")).get(
                 pk=request.data["notebook_id"]
@@ -234,7 +189,110 @@
             notebooks_queryset(self.request), pk=self.kwargs["notebook_id"]
         )
 
         return Task.objects.filter(
             notebook_id=notebook.id,
             session_id=self.kwargs["session_id"],
         )
+
+
+class CreateRestAPITask(APIView):
+    def post(self, request, site_id, notebook_slug):
+        try:
+            notebook = (
+                notebooks_queryset(request, site_id).filter(slug=notebook_slug).latest("id")
+            )
+        except Notebook.DoesNotExist:
+            raise Http404()
+        try:
+            with transaction.atomic():
+                task = RestAPITask(
+                    session_id=uuid.uuid4().hex,
+                    state="CREATED",
+                    notebook=notebook,
+                    params=json.dumps(request.data),
+                )
+                if not request.user.is_anonymous:
+                    task.created_by = request.user
+                task.save()
+
+                worker = Worker(
+                    session_id=task.session_id,
+                    notebook_id=notebook.id,
+                    state="Queued",
+                )
+                if not request.user.is_anonymous:
+                    worker.run_by = request.user
+                worker.save()
+                
+                server_address = request.build_absolute_uri('/')
+                job_params = {
+                    "notebook_id": notebook.id,
+                    "session_id": task.session_id,
+                    "worker_id": worker.id,
+                    #
+                    # ugly hack for docker deployment
+                    #
+                    "server_url": server_address
+                    if "0.0.0.0" not in server_address
+                    else server_address + ":9000",
+                }
+                
+                transaction.on_commit(lambda: task_start_websocket_worker.delay(job_params))
+
+            return Response({"task_id": task.session_id}, status=status.HTTP_201_CREATED)
+        except Exception as e:
+            raise APIException(str(e))
+
+
+class GetRestAPITask(APIView):
+    def get(self, requset, task_id):
+        try:
+            task_id = task_id.replace("/", "")
+            tasks = RestAPITask.objects.filter(
+                session_id=task_id
+            )
+            if not tasks:
+                raise Http404()
+            task = tasks.latest("id")
+            
+            if task.state == "DONE":
+                result = {"state": "done", "message": "Request successfully computed", "result": {}}
+                if task.response != "":
+                    result["result"] = json.loads(task.response)
+                #if task.nb_html_path != "":
+                #    result["notebook_html"] = task.nb_html_path
+
+                return Response(result, status=status.HTTP_200_OK)
+            if task.state == "ERROR":
+                return Response(
+                    {"state": "error", "message": f"Error when processing task, {task.response}"}, status=status.HTTP_500_INTERNAL_SERVER_ERROR
+                )
+            return Response({"state": "running", "message": "Still processing your request, please retry in 3 seconds"}, status=status.HTTP_202_ACCEPTED)
+        except RestAPITask.DoesNotExist:
+            raise Http404()
+
+class ListRestAPITasks(APIView):
+    
+    #permission_classes = [permissions.IsAuthenticated, HasEditRights]
+    
+    def get(self, requset, site_id, notebook_id):
+        try:
+            print(site_id, notebook_id)
+            tasks = RestAPITask.objects.filter(notebook_id=notebook_id)
+            print(tasks)
+            tasks_data = []
+            for t in tasks:
+                task = {
+                    "id": t.id,
+                    "state": t.state,
+                    "params": t.params,
+                    "response": t.response,
+                    "session_id": t.session_id,
+                    "created_at": t.created_at,
+                    "updated_at": t.updated_at
+                }
+                tasks_data += [task]
+            return Response(tasks_data, status=status.HTTP_200_OK)
+        except Exception as e:
+            print(str(e))
+            raise Http404()
```

### Comparing `mercury-2.3.9/mercury/apps/workers/constants.py` & `mercury-2.4.0/mercury/apps/workers/constants.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/workers/migrations/0001_initial.py` & `mercury-2.4.0/mercury/apps/workers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/workers/migrations/0002_machine.py` & `mercury-2.4.0/mercury/apps/workers/migrations/0002_machine.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py` & `mercury-2.4.0/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/workers/models.py` & `mercury-2.4.0/mercury/apps/workers/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/workers/urls.py` & `mercury-2.4.0/mercury/apps/workers/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     GetWorker,
     IsWorkerStale,
     SetWorkerState,
     WorkerGetNb,
     WorkerUpdateNb,
     MachineInfo,
     WorkerGetOwnerAndUser,
+    AnalyticsView,
+    UpdateRestApiTask,
 )
 
 workers_urlpatterns = [
     re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/nb",
         WorkerGetNb.as_view(),
     ),
@@ -40,8 +42,17 @@
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/delete-worker",
         DeleteWorker.as_view(),
     ),
     re_path(
         "api/v1/machine-info",
         MachineInfo.as_view(),
     ),
+    re_path(
+        "api/v1/(?P<site_id>.+)/analytics",
+        AnalyticsView.as_view(),
+    ),
+    re_path(
+        "api/v1/update-rest-task/(?P<session_id>.+)",
+        UpdateRestApiTask.as_view(),
+    ),
+ 
 ]
```

### Comparing `mercury-2.3.9/mercury/apps/ws/client.py` & `mercury-2.4.0/mercury/apps/ws/client.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/ws/middleware.py` & `mercury-2.4.0/mercury/apps/ws/middleware.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/ws/tasks.py` & `mercury-2.4.0/mercury/apps/ws/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/ws/utils.py` & `mercury-2.4.0/mercury/apps/ws/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/apps/ws/worker.py` & `mercury-2.4.0/mercury/apps/ws/worker.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/demo.py` & `mercury-2.4.0/mercury/demo.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/manage.py` & `mercury-2.4.0/mercury/manage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/mercury.py` & `mercury-2.4.0/mercury/mercury.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from widgets.confetti import Confetti
 from widgets.chat import Chat
 from widgets.numberbox import NumberBox
 from widgets.in_mercury import in_mercury
 from widgets.user import user
 from widgets.pdf import PDF
 from widgets.table import Table
+from widgets.apiresponse import APIResponse
 
 def print_version():
     try:
         mercury_version = ""
         with open(
             os.path.join(os.path.dirname(os.path.abspath(__file__)), "__init__.py")
         ) as fin:
```

### Comparing `mercury-2.3.9/mercury/requirements.txt` & `mercury-2.4.0/mercury/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-django==4.2.3
+django==4.2.7
 djangorestframework==3.14.0
 django-filter==21.1
 markdown==3.3.6
 celery>=5.1.2
 sqlalchemy==1.4.27
 gevent
 nbconvert>=7.8.0
```

### Comparing `mercury-2.3.9/mercury/server/asgi.py` & `mercury-2.4.0/mercury/server/asgi.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/server/celery.py` & `mercury-2.4.0/mercury/server/celery.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/server/settings.py` & `mercury-2.4.0/mercury/server/settings.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/server/urls.py` & `mercury-2.4.0/mercury/server/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/server/views.py` & `mercury-2.4.0/mercury/server/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/start_instance.py` & `mercury-2.4.0/mercury/start_instance.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/app.py` & `mercury-2.4.0/mercury/widgets/app.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/button.py` & `mercury-2.4.0/mercury/widgets/button.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/chat.py` & `mercury-2.4.0/mercury/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/checkbox.py` & `mercury-2.4.0/mercury/widgets/checkbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self.hidden = hidden
         if WidgetsManager.widget_exists(self.code_uid):
             self.checkbox = WidgetsManager.get_widget(self.code_uid)
             self.checkbox.description = label
             self.checkbox.disabled = disabled
         else:
             self.checkbox = ipywidgets.Checkbox(
-                value=value,
+                value=WidgetsManager.get_preset_value(url_key, value),
                 description=label,
                 style={"description_width": "initial"},
                 disabled=disabled,
             )
             WidgetsManager.add_widget(
                 self.checkbox.model_id, self.code_uid, self.checkbox
             )
```

### Comparing `mercury-2.3.9/mercury/widgets/file.py` & `mercury-2.4.0/mercury/widgets/file.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/in_mercury.py` & `mercury-2.4.0/mercury/widgets/in_mercury.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/json.py` & `mercury-2.4.0/mercury/widgets/json.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/manager.py` & `mercury-2.4.0/mercury/widgets/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,24 @@
 
 
 class WidgetsManager:
     widgets = {}  # model_id -> widget
     code2model = {}  # code generated uid  -> model_id
     cell_index = 0  # current cell index
 
+    preset_values = {} # url_key -> value
+
+    @staticmethod
+    def set_preset_value(url_key, value):
+        WidgetsManager.preset_values[url_key] = value
+
+    @staticmethod
+    def get_preset_value(url_key, value=None):
+        return WidgetsManager.preset_values.get(url_key, value)
+    
     @staticmethod
     def rand_uid():
         if os.environ.get("RUN_MERCURY") is None:
             h = uuid.uuid4().hex.replace("-", "")
             return f"-rand{h[:8]}"
         return ""
 
@@ -200,9 +210,14 @@
                 "input": "button",
                 "value": output.get("value", False),
                 "label": output.get("label", ""),
                 "style": output.get("style", "primary"),
                 "disabled": output.get("disabled", False),
                 "hidden": output.get("hidden", False),
             }
+        elif widget_type == "APIResponse":
+            return {
+                "output": "apiresponse",
+                "value": "",
+            }
 
         return {}
```

### Comparing `mercury-2.3.9/mercury/widgets/multiselect.py` & `mercury-2.4.0/mercury/widgets/multiselect.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             if list(self.select.options) != choices:
                 self.select.options = choices
                 self.select.value = value
             self.select.description = label
             self.select.disabled = disabled
         else:
             self.select = ipywidgets.SelectMultiple(
-                value=value,
+                value=WidgetsManager.get_preset_value(url_key, value),
                 options=choices,
                 description=label,
                 style={"description_width": "initial"},
                 disabled=disabled,
             )
             WidgetsManager.add_widget(self.select.model_id, self.code_uid, self.select)
         display(self)
```

### Comparing `mercury-2.3.9/mercury/widgets/note.py` & `mercury-2.4.0/mercury/widgets/note.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/numberbox.py` & `mercury-2.4.0/mercury/widgets/numberbox.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/numeric.py` & `mercury-2.4.0/mercury/widgets/numeric.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/outputdir.py` & `mercury-2.4.0/mercury/widgets/outputdir.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/range.py` & `mercury-2.4.0/mercury/widgets/range.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,16 +106,34 @@
         else:
             RangeConstructor = ipywidgets.IntRangeSlider
             number_format = "d"
             if isinstance(step, float):
                 RangeConstructor = ipywidgets.FloatRangeSlider
                 number_format = get_number_format(step)
 
+            try:
+                init_value = WidgetsManager.get_preset_value(url_key, None)
+                if init_value is None:
+                    init_value = value
+                else:
+                    init_value = init_value.split(",")
+                    if len(init_value) != 2:
+                        init_value = value
+                    else:
+                        if isinstance(step, float):
+                            init_value[0] = float(init_value[0])
+                            init_value[1] = float(init_value[1])
+                        else:
+                            init_value[0] = int(init_value[0])
+                            init_value[1] = int(init_value[1])
+            except Exception:
+                init_value = value
+
             self.range = RangeConstructor(
-                value=value,
+                value=init_value,
                 min=min,
                 max=max,
                 description=label,
                 step=step,
                 style={"description_width": "initial"},
                 disabled=disabled,
                 readout_format=number_format,
```

### Comparing `mercury-2.3.9/mercury/widgets/select.py` & `mercury-2.4.0/mercury/widgets/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             if list(self.dropdown.options) != choices:
                 self.dropdown.options = choices
                 self.dropdown.value = value
             self.dropdown.description = label
             self.dropdown.disabled = disabled
         else:
             self.dropdown = ipywidgets.Dropdown(
-                value=value,
+                value=WidgetsManager.get_preset_value(url_key, value),
                 options=choices,
                 description=label,
                 style={"description_width": "initial"},
                 disabled=disabled,
             )
             WidgetsManager.add_widget(
                 self.dropdown.model_id, self.code_uid, self.dropdown
```

### Comparing `mercury-2.3.9/mercury/widgets/slider.py` & `mercury-2.4.0/mercury/widgets/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             SliderConstructor = ipywidgets.IntSlider
             number_format = "d"
             if isinstance(step, float):
                 SliderConstructor = ipywidgets.FloatSlider
                 number_format = get_number_format(step)
 
             self.slider = SliderConstructor(
-                value=value,
+                value=WidgetsManager.get_preset_value(url_key, value),
                 min=min,
                 max=max,
                 description=label,
                 step=step,
                 style={"description_width": "initial"},
                 disabled=disabled,
                 readout_format=number_format,
```

### Comparing `mercury-2.3.9/mercury/widgets/table.py` & `mercury-2.4.0/mercury/widgets/table.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury/widgets/text.py` & `mercury-2.4.0/mercury/widgets/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         self.sanitize = sanitize
         if WidgetsManager.widget_exists(self.code_uid):
             self.text = WidgetsManager.get_widget(self.code_uid)
             self.text.description = label
             self.text.disabled = disabled
         else:
             self.text = ipywidgets.Textarea(
-                value=value, description=label, disabled=disabled
+                value=WidgetsManager.get_preset_value(url_key, value), description=label, disabled=disabled
             )
             WidgetsManager.add_widget(self.text.model_id, self.code_uid, self.text)
         display(self)
 
     @property
     def value(self):
         return self.text.value
```

### Comparing `mercury-2.3.9/mercury/widgets/user.py` & `mercury-2.4.0/mercury/widgets/user.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.9/mercury.egg-info/PKG-INFO` & `mercury-2.4.0/mercury.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.3.9
+Version: 2.4.0
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Author: MLJAR Sp. z o.o.
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
-
 <p align="center">
   <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/main.png#gh-light-mode-only" width="100%" />  
 </p>
 <p align="center">
   <img 
@@ -30,15 +29,15 @@
 </p>
 
 [![Tests](https://github.com/mljar/mercury/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mercury/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mercury.svg)](https://badge.fury.io/py/mercury)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mercury.svg)](https://pypi.python.org/pypi/mercury/)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-mercury/badges/license.svg)](https://anaconda.org/conda-forge/mljar-mercury)
 
-# Build Web Apps in Jupyter Notebook
+# Convert Jupyter Notebook to Web App
 
 Mercury allows you to add interactive widgets in Python notebooks, so you can share notebooks as web applications. Forget about rewriting notebooks to web frameworks just to share your results. Mercury offers a set of widgets with simple re-execution of cells.
 
 You can build with Mercury:
 - Turn your notebook into beautiful [Web Apps](https://runmercury.com/tutorials/web-app-python-jupyter-notebook/),
 - Create interactive [Presentations](https://runmercury.com/tutorials/presentation-python-jupyter-notebook/) with widgets, you can recompute slides during the show,
 - Share notebooks as static [Websites](https://runmercury.com/tutorials/website-python-jupyter-notebook/),
@@ -76,14 +75,15 @@
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets3.png#gh-light-mode-only" width="100%" />  
 </p>
  <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets_black.png#gh-dark-mode-only" width="100%" />  
 </p>
+
 ## Integrations
  
 Mercury works with virtually every Python package!
 Among the most important are machine learning libraries such as Scikit-Learn, Pandas, and Seaborn or visualization libraries: Plotly, matplotlib, Vega-Altair, and Ipyvizzu.
  <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/Integrations.png#gh-light-mode-only" width="100%" />
```

### Comparing `mercury-2.3.9/setup.py` & `mercury-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join(path, filename))
     return paths
 
 setup(
     name="mercury",
-    version="2.3.9",
+    version="2.4.0",
     author="MLJAR Sp. z o.o.",
     maintainer="MLJAR Sp. z o.o.",
     maintainer_email="contact@mljar.com",
     description="Turn Jupyter Notebook to Web App and share with non-technical users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=open("mercury/requirements.txt").readlines(),
```


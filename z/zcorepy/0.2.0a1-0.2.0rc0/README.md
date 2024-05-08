# Comparing `tmp/zcorepy-0.2.0a1.tar.gz` & `tmp/zcorepy-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcorepy-0.2.0a1.tar", last modified: Wed May  8 05:15:10 2024, max compression
+gzip compressed data, was "zcorepy-0.2.0rc0.tar", last modified: Wed May  8 13:23:04 2024, max compression
```

## Comparing `zcorepy-0.2.0a1.tar` & `zcorepy-0.2.0rc0.tar`

### file list

```diff
@@ -1,282 +1,274 @@
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.123968 zcorepy-0.2.0a1/
--rw-r--r--   0 harshshah   (501) staff       (20)    10878 2024-03-05 18:32:15.000000 zcorepy-0.2.0a1/LICENSE
--rw-r--r--   0 harshshah   (501) staff       (20)     5118 2024-05-08 05:15:10.121765 zcorepy-0.2.0a1/PKG-INFO
--rw-r--r--   0 harshshah   (501) staff       (20)     3512 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/README.md
--rw-r--r--   0 harshshah   (501) staff       (20)       38 2024-05-08 05:15:10.124145 zcorepy-0.2.0a1/setup.cfg
--rw-r--r--   0 harshshah   (501) staff       (20)     1449 2024-05-08 05:14:39.000000 zcorepy-0.2.0a1/setup.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.286888 zcorepy-0.2.0a1/src/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.299739 zcorepy-0.2.0a1/src/zcore/
--rw-r--r--   0 harshshah   (501) staff       (20)       41 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.301480 zcorepy-0.2.0a1/src/zcore/api/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.302980 zcorepy-0.2.0a1/src/zcore/api/app_auth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.305144 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.314686 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      237 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      281 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5419 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2757 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/views.py
--rw-r--r--   0 harshshah   (501) staff       (20)      156 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/app_auth/urls.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.319815 zcorepy-0.2.0a1/src/zcore/api/platform/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.321087 zcorepy-0.2.0a1/src/zcore/api/platform/auth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/auth/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.334158 zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      558 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      537 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6086 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.336416 zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.343018 zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      369 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      254 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/v1/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)    11929 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.346488 zcorepy-0.2.0a1/src/zcore/api/platform/packages/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/packages/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.352152 zcorepy-0.2.0a1/src/zcore/api/platform/packages/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/packages/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      217 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/packages/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2606 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/packages/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.353852 zcorepy-0.2.0a1/src/zcore/api/platform/permissions/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/permissions/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.371803 zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1945 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      583 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6513 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.378180 zcorepy-0.2.0a1/src/zcore/api/platform/tasks/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tasks/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.384857 zcorepy-0.2.0a1/src/zcore/api/platform/tasks/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tasks/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1366 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tasks/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      213 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tasks/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4920 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tasks/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.385841 zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.393432 zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4832 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1926 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)    21234 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/views.py
--rw-r--r--   0 harshshah   (501) staff       (20)      291 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/api/platform/urls.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.397508 zcorepy-0.2.0a1/src/zcore/apps/
--rw-r--r--   0 harshshah   (501) staff       (20)      176 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.415949 zcorepy-0.2.0a1/src/zcore/apps/appauth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      124 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      221 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/apps.py
--rw-r--r--   0 harshshah   (501) staff       (20)      929 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/auth_backend.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.597115 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     7465 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      618 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0002_default_user_roles.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1124 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1633 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0004_oldpasswords.py
--rw-r--r--   0 harshshah   (501) staff       (20)      325 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0005_remove_appusermodel_user.py
--rw-r--r--   0 harshshah   (501) staff       (20)      396 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0006_appusermodel_app_objects.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     9191 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/models.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.601975 zcorepy-0.2.0a1/src/zcore/apps/appauth/platform/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/platform/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      265 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/platform/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1556 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/platform/views.py
--rw-r--r--   0 harshshah   (501) staff       (20)      356 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      477 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/signals.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.605866 zcorepy-0.2.0a1/src/zcore/apps/appauth/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)      738 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/templates/app.html
--rw-r--r--   0 harshshah   (501) staff       (20)      919 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/templates/app_login_signup.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      203 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      682 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/appauth/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.629344 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/
--rw-r--r--   0 harshshah   (501) staff       (20)       59 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      950 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.631149 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/fields/
--rw-r--r--   0 harshshah   (501) staff       (20)     4411 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/fields/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.632599 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/management/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/management/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.635281 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/management/commands/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/management/commands/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/management/commands/reload_tenant.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.636591 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)    15486 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)      567 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/permissions.py
--rw-r--r--   0 harshshah   (501) staff       (20)      350 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/registry.py
--rw-r--r--   0 harshshah   (501) staff       (20)      385 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/signals.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.637270 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)    29339 2024-05-08 05:13:42.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/templates/default_landing.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      224 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3141 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.647128 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)    17473 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/lifecycle.py
--rw-r--r--   0 harshshah   (501) staff       (20)      737 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)      897 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/wtree.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.656032 zcorepy-0.2.0a1/src/zcore/apps/object_store/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      130 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      166 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.661502 zcorepy-0.2.0a1/src/zcore/apps/object_store/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)      784 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2485 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/object_store/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.697900 zcorepy-0.2.0a1/src/zcore/apps/permissions/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      242 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      165 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.709774 zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     3203 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      678 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
--rw-r--r--   0 harshshah   (501) staff       (20)      669 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0003_default_policy.py
--rw-r--r--   0 harshshah   (501) staff       (20)      762 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5050 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/mixin.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3748 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/permissions/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.713380 zcorepy-0.2.0a1/src/zcore/apps/shared/
--rw-r--r--   0 harshshah   (501) staff       (20)      454 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.739833 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2579 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/abstract_model.py
--rw-r--r--   0 harshshah   (501) staff       (20)      140 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      267 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/apps.py
--rw-r--r--   0 harshshah   (501) staff       (20)      940 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/auth_backend.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.747252 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     5327 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      914 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     7170 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/models.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.102772 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/templates/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.754122 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/templates/app_panel/
--rw-r--r--   0 harshshah   (501) staff       (20)     4939 2024-05-08 05:13:42.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/templates/app_panel/app_panel_login.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      664 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1117 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.836970 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      180 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      161 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.838486 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.852904 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2263 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/sync_static.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2780 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/ws_makemigration.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1457 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/ws_migrate.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.864745 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)    54320 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      363 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1095 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1136 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5728 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1890 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/tasks.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.865194 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)      676 2024-05-08 05:13:42.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/templates/app_panel.html
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.866238 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/templatetags/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/templatetags/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      560 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/templatetags/zstatic.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      147 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1546 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)      385 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.867133 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/workspace_folder_template/
--rw-r--r--   0 harshshah   (501) staff       (20)       30 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.869557 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/
--rw-r--r--   0 harshshah   (501) staff       (20)       22 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
--rw-r--r--   0 harshshah   (501) staff       (20)       93 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.889505 zcorepy-0.2.0a1/src/zcore/apps/tasks/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/tasks/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      153 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/tasks/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.892768 zcorepy-0.2.0a1/src/zcore/apps/tasks/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     2952 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/tasks/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/tasks/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2648 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/tasks/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2649 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/apps/tasks/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.267906 zcorepy-0.2.0a1/src/zcore/assets/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.253667 zcorepy-0.2.0a1/src/zcore/assets/app_landing/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.894621 zcorepy-0.2.0a1/src/zcore/assets/app_landing/css/
--rw-r--r--   0 harshshah   (501) staff       (20)     5763 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_landing/css/styles.css
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.265687 zcorepy-0.2.0a1/src/zcore/assets/app_panel/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.896235 zcorepy-0.2.0a1/src/zcore/assets/app_panel/css/
--rw-r--r--   0 harshshah   (501) staff       (20)    10247 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_panel/css/styles.css
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.956747 zcorepy-0.2.0a1/src/zcore/assets/app_panel/images/
--rw-r--r--   0 harshshah   (501) staff       (20)     3499 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_panel/images/zelthyLogo.svg
--rw-r--r--   0 harshshah   (501) staff       (20)     3906 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_panel/images/zelthyLogoIpad.svg
--rw-r--r--   0 harshshah   (501) staff       (20)     3913 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_panel/images/zelthyLogoIphone.svg
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.014907 zcorepy-0.2.0a1/src/zcore/assets/app_panel/js/
--rw-r--r--   0 harshshah   (501) staff       (20)  6158509 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_panel/js/build.v1.0.42.min.js
--rw-r--r--   0 harshshah   (501) staff       (20)  6158490 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_panel/js/build.v1.0.43.min.js
--rw-r--r--   0 harshshah   (501) staff       (20)  6158320 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/app_panel/js/build.v1.0.44.min.js
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.268267 zcorepy-0.2.0a1/src/zcore/assets/js/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:09.268962 zcorepy-0.2.0a1/src/zcore/assets/js/jquery/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.032092 zcorepy-0.2.0a1/src/zcore/assets/js/jquery/3.7.1/
--rw-r--r--   0 harshshah   (501) staff       (20)    87532 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/assets/js/jquery/3.7.1/jquery.min.js
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.044343 zcorepy-0.2.0a1/src/zcore/cli/
--rw-r--r--   0 harshshah   (501) staff       (20)      331 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      617 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/install_package.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1201 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/package_info.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.045828 zcorepy-0.2.0a1/src/zcore/cli/project_template/
--rwxr-xr-x   0 harshshah   (501) staff       (20)      672 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/manage.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.079378 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/
--rw-r--r--   0 harshshah   (501) staff       (20)       76 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/asgi.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3713 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/settings.py
--rw-r--r--   0 harshshah   (501) staff       (20)      767 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/urls_public.py
--rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/urls_tenants.py
--rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/wsgi.py
--rw-r--r--   0 harshshah   (501) staff       (20)     7084 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/start_project.py
--rw-r--r--   0 harshshah   (501) staff       (20)      688 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/cli/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.084436 zcorepy-0.2.0a1/src/zcore/config/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/config/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      552 2024-05-08 05:13:42.000000 zcorepy-0.2.0a1/src/zcore/config/celery.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.087227 zcorepy-0.2.0a1/src/zcore/config/settings/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/config/settings/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4942 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/config/settings/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      856 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/config/urls_public.py
--rw-r--r--   0 harshshah   (501) staff       (20)      708 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/config/urls_tenants.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.103914 zcorepy-0.2.0a1/src/zcore/core/
--rw-r--r--   0 harshshah   (501) staff       (20)       40 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.106187 zcorepy-0.2.0a1/src/zcore/core/api/
--rw-r--r--   0 harshshah   (501) staff       (20)      205 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/api/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2155 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/api/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      847 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/api/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1097 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/common_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)      810 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/custom_pluginbase.py
--rw-r--r--   0 harshshah   (501) staff       (20)      725 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/exception_handlers.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.108118 zcorepy-0.2.0a1/src/zcore/core/generic_views/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/generic_views/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1546 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/generic_views/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5955 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/internal_requests.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1096 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/model_mixins.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6624 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/package_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2576 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/permissions.py
--rw-r--r--   0 harshshah   (501) staff       (20)      890 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/profile_mixin.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2100 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/storage_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1242 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/tasks.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1803 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/template_loader.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4543 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/tenant_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3014 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/core/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.114017 zcorepy-0.2.0a1/src/zcore/middleware/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/middleware/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1772 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/middleware/request.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5456 2024-05-06 09:37:40.000000 zcorepy-0.2.0a1/src/zcore/middleware/tenant.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 05:15:10.119747 zcorepy-0.2.0a1/src/zcorepy.egg-info/
--rw-r--r--   0 harshshah   (501) staff       (20)     5118 2024-05-08 05:15:05.000000 zcorepy-0.2.0a1/src/zcorepy.egg-info/PKG-INFO
--rw-r--r--   0 harshshah   (501) staff       (20)     9300 2024-05-08 05:15:05.000000 zcorepy-0.2.0a1/src/zcorepy.egg-info/SOURCES.txt
--rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-08 05:15:05.000000 zcorepy-0.2.0a1/src/zcorepy.egg-info/dependency_links.txt
--rw-r--r--   0 harshshah   (501) staff       (20)       40 2024-05-08 05:15:05.000000 zcorepy-0.2.0a1/src/zcorepy.egg-info/entry_points.txt
--rw-r--r--   0 harshshah   (501) staff       (20)      677 2024-05-08 05:15:05.000000 zcorepy-0.2.0a1/src/zcorepy.egg-info/requires.txt
--rw-r--r--   0 harshshah   (501) staff       (20)        6 2024-05-08 05:15:05.000000 zcorepy-0.2.0a1/src/zcorepy.egg-info/top_level.txt
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.325747 zcorepy-0.2.0rc0/
+-rw-r--r--   0 harshshah   (501) staff       (20)    10878 2024-03-05 18:32:15.000000 zcorepy-0.2.0rc0/LICENSE
+-rw-r--r--   0 harshshah   (501) staff       (20)     5119 2024-05-08 13:23:04.324840 zcorepy-0.2.0rc0/PKG-INFO
+-rw-r--r--   0 harshshah   (501) staff       (20)     3512 2024-05-08 12:44:20.000000 zcorepy-0.2.0rc0/README.md
+-rw-r--r--   0 harshshah   (501) staff       (20)       38 2024-05-08 13:23:04.325989 zcorepy-0.2.0rc0/setup.cfg
+-rw-r--r--   0 harshshah   (501) staff       (20)     1445 2024-05-08 13:22:37.000000 zcorepy-0.2.0rc0/setup.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.169086 zcorepy-0.2.0rc0/src/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.170934 zcorepy-0.2.0rc0/src/zcore/
+-rw-r--r--   0 harshshah   (501) staff       (20)       41 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.171235 zcorepy-0.2.0rc0/src/zcore/api/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.171692 zcorepy-0.2.0rc0/src/zcore/api/app_auth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.171936 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.173183 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      237 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      281 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5419 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2753 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/views.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      156 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/app_auth/urls.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.173610 zcorepy-0.2.0rc0/src/zcore/api/platform/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.173846 zcorepy-0.2.0rc0/src/zcore/api/platform/auth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/auth/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.174916 zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      558 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      537 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6079 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.175425 zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.178152 zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      369 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      254 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/v1/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    11926 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.178606 zcorepy-0.2.0rc0/src/zcore/api/platform/packages/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/packages/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.180091 zcorepy-0.2.0rc0/src/zcore/api/platform/packages/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/packages/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      217 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/packages/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2601 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/packages/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.180497 zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.182198 zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1945 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      583 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6507 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.182712 zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.184156 zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1366 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      213 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4914 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.185076 zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.187443 zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4832 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1926 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    21220 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/views.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      291 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/api/platform/urls.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.188055 zcorepy-0.2.0rc0/src/zcore/apps/
+-rw-r--r--   0 harshshah   (501) staff       (20)      176 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.192252 zcorepy-0.2.0rc0/src/zcore/apps/appauth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      124 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      221 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/apps.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      929 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/auth_backend.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.194791 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     7465 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      618 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0002_default_user_roles.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1124 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1633 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0004_oldpasswords.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      325 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0005_remove_appusermodel_user.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      396 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0006_appusermodel_app_objects.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     9188 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      356 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      477 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/signals.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.195497 zcorepy-0.2.0rc0/src/zcore/apps/appauth/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)      738 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/templates/app.html
+-rw-r--r--   0 harshshah   (501) staff       (20)      919 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/templates/app_login_signup.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      203 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      682 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/appauth/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.202238 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/
+-rw-r--r--   0 harshshah   (501) staff       (20)       59 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      950 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.202940 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/fields/
+-rw-r--r--   0 harshshah   (501) staff       (20)     4411 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/fields/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.203334 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/management/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/management/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.203802 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/management/commands/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/management/commands/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/management/commands/reload_tenant.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.204069 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    15486 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      567 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/permissions.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      350 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/registry.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      385 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/signals.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.204275 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)    29339 2024-05-08 05:13:42.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/templates/default_landing.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      224 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3141 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.206647 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/workspace/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/workspace/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    17473 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/workspace/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/workspace/lifecycle.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      897 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/workspace/wtree.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.208996 zcorepy-0.2.0rc0/src/zcore/apps/object_store/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      130 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      166 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.210079 zcorepy-0.2.0rc0/src/zcore/apps/object_store/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)      784 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2485 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/object_store/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.213332 zcorepy-0.2.0rc0/src/zcore/apps/permissions/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      242 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      165 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.216480 zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     3203 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      678 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      669 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0003_default_policy.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      762 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5050 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/mixin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3748 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/permissions/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.216740 zcorepy-0.2.0rc0/src/zcore/apps/shared/
+-rw-r--r--   0 harshshah   (501) staff       (20)      454 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.221508 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2578 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/abstract_model.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      140 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      267 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/apps.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      940 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/auth_backend.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.222537 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5327 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      914 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     7168 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/models.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.159412 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/templates/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.222749 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/templates/app_panel/
+-rw-r--r--   0 harshshah   (501) staff       (20)     4939 2024-05-08 05:13:42.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/templates/app_panel/app_panel_login.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      664 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1115 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.226148 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      180 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      161 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.226448 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.227379 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2263 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/sync_static.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2780 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/ws_makemigration.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1457 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/ws_migrate.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.229750 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)    54320 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      363 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1095 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1136 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5728 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1890 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/tasks.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.229978 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)      676 2024-05-08 05:13:42.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/templates/app_panel.html
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.231335 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/templatetags/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/templatetags/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      560 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/templatetags/zstatic.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      147 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1546 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      383 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.232430 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/workspace_folder_template/
+-rw-r--r--   0 harshshah   (501) staff       (20)       30 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.234186 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/
+-rw-r--r--   0 harshshah   (501) staff       (20)       22 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
+-rw-r--r--   0 harshshah   (501) staff       (20)       93 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.237423 zcorepy-0.2.0rc0/src/zcore/apps/tasks/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/tasks/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      153 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/tasks/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.238862 zcorepy-0.2.0rc0/src/zcore/apps/tasks/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     2952 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/tasks/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/tasks/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2647 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/apps/tasks/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2649 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/apps/tasks/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.166225 zcorepy-0.2.0rc0/src/zcore/assets/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.165404 zcorepy-0.2.0rc0/src/zcore/assets/app_landing/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.239783 zcorepy-0.2.0rc0/src/zcore/assets/app_landing/css/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5763 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_landing/css/styles.css
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.166071 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.241841 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/css/
+-rw-r--r--   0 harshshah   (501) staff       (20)    10247 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/css/styles.css
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.248512 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/images/
+-rw-r--r--   0 harshshah   (501) staff       (20)     3499 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/images/zelthyLogo.svg
+-rw-r--r--   0 harshshah   (501) staff       (20)     3906 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/images/zelthyLogoIpad.svg
+-rw-r--r--   0 harshshah   (501) staff       (20)     3913 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/images/zelthyLogoIphone.svg
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.262336 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/js/
+-rw-r--r--   0 harshshah   (501) staff       (20)  6158509 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/js/build.v1.0.42.min.js
+-rw-r--r--   0 harshshah   (501) staff       (20)  6158490 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/js/build.v1.0.43.min.js
+-rw-r--r--   0 harshshah   (501) staff       (20)  6158320 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/app_panel/js/build.v1.0.44.min.js
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.166468 zcorepy-0.2.0rc0/src/zcore/assets/js/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.166714 zcorepy-0.2.0rc0/src/zcore/assets/js/jquery/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.268253 zcorepy-0.2.0rc0/src/zcore/assets/js/jquery/3.7.1/
+-rw-r--r--   0 harshshah   (501) staff       (20)    87532 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/assets/js/jquery/3.7.1/jquery.min.js
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.271928 zcorepy-0.2.0rc0/src/zcore/cli/
+-rw-r--r--   0 harshshah   (501) staff       (20)      331 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      617 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/install_package.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1201 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/package_info.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.272602 zcorepy-0.2.0rc0/src/zcore/cli/project_template/
+-rwxr-xr-x   0 harshshah   (501) staff       (20)      672 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/manage.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.282711 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/
+-rw-r--r--   0 harshshah   (501) staff       (20)       76 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/asgi.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3713 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/settings.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      767 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/urls_public.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/urls_tenants.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/wsgi.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     7084 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/start_project.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      688 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/cli/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.287671 zcorepy-0.2.0rc0/src/zcore/config/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/config/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      552 2024-05-08 05:13:42.000000 zcorepy-0.2.0rc0/src/zcore/config/celery.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.289488 zcorepy-0.2.0rc0/src/zcore/config/settings/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/config/settings/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4940 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/config/settings/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      856 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/config/urls_public.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      708 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/config/urls_tenants.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.306128 zcorepy-0.2.0rc0/src/zcore/core/
+-rw-r--r--   0 harshshah   (501) staff       (20)       39 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/core/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.309074 zcorepy-0.2.0rc0/src/zcore/core/api/
+-rw-r--r--   0 harshshah   (501) staff       (20)      200 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/core/api/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2104 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/core/api/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      846 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/core/api/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1097 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/common_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      810 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/custom_pluginbase.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.310842 zcorepy-0.2.0rc0/src/zcore/core/generic_views/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/generic_views/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1538 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/core/generic_views/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5955 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/internal_requests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1096 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/model_mixins.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6624 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/package_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2576 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/permissions.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2100 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/storage_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1237 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/core/tasks.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1803 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/template_loader.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3014 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/core/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.314862 zcorepy-0.2.0rc0/src/zcore/middleware/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/middleware/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1772 2024-05-06 09:37:40.000000 zcorepy-0.2.0rc0/src/zcore/middleware/request.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5455 2024-05-08 12:42:23.000000 zcorepy-0.2.0rc0/src/zcore/middleware/tenant.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-08 13:23:04.322819 zcorepy-0.2.0rc0/src/zcorepy.egg-info/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5119 2024-05-08 13:23:02.000000 zcorepy-0.2.0rc0/src/zcorepy.egg-info/PKG-INFO
+-rw-r--r--   0 harshshah   (501) staff       (20)     9026 2024-05-08 13:23:03.000000 zcorepy-0.2.0rc0/src/zcorepy.egg-info/SOURCES.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-08 13:23:03.000000 zcorepy-0.2.0rc0/src/zcorepy.egg-info/dependency_links.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)       40 2024-05-08 13:23:03.000000 zcorepy-0.2.0rc0/src/zcorepy.egg-info/entry_points.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)      677 2024-05-08 13:23:03.000000 zcorepy-0.2.0rc0/src/zcorepy.egg-info/requires.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)        6 2024-05-08 13:23:03.000000 zcorepy-0.2.0rc0/src/zcorepy.egg-info/top_level.txt
```

### Comparing `zcorepy-0.2.0a1/LICENSE` & `zcorepy-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/PKG-INFO` & `zcorepy-0.2.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcorepy
-Version: 0.2.0a1
+Version: 0.2.0rc0
 Summary: ZCore: multi-tenant Django framework for building business apps
 Home-page: https://github.com/Healthlane-Technologies/zelthy3
 Author: Zelthy ("Healthlane Technologies")
 Author-email: maintainers@zelthy.com
 License: Apache License 2.0
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
@@ -50,15 +50,15 @@
     </a>
 </h1>
 
 
 [Website](https://www.zelthy.com/framework) • [Getting Started](https://docs.zelthy.com/docs/category/getting-started) • [Docs](https://docs.zelthy.com/)
 
 
-[![PyPI version](https://badge.fury.io/py/zelthy3.svg)](https://badge.fury.io/py/zelthy3)
+[![PyPI version](https://badge.fury.io/py/zcorepy.svg)](https://badge.fury.io/py/zcorepy)
 ![docs](https://img.shields.io/github/actions/workflow/status/Healthlane-Technologies/zelthy3/docs.yml?branch=main)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 
 ## ZCore is an open source multi-tenant Django framework for building enterprise apps
 
 - Quickly build enterprise ready apps, leveraging the power of Django and ZCore package ecosystem
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcorepy Version: 0.2.0a1 Summary: ZCore: multi-
+Metadata-Version: 2.1 Name: zcorepy Version: 0.2.0rc0 Summary: ZCore: multi-
 tenant Django framework for building business apps Home-page: https://
 github.com/Healthlane-Technologies/zelthy3 Author: Zelthy ("Healthlane
 Technologies") Author-email: maintainers@zelthy.com License: Apache License 2.0
 Classifier: Framework :: Django Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 django==4.2.11 Requires-Dist: psycopg2-binary Requires-Dist: django-tenants
 Requires-Dist: djangorestframework Requires-Dist: django-rest-knox Requires-
@@ -19,16 +19,16 @@
 Requires-Dist: pydub==0.25.1 Requires-Dist: django-celery-results==2.5.1
 Requires-Dist: django-environ==0.11.2 Requires-Dist: pytz==2024.1 Requires-
 Dist: django-session-security==2.6.7 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: python3-saml==1.16.0
                              ************ _[[_ZZ_CC_oo_rr_ee_]] ************
 [Website](https://www.zelthy.com/framework) â¢ [Getting Started](https://
 docs.zelthy.com/docs/category/getting-started) â¢ [Docs](https://
-docs.zelthy.com/) [![PyPI version](https://badge.fury.io/py/zelthy3.svg)]
-(https://badge.fury.io/py/zelthy3) ![docs](https://img.shields.io/github/
+docs.zelthy.com/) [![PyPI version](https://badge.fury.io/py/zcorepy.svg)]
+(https://badge.fury.io/py/zcorepy) ![docs](https://img.shields.io/github/
 actions/workflow/status/Healthlane-Technologies/zelthy3/docs.yml?branch=main)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
 opensource.org/licenses/Apache-2.0) ## ZCore is an open source multi-tenant
 Django framework for building enterprise apps - Quickly build enterprise ready
 apps, leveraging the power of Django and ZCore package ecosystem - Host
 multiple apps on a single deployment with complete isolation - Each app can
 have its own data models and workflows - Built-in user management and user
```

### Comparing `zcorepy-0.2.0a1/README.md` & `zcorepy-0.2.0rc0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     </a>
 </h1>
 
 
 [Website](https://www.zelthy.com/framework) • [Getting Started](https://docs.zelthy.com/docs/category/getting-started) • [Docs](https://docs.zelthy.com/)
 
 
-[![PyPI version](https://badge.fury.io/py/zelthy3.svg)](https://badge.fury.io/py/zelthy3)
+[![PyPI version](https://badge.fury.io/py/zcorepy.svg)](https://badge.fury.io/py/zcorepy)
 ![docs](https://img.shields.io/github/actions/workflow/status/Healthlane-Technologies/zelthy3/docs.yml?branch=main)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 
 ## ZCore is an open source multi-tenant Django framework for building enterprise apps
 
 - Quickly build enterprise ready apps, leveraging the power of Django and ZCore package ecosystem
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                              ************ _[[_ZZ_CC_oo_rr_ee_]] ************
 [Website](https://www.zelthy.com/framework) â¢ [Getting Started](https://
 docs.zelthy.com/docs/category/getting-started) â¢ [Docs](https://
-docs.zelthy.com/) [![PyPI version](https://badge.fury.io/py/zelthy3.svg)]
-(https://badge.fury.io/py/zelthy3) ![docs](https://img.shields.io/github/
+docs.zelthy.com/) [![PyPI version](https://badge.fury.io/py/zcorepy.svg)]
+(https://badge.fury.io/py/zcorepy) ![docs](https://img.shields.io/github/
 actions/workflow/status/Healthlane-Technologies/zelthy3/docs.yml?branch=main)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
 opensource.org/licenses/Apache-2.0) ## ZCore is an open source multi-tenant
 Django framework for building enterprise apps - Quickly build enterprise ready
 apps, leveraging the power of Django and ZCore package ecosystem - Host
 multiple apps on a single deployment with complete isolation - Each app can
 have its own data models and workflows - Built-in user management and user
```

### Comparing `zcorepy-0.2.0a1/setup.py` & `zcorepy-0.2.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 PROJECT_DIR = os.path.dirname(__file__)
 REQUIREMENTS_DIR = os.path.join(PROJECT_DIR, "requirements")
 
 README = os.path.join(PROJECT_DIR, "README.md")
 
-PLATFORM_VERSION = "0.2.0-alpha1"
+PLATFORM_VERSION = "0.2.0-rc"
 
 
 def get_requirements(env):
     with open(os.path.join(REQUIREMENTS_DIR, f"{env}.txt")) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
```

### Comparing `zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/utils.py` & `zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/app_auth/profile/v1/views.py` & `zcorepy-0.2.0rc0/src/zcore/api/app_auth/profile/v1/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from django.contrib.auth import authenticate
 from django.core.exceptions import ValidationError
 
 from zcore.core.api import (
     get_api_response,
-    ZelthyGenericAppAPIView,
-    ZelthySessionAppAPIView,
+    ZCoreGenericAppAPIView,
+    ZCoreSessionAppAPIView,
 )
 from zcore.api.app_auth.profile.v1.utils import PasswordValidationMixin
 from zcore.apps.appauth.models import OldPasswords
 
 from .serializers import ProfileSerializer
 
 
-class ProfileViewAPIV1(ZelthyGenericAppAPIView):
+class ProfileViewAPIV1(ZCoreGenericAppAPIView):
     def get(self, request, *args, **kwargs):
         serializer = ProfileSerializer(request.user)
         success = True
         response = {"message": "success", "profile_data": serializer.data}
         status = 200
         return get_api_response(success, response, status)
 
@@ -26,15 +26,15 @@
         if success:
             status = 200
         else:
             status = 400
         return get_api_response(success, response, status)
 
 
-class PasswordChangeViewAPIV1(ZelthySessionAppAPIView, PasswordValidationMixin):
+class PasswordChangeViewAPIV1(ZCoreSessionAppAPIView, PasswordValidationMixin):
     def clean_password(self, email, password):
         """
         Validates that the email is not already in use.
         """
         try:
             user = authenticate(username=email, password=password)
         except:
```

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/serializers.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/urls.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/auth/v1/views.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/auth/v1/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django.db.models import Q
 from django.conf import settings
 
 from zcore.core.api import (
     get_api_response,
-    ZelthyGenericPlatformAPIView,
+    ZCoreGenericPlatformAPIView,
 )
-from zcore.core.api.utils import ZelthyAPIPagination
+from zcore.core.api.utils import ZCoreAPIPagination
 from zcore.apps.shared.platformauth.models import PlatformUserModel
 from zcore.apps.shared.tenancy.models import TenantModel
 from zcore.core.permissions import IsSuperAdminPlatformUser
 from zcore.core.utils import get_search_columns
 
 from .serializers import PlatformUserSerializerModel
 
 
-class PlatformUserViewAPIV1(ZelthyGenericPlatformAPIView, ZelthyAPIPagination):
+class PlatformUserViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
     permission_classes = (IsSuperAdminPlatformUser,)
-    pagination_class = ZelthyAPIPagination
+    pagination_class = ZCoreAPIPagination
 
     def get_dropdown_options(self):
         options = {}
         options["apps"] = [
             {"id": str(t.uuid), "label": t.name}
             for t in TenantModel.objects.all().exclude(schema_name="public")
         ]
@@ -100,15 +100,15 @@
         except Exception as e:
             result = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, result, status)
 
 
-class PlatformUserDetailViewAPIV1(ZelthyGenericPlatformAPIView):
+class PlatformUserDetailViewAPIV1(ZCoreGenericPlatformAPIView):
     permission_classes = (IsSuperAdminPlatformUser,)
 
     def get_obj(self, **kwargs):
         obj = PlatformUserModel.objects.get(id=kwargs.get("user_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
@@ -140,15 +140,15 @@
             success = False
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
-class AppPanelDetailsView(ZelthyGenericPlatformAPIView):
+class AppPanelDetailsView(ZCoreGenericPlatformAPIView):
     def get_obj(self, request, **kwargs):
         obj = PlatformUserModel.objects.get(id=request.user.id)
         return obj
 
     def get(self, request, *args, **kwargs):
         try:
             obj = self.get_obj(request, **kwargs)
```

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/codeassist/v1/views.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/codeassist/v1/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import os
 import importlib
 
 from django.utils.decorators import method_decorator
 from django.conf import settings
 
 from zcore.core.common_utils import set_app_schema_path
-from zcore.core.api import get_api_response, ZelthyGenericPlatformAPIView
+from zcore.core.api import get_api_response, ZCoreGenericPlatformAPIView
 
 from zcore.apps.permissions.models import PolicyModel
 from zcore.apps.appauth.models import AppUserModel, UserRoleModel
 from zcore.apps.shared.tenancy.models import TenantModel
 
 from .utils import lambda_invocation
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class ConversationViewAPIV1(ZelthyGenericPlatformAPIView):
+class ConversationViewAPIV1(ZCoreGenericPlatformAPIView):
     def get_app_obj(self, **kwargs):
         obj = TenantModel.objects.get(uuid=kwargs.get("app_uuid"))
         return obj
 
     def get_settings_path(self, **kwargs):
         obj = self.get_app_obj(**kwargs)
         path = str(settings.BASE_DIR) + f"/workspaces/{obj.name}/settings.json"
@@ -53,15 +53,15 @@
 
         response_data = lambda_invocation(data)
         response = response_data["response"]
         return get_api_response(True, response, 200)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class ExecutionViewAPIV1(ZelthyGenericPlatformAPIView):
+class ExecutionViewAPIV1(ZCoreGenericPlatformAPIView):
     def get_app_obj(self, **kwargs):
         obj = TenantModel.objects.get(uuid=kwargs.get("app_uuid"))
         return obj
 
     def get_settings_path(self, **kwargs):
         obj = self.get_app_obj(**kwargs)
         path = str(settings.BASE_DIR) + f"/workspaces/{obj.name}/settings.json"
```

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/packages/v1/views.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/packages/v1/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from django.utils.decorators import method_decorator
 from django.core import signing
 
-from zcore.core.api import get_api_response, ZelthyGenericPlatformAPIView
+from zcore.core.api import get_api_response, ZCoreGenericPlatformAPIView
 from zcore.core.package_utils import (
     get_all_packages,
     install_package,
     get_package_configuration_url,
 )
-from zcore.core.api.utils import ZelthyAPIPagination
+from zcore.core.api.utils import ZCoreAPIPagination
 from zcore.apps.shared.tenancy.models import TenantModel, Domain
 
 
-class PackagesViewAPIV1(ZelthyGenericPlatformAPIView, ZelthyAPIPagination):
-    pagination_class = ZelthyAPIPagination
+class PackagesViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
+    pagination_class = ZCoreAPIPagination
 
     def get_app_obj(self, app_uuid):
         obj = TenantModel.objects.get(uuid=app_uuid)
         return obj
 
     def get(self, request, app_uuid, *args, **kwargs):
         action = request.GET.get("action", None)
```

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/serializers.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/urls.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/permissions/v1/views.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/permissions/v1/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 from django.utils.decorators import method_decorator
 from django.db.models import Q
 from django.db import connection
 
 from zcore.core.api import (
     get_api_response,
-    ZelthyGenericPlatformAPIView,
+    ZCoreGenericPlatformAPIView,
 )
 from zcore.core.utils import get_search_columns
 from zcore.apps.shared.tenancy.models import TenantModel
 from zcore.apps.shared.tenancy.utils import TIMEZONES, DATETIMEFORMAT
 from zcore.apps.permissions.models import PolicyModel, PermissionsModel
 from zcore.core.common_utils import set_app_schema_path
-from zcore.core.api.utils import ZelthyAPIPagination
+from zcore.core.api.utils import ZCoreAPIPagination
 from zcore.core.permissions import IsPlatformUserAllowedApp
 from zcore.apps.appauth.models import UserRoleModel
 from zcore.apps.dynamic_models.workspace.base import Workspace
 
 
 from .serializers import PolicySerializer
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class PolicyViewAPIV1(ZelthyGenericPlatformAPIView, ZelthyAPIPagination):
-    pagination_class = ZelthyAPIPagination
+class PolicyViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
+    pagination_class = ZCoreAPIPagination
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_queryset(self, search, columns={}):
         field_name_query_mapping = {
             "policy_name": "name__icontains",
             "description": "description__icontains",
             "policy_id": "id__icontains",
@@ -116,15 +116,15 @@
 
             result = {"message": error_message}
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class PolicyDetailViewAPIV1(ZelthyGenericPlatformAPIView):
+class PolicyDetailViewAPIV1(ZCoreGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = PolicyModel.objects.get(id=kwargs.get("policy_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
```

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/tasks/v1/serializers.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/tasks/v1/views.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/tasks/v1/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import traceback
 
 from django.utils.decorators import method_decorator
 from django.db import connection
 from django.db.models import Q
 
-from zcore.core.api import get_api_response, ZelthyGenericPlatformAPIView
+from zcore.core.api import get_api_response, ZCoreGenericPlatformAPIView
 from zcore.apps.tasks.models import AppTask
-from zcore.core.api.utils import ZelthyAPIPagination
+from zcore.core.api.utils import ZCoreAPIPagination
 from zcore.core.common_utils import set_app_schema_path
 from zcore.apps.dynamic_models.workspace.base import Workspace
 from zcore.apps.shared.tenancy.models import TenantModel
 from zcore.core.utils import get_search_columns
 
 
 from .serializers import TaskSerializer
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class AppTaskView(ZelthyGenericPlatformAPIView, ZelthyAPIPagination):
-    pagination_class = ZelthyAPIPagination
+class AppTaskView(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
+    pagination_class = ZCoreAPIPagination
 
     def get_queryset(self, search, columns={}):
         name_field_query_mappping = {
             "name": "name__icontains",
             "id": "id__icontains",
             "attached_policies": "attached_policies__name__icontains",
             "is_enabled": "is_enabled",
@@ -81,15 +81,15 @@
             response = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, response, status)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class AppTaskDetailView(ZelthyGenericPlatformAPIView):
+class AppTaskDetailView(ZCoreGenericPlatformAPIView):
     def get(self, request, app_uuid, task_uuid, *args, **kwargs):
         try:
             app_task = AppTask.objects.get(id=task_uuid)
             serializer = TaskSerializer(instance=app_task)
             response = {"task": serializer.data}
             status = 200
             success = True
```

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/serializers.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/urls.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/api/platform/tenancy/v1/views.py` & `zcorepy-0.2.0rc0/src/zcore/api/platform/tenancy/v1/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 
 from django.conf import settings
 from django.utils.decorators import method_decorator
 from django.db.models import Q
 
 from zcore.core.api import (
     get_api_response,
-    ZelthyGenericPlatformAPIView,
+    ZCoreGenericPlatformAPIView,
 )
 from zcore.apps.shared.tenancy.models import TenantModel, ThemesModel
 from zcore.apps.shared.tenancy.utils import TIMEZONES, DATETIMEFORMAT, DATEFORMAT
 from zcore.apps.appauth.models import UserRoleModel, AppUserModel
 from zcore.apps.permissions.models import PolicyModel
 from zcore.core.common_utils import set_app_schema_path
-from zcore.core.api.utils import ZelthyAPIPagination
+from zcore.core.api.utils import ZCoreAPIPagination
 from zcore.core.permissions import IsPlatformUserAllowedApp
 from zcore.core.utils import get_search_columns
 
 from .serializers import (
     TenantSerializerModel,
     UserRoleSerializerModel,
     AppUserModelSerializerModel,
     ThemeModelSerializer,
 )
 
 
-class AppViewAPIV1(ZelthyGenericPlatformAPIView):
+class AppViewAPIV1(ZCoreGenericPlatformAPIView):
     def get(self, request, *args, **kwargs):
         try:
             action = request.GET.get("action")
             if action == "get_app_creation_status":
                 task_id = request.GET.get("task_id")
                 try:
                     task = TaskResult.objects.get(task_id=task_id)
@@ -112,15 +112,15 @@
             # logger.error(traceback.format_exc())
             result = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, result, status)
 
 
-class AppDetailViewAPIV1(ZelthyGenericPlatformAPIView):
+class AppDetailViewAPIV1(ZCoreGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = TenantModel.objects.get(uuid=kwargs.get("app_uuid"))
         return obj
 
     def get_dropdown_options(self):
@@ -185,16 +185,16 @@
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserRoleViewAPIV1(ZelthyGenericPlatformAPIView, ZelthyAPIPagination):
-    pagination_class = ZelthyAPIPagination
+class UserRoleViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
+    pagination_class = ZCoreAPIPagination
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_dropdown_options(self):
         options = {}
         options["policies"] = [
             {"id": t.id, "label": t.name}
             for t in PolicyModel.objects.all().order_by("-modified_at")
@@ -274,15 +274,15 @@
 
             result = {"message": error_message}
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserRoleDetailViewAPIV1(ZelthyGenericPlatformAPIView):
+class UserRoleDetailViewAPIV1(ZCoreGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = UserRoleModel.objects.get(id=kwargs.get("role_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
@@ -333,16 +333,16 @@
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserViewAPIV1(ZelthyGenericPlatformAPIView, ZelthyAPIPagination):
-    pagination_class = ZelthyAPIPagination
+class UserViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
+    pagination_class = ZCoreAPIPagination
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_dropdown_options(self):
         options = {}
         options["roles"] = [
             {"id": t.id, "label": t.name}
             for t in UserRoleModel.objects.all().exclude(
@@ -422,15 +422,15 @@
             result = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, result, status)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserDetailViewAPIV1(ZelthyGenericPlatformAPIView):
+class UserDetailViewAPIV1(ZCoreGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = AppUserModel.objects.get(id=kwargs.get("user_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
@@ -462,15 +462,15 @@
             success = False
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
-class ThemeViewAPIV1(ZelthyGenericPlatformAPIView):
+class ThemeViewAPIV1(ZCoreGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_app_tenant(self):
         tenant_obj = TenantModel.objects.get(uuid=self.kwargs["app_uuid"])
         return tenant_obj
 
     def get(self, request, *args, **kwargs):
@@ -522,15 +522,15 @@
                 error_message = "Invalid data"
 
             result = {"message": error_message}
 
         return get_api_response(success, result, status_code)
 
 
-class ThemeDetailViewAPIV1(ZelthyGenericPlatformAPIView):
+class ThemeDetailViewAPIV1(ZCoreGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = ThemesModel.objects.get(
             tenant__uuid=kwargs.get("app_uuid"), id=kwargs.get("theme_id")
         )
         return obj
```

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/auth_backend.py` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/auth_backend.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0001_initial.py` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0002_default_user_roles.py` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0002_default_user_roles.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/migrations/0004_oldpasswords.py` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/migrations/0004_oldpasswords.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/models.py` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from django.db.models import Q
 from django.conf import settings
 from django.contrib.auth.hashers import check_password
 
 from zcore.core.model_mixins import FullAuditMixin
 
 from zcore.apps.object_store.models import ObjectStore
-from zcore.apps.shared.platformauth.abstract_model import AbstractZelthyUserModel
+from zcore.apps.shared.platformauth.abstract_model import AbstractZCoreUserModel
 
 
 from zcore.core.model_mixins import FullAuditMixin
 from zcore.apps.shared.platformauth.abstract_model import (
-    AbstractZelthyUserModel,
+    AbstractZCoreUserModel,
     AbstractOldPasswords,
 )
 
 from ..permissions.models import PolicyModel, PolicyGroupModel
 
 # from .perm_mixin import PolicyQsMixin
 from ..permissions.mixin import PermissionMixin
@@ -52,15 +52,15 @@
     def delete(self, *args, **kwargs):
         if self.is_default:
             # Prevent deletion of the default object
             raise ValueError("Cannot delete the default object.")
         super().delete(*args, **kwargs)
 
 
-class AppUserModel(AbstractZelthyUserModel, PermissionMixin):
+class AppUserModel(AbstractZCoreUserModel, PermissionMixin):
     roles = models.ManyToManyField(UserRoleModel, related_name="users")
     policies = models.ManyToManyField(PolicyModel, related_name="user_policies")
     policy_groups = models.ManyToManyField(
         PolicyGroupModel, related_name="user_policy_groups"
     )
     app_objects = models.JSONField(null=True)
```

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/templates/app.html` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/templates/app.html`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/templates/app_login_signup.html` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/templates/app_login_signup.html`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/appauth/views.py` & `zcorepy-0.2.0rc0/src/zcore/apps/appauth/views.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/apps.py` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/apps.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/fields/__init__.py` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/models.py` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/models.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/permissions.py` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/permissions.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/templates/default_landing.html` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/templates/default_landing.html`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/views.py` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/views.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/base.py` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/workspace/base.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/dynamic_models/workspace/wtree.py` & `zcorepy-0.2.0rc0/src/zcore/apps/dynamic_models/workspace/wtree.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/object_store/migrations/0001_initial.py` & `zcorepy-0.2.0rc0/src/zcore/apps/object_store/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/object_store/models.py` & `zcorepy-0.2.0rc0/src/zcore/apps/object_store/models.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0001_initial.py` & `zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py` & `zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0003_default_policy.py` & `zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0003_default_policy.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py` & `zcorepy-0.2.0rc0/src/zcore/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/permissions/mixin.py` & `zcorepy-0.2.0rc0/src/zcore/apps/permissions/mixin.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/permissions/models.py` & `zcorepy-0.2.0rc0/src/zcore/apps/permissions/models.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/abstract_model.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/abstract_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # from backend.core.storage_utils import S3PrivateFileField, RandomUniqueFileName
 from zcore.core.storage_utils import RandomUniqueFileName
 from zcore.core.model_mixins import FullAuditMixin
 from phonenumber_field.modelfields import PhoneNumberField
 
 
-class AbstractZelthyUserModel(AbstractBaseUser, FullAuditMixin):
+class AbstractZCoreUserModel(AbstractBaseUser, FullAuditMixin):
     name = models.CharField("full name of user", max_length=75)
     email = models.EmailField("email address", null=True, blank=True)
     mobile = PhoneNumberField("mobile number", null=True, blank=True)
     is_active = models.BooleanField(
         "active",
         default=True,
         help_text=(
```

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/auth_backend.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/auth_backend.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/migrations/0001_initial.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/models.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from django.utils.translation import gettext_lazy as _
 from django.utils import timezone
 
 from django.contrib.auth.models import User
 
 from zcore.apps.shared.tenancy.models import TenantModel
 
-from .abstract_model import AbstractZelthyUserModel
+from .abstract_model import AbstractZCoreUserModel
 
 from zcore.core.model_mixins import FullAuditMixin
 
 
-class PlatformUserModel(AbstractZelthyUserModel):
+class PlatformUserModel(AbstractZCoreUserModel):
     is_staff = models.BooleanField(
         _("staff status"),
         default=False,
         help_text="For Django Admin Access. Can be deprecated later",
     )
     is_superadmin = models.BooleanField(
         _("Super Admin"),
```

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/templates/app_panel/app_panel_login.html` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/templates/app_panel/app_panel_login.html`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/urls.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/urls.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/platformauth/views.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/platformauth/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.contrib.auth.views import LoginView
 from django.shortcuts import redirect
 from rest_framework.views import APIView
-from zcore.core.api import ZelthySessionPlatformAPIView, get_api_response
+from zcore.core.api import ZCoreSessionPlatformAPIView, get_api_response
 
 
 # Create your views here.
 class PlatformUserLoginView(LoginView):
     """
     View to render the login page html.
     """
@@ -17,15 +17,15 @@
         return redirect("/platform")
 
 
 class PlatformUserLoginAPIV1(APIView):
     pass
 
 
-class PlatformUserProfileAPIV1(ZelthySessionPlatformAPIView):
+class PlatformUserProfileAPIV1(ZCoreSessionPlatformAPIView):
     """ """
 
     def get_profile_data(self, request):
         data = {}
         data["name"] = request.user.platform_user.name
         data["email"] = request.user.platform_user.email
         data["mobile"] = request.user.platform_user.mobile
```

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/sync_static.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/sync_static.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/ws_makemigration.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/ws_makemigration.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/management/commands/ws_migrate.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/management/commands/ws_migrate.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/0001_initial.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/models.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/models.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/tasks.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/tasks.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/templates/app_panel.html` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/templates/app_panel.html`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/templatetags/zstatic.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/templatetags/zstatic.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/shared/tenancy/utils.py` & `zcorepy-0.2.0rc0/src/zcore/apps/shared/tenancy/utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/tasks/migrations/0001_initial.py` & `zcorepy-0.2.0rc0/src/zcore/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/tasks/models.py` & `zcorepy-0.2.0rc0/src/zcore/apps/tasks/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from zcore.apps.permissions.models import PolicyModel
 
 
 class AppTask(FullAuditMixin):
     name = models.CharField(max_length=255, unique=True)
     is_enabled = models.BooleanField(default=False)
     is_deleted = models.BooleanField(default=False)
-    task = "zcore.core.tasks.zelthy_task_executor"
+    task = "zcore.core.tasks.zcore_task_executor"
     interval = models.ForeignKey(
         IntervalSchedule,
         on_delete=models.CASCADE,
         null=True,
         blank=True,
         verbose_name="interval",
     )
```

### Comparing `zcorepy-0.2.0a1/src/zcore/apps/tasks/utils.py` & `zcorepy-0.2.0rc0/src/zcore/apps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_landing/css/styles.css` & `zcorepy-0.2.0rc0/src/zcore/assets/app_landing/css/styles.css`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_panel/css/styles.css` & `zcorepy-0.2.0rc0/src/zcore/assets/app_panel/css/styles.css`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_panel/images/zelthyLogo.svg` & `zcorepy-0.2.0rc0/src/zcore/assets/app_panel/images/zelthyLogo.svg`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_panel/images/zelthyLogoIpad.svg` & `zcorepy-0.2.0rc0/src/zcore/assets/app_panel/images/zelthyLogoIpad.svg`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_panel/images/zelthyLogoIphone.svg` & `zcorepy-0.2.0rc0/src/zcore/assets/app_panel/images/zelthyLogoIphone.svg`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_panel/js/build.v1.0.42.min.js` & `zcorepy-0.2.0rc0/src/zcore/assets/app_panel/js/build.v1.0.42.min.js`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_panel/js/build.v1.0.43.min.js` & `zcorepy-0.2.0rc0/src/zcore/assets/app_panel/js/build.v1.0.43.min.js`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/app_panel/js/build.v1.0.44.min.js` & `zcorepy-0.2.0rc0/src/zcore/assets/app_panel/js/build.v1.0.44.min.js`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/assets/js/jquery/3.7.1/jquery.min.js` & `zcorepy-0.2.0rc0/src/zcore/assets/js/jquery/3.7.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/cli/install_package.py` & `zcorepy-0.2.0rc0/src/zcore/cli/install_package.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/cli/package_info.py` & `zcorepy-0.2.0rc0/src/zcore/cli/package_info.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/cli/project_template/manage.py` & `zcorepy-0.2.0rc0/src/zcore/cli/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/settings.py` & `zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/settings.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/cli/project_template/project_name/urls.py` & `zcorepy-0.2.0rc0/src/zcore/cli/project_template/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/cli/start_project.py` & `zcorepy-0.2.0rc0/src/zcore/cli/start_project.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/cli/utils.py` & `zcorepy-0.2.0rc0/src/zcore/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/config/celery.py` & `zcorepy-0.2.0rc0/src/zcore/config/celery.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/config/settings/base.py` & `zcorepy-0.2.0rc0/src/zcore/config/settings/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ]
 
 TENANT_MODEL = "tenancy.TenantModel"
 TENANT_DOMAIN_MODEL = "tenancy.Domain"
 
 
 MIDDLEWARE = [
-    "zcore.middleware.tenant.ZelthyTenantMainMiddleware",
+    "zcore.middleware.tenant.ZCoreTenantMainMiddleware",
     # 'zcore.middleware.context_middleware.SimpleContextMiddleware',
     # 'zcore.middleware.tenant_url_switch.url_switch_middleware',
     # 'django_tenants.middleware.main.TenantMainMiddleware',
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
@@ -140,15 +140,15 @@
     "ukcrisp",
     "uni_form",
     "bootstrap5",
 )
 
 CRISPY_TEMPLATE_PACK = "bootstrap5"
 
-SESSION_COOKIE_NAME = "zelthycookie"
+SESSION_COOKIE_NAME = "zcorecookie"
 SESSION_COOKIE_SECURE = True
 CSRF_COOKIE_SECURE = True
 
 LOGOUT_REDIRECT_URL = "/admin/login"
 
 PASSWORD_MIN_LENGTH = 8
 PASSWORD_NO_REPEAT_DAYS = 180
```

### Comparing `zcorepy-0.2.0a1/src/zcore/config/urls_public.py` & `zcorepy-0.2.0rc0/src/zcore/config/urls_public.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/config/urls_tenants.py` & `zcorepy-0.2.0rc0/src/zcore/config/urls_tenants.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/api/base.py` & `zcorepy-0.2.0rc0/src/zcore/core/api/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 from rest_framework.views import APIView
 from rest_framework.authentication import SessionAuthentication
 from knox.auth import TokenAuthentication
 
 from ..permissions import IsAuthenticatedPlatformUser, IsAuthenticatedAppUser
 
 
-
-class ZelthySessionPlatformAPIView(APIView):
+class ZCoreSessionPlatformAPIView(APIView):
     """
     This is the base class for developing Platform APIs that need to support only session based
     authentication. Expected use cases include APIs that must be supported only with session and NOT token
     """
 
-    authentication_classes = (SessionAuthentication, )
+    authentication_classes = (SessionAuthentication,)
     permission_classes = (IsAuthenticatedPlatformUser,)
-    
 
-class ZelthySessionAppAPIView(APIView):
+
+class ZCoreSessionAppAPIView(APIView):
     """
     Base API view for developing Session Authenticated Platform APIs
     Use Case: Platform APIs accessed by the web apps on the same domain
     CSRF Not Exempted
-    This API expects zelthycookie & csrftoken as Cookies. zelthycookie should 
+    This API expects zcorecookie & csrftoken as Cookies. zcorecookie should
     represent an active platform user.
     Additional Perms: Request should pass whitelisting setting of Platform
     """
 
-    authentication_classes = (SessionAuthentication, )
+    authentication_classes = (SessionAuthentication,)
     permission_classes = (IsAuthenticatedAppUser,)
 
 
-
-class ZelthyTokenPlatformAPIView(APIView):
+class ZCoreTokenPlatformAPIView(APIView):
     """
     This is the base class for developing Platform APIs that need to support only token based
     authentication. Expected use cases include APIs that will be used by third parties only
     """
 
-    authentication_classes = (TokenAuthentication, )
+    authentication_classes = (TokenAuthentication,)
     permission_classes = (IsAuthenticatedPlatformUser,)
 
 
-
-
-class ZelthyGenericPlatformAPIView(APIView):
+class ZCoreGenericPlatformAPIView(APIView):
     """
     This is the base auth class for developing Platform APIs that need to support both
     token based authentication as well as session cookie based authentication.
-    The Zelthy platform webapp must use session based authentication and should provide csrftoken as well.
+    The ZCore platform webapp must use session based authentication and should provide csrftoken as well.
     """
 
-    authentication_classes = (SessionAuthentication,
-                                TokenAuthentication)
+    authentication_classes = (SessionAuthentication, TokenAuthentication)
     permission_classes = (IsAuthenticatedPlatformUser,)
 
-class ZelthyGenericAppAPIView(APIView):
 
+class ZCoreGenericAppAPIView(APIView):
     authentication_classes = (TokenAuthentication, SessionAuthentication)
-    permission_classes = (IsAuthenticatedAppUser,)
+    permission_classes = (IsAuthenticatedAppUser,)
```

### Comparing `zcorepy-0.2.0a1/src/zcore/core/api/utils.py` & `zcorepy-0.2.0rc0/src/zcore/core/api/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from collections import OrderedDict
 
 from django.http import HttpResponse
 from rest_framework.pagination import PageNumberPagination
 
 
-class ZelthyAPIPagination(PageNumberPagination):
+class ZCoreAPIPagination(PageNumberPagination):
     page_size = 10
     page_size_query_param = "page_size"
     max_page_size = 100
 
     def get_paginated_response_data(self, data):
         return OrderedDict(
             [
```

### Comparing `zcorepy-0.2.0a1/src/zcore/core/common_utils.py` & `zcorepy-0.2.0rc0/src/zcore/core/common_utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/custom_pluginbase.py` & `zcorepy-0.2.0rc0/src/zcore/core/custom_pluginbase.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/generic_views/base.py` & `zcorepy-0.2.0rc0/src/zcore/core/generic_views/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from django.views.generic import View, TemplateView
 from django.contrib.auth.decorators import login_required
 from ..permissions import IsAuthenticatedPlatformUser, IsAuthenticatedAppUser
 
 
-class ZelthySessionPlatformView(IsAuthenticatedPlatformUser, View):
+class ZCoreSessionPlatformView(IsAuthenticatedPlatformUser, View):
     """
     View only accessible to authenticated platform users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = None
         return login_required(
-            super(ZelthySessionPlatformView, cls).as_view(), login_url=login_url
+            super(ZCoreSessionPlatformView, cls).as_view(), login_url=login_url
         )
 
 
-class ZelthySessionPlatformTemplateView(IsAuthenticatedPlatformUser, TemplateView):
+class ZCoreSessionPlatformTemplateView(IsAuthenticatedPlatformUser, TemplateView):
     """
     TemplateView only accessible to authenticated platform users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = "/admin/login/"
         return login_required(
-            super(ZelthySessionPlatformTemplateView, cls).as_view(), login_url=login_url
+            super(ZCoreSessionPlatformTemplateView, cls).as_view(), login_url=login_url
         )
 
 
-class ZelthySessionAppView(IsAuthenticatedAppUser, View):
+class ZCoreSessionAppView(IsAuthenticatedAppUser, View):
     """
     View only accessible to authenticated app users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = None
         return login_required(
-            super(ZelthySessionAppView, cls).as_view(), login_url=login_url
+            super(ZCoreSessionAppView, cls).as_view(), login_url=login_url
         )
 
-class ZelthySessionAppTemplateView(IsAuthenticatedAppUser, TemplateView):
+class ZCoreSessionAppTemplateView(IsAuthenticatedAppUser, TemplateView):
     """
     TemplateView only accessible to authenticated app users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = None
         return login_required(
-            super(ZelthySessionAppTemplateView, cls).as_view(), login_url=login_url
+            super(ZCoreSessionAppTemplateView, cls).as_view(), login_url=login_url
         )
```

### Comparing `zcorepy-0.2.0a1/src/zcore/core/internal_requests.py` & `zcorepy-0.2.0rc0/src/zcore/core/internal_requests.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/model_mixins.py` & `zcorepy-0.2.0rc0/src/zcore/core/model_mixins.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/package_utils.py` & `zcorepy-0.2.0rc0/src/zcore/core/package_utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/permissions.py` & `zcorepy-0.2.0rc0/src/zcore/core/permissions.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/storage_utils.py` & `zcorepy-0.2.0rc0/src/zcore/core/storage_utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/tasks.py` & `zcorepy-0.2.0rc0/src/zcore/core/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import partial
 from celery import shared_task, current_task
 from django.db import connection
 
 
 @shared_task
-def zelthy_task_executor(tenant_name, task_name, *args, **kwargs):
+def zcore_task_executor(tenant_name, task_name, *args, **kwargs):
     from zcore.apps.dynamic_models.workspace.base import Workspace
     from zcore.apps.shared.tenancy.models import TenantModel
     from zcore.apps.tasks.models import AppTask
 
     tenant = TenantModel.objects.get(name=tenant_name)
 
     connection.set_tenant(tenant)
@@ -21,18 +21,18 @@
         task_module = task_obj.name.rsplit(".", 1)[0]
         func_name = task_obj.name.rsplit(".", 1)[1]
         _task = ws.plugin_source.load_plugin(f"{task_module}")
         task_fun = getattr(_task, func_name)
         return task_fun(*args, **kwargs)
 
 
-def zelthy_task(task_fun, *args, **kwargs):
-    def get_zelthy_task_executor(**options):
-        return zelthy_task_executor
+def zcore_task(task_fun, *args, **kwargs):
+    def get_zcore_task_executor(**options):
+        return zcore_task_executor
 
     def original_function(*args, **kwargs):
         return task_fun(*args, **kwargs)
 
-    task_executor = get_zelthy_task_executor()
+    task_executor = get_zcore_task_executor()
     task_executor.original_function = original_function
 
     return task_executor
```

### Comparing `zcorepy-0.2.0a1/src/zcore/core/template_loader.py` & `zcorepy-0.2.0rc0/src/zcore/core/template_loader.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/core/utils.py` & `zcorepy-0.2.0rc0/src/zcore/core/utils.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/middleware/request.py` & `zcorepy-0.2.0rc0/src/zcore/middleware/request.py`

 * *Files identical despite different names*

### Comparing `zcorepy-0.2.0a1/src/zcore/middleware/tenant.py` & `zcorepy-0.2.0rc0/src/zcore/middleware/tenant.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     get_public_schema_urlconf,
 )
 from django_tenants.middleware.main import TenantMainMiddleware
 from django.conf import settings
 from django.utils import timezone
 
 
-class ZelthyTenantMainMiddleware(TenantMainMiddleware):
+class ZCoreTenantMainMiddleware(TenantMainMiddleware):
     TENANT_NOT_FOUND_EXCEPTION = Http404
 
     @staticmethod
     def hostname_from_request(request):
         """
         Static method to extract hostname from request.
```

### Comparing `zcorepy-0.2.0a1/src/zcorepy.egg-info/PKG-INFO` & `zcorepy-0.2.0rc0/src/zcorepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcorepy
-Version: 0.2.0a1
+Version: 0.2.0rc0
 Summary: ZCore: multi-tenant Django framework for building business apps
 Home-page: https://github.com/Healthlane-Technologies/zelthy3
 Author: Zelthy ("Healthlane Technologies")
 Author-email: maintainers@zelthy.com
 License: Apache License 2.0
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
@@ -50,15 +50,15 @@
     </a>
 </h1>
 
 
 [Website](https://www.zelthy.com/framework) • [Getting Started](https://docs.zelthy.com/docs/category/getting-started) • [Docs](https://docs.zelthy.com/)
 
 
-[![PyPI version](https://badge.fury.io/py/zelthy3.svg)](https://badge.fury.io/py/zelthy3)
+[![PyPI version](https://badge.fury.io/py/zcorepy.svg)](https://badge.fury.io/py/zcorepy)
 ![docs](https://img.shields.io/github/actions/workflow/status/Healthlane-Technologies/zelthy3/docs.yml?branch=main)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 
 ## ZCore is an open source multi-tenant Django framework for building enterprise apps
 
 - Quickly build enterprise ready apps, leveraging the power of Django and ZCore package ecosystem
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcorepy Version: 0.2.0a1 Summary: ZCore: multi-
+Metadata-Version: 2.1 Name: zcorepy Version: 0.2.0rc0 Summary: ZCore: multi-
 tenant Django framework for building business apps Home-page: https://
 github.com/Healthlane-Technologies/zelthy3 Author: Zelthy ("Healthlane
 Technologies") Author-email: maintainers@zelthy.com License: Apache License 2.0
 Classifier: Framework :: Django Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 django==4.2.11 Requires-Dist: psycopg2-binary Requires-Dist: django-tenants
 Requires-Dist: djangorestframework Requires-Dist: django-rest-knox Requires-
@@ -19,16 +19,16 @@
 Requires-Dist: pydub==0.25.1 Requires-Dist: django-celery-results==2.5.1
 Requires-Dist: django-environ==0.11.2 Requires-Dist: pytz==2024.1 Requires-
 Dist: django-session-security==2.6.7 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: python3-saml==1.16.0
                              ************ _[[_ZZ_CC_oo_rr_ee_]] ************
 [Website](https://www.zelthy.com/framework) â¢ [Getting Started](https://
 docs.zelthy.com/docs/category/getting-started) â¢ [Docs](https://
-docs.zelthy.com/) [![PyPI version](https://badge.fury.io/py/zelthy3.svg)]
-(https://badge.fury.io/py/zelthy3) ![docs](https://img.shields.io/github/
+docs.zelthy.com/) [![PyPI version](https://badge.fury.io/py/zcorepy.svg)]
+(https://badge.fury.io/py/zcorepy) ![docs](https://img.shields.io/github/
 actions/workflow/status/Healthlane-Technologies/zelthy3/docs.yml?branch=main)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
 opensource.org/licenses/Apache-2.0) ## ZCore is an open source multi-tenant
 Django framework for building enterprise apps - Quickly build enterprise ready
 apps, leveraging the power of Django and ZCore package ecosystem - Host
 multiple apps on a single deployment with complete isolation - Each app can
 have its own data models and workflows - Built-in user management and user
```

### Comparing `zcorepy-0.2.0a1/src/zcorepy.egg-info/SOURCES.txt` & `zcorepy-0.2.0rc0/src/zcorepy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,14 @@
 src/zcore/apps/appauth/migrations/0001_initial.py
 src/zcore/apps/appauth/migrations/0002_default_user_roles.py
 src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
 src/zcore/apps/appauth/migrations/0004_oldpasswords.py
 src/zcore/apps/appauth/migrations/0005_remove_appusermodel_user.py
 src/zcore/apps/appauth/migrations/0006_appusermodel_app_objects.py
 src/zcore/apps/appauth/migrations/__init__.py
-src/zcore/apps/appauth/platform/__init__.py
-src/zcore/apps/appauth/platform/urls.py
-src/zcore/apps/appauth/platform/views.py
 src/zcore/apps/appauth/templates/app.html
 src/zcore/apps/appauth/templates/app_login_signup.html
 src/zcore/apps/dynamic_models/__init__.py
 src/zcore/apps/dynamic_models/admin.py
 src/zcore/apps/dynamic_models/apps.py
 src/zcore/apps/dynamic_models/models.py
 src/zcore/apps/dynamic_models/permissions.py
@@ -80,15 +77,14 @@
 src/zcore/apps/dynamic_models/management/commands/__init__.py
 src/zcore/apps/dynamic_models/management/commands/reload_tenant.py
 src/zcore/apps/dynamic_models/migrations/__init__.py
 src/zcore/apps/dynamic_models/templates/default_landing.html
 src/zcore/apps/dynamic_models/workspace/__init__.py
 src/zcore/apps/dynamic_models/workspace/base.py
 src/zcore/apps/dynamic_models/workspace/lifecycle.py
-src/zcore/apps/dynamic_models/workspace/utils.py
 src/zcore/apps/dynamic_models/workspace/wtree.py
 src/zcore/apps/object_store/__init__.py
 src/zcore/apps/object_store/admin.py
 src/zcore/apps/object_store/apps.py
 src/zcore/apps/object_store/models.py
 src/zcore/apps/object_store/tests.py
 src/zcore/apps/object_store/views.py
@@ -178,24 +174,21 @@
 src/zcore/config/urls_public.py
 src/zcore/config/urls_tenants.py
 src/zcore/config/settings/__init__.py
 src/zcore/config/settings/base.py
 src/zcore/core/__init__.py
 src/zcore/core/common_utils.py
 src/zcore/core/custom_pluginbase.py
-src/zcore/core/exception_handlers.py
 src/zcore/core/internal_requests.py
 src/zcore/core/model_mixins.py
 src/zcore/core/package_utils.py
 src/zcore/core/permissions.py
-src/zcore/core/profile_mixin.py
 src/zcore/core/storage_utils.py
 src/zcore/core/tasks.py
 src/zcore/core/template_loader.py
-src/zcore/core/tenant_utils.py
 src/zcore/core/utils.py
 src/zcore/core/api/__init__.py
 src/zcore/core/api/base.py
 src/zcore/core/api/utils.py
 src/zcore/core/generic_views/__init__.py
 src/zcore/core/generic_views/base.py
 src/zcore/middleware/__init__.py
```

### Comparing `zcorepy-0.2.0a1/src/zcorepy.egg-info/requires.txt` & `zcorepy-0.2.0rc0/src/zcorepy.egg-info/requires.txt`

 * *Files identical despite different names*


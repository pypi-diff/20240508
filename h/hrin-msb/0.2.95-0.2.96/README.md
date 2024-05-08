# Comparing `tmp/hrin_msb-0.2.95.tar.gz` & `tmp/hrin_msb-0.2.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrin_msb-0.2.95.tar", max compression
+gzip compressed data, was "hrin_msb-0.2.96.tar", max compression
```

## Comparing `hrin_msb-0.2.95.tar` & `hrin_msb-0.2.96.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1510 2024-04-03 03:12:46.690806 hrin_msb-0.2.95/hrin_msb.py
--rw-r--r--   0        0        0     1092 2023-12-01 10:11:17.921598 hrin_msb-0.2.95/LICENSE
--rw-r--r--   0        0        0        0 2023-12-01 10:15:20.273536 hrin_msb-0.2.95/msb/__init__.py
--rw-r--r--   0        0        0      173 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/__init__.py
--rw-r--r--   0        0        0     2810 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/api_view.py
--rw-r--r--   0        0        0     5324 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/api_viewset.py
--rw-r--r--   0        0        0      945 2023-12-01 10:15:20.283701 hrin_msb-0.2.95/msb/apis/constants.py
--rw-r--r--   0        0        0      995 2023-12-01 10:15:20.291748 hrin_msb-0.2.95/msb/apis/errors.py
--rw-r--r--   0        0        0      576 2023-12-01 10:15:20.293791 hrin_msb-0.2.95/msb/apis/exceptions.py
--rw-r--r--   0        0        0     3834 2023-12-01 10:15:20.293791 hrin_msb-0.2.95/msb/apis/funcs.py
--rw-r--r--   0        0        0      262 2024-04-03 03:10:28.578136 hrin_msb-0.2.95/msb/auth/__init__.py
--rw-r--r--   0        0        0      769 2023-12-01 10:15:20.293791 hrin_msb-0.2.95/msb/auth/authenticators.py
--rw-r--r--   0        0        0     3491 2023-12-01 10:15:20.301895 hrin_msb-0.2.95/msb/auth/constants.py
--rw-r--r--   0        0        0     1838 2024-04-03 03:08:51.994576 hrin_msb-0.2.95/msb/auth/decorators.py
--rw-r--r--   0        0        0     2801 2023-12-01 10:15:20.301895 hrin_msb-0.2.95/msb/auth/defaults.py
--rw-r--r--   0        0        0      989 2023-12-01 10:15:20.301895 hrin_msb-0.2.95/msb/auth/exceptions.py
--rw-r--r--   0        0        0     4682 2024-04-03 03:06:34.009238 hrin_msb-0.2.95/msb/auth/permissions.py
--rw-r--r--   0        0        0     1188 2023-12-01 10:15:20.311939 hrin_msb-0.2.95/msb/auth/results.py
--rw-r--r--   0        0        0     2928 2023-12-01 10:15:20.313988 hrin_msb-0.2.95/msb/auth/serializers.py
--rw-r--r--   0        0        0     3523 2023-12-01 10:15:20.313988 hrin_msb-0.2.95/msb/auth/session.py
--rw-r--r--   0        0        0     1791 2023-12-01 10:15:20.313988 hrin_msb-0.2.95/msb/auth/token.py
--rw-r--r--   0        0        0     2996 2023-12-01 10:15:20.322135 hrin_msb-0.2.95/msb/auth/users.py
--rw-r--r--   0        0        0     2414 2023-12-01 10:15:20.322135 hrin_msb-0.2.95/msb/auth/validators.py
--rw-r--r--   0        0        0       28 2023-12-01 10:15:20.322135 hrin_msb-0.2.95/msb/cipher/__init__.py
--rw-r--r--   0        0        0       34 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/asymmetric_cipher.py
--rw-r--r--   0        0        0     2241 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/cipher.py
--rw-r--r--   0        0        0        0 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/constants.py
--rw-r--r--   0        0        0      160 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/exceptions.py
--rw-r--r--   0        0        0      714 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/cipher/symmetric_cipher.py
--rw-r--r--   0        0        0      295 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/dataclasses/__init__.py
--rw-r--r--   0        0        0     1760 2023-12-01 10:15:20.332148 hrin_msb-0.2.95/msb/dataclasses/_email.py
--rw-r--r--   0        0        0      928 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/_singleton.py
--rw-r--r--   0        0        0      759 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/_wrappers.py
--rw-r--r--   0        0        0     1840 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/notification.py
--rw-r--r--   0        0        0     4546 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/dataclasses/search_parameter.py
--rw-r--r--   0        0        0      354 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/datetime/__init__.py
--rw-r--r--   0        0        0      370 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/datetime/constants.py
--rw-r--r--   0        0        0     2419 2023-12-01 10:15:20.347794 hrin_msb-0.2.95/msb/datetime/wrappers.py
--rw-r--r--   0        0        0      107 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/__init__.py
--rw-r--r--   0        0        0     1231 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/config_model.py
--rw-r--r--   0        0        0      672 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/constants.py
--rw-r--r--   0        0        0     2558 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/logging_models.py
--rw-r--r--   0        0        0      767 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/metafields.py
--rw-r--r--   0        0        0     1294 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/model_fields.py
--rw-r--r--   0        0        0      506 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/models.py
--rw-r--r--   0        0        0     5219 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/msb_model.py
--rw-r--r--   0        0        0     1096 2023-12-01 10:15:20.363417 hrin_msb-0.2.95/msb/db/msb_model_manager.py
--rw-r--r--   0        0        0     3747 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/db/routers.py
--rw-r--r--   0        0        0      198 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/__init__.py
--rw-r--r--   0        0        0      752 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/constants.py
--rw-r--r--   0        0        0     1928 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/dataclasses.py
--rw-r--r--   0        0        0     3426 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/django.py
--rw-r--r--   0        0        0     2256 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/funcs.py
--rw-r--r--   0        0        0     4392 2023-12-01 10:15:20.379040 hrin_msb-0.2.95/msb/devtools/tasks.py
--rw-r--r--   0        0        0      162 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/__init__.py
--rw-r--r--   0        0        0     3006 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/config.py
--rw-r--r--   0        0        0     6422 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/constants.py
--rw-r--r--   0        0        0     1444 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/core.py
--rw-r--r--   0        0        0      382 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/exceptions.py
--rw-r--r--   0        0        0     5541 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/loging.py
--rw-r--r--   0        0        0     8624 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/env/settings.py
--rw-r--r--   0        0        0      117 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/exceptions/__init__.py
--rw-r--r--   0        0        0     1271 2023-12-01 10:15:20.394667 hrin_msb-0.2.95/msb/exceptions/_exception.py
--rw-r--r--   0        0        0      442 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/exceptions/handlers.py
--rw-r--r--   0        0        0      132 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/__init__.py
--rw-r--r--   0        0        0      951 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/core.py
--rw-r--r--   0        0        0     1038 2023-12-15 05:16:26.702070 hrin_msb-0.2.95/msb/files/csv.py
--rw-r--r--   0        0        0      181 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/dataclasses.py
--rw-r--r--   0        0        0     1407 2023-12-15 05:17:09.529420 hrin_msb-0.2.95/msb/files/docx.py
--rw-r--r--   0        0        0      604 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/exceptions.py
--rw-r--r--   0        0        0      329 2023-12-01 10:15:20.410291 hrin_msb-0.2.95/msb/files/factory.py
--rw-r--r--   0        0        0      198 2023-12-01 10:15:20.425914 hrin_msb-0.2.95/msb/files/messages.py
--rw-r--r--   0        0        0     1074 2023-12-15 05:17:09.516269 hrin_msb-0.2.95/msb/files/pdf.py
--rw-r--r--   0        0        0      515 2023-12-01 10:15:20.425914 hrin_msb-0.2.95/msb/http/__init__.py
--rw-r--r--   0        0        0     6420 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/client.py
--rw-r--r--   0        0        0      692 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/constants.py
--rw-r--r--   0        0        0     6835 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/dataclasses.py
--rw-r--r--   0        0        0      988 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/exceptions.py
--rw-r--r--   0        0        0     1491 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/request.py
--rw-r--r--   0        0        0     3390 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/response.py
--rw-r--r--   0        0        0     1008 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/utils.py
--rw-r--r--   0        0        0     4809 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/http/wrappers.py
--rw-r--r--   0        0        0      169 2023-12-01 10:15:20.432429 hrin_msb-0.2.95/msb/logging/__init__.py
--rw-r--r--   0        0        0     5281 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/logging/config.py
--rw-r--r--   0        0        0     1440 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/logging/constants.py
--rw-r--r--   0        0        0      593 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/logging/handlers.py
--rw-r--r--   0        0        0      229 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/__init__.py
--rw-r--r--   0        0        0     5338 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/api_service.py
--rw-r--r--   0        0        0     1784 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/exceptions.py
--rw-r--r--   0        0        0      183 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/isr_service.py
--rw-r--r--   0        0        0      702 2023-12-01 10:15:20.448072 hrin_msb-0.2.95/msb/services/msb_service.py
--rw-r--r--   0        0        0     1658 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/services/notification_service.py
--rw-r--r--   0        0        0     1996 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/services/queue_service.py
--rw-r--r--   0        0        0       25 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/__init__.py
--rw-r--r--   0        0        0     4639 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/api_test.py
--rw-r--r--   0        0        0      450 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/constants.py
--rw-r--r--   0        0        0     1983 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/core.py
--rw-r--r--   0        0        0     3665 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/testdata.py
--rw-r--r--   0        0        0      476 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/testing/unit_test.py
--rw-r--r--   0        0        0        0 2023-12-01 10:15:20.463695 hrin_msb-0.2.95/msb/utils/__init__.py
--rw-r--r--   0        0        0      714 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/__init__.py
--rw-r--r--   0        0        0     2198 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/decorators.py
--rw-r--r--   0        0        0     1065 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/exceptions.py
--rw-r--r--   0        0        0     1059 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/rules.py
--rw-r--r--   0        0        0     6480 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/schema.py
--rw-r--r--   0        0        0     2931 2023-12-01 10:15:20.479325 hrin_msb-0.2.95/msb/validation/utils.py
--rw-r--r--   0        0        0      933 2024-04-03 03:23:04.155125 hrin_msb-0.2.95/pyproject.toml
--rw-r--r--   0        0        0     8779 2024-04-03 03:23:04.147120 hrin_msb-0.2.95/README.md
--rw-r--r--   0        0        0     9653 1970-01-01 00:00:00.000000 hrin_msb-0.2.95/PKG-INFO
+-rw-r--r--   0        0        0     1510 2024-04-03 03:12:46.690806 hrin_msb-0.2.96/hrin_msb.py
+-rw-r--r--   0        0        0     1092 2023-12-01 10:11:17.921598 hrin_msb-0.2.96/LICENSE
+-rw-r--r--   0        0        0        0 2023-12-01 10:15:20.273536 hrin_msb-0.2.96/msb/__init__.py
+-rw-r--r--   0        0        0      173 2023-12-01 10:15:20.283701 hrin_msb-0.2.96/msb/apis/__init__.py
+-rw-r--r--   0        0        0     2810 2023-12-01 10:15:20.283701 hrin_msb-0.2.96/msb/apis/api_view.py
+-rw-r--r--   0        0        0     5324 2023-12-01 10:15:20.283701 hrin_msb-0.2.96/msb/apis/api_viewset.py
+-rw-r--r--   0        0        0      945 2023-12-01 10:15:20.283701 hrin_msb-0.2.96/msb/apis/constants.py
+-rw-r--r--   0        0        0      995 2023-12-01 10:15:20.291748 hrin_msb-0.2.96/msb/apis/errors.py
+-rw-r--r--   0        0        0      576 2023-12-01 10:15:20.293791 hrin_msb-0.2.96/msb/apis/exceptions.py
+-rw-r--r--   0        0        0     3834 2023-12-01 10:15:20.293791 hrin_msb-0.2.96/msb/apis/funcs.py
+-rw-r--r--   0        0        0      262 2024-04-03 03:10:28.578136 hrin_msb-0.2.96/msb/auth/__init__.py
+-rw-r--r--   0        0        0      769 2023-12-01 10:15:20.293791 hrin_msb-0.2.96/msb/auth/authenticators.py
+-rw-r--r--   0        0        0     3491 2023-12-01 10:15:20.301895 hrin_msb-0.2.96/msb/auth/constants.py
+-rw-r--r--   0        0        0     1954 2024-05-08 05:41:14.713048 hrin_msb-0.2.96/msb/auth/decorators.py
+-rw-r--r--   0        0        0     2801 2023-12-01 10:15:20.301895 hrin_msb-0.2.96/msb/auth/defaults.py
+-rw-r--r--   0        0        0      989 2023-12-01 10:15:20.301895 hrin_msb-0.2.96/msb/auth/exceptions.py
+-rw-r--r--   0        0        0     4682 2024-04-03 03:06:34.009238 hrin_msb-0.2.96/msb/auth/permissions.py
+-rw-r--r--   0        0        0     1188 2023-12-01 10:15:20.311939 hrin_msb-0.2.96/msb/auth/results.py
+-rw-r--r--   0        0        0     2928 2023-12-01 10:15:20.313988 hrin_msb-0.2.96/msb/auth/serializers.py
+-rw-r--r--   0        0        0     3523 2023-12-01 10:15:20.313988 hrin_msb-0.2.96/msb/auth/session.py
+-rw-r--r--   0        0        0     1791 2023-12-01 10:15:20.313988 hrin_msb-0.2.96/msb/auth/token.py
+-rw-r--r--   0        0        0     2996 2023-12-01 10:15:20.322135 hrin_msb-0.2.96/msb/auth/users.py
+-rw-r--r--   0        0        0     2414 2023-12-01 10:15:20.322135 hrin_msb-0.2.96/msb/auth/validators.py
+-rw-r--r--   0        0        0       28 2023-12-01 10:15:20.322135 hrin_msb-0.2.96/msb/cipher/__init__.py
+-rw-r--r--   0        0        0       34 2023-12-01 10:15:20.332148 hrin_msb-0.2.96/msb/cipher/asymmetric_cipher.py
+-rw-r--r--   0        0        0     2241 2023-12-01 10:15:20.332148 hrin_msb-0.2.96/msb/cipher/cipher.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:15:20.332148 hrin_msb-0.2.96/msb/cipher/constants.py
+-rw-r--r--   0        0        0      160 2023-12-01 10:15:20.332148 hrin_msb-0.2.96/msb/cipher/exceptions.py
+-rw-r--r--   0        0        0      714 2023-12-01 10:15:20.332148 hrin_msb-0.2.96/msb/cipher/symmetric_cipher.py
+-rw-r--r--   0        0        0      295 2023-12-01 10:15:20.332148 hrin_msb-0.2.96/msb/dataclasses/__init__.py
+-rw-r--r--   0        0        0     1760 2023-12-01 10:15:20.332148 hrin_msb-0.2.96/msb/dataclasses/_email.py
+-rw-r--r--   0        0        0      928 2023-12-01 10:15:20.347794 hrin_msb-0.2.96/msb/dataclasses/_singleton.py
+-rw-r--r--   0        0        0      759 2023-12-01 10:15:20.347794 hrin_msb-0.2.96/msb/dataclasses/_wrappers.py
+-rw-r--r--   0        0        0     1840 2023-12-01 10:15:20.347794 hrin_msb-0.2.96/msb/dataclasses/notification.py
+-rw-r--r--   0        0        0     4546 2023-12-01 10:15:20.347794 hrin_msb-0.2.96/msb/dataclasses/search_parameter.py
+-rw-r--r--   0        0        0      354 2023-12-01 10:15:20.347794 hrin_msb-0.2.96/msb/datetime/__init__.py
+-rw-r--r--   0        0        0      370 2023-12-01 10:15:20.347794 hrin_msb-0.2.96/msb/datetime/constants.py
+-rw-r--r--   0        0        0     2419 2023-12-01 10:15:20.347794 hrin_msb-0.2.96/msb/datetime/wrappers.py
+-rw-r--r--   0        0        0      107 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/__init__.py
+-rw-r--r--   0        0        0     1231 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/config_model.py
+-rw-r--r--   0        0        0      672 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/constants.py
+-rw-r--r--   0        0        0     2558 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/logging_models.py
+-rw-r--r--   0        0        0      767 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/metafields.py
+-rw-r--r--   0        0        0     1294 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/model_fields.py
+-rw-r--r--   0        0        0      506 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/models.py
+-rw-r--r--   0        0        0     5219 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/msb_model.py
+-rw-r--r--   0        0        0     1096 2023-12-01 10:15:20.363417 hrin_msb-0.2.96/msb/db/msb_model_manager.py
+-rw-r--r--   0        0        0     3747 2023-12-01 10:15:20.379040 hrin_msb-0.2.96/msb/db/routers.py
+-rw-r--r--   0        0        0      198 2023-12-01 10:15:20.379040 hrin_msb-0.2.96/msb/devtools/__init__.py
+-rw-r--r--   0        0        0      752 2023-12-01 10:15:20.379040 hrin_msb-0.2.96/msb/devtools/constants.py
+-rw-r--r--   0        0        0     1928 2023-12-01 10:15:20.379040 hrin_msb-0.2.96/msb/devtools/dataclasses.py
+-rw-r--r--   0        0        0     3426 2023-12-01 10:15:20.379040 hrin_msb-0.2.96/msb/devtools/django.py
+-rw-r--r--   0        0        0     2256 2023-12-01 10:15:20.379040 hrin_msb-0.2.96/msb/devtools/funcs.py
+-rw-r--r--   0        0        0     4392 2023-12-01 10:15:20.379040 hrin_msb-0.2.96/msb/devtools/tasks.py
+-rw-r--r--   0        0        0      162 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/env/__init__.py
+-rw-r--r--   0        0        0     3006 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/env/config.py
+-rw-r--r--   0        0        0     6422 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/env/constants.py
+-rw-r--r--   0        0        0     1444 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/env/core.py
+-rw-r--r--   0        0        0      382 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/env/exceptions.py
+-rw-r--r--   0        0        0     5541 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/env/loging.py
+-rw-r--r--   0        0        0     8624 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/env/settings.py
+-rw-r--r--   0        0        0      117 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/exceptions/__init__.py
+-rw-r--r--   0        0        0     1271 2023-12-01 10:15:20.394667 hrin_msb-0.2.96/msb/exceptions/_exception.py
+-rw-r--r--   0        0        0      442 2023-12-01 10:15:20.410291 hrin_msb-0.2.96/msb/exceptions/handlers.py
+-rw-r--r--   0        0        0      132 2023-12-01 10:15:20.410291 hrin_msb-0.2.96/msb/files/__init__.py
+-rw-r--r--   0        0        0      951 2023-12-01 10:15:20.410291 hrin_msb-0.2.96/msb/files/core.py
+-rw-r--r--   0        0        0     1038 2023-12-15 05:16:26.702070 hrin_msb-0.2.96/msb/files/csv.py
+-rw-r--r--   0        0        0      181 2023-12-01 10:15:20.410291 hrin_msb-0.2.96/msb/files/dataclasses.py
+-rw-r--r--   0        0        0     1407 2023-12-15 05:17:09.529420 hrin_msb-0.2.96/msb/files/docx.py
+-rw-r--r--   0        0        0      604 2023-12-01 10:15:20.410291 hrin_msb-0.2.96/msb/files/exceptions.py
+-rw-r--r--   0        0        0      329 2023-12-01 10:15:20.410291 hrin_msb-0.2.96/msb/files/factory.py
+-rw-r--r--   0        0        0      198 2023-12-01 10:15:20.425914 hrin_msb-0.2.96/msb/files/messages.py
+-rw-r--r--   0        0        0     1074 2023-12-15 05:17:09.516269 hrin_msb-0.2.96/msb/files/pdf.py
+-rw-r--r--   0        0        0      515 2023-12-01 10:15:20.425914 hrin_msb-0.2.96/msb/http/__init__.py
+-rw-r--r--   0        0        0     6420 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/client.py
+-rw-r--r--   0        0        0      692 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/constants.py
+-rw-r--r--   0        0        0     6835 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/dataclasses.py
+-rw-r--r--   0        0        0      988 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/exceptions.py
+-rw-r--r--   0        0        0     1491 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/request.py
+-rw-r--r--   0        0        0     3390 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/response.py
+-rw-r--r--   0        0        0     1008 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/utils.py
+-rw-r--r--   0        0        0     4809 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/http/wrappers.py
+-rw-r--r--   0        0        0      169 2023-12-01 10:15:20.432429 hrin_msb-0.2.96/msb/logging/__init__.py
+-rw-r--r--   0        0        0     5281 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/logging/config.py
+-rw-r--r--   0        0        0     1440 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/logging/constants.py
+-rw-r--r--   0        0        0      593 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/logging/handlers.py
+-rw-r--r--   0        0        0      229 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/services/__init__.py
+-rw-r--r--   0        0        0     5338 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/services/api_service.py
+-rw-r--r--   0        0        0     1784 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/services/exceptions.py
+-rw-r--r--   0        0        0      183 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/services/isr_service.py
+-rw-r--r--   0        0        0      702 2023-12-01 10:15:20.448072 hrin_msb-0.2.96/msb/services/msb_service.py
+-rw-r--r--   0        0        0     1658 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/services/notification_service.py
+-rw-r--r--   0        0        0     1996 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/services/queue_service.py
+-rw-r--r--   0        0        0       25 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/testing/__init__.py
+-rw-r--r--   0        0        0     4639 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/testing/api_test.py
+-rw-r--r--   0        0        0      450 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/testing/constants.py
+-rw-r--r--   0        0        0     1983 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/testing/core.py
+-rw-r--r--   0        0        0     3665 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/testing/testdata.py
+-rw-r--r--   0        0        0      476 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/testing/unit_test.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:15:20.463695 hrin_msb-0.2.96/msb/utils/__init__.py
+-rw-r--r--   0        0        0      714 2023-12-01 10:15:20.479325 hrin_msb-0.2.96/msb/validation/__init__.py
+-rw-r--r--   0        0        0     2198 2023-12-01 10:15:20.479325 hrin_msb-0.2.96/msb/validation/decorators.py
+-rw-r--r--   0        0        0     1065 2023-12-01 10:15:20.479325 hrin_msb-0.2.96/msb/validation/exceptions.py
+-rw-r--r--   0        0        0     1059 2023-12-01 10:15:20.479325 hrin_msb-0.2.96/msb/validation/rules.py
+-rw-r--r--   0        0        0     6480 2023-12-01 10:15:20.479325 hrin_msb-0.2.96/msb/validation/schema.py
+-rw-r--r--   0        0        0     2931 2023-12-01 10:15:20.479325 hrin_msb-0.2.96/msb/validation/utils.py
+-rw-r--r--   0        0        0      933 2024-05-08 05:42:38.788926 hrin_msb-0.2.96/pyproject.toml
+-rw-r--r--   0        0        0     8888 2024-05-08 05:42:17.557093 hrin_msb-0.2.96/README.md
+-rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 hrin_msb-0.2.96/PKG-INFO
```

### Comparing `hrin_msb-0.2.95/hrin_msb.py` & `hrin_msb-0.2.96/hrin_msb.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/LICENSE` & `hrin_msb-0.2.96/LICENSE`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/apis/api_view.py` & `hrin_msb-0.2.96/msb/apis/api_view.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/apis/api_viewset.py` & `hrin_msb-0.2.96/msb/apis/api_viewset.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/apis/constants.py` & `hrin_msb-0.2.96/msb/apis/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/apis/errors.py` & `hrin_msb-0.2.96/msb/apis/errors.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/apis/exceptions.py` & `hrin_msb-0.2.96/msb/apis/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/apis/funcs.py` & `hrin_msb-0.2.96/msb/apis/funcs.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/authenticators.py` & `hrin_msb-0.2.96/msb/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/constants.py` & `hrin_msb-0.2.96/msb/auth/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/decorators.py` & `hrin_msb-0.2.96/msb/auth/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,19 @@
 		@wraps(func)
 		def wrapper_function(cls, request, *args, **kwargs):
 			"""
 			This function takes the IPs allowed.
 			It validates all the IP in the request header and if it is not in the allowed IPs,
 			it will raise an exception.
 			"""
-			if request._auth.get('ip') not in allowed_ips:
+			client_ip = request.META.get('HTTP_X_FORWARDED_FOR')
+			if not client_ip:
+				client_ip = request.META.get('REMOTE_ADDR')
+
+			if client_ip not in allowed_ips:
 				raise MsbAuthExceptions.UnauthorizedAccess
 
 			return func(cls, request, *args, **kwargs)
 
 		return wrapper_function
 
 	return decorator_function
```

### Comparing `hrin_msb-0.2.95/msb/auth/defaults.py` & `hrin_msb-0.2.96/msb/auth/defaults.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/exceptions.py` & `hrin_msb-0.2.96/msb/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/permissions.py` & `hrin_msb-0.2.96/msb/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/results.py` & `hrin_msb-0.2.96/msb/auth/results.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/serializers.py` & `hrin_msb-0.2.96/msb/auth/serializers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/session.py` & `hrin_msb-0.2.96/msb/auth/session.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/token.py` & `hrin_msb-0.2.96/msb/auth/token.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/users.py` & `hrin_msb-0.2.96/msb/auth/users.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/auth/validators.py` & `hrin_msb-0.2.96/msb/auth/validators.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/cipher/cipher.py` & `hrin_msb-0.2.96/msb/cipher/cipher.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/cipher/symmetric_cipher.py` & `hrin_msb-0.2.96/msb/cipher/symmetric_cipher.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/dataclasses/_email.py` & `hrin_msb-0.2.96/msb/dataclasses/_email.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/dataclasses/_singleton.py` & `hrin_msb-0.2.96/msb/dataclasses/_singleton.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/dataclasses/_wrappers.py` & `hrin_msb-0.2.96/msb/dataclasses/_wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/dataclasses/notification.py` & `hrin_msb-0.2.96/msb/dataclasses/notification.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/dataclasses/search_parameter.py` & `hrin_msb-0.2.96/msb/dataclasses/search_parameter.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/datetime/wrappers.py` & `hrin_msb-0.2.96/msb/datetime/wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/config_model.py` & `hrin_msb-0.2.96/msb/db/config_model.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/constants.py` & `hrin_msb-0.2.96/msb/db/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/logging_models.py` & `hrin_msb-0.2.96/msb/db/logging_models.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/metafields.py` & `hrin_msb-0.2.96/msb/db/metafields.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/model_fields.py` & `hrin_msb-0.2.96/msb/db/model_fields.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/msb_model.py` & `hrin_msb-0.2.96/msb/db/msb_model.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/msb_model_manager.py` & `hrin_msb-0.2.96/msb/db/msb_model_manager.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/db/routers.py` & `hrin_msb-0.2.96/msb/db/routers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/devtools/constants.py` & `hrin_msb-0.2.96/msb/devtools/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/devtools/dataclasses.py` & `hrin_msb-0.2.96/msb/devtools/dataclasses.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/devtools/django.py` & `hrin_msb-0.2.96/msb/devtools/django.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/devtools/funcs.py` & `hrin_msb-0.2.96/msb/devtools/funcs.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/devtools/tasks.py` & `hrin_msb-0.2.96/msb/devtools/tasks.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/env/config.py` & `hrin_msb-0.2.96/msb/env/config.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/env/constants.py` & `hrin_msb-0.2.96/msb/env/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/env/core.py` & `hrin_msb-0.2.96/msb/env/core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/env/loging.py` & `hrin_msb-0.2.96/msb/env/loging.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/env/settings.py` & `hrin_msb-0.2.96/msb/env/settings.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/exceptions/_exception.py` & `hrin_msb-0.2.96/msb/exceptions/_exception.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/files/core.py` & `hrin_msb-0.2.96/msb/files/core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/files/csv.py` & `hrin_msb-0.2.96/msb/files/csv.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/files/docx.py` & `hrin_msb-0.2.96/msb/files/docx.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/files/exceptions.py` & `hrin_msb-0.2.96/msb/files/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/files/pdf.py` & `hrin_msb-0.2.96/msb/files/pdf.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/__init__.py` & `hrin_msb-0.2.96/msb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/client.py` & `hrin_msb-0.2.96/msb/http/client.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/constants.py` & `hrin_msb-0.2.96/msb/http/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/dataclasses.py` & `hrin_msb-0.2.96/msb/http/dataclasses.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/exceptions.py` & `hrin_msb-0.2.96/msb/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/request.py` & `hrin_msb-0.2.96/msb/http/request.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/response.py` & `hrin_msb-0.2.96/msb/http/response.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/utils.py` & `hrin_msb-0.2.96/msb/http/utils.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/http/wrappers.py` & `hrin_msb-0.2.96/msb/http/wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/logging/config.py` & `hrin_msb-0.2.96/msb/logging/config.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/logging/constants.py` & `hrin_msb-0.2.96/msb/logging/constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/logging/handlers.py` & `hrin_msb-0.2.96/msb/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/services/api_service.py` & `hrin_msb-0.2.96/msb/services/api_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/services/exceptions.py` & `hrin_msb-0.2.96/msb/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/services/msb_service.py` & `hrin_msb-0.2.96/msb/services/msb_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/services/notification_service.py` & `hrin_msb-0.2.96/msb/services/notification_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/services/queue_service.py` & `hrin_msb-0.2.96/msb/services/queue_service.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/testing/api_test.py` & `hrin_msb-0.2.96/msb/testing/api_test.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/testing/core.py` & `hrin_msb-0.2.96/msb/testing/core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/testing/testdata.py` & `hrin_msb-0.2.96/msb/testing/testdata.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/validation/__init__.py` & `hrin_msb-0.2.96/msb/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/validation/decorators.py` & `hrin_msb-0.2.96/msb/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/validation/exceptions.py` & `hrin_msb-0.2.96/msb/validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/validation/rules.py` & `hrin_msb-0.2.96/msb/validation/rules.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/validation/schema.py` & `hrin_msb-0.2.96/msb/validation/schema.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/msb/validation/utils.py` & `hrin_msb-0.2.96/msb/validation/utils.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.95/pyproject.toml` & `hrin_msb-0.2.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hrin-msb"
-version = "0.2.95"
+version = "0.2.96"
 description = ""
 authors = [
     "Prakash Mishra <prakash.mishra@intimetec.com>",
     "Mohit Verma<mohit.verma@intimetec.com>",
     "Prajwal S <prajwal.s@intimetec.com>",
     "Sathwik Somayaji S <sathwik.s.s@intimetec.com>",
 ]
```

### Comparing `hrin_msb-0.2.95/README.md` & `hrin_msb-0.2.96/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -250,7 +250,11 @@
 1. Fixed : UserRole.__init__() got an unexpected keyword argument 'access_type'
 2. Added: recover method in model
 3. Refactor : moved all constants to `msb_constants`
 
 ### -- Version 0.2.95
 
 1. Added: Added decorator `verify_ip` to restrict the CRON Jobs tasks
+
+### -- Version 0.2.96
+
+1. Modified: Modified decorator `verify_ip` to work for unauthenticated requests
```

### Comparing `hrin_msb-0.2.95/PKG-INFO` & `hrin_msb-0.2.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrin-msb
-Version: 0.2.95
+Version: 0.2.96
 Summary: 
 Author: Prakash Mishra
 Author-email: prakash.mishra@intimetec.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -280,7 +280,11 @@
 2. Added: recover method in model
 3. Refactor : moved all constants to `msb_constants`
 
 ### -- Version 0.2.95
 
 1. Added: Added decorator `verify_ip` to restrict the CRON Jobs tasks
 
+### -- Version 0.2.96
+
+1. Modified: Modified decorator `verify_ip` to work for unauthenticated requests
+
```


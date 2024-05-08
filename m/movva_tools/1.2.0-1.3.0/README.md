# Comparing `tmp/movva_tools-1.2.0.tar.gz` & `tmp/movva_tools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movva_tools-1.2.0.tar", max compression
+gzip compressed data, was "movva_tools-1.3.0.tar", max compression
```

## Comparing `movva_tools-1.2.0.tar` & `movva_tools-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       87 2023-09-28 10:29:10.291654 movva_tools-1.2.0/README.md
--rw-r--r--   0        0        0      175 2023-11-30 17:04:01.622621 movva_tools-1.2.0/movva_tools/__init__.py
--rw-r--r--   0        0        0      154 2023-09-28 10:29:10.291654 movva_tools-1.2.0/movva_tools/base_exception.py
--rw-r--r--   0        0        0     3303 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/constants.py
--rw-r--r--   0        0        0     2631 2023-09-28 15:15:46.604573 movva_tools-1.2.0/movva_tools/databases.py
--rw-r--r--   0        0        0      637 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/decorators.py
--rw-r--r--   0        0        0     1996 2023-11-16 13:16:58.036191 movva_tools-1.2.0/movva_tools/examples/copy_flow_example.py
--rw-r--r--   0        0        0     1676 2023-11-16 13:18:08.634409 movva_tools-1.2.0/movva_tools/examples/import_contacts_example.py
--rw-r--r--   0        0        0     1641 2023-10-13 15:28:13.270038 movva_tools-1.2.0/movva_tools/exceptions.py
--rw-r--r--   0        0        0     8910 2023-09-28 15:44:14.538563 movva_tools-1.2.0/movva_tools/import_contacts.py
--rw-r--r--   0        0        0       97 2023-11-16 13:15:48.286193 movva_tools-1.2.0/movva_tools/integrations/__init__.py
--rw-r--r--   0        0        0     2244 2024-05-07 19:01:49.033794 movva_tools-1.2.0/movva_tools/integrations/google_drive.py
--rw-r--r--   0        0        0    10101 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/integrations/google_integration.py
--rw-r--r--   0        0        0      848 2023-11-30 16:38:20.085932 movva_tools-1.2.0/movva_tools/models/__init__.py
--rw-r--r--   0        0        0      490 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/api_token_model.py
--rw-r--r--   0        0        0     2507 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/campaign_models.py
--rw-r--r--   0        0        0     2014 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/channel_models.py
--rw-r--r--   0        0        0     3363 2024-05-06 12:45:47.658291 movva_tools-1.2.0/movva_tools/models/contacts_models.py
--rw-r--r--   0        0        0     9630 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/flow_models.py
--rw-r--r--   0        0        0     1348 2023-11-30 17:53:45.673645 movva_tools-1.2.0/movva_tools/models/messages_models.py
--rw-r--r--   0        0        0     1369 2023-09-28 15:17:44.535564 movva_tools-1.2.0/movva_tools/models/organization_models.py
--rw-r--r--   0        0        0      638 2023-09-28 15:17:43.643571 movva_tools-1.2.0/movva_tools/models/user_models.py
--rw-r--r--   0        0        0       76 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/notifications/__init__.py
--rw-r--r--   0        0        0     5710 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/notifications/slack.py
--rw-r--r--   0        0        0     1362 2023-09-28 10:29:10.291654 movva_tools-1.2.0/movva_tools/parsers.py
--rw-r--r--   0        0        0      479 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/serializers/__init__.py
--rw-r--r--   0        0        0      205 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/serializers/base_serializer.py
--rw-r--r--   0        0        0     1340 2023-11-16 13:02:39.308774 movva_tools-1.2.0/movva_tools/serializers/campaign_event_serializer.py
--rw-r--r--   0        0        0      469 2023-11-16 13:02:39.308774 movva_tools-1.2.0/movva_tools/serializers/campaign_serializer.py
--rw-r--r--   0        0        0      427 2023-11-16 13:02:39.312774 movva_tools-1.2.0/movva_tools/serializers/contact_group_serializer.py
--rw-r--r--   0        0        0      432 2023-11-16 13:18:23.218068 movva_tools-1.2.0/movva_tools/serializers/flow_revision_serializer.py
--rw-r--r--   0        0        0      453 2023-11-16 13:18:24.762033 movva_tools-1.2.0/movva_tools/serializers/flow_serializer.py
--rw-r--r--   0        0        0      422 2023-11-16 13:02:39.308774 movva_tools-1.2.0/movva_tools/serializers/organization_serializer.py
--rw-r--r--   0        0        0      658 2023-11-30 17:04:20.189985 movva_tools-1.2.0/movva_tools/services/__init__.py
--rw-r--r--   0        0        0     1205 2024-05-06 12:19:06.870867 movva_tools-1.2.0/movva_tools/services/api_token_service.py
--rw-r--r--   0        0        0      920 2023-09-28 16:12:52.612769 movva_tools-1.2.0/movva_tools/services/base_service.py
--rw-r--r--   0        0        0     4644 2023-11-16 13:18:26.202000 movva_tools-1.2.0/movva_tools/services/campaign_service.py
--rw-r--r--   0        0        0     1573 2023-11-16 13:15:42.558369 movva_tools-1.2.0/movva_tools/services/channel_service.py
--rw-r--r--   0        0        0     4044 2024-05-06 14:18:16.752989 movva_tools-1.2.0/movva_tools/services/contacts_service.py
--rw-r--r--   0        0        0    23957 2023-11-30 16:39:12.101496 movva_tools-1.2.0/movva_tools/services/flow_service.py
--rw-r--r--   0        0        0     3007 2024-05-06 18:33:02.915329 movva_tools-1.2.0/movva_tools/services/messages_service.py
--rw-r--r--   0        0        0      986 2023-11-16 13:16:59.992139 movva_tools-1.2.0/movva_tools/services/organization_service.py
--rw-r--r--   0        0        0      739 2023-11-16 13:18:13.646291 movva_tools-1.2.0/movva_tools/services/user_service.py
--rw-r--r--   0        0        0     1818 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/utils.py
--rw-r--r--   0        0        0      982 2023-09-28 16:52:41.474439 movva_tools-1.2.0/movva_tools/validators.py
--rw-r--r--   0        0        0      919 2024-05-07 19:15:06.058737 movva_tools-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 movva_tools-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-09-28 10:29:10.291654 movva_tools-1.3.0/README.md
+-rw-r--r--   0        0        0      175 2023-11-30 17:04:01.622621 movva_tools-1.3.0/movva_tools/__init__.py
+-rw-r--r--   0        0        0      154 2023-09-28 10:29:10.291654 movva_tools-1.3.0/movva_tools/base_exception.py
+-rw-r--r--   0        0        0     3303 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/constants.py
+-rw-r--r--   0        0        0     3295 2024-05-07 22:07:52.023693 movva_tools-1.3.0/movva_tools/databases.py
+-rw-r--r--   0        0        0      637 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/decorators.py
+-rw-r--r--   0        0        0     1996 2023-11-16 13:16:58.036191 movva_tools-1.3.0/movva_tools/examples/copy_flow_example.py
+-rw-r--r--   0        0        0     1676 2023-11-16 13:18:08.634409 movva_tools-1.3.0/movva_tools/examples/import_contacts_example.py
+-rw-r--r--   0        0        0     1641 2023-10-13 15:28:13.270038 movva_tools-1.3.0/movva_tools/exceptions.py
+-rw-r--r--   0        0        0     8910 2023-09-28 15:44:14.538563 movva_tools-1.3.0/movva_tools/import_contacts.py
+-rw-r--r--   0        0        0       97 2023-11-16 13:15:48.286193 movva_tools-1.3.0/movva_tools/integrations/__init__.py
+-rw-r--r--   0        0        0     2436 2024-05-08 16:23:48.013011 movva_tools-1.3.0/movva_tools/integrations/google_drive.py
+-rw-r--r--   0        0        0    10101 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/integrations/google_integration.py
+-rw-r--r--   0        0        0      848 2023-11-30 16:38:20.085932 movva_tools-1.3.0/movva_tools/models/__init__.py
+-rw-r--r--   0        0        0      490 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/models/api_token_model.py
+-rw-r--r--   0        0        0     2507 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/models/campaign_models.py
+-rw-r--r--   0        0        0     2014 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/models/channel_models.py
+-rw-r--r--   0        0        0     3363 2024-05-06 12:45:47.658291 movva_tools-1.3.0/movva_tools/models/contacts_models.py
+-rw-r--r--   0        0        0     9630 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/models/flow_models.py
+-rw-r--r--   0        0        0     1348 2023-11-30 17:53:45.673645 movva_tools-1.3.0/movva_tools/models/messages_models.py
+-rw-r--r--   0        0        0     1369 2023-09-28 15:17:44.535564 movva_tools-1.3.0/movva_tools/models/organization_models.py
+-rw-r--r--   0        0        0      638 2023-09-28 15:17:43.643571 movva_tools-1.3.0/movva_tools/models/user_models.py
+-rw-r--r--   0        0        0       76 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/notifications/__init__.py
+-rw-r--r--   0        0        0     5710 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/notifications/slack.py
+-rw-r--r--   0        0        0     1362 2023-09-28 10:29:10.291654 movva_tools-1.3.0/movva_tools/parsers.py
+-rw-r--r--   0        0        0      479 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/serializers/__init__.py
+-rw-r--r--   0        0        0      205 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/serializers/base_serializer.py
+-rw-r--r--   0        0        0     1340 2023-11-16 13:02:39.308774 movva_tools-1.3.0/movva_tools/serializers/campaign_event_serializer.py
+-rw-r--r--   0        0        0      469 2023-11-16 13:02:39.308774 movva_tools-1.3.0/movva_tools/serializers/campaign_serializer.py
+-rw-r--r--   0        0        0      427 2023-11-16 13:02:39.312774 movva_tools-1.3.0/movva_tools/serializers/contact_group_serializer.py
+-rw-r--r--   0        0        0      432 2023-11-16 13:18:23.218068 movva_tools-1.3.0/movva_tools/serializers/flow_revision_serializer.py
+-rw-r--r--   0        0        0      453 2023-11-16 13:18:24.762033 movva_tools-1.3.0/movva_tools/serializers/flow_serializer.py
+-rw-r--r--   0        0        0      422 2023-11-16 13:02:39.308774 movva_tools-1.3.0/movva_tools/serializers/organization_serializer.py
+-rw-r--r--   0        0        0      658 2023-11-30 17:04:20.189985 movva_tools-1.3.0/movva_tools/services/__init__.py
+-rw-r--r--   0        0        0     1205 2024-05-06 12:19:06.870867 movva_tools-1.3.0/movva_tools/services/api_token_service.py
+-rw-r--r--   0        0        0     1455 2024-05-07 22:09:30.831153 movva_tools-1.3.0/movva_tools/services/base_service.py
+-rw-r--r--   0        0        0     4892 2024-05-07 22:13:43.989611 movva_tools-1.3.0/movva_tools/services/campaign_service.py
+-rw-r--r--   0        0        0     1822 2024-05-07 22:14:25.213343 movva_tools-1.3.0/movva_tools/services/channel_service.py
+-rw-r--r--   0        0        0     4541 2024-05-07 22:14:48.069193 movva_tools-1.3.0/movva_tools/services/contacts_service.py
+-rw-r--r--   0        0        0    24935 2024-05-07 22:15:42.308832 movva_tools-1.3.0/movva_tools/services/flow_service.py
+-rw-r--r--   0        0        0     3172 2024-05-07 22:18:40.151613 movva_tools-1.3.0/movva_tools/services/messages_service.py
+-rw-r--r--   0        0        0     1235 2024-05-07 22:16:46.020401 movva_tools-1.3.0/movva_tools/services/organization_service.py
+-rw-r--r--   0        0        0      974 2024-05-07 22:16:54.108346 movva_tools-1.3.0/movva_tools/services/user_service.py
+-rw-r--r--   0        0        0     1818 2023-11-16 12:54:55.447688 movva_tools-1.3.0/movva_tools/utils.py
+-rw-r--r--   0        0        0      982 2023-09-28 16:52:41.474439 movva_tools-1.3.0/movva_tools/validators.py
+-rw-r--r--   0        0        0      919 2024-05-08 16:25:03.440642 movva_tools-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 movva_tools-1.3.0/PKG-INFO
```

### Comparing `movva_tools-1.2.0/movva_tools/constants.py` & `movva_tools-1.3.0/movva_tools/constants.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/decorators.py` & `movva_tools-1.3.0/movva_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/examples/copy_flow_example.py` & `movva_tools-1.3.0/movva_tools/examples/copy_flow_example.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/examples/import_contacts_example.py` & `movva_tools-1.3.0/movva_tools/examples/import_contacts_example.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/exceptions.py` & `movva_tools-1.3.0/movva_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/import_contacts.py` & `movva_tools-1.3.0/movva_tools/import_contacts.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/integrations/google_drive.py` & `movva_tools-1.3.0/movva_tools/integrations/google_drive.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaIoBaseDownload
 import io
 import pandas as pd
 import logging
 
 
+logging.basicConfig(
+    level=logging.INFO,
+    format=f"%(levelname)-8s %(name)s: \n %(message)s"
+)
+logger = logging.getLogger(name='GoogleDriveLogger')
+logger.setLevel(level=logging.INFO)
+
+
 class GoogleDriveIntegration:
     def __init__(self, folder_id, mimeType, credentials) -> None:
         self.folder_id = folder_id
         self.mime_type = mimeType
         self.credentials = self._set_credentials(credentials)
         self.drive_service = self._set_drive_service()
 
         self._df = None
-        self._logger = logging
+        self._logger = logger
 
     def _set_credentials(self, credentials):
         # Configurar as credenciais de autenticação
         return Credentials.from_authorized_user_info(credentials)
 
     def _set_drive_service(self):
         return build('drive', 'v3', credentials=self.credentials)
```

### Comparing `movva_tools-1.2.0/movva_tools/integrations/google_integration.py` & `movva_tools-1.3.0/movva_tools/integrations/google_integration.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/__init__.py` & `movva_tools-1.3.0/movva_tools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/campaign_models.py` & `movva_tools-1.3.0/movva_tools/models/campaign_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/channel_models.py` & `movva_tools-1.3.0/movva_tools/models/channel_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/contacts_models.py` & `movva_tools-1.3.0/movva_tools/models/contacts_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/flow_models.py` & `movva_tools-1.3.0/movva_tools/models/flow_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/messages_models.py` & `movva_tools-1.3.0/movva_tools/models/messages_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/organization_models.py` & `movva_tools-1.3.0/movva_tools/models/organization_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/models/user_models.py` & `movva_tools-1.3.0/movva_tools/models/user_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/notifications/slack.py` & `movva_tools-1.3.0/movva_tools/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/parsers.py` & `movva_tools-1.3.0/movva_tools/parsers.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/serializers/campaign_event_serializer.py` & `movva_tools-1.3.0/movva_tools/serializers/campaign_event_serializer.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/services/__init__.py` & `movva_tools-1.3.0/movva_tools/services/__init__.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/services/api_token_service.py` & `movva_tools-1.3.0/movva_tools/services/api_token_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/services/campaign_service.py` & `movva_tools-1.3.0/movva_tools/services/campaign_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,26 @@
 
 from movva_tools.services.contacts_service import ContactService
 from movva_tools.services.base_service import BaseService
 
 
 class CampaingService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-
-        super().__init__(db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # services
         self.contact_service = ContactService(
             db_connection=self.db_connection
         )
 
         # model table entities
```

### Comparing `movva_tools-1.2.0/movva_tools/services/channel_service.py` & `movva_tools-1.3.0/movva_tools/services/channel_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,16 +7,26 @@
 
 from movva_tools.models.channel_models import RapidProChannel
 from movva_tools.models.organization_models import RapidProOrganization
 
 
 class ChannelService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-        super().__init__(db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # model table entities
         self.Channel = RapidProChannel
 
     def get_channel_by_name(self, name: str, org: RapidProOrganization):
         channel = self.db_connection.session.query(
             self.Channel
```

### Comparing `movva_tools-1.2.0/movva_tools/services/contacts_service.py` & `movva_tools-1.3.0/movva_tools/services/contacts_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,17 +6,26 @@
 from movva_tools.exceptions import ObjectDoesNotExistException
 from movva_tools.models.contacts_models import RapidProContactURN
 from sqlalchemy import or_
 
 
 class ContactService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-
-        super().__init__(db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # model table entities
         self.Contact = RapidProContacts
         self.ContactFields = RapidProContactFields
         self.ContactGroups = RapidProContactGroups
         self.ContactGroupsContacts = RapidProContactGroupsContacts
 
@@ -82,16 +91,26 @@
             raise ObjectDoesNotExistException(
                 dababase_object=self.ContactFields
             )
 
 
 class ContactURNService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-        super().__init__(db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         self.ContactURN = RapidProContactURN
 
     def get_contact_urn_by_contact_id(self, contact_id):
 
         contact_urn = self.db_connection.session.query(
             self.ContactURN
```

### Comparing `movva_tools-1.2.0/movva_tools/services/flow_service.py` & `movva_tools-1.3.0/movva_tools/services/flow_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,17 +41,26 @@
 from movva_tools.utils import break_list_into_groups, datetime_string_parser
 from movva_tools.validators import FlowNameValidator
 from movva_tools.integrations.google_integration import FlowGoogleSheets
 
 
 class FlowService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-
-        super().__init__(db_connection=db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # model table entities
         self.flow = RapidProFlows
         self.flow_revision = RapidProFlowsRevision
         self.org = RapidProOrganization
 
         # services
@@ -180,17 +189,26 @@
             org=org,
             user=user,
             flow_name=flow_name
         )
 
 
 class FlowLabelService(BaseService):
-    def __init__(self, db_connection=None) -> None:
-
-        super().__init__(db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # model table entities
         self.Flow = RapidProFlows
         self.Organization = RapidProOrganization
         self.FlowLabel = RapidProFlowLabel
         self.FlowsFlowLabels = RapidProFlowsFlowLabels
 
@@ -250,17 +268,26 @@
 
     def create(self, name: str, org: RapidProOrganization, flow: RapidProFlows):
         return self._create_flow_label(name, org, flow)
 
 
 class FlowDependenciesService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-
-        super().__init__(db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # model table entities
         self.FlowChannelDependencies = RapidProFlowChannelDependencies
 
         self.FlowGroupDependencies = RapidProFlowGroupDependencies
 
         self.FlowFieldDependencies = RapidProFlowFieldDependencies
@@ -297,17 +324,26 @@
         group: RapidProContactGroups, flowlabel: RapidProFlowLabel
     ):
         return self._set_flow_dependencies(flow, channel, group, flowlabel)
 
 
 class CopyFlowAndScheduleService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-
-        super().__init__(db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # spreadsheet reader to copy flow
         self.spreadsheet_reader = FlowGoogleSheets
 
         # model table entities
         self.flow_revision = RapidProFlowsRevision
```

### Comparing `movva_tools-1.2.0/movva_tools/services/messages_service.py` & `movva_tools-1.3.0/movva_tools/services/messages_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from movva_tools.exceptions import ObjectDoesNotExistException
 from movva_tools.models.messages_models import RapidProMessages
 from movva_tools.models.contacts_models import RapidProContacts, RapidProContactURN
 from movva_tools.services.base_service import BaseService
-from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
 
 
 class MessageService(BaseService):
-    def __init__(self, db_connection=None) -> None:
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
 
-        super().__init__(db_connection=db_connection)
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
         self.event_loop = None
 
         # model table entities
         self.Message = RapidProMessages
         self.Contact = RapidProContacts
         self.ContactURN = RapidProContactURN
```

### Comparing `movva_tools-1.2.0/movva_tools/services/user_service.py` & `movva_tools-1.3.0/movva_tools/services/user_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,26 @@
 from movva_tools.models.user_models import RapidProUser
 from movva_tools.exceptions import ObjectDoesNotExistException
 from movva_tools.services.base_service import BaseService
 
 
 class UserService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
-        super().__init__(db_connection=db_connection)
+    def __init__(
+        self,
+        _user=None, _host=None, _port=None, _db_name=None, _password=None,
+        db_connection=None
+    ) -> None:
+
+        super().__init__(
+            _user=_user, _password=_password,
+            _host=_host, _port=_port,
+            _db_name=_db_name,
+            db_connection=db_connection
+        )
 
         # model table entities
         self.user = RapidProUser
 
     def get_default_user(self):
 
         default_user = self.db_connection.session.query(self.user).filter_by(
```

### Comparing `movva_tools-1.2.0/movva_tools/utils.py` & `movva_tools-1.3.0/movva_tools/utils.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/movva_tools/validators.py` & `movva_tools-1.3.0/movva_tools/validators.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.2.0/pyproject.toml` & `movva_tools-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "movva_tools"
-version = "1.2.0"
+version = "1.3.0"
 description = "Package that contains integrations and tools to use in issues of Movva organization."
 authors = ["WillamesCampos <willwjccampos@gmail.com>"]
 readme = "README.md"
 packages = [{include = "movva_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `movva_tools-1.2.0/PKG-INFO` & `movva_tools-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movva_tools
-Version: 1.2.0
+Version: 1.3.0
 Summary: Package that contains integrations and tools to use in issues of Movva organization.
 Author: WillamesCampos
 Author-email: willwjccampos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

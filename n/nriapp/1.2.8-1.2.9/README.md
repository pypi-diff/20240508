# Comparing `tmp/nriapp-1.2.8.tar.gz` & `tmp/nriapp-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.2.8.tar", last modified: Sun Mar 24 23:02:56 2024, max compression
+gzip compressed data, was "nriapp-1.2.9.tar", last modified: Wed May  8 16:45:32 2024, max compression
```

## Comparing `nriapp-1.2.8.tar` & `nriapp-1.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 23:02:56.237599 nriapp-1.2.8/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.2.8/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      389 2024-03-24 23:02:56.237599 nriapp-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.2.8/README
--rw-rw-rw-   0        0        0      332 2023-09-06 14:51:48.000000 nriapp-1.2.8/requirements.txt
--rw-rw-rw-   0        0        0       86 2024-03-24 23:02:56.237599 nriapp-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1598 2024-03-24 22:57:04.000000 nriapp-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-24 23:02:56.128399 nriapp-1.2.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-24 23:02:56.221999 nriapp-1.2.8/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     4421 2023-11-15 07:16:10.000000 nriapp-1.2.8/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2024-03-24 23:02:56.221999 nriapp-1.2.8/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2024-03-24 23:02:56.221999 nriapp-1.2.8/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1605 2024-02-20 04:45:58.000000 nriapp-1.2.8/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    26801 2024-02-21 23:03:06.000000 nriapp-1.2.8/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    19597 2023-10-29 03:29:13.000000 nriapp-1.2.8/src/nriapp/core/mdr.py
--rw-rw-rw-   0        0        0    31779 2024-02-21 05:01:00.000000 nriapp-1.2.8/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   110624 2024-03-22 05:17:12.000000 nriapp-1.2.8/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      634 2023-08-22 13:57:02.000000 nriapp-1.2.8/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2024-03-24 23:02:56.237599 nriapp-1.2.8/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5914 2024-01-18 00:18:09.000000 nriapp-1.2.8/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     9299 2024-03-19 00:31:03.000000 nriapp-1.2.8/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     6788 2023-08-25 17:31:00.000000 nriapp-1.2.8/src/nriapp/helper/login_snyper.py
--rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1450 2024-03-24 04:15:07.000000 nriapp-1.2.8/src/nriapp/helper/requestheader.py
--rw-rw-rw-   0        0        0    15815 2023-04-19 13:47:32.000000 nriapp-1.2.8/src/nriapp/helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-24 23:02:56.221999 nriapp-1.2.8/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      389 2024-03-24 23:02:56.000000 nriapp-1.2.8/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1153 2024-03-24 23:02:56.000000 nriapp-1.2.8/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 23:02:56.000000 nriapp-1.2.8/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-24 23:02:56.000000 nriapp-1.2.8/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      159 2024-03-24 23:02:56.000000 nriapp-1.2.8/src/nriapp/nriapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-24 23:02:56.000000 nriapp-1.2.8/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    43291 2024-02-22 02:32:36.000000 nriapp-1.2.8/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:45:32.420060 nriapp-1.2.9/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      389 2024-05-08 16:45:32.420060 nriapp-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.2.9/README
+-rw-rw-rw-   0        0        0      332 2023-09-06 14:51:48.000000 nriapp-1.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-05-08 16:45:32.435660 nriapp-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1598 2024-05-08 16:44:19.000000 nriapp-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:45:32.201659 nriapp-1.2.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 16:45:32.342060 nriapp-1.2.9/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     4421 2023-11-15 07:16:10.000000 nriapp-1.2.9/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 16:45:32.342060 nriapp-1.2.9/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:45:32.404460 nriapp-1.2.9/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1605 2024-02-20 04:45:58.000000 nriapp-1.2.9/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    26801 2024-02-21 23:03:06.000000 nriapp-1.2.9/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    19597 2023-10-29 03:29:13.000000 nriapp-1.2.9/src/nriapp/core/mdr.py
+-rw-rw-rw-   0        0        0    34490 2024-05-07 20:56:44.000000 nriapp-1.2.9/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   110626 2024-04-11 23:47:58.000000 nriapp-1.2.9/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      634 2023-08-22 13:57:02.000000 nriapp-1.2.9/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:45:32.420060 nriapp-1.2.9/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5914 2024-01-18 00:18:09.000000 nriapp-1.2.9/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0    10739 2024-05-07 20:55:08.000000 nriapp-1.2.9/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     6788 2023-08-25 17:31:00.000000 nriapp-1.2.9/src/nriapp/helper/login_snyper.py
+-rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     2451 2024-05-07 11:37:14.000000 nriapp-1.2.9/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0    15815 2023-04-19 13:47:32.000000 nriapp-1.2.9/src/nriapp/helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:45:32.326460 nriapp-1.2.9/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      389 2024-05-08 16:45:31.000000 nriapp-1.2.9/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1153 2024-05-08 16:45:31.000000 nriapp-1.2.9/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 16:45:31.000000 nriapp-1.2.9/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-08 16:45:31.000000 nriapp-1.2.9/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      159 2024-05-08 16:45:31.000000 nriapp-1.2.9/src/nriapp/nriapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-08 16:45:31.000000 nriapp-1.2.9/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    43291 2024-02-22 02:32:36.000000 nriapp-1.2.9/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.2.8/LICENSE` & `nriapp-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/setup.py` & `nriapp-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.2.08',
+   version='1.2.09',
    description='This is an internal tool for querying MS 365 Defender using MSGraph and MS Sentinels API with NRI\n'
                'Added capability for MDR portal\n'
                'Changes: Fixed the impacted assets in new template.',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
```

### Comparing `nriapp-1.2.8/src/nriapp/changelog.txt` & `nriapp-1.2.9/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.2.9/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/core/dataexplorer.py` & `nriapp-1.2.9/src/nriapp/core/dataexplorer.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/core/mdr.py` & `nriapp-1.2.9/src/nriapp/core/mdr.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/core/msgraphapi.py` & `nriapp-1.2.9/src/nriapp/core/msgraphapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         self._session = requests.Session()
 #        self.auth_page = 'https://portal.azure.com/api/DelegationToken'
 #        self.auth_page = 'https://endpoint.microsoft.com/api/DelegationToken'  #October 4, 2023 old
         self.auth_page = 'https://intune.microsoft.com/api/DelegationToken' #October 4, 2023 new
 #        self.auth_page = 'https://portal.azure.com/api/DelegationToken?feature.cacheextensionapp=true&feature.internalgraphapiversion=true&feature.tokencaching=true'
         self.headers = kwargs.get('headers', {'content-type' : 'application/json'})
         self.cookies = kwargs.get('cookies', {})
+#        self.access_token = kwargs.get('token', {})
+#        self.delegation = kwargs.get('delegation', {})
 #        self.auth_folder = kwargs.get('output', "")
         self.body = kwargs.get('json', '')
 
         self.users_auth = ""
         self.iam_auth = ""
         self.devices_auth = ""
         self.email = email
@@ -103,38 +105,39 @@
                 continue
         return response            
 
     def get_aad_authorization(self):
         
         json_data = {
         'extensionName': 'Microsoft_AAD_UsersAndTenants',
+#        'extensionName': 'Microsoft_Intune',
         'resourceName': 'microsoft.graph',
         'tenant': TENANT_ID,
 #        'portalAuthorization': self._authorization['portalAuthorization'],
 #        'altPortalAuthorization': self._authorization['altPortalAuthorization']
         'portalAuthorization': self._portalAuthorization,
-        'altPortalAuthorization': self._portalAuthorization
+        'altPortalAuthorization': "" #self._portalAuthorization
 
         }
 
         response = self._session.post(self.auth_page, json=json_data, verify=False)
 
         for _ in range(5):
             if response.status_code == 440:
 #                raise Exception("Reset")
-                Login.Login().delete_session()
-                Login.Login(self.email).login()
+                login.Login().delete_session()
+                login.Login(self.email).login()
                 self.load_session()
                 response = self._session.post(self.auth_page, json=json_data, verify=False)                      #Need exception handling
                 if response.status_code == 200:
                     break
             elif response.status_code == 200:
                 break
 
-            elif response.status_code == 500:
+            elif response.status_code == 500 or response.status_code == 504:
                 message = json.loads(response.text)
                 dbgPrint.error(message["Message"])
                 sys.exit()
 
         bearer = json.loads(response.text)
         users_auth = bearer["value"]["authHeader"]
 
@@ -145,78 +148,138 @@
         json_data = {
         'extensionName': 'Microsoft_Intune_DeviceSettings',
         'resourceName': 'microsoft.graph',
         'tenant': TENANT_ID,
 #        'portalAuthorization': self._authorization['portalAuthorization'],
 #        'altPortalAuthorization': self._authorization['altPortalAuthorization']
         'portalAuthorization': self._portalAuthorization,
-        'altPortalAuthorization': self._portalAuthorization
+        'altPortalAuthorization': "" #self._portalAuthorization
         }
 
         response = self._session.post(self.auth_page, json=json_data, verify=False)
+
+        for _ in range(5):
+            if response.status_code == 440:
+#                raise Exception("Reset")
+                login.Login().delete_session()
+                login.Login(self.email).login()
+                self.load_session()
+                response = self._session.post(self.auth_page, json=json_data, verify=False)                      #Need exception handling
+                if response.status_code == 200:
+                    break
+            elif response.status_code == 200:
+                break
+
+            elif response.status_code == 500 or response.status_code == 504:
+                message = json.loads(response.text)
+                dbgPrint.error(message["Message"])
+                sys.exit()
+
         bearer = json.loads(response.text)
         intune_auth = bearer["value"]["authHeader"]
         return intune_auth
 
     def get_iam_authorization(self):
         json_data = {
         'extensionName': 'Microsoft_AAD_IAM',
         'resourceName': 'microsoft.graph',
         'tenant': TENANT_ID,
 #        'portalAuthorization': self._authorization['portalAuthorization'],
 #        'altPortalAuthorization': self._authorization['altPortalAuthorization']
         'portalAuthorization': self._portalAuthorization,
-        'altPortalAuthorization': self._portalAuthorization
+        'altPortalAuthorization': "" #self._portalAuthorization
         }
 
         response = self._session.post(self.auth_page, json=json_data, verify=False)
+
+        for _ in range(5):
+            if response.status_code == 440:
+#                raise Exception("Reset")
+                login.Login().delete_session()
+                login.Login(self.email).login()
+                self.load_session()
+                response = self._session.post(self.auth_page, json=json_data, verify=False)                      #Need exception handling
+                if response.status_code == 200:
+                    break
+            elif response.status_code == 200:
+                break
+
+            elif response.status_code == 500 or response.status_code == 504:
+                message = json.loads(response.text)
+                dbgPrint.error(message["Message"])
+                sys.exit()
+
         bearer = json.loads(response.text)
         iam_auth = bearer["value"]["authHeader"]
         return iam_auth
 
     def get_enrollment_authorization(self):
 
         json_data = {
         'extensionName': 'Microsoft_Intune_Enrollment',
         'resourceName': 'microsoft.graph',
         'tenant': TENANT_ID,
 #        'portalAuthorization': self._authorization['portalAuthorization'],
 #        'altPortalAuthorization': self._authorization['altPortalAuthorization']        
         'portalAuthorization': self._portalAuthorization,
-        'altPortalAuthorization': self._portalAuthorization
+        'altPortalAuthorization': ""
         }
 
         response = self.tryrequest(self.auth_page, json=json_data)
+
+        for _ in range(5):
+            if response.status_code == 440:
+#                raise Exception("Reset")
+                login.Login().delete_session()
+                login.Login(self.email).login()
+                self.load_session()
+                response = self._session.post(self.auth_page, json=json_data, verify=False)                      #Need exception handling
+                if response.status_code == 200:
+                    break
+            elif response.status_code == 200:
+                break
+
+            elif response.status_code == 500 or response.status_code == 504:
+                message = json.loads(response.text)
+                dbgPrint.error(message["Message"])
+                sys.exit()
+
         bearer = json.loads(response.text)
         enrollment_auth = bearer["value"]["authHeader"]
         return enrollment_auth
 
     def save_session(self):
 
         session_path = os.path.abspath(os.path.dirname(__file__)) + "\..\session"
         session_file = session_path + "\\msgraph.pkl"
 
         if not os.path.exists(session_path):
             os.makedirs(session_path)
         with open(session_file, 'wb') as f:
             pickle.dump(self.cookies, f)
             pickle.dump(self.body, f)
+#            pickle.dump(self.access_token,f)
+#            pickle.dump(self.delegation, f)
 
 
     def load_session(self):
 
         session_path = os.path.abspath(os.path.dirname(__file__)) + "\..\session"
         session_file = session_path + "\\msgraph.pkl"
 
         if os.path.exists(session_file):
             with open(session_file, 'rb') as f:
                 cookies = pickle.load(f)
                 json_data = pickle.load(f)
+#                access_token = pickle.load(f)
+#                delegation = pickle.load(f)
             self.cookies = cookies
             self.body = json_data
+#            self.access_token = access_token
+#            self.delegation = delegation
             self.__init__(self.email, cookies=cookies, json=json_data)
             self.users_auth = self.get_aad_authorization()
             self.devices_auth = self.get_intune_authorization()
             self.iam_auth = self.get_iam_authorization()
             self.intune_enrollment_auth = self.get_enrollment_authorization()
         else:
             session = login.Login(self.email)
```

### Comparing `nriapp-1.2.8/src/nriapp/core/mssentinelapi.py` & `nriapp-1.2.9/src/nriapp/core/mssentinelapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
                         
                         data["title"] = title
                         data["displayName"] = displayName
                         data["objectId"]  =  objectId
                         data["ipAddress"] = ipAddress
                         data["isp"] =  isp
                         data["objectName"] = objectName
-                    if self.type == "identityLogonEvent":
+                    elif self.type == "identityLogonEvent":
                         data["type"] = self.type
                         logonType = {i["key"]:i["value"] for i in self.details if i["key"]=="Logon type"}
                         accountDisplayName = {i["key"]:i["value"] for i in self.details if i["key"]=="Account display name"}
                         objectId = {i["key"]:i["value"] for i in self.details if i["key"]=="Account object id"}
                         application = {i["key"]:i["value"] for i in self.details if i["key"]=="Application"}
                         iPAddress = {i["key"]:i["value"] for i in self.details if i["key"]=="IPAddress"}
                         userAgent = {i["key"]:i["value"] for i in self.details if i["key"]=="User agent"}
```

### Comparing `nriapp-1.2.8/src/nriapp/core/multifactor.py` & `nriapp-1.2.9/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/core/vtquery.py` & `nriapp-1.2.9/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/helper/doc.py` & `nriapp-1.2.9/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/helper/login.py` & `nriapp-1.2.9/src/nriapp/helper/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 from seleniumwire import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager            #for ChromeDriver installation
+from webdriver_manager.firefox import GeckoDriverManager            #for ChromeDriver installation
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import TimeoutException, NoSuchElementException
 from selenium.webdriver.chrome.service import Service as ChromeService
-
+from selenium.webdriver.firefox.service import Service as FirefoxService
 
 import sys, json
 import urllib.request
 
 sys.path.append("..") # Adds higher directory to python modules path.
 
 from config.config import *
@@ -67,20 +68,27 @@
     def web_app(self, driver, web_app, email, organization):
 
         if driver.current_url == 'data:,':
             driver.get(web_app)
         else:
             driver.execute_script("window.open('');")
             driver.switch_to.window(driver.window_handles[len(driver.window_handles)-1])
-            driver.get(web_app)
+            while(True):
+                try:
+                    driver.get(web_app)
+                    break
+                except:
+                    driver.get(web_app)
 
         self.wait(driver, 20, By.XPATH, "//div[contains(text(),'Sign-in options')]")
-        driver.find_element(By.XPATH, "//div[contains(text(),'Sign-in options')]").click()
+        element = driver.find_element(By.XPATH, "//div[contains(text(),'Sign-in options')]")
+        WebDriverWait(driver,20).until(EC.element_to_be_clickable(element)).click()
         self.wait(driver, 20, By.XPATH, "//div[@data-test-cred-id='organization']")
-        driver.find_element(By.XPATH, "//div[@data-test-cred-id='organization']").click()
+        element = driver.find_element(By.XPATH, "//div[@data-test-cred-id='organization']")
+        WebDriverWait(driver,20).until(EC.element_to_be_clickable(element)).click()
         self.wait(driver, 20, By.ID, "searchOrganizationInput")
         driver.find_element(By.ID, "searchOrganizationInput").send_keys(organization)
         driver.find_element(By.ID, "idSIButton9").click()
         time.sleep(3)
 
         if "login.microsoftonline.com" not in driver.current_url:
             return
@@ -97,29 +105,33 @@
                 one_time_code = WebDriverWait(driver, 20).until(EC.visibility_of_element_located((By.XPATH, "//input[@id='idTxtBx_OTC_Password']"))).get_attribute("value")
             except:
                 if "login.microsoftonline.com" not in driver.current_url:
                     dbgPrint.debug("[+] Button override")
                     override = True
                     break
             if len(one_time_code) == 8:
-                driver.find_element(By.ID, "idSIButton9").click()
-
+                element = driver.find_element(By.ID, "idSIButton9")
+                WebDriverWait(driver,20).until(EC.element_to_be_clickable(element)).click()
 
     def create_driver(self):
 
         try:
-            service = ChromeService(ChromeDriverManager().install())
+#            service = ChromeService(ChromeDriverManager().install())
+            service = FirefoxService(GeckoDriverManager().install())
         except ValueError:
             latest_chromedriver_version_url = "https://chromedriver.storage.googleapis.com/LATEST_RELEASE"
             latest_chromedriver_version = urllib.request.urlopen(latest_chromedriver_version_url).read().decode('utf-8')
             service = ChromeService(ChromeDriverManager(version=latest_chromedriver_version).install())
-        options = webdriver.ChromeOptions()
-        options.add_argument('--disable-logging')
-        options.add_experimental_option('excludeSwitches', ['enable-logging'])          #Disable logging of webdriver
-        driver = webdriver.Chrome(service=service, options=options)                     #August 26, 2023
+#        options = webdriver.ChromeOptions()
+        options = webdriver.FirefoxOptions()
+#        options.add_argument('--disable-logging')
+#        options.add_experimental_option('excludeSwitches', ['enable-logging'])          #Disable logging of webdriver #Chrome
+#        driver = webdriver.Chrome(service=service, options=options)                     #August 26, 2023
+        options.binary_location = "C:\\Program Files (x86)\\Mozilla Firefox\\firefox.exe"
+        driver = webdriver.Firefox(service=service, options=options)                     #April 12, 2024
 #        driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager(version="114.0.5735.90").install()), options=options)  #New update 8/15/2023 11:35:31 PM
         return driver
 
     def login(self):
         self.driver = self.create_driver()   
         dbgPrint.info("[+] Checking session...")
 
@@ -136,33 +148,40 @@
         self.web_app(self.driver , security_page, self.email, self.organization)
 #        self.web_app(driver , security_page, "kwijp.onmicrosoft.com", self.email)
 
         self.wait(self.driver, 20, By.XPATH, "//div[@class='ms-List-page']")
 
         time.sleep(10)             
         auth_header = helper.RequestHeader(self.driver, "api/v2/auth")
+        auth_header.get_headers()
         cookie = auth_header.get_param("cookie")
 
         dbgPrint.debug("[+] Retrieving current cookie...\n")
 
         mde.MSSentinelApi(cookies=cookie).save_session()
 
-        self.web_app(self.driver , "https://intune.microsoft.com/#dashboard", self.email, self.organization)
-
+#        self.web_app(self.driver , "https://intune.microsoft.com/#dashboard", self.email, self.organization)
+        self.web_app(self.driver , "https://intune.microsoft.com/#home", self.email, self.organization)
 #        self.wait(self.driver, 20, By.XPATH, "//div[@class='ext-FlexColumn']//div//div[@data-bind='pcControl: card']")
-        self.wait(self.driver, 20, By.XPATH, "//*[@id='_weave_e_40']")
-
+#        self.wait(self.driver, 20, By.XPATH, "//*[@id='_weave_e_40']")
+        self.wait(self.driver, 20, By.XPATH, "//*[@name='Home.ReactView']")
         dbgPrint.info("Sleeping for 15s")
 
         time.sleep(20)
 
-        http_rqst = helper.RequestHeader(self.driver, "api/DelegationToken")         #1/27/2023 5:00:48 PM 
+        http_rqst = helper.RequestHeader(self.driver, "api/DelegationToken")        #1/27/2023 5:00:48 PM 
+        http_rqst.get_headers()
         cookie = http_rqst.get_param("cookie")
 
         json_data = json.loads(http_rqst.body)
+#        delegation_token = json.loads(http_rqst.body)
+
+#        http_rqst = helper.RequestHeader(self.driver, "oauth2/v2.0/token")
+#        http_rqst.get_headers_special("scope", "email openid profile")
+#        token = json.loads(http_rqst.response_body)["access_token"]
 
         msgraph.MSGraphApi(cookies=cookie, json=json_data, verify=False).save_session()
 
 #        self.web_app(self.driver , "https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", self.email, self.organization)
 
 #        self.wait(self.driver, 20, By.ID, "UserListGrid_ActionBarContainer")
 
@@ -170,15 +189,15 @@
 #        http_rqst = helper.RequestHeader(self.driver, "/GenericGetAvailableFilters.ajax")         #1/27/2023 5:00:48 PM 
 #        cookies = http_rqst.get_param("Cookie")
 #        headers = dict(http_rqst.headers._headers)
 #        page = mfa.MultiFactor(cookies=cookies, headers=headers)            
 
 #        page.save_session()
 
-        self.driver.quit()
+#        self.driver.quit()
 
     def mfa_login(self, email):
         self.driver = self.create_driver()  
         self.web_app(self.driver , "https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", email, self.organization)
 
         self.wait(self.driver, 20, By.ID, "UserListGrid_ActionBarContainer")
 #            self.wait(driver, 20, By.XPATH, "//img[@boxtype='Image' and @title='Search']")
```

### Comparing `nriapp-1.2.8/src/nriapp/helper/login_snyper.py` & `nriapp-1.2.9/src/nriapp/helper/login_snyper.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/helper/pylog.py` & `nriapp-1.2.9/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/helper/utils.py` & `nriapp-1.2.9/src/nriapp/helper/utils.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.2.9/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.2.8/src/nriapp/nriapp.py` & `nriapp-1.2.9/src/nriapp/nriapp.py`

 * *Files identical despite different names*


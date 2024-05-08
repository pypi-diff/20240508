# Comparing `tmp/jenkins_pysdk-1.3.tar.gz` & `tmp/jenkins_pysdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkins_pysdk-1.3.tar", last modified: Sun Apr 21 15:01:27 2024, max compression
+gzip compressed data, was "jenkins_pysdk-1.3.2.tar", last modified: Wed May  8 19:42:51 2024, max compression
```

## Comparing `jenkins_pysdk-1.3.tar` & `jenkins_pysdk-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:01:27.304941 jenkins_pysdk-1.3/
--rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-1.3/LICENSE
--rw-rw-rw-   0        0        0     3084 2024-04-21 15:01:27.304437 jenkins_pysdk-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2555 2024-04-20 21:25:01.000000 jenkins_pysdk-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 15:01:27.299438 jenkins_pysdk-1.3/jenkins_pysdk/
--rw-rw-rw-   0        0        0        2 2024-04-14 12:07:11.000000 jenkins_pysdk-1.3/jenkins_pysdk/__init__.py
--rw-rw-rw-   0        0        0      842 2024-04-11 20:11:04.000000 jenkins_pysdk-1.3/jenkins_pysdk/_logger.py
--rw-rw-rw-   0        0        0     5431 2024-04-18 19:59:55.000000 jenkins_pysdk-1.3/jenkins_pysdk/builders.py
--rw-rw-rw-   0        0        0    15758 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3/jenkins_pysdk/builds.py
--rw-rw-rw-   0        0        0     4229 2024-04-21 13:52:11.000000 jenkins_pysdk-1.3/jenkins_pysdk/consts.py
--rw-rw-rw-   0        0        0     7818 2024-04-21 13:45:33.000000 jenkins_pysdk-1.3/jenkins_pysdk/core.py
--rw-rw-rw-   0        0        0    13349 2024-04-21 09:31:25.000000 jenkins_pysdk-1.3/jenkins_pysdk/credentials.py
--rw-rw-rw-   0        0        0     1869 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3/jenkins_pysdk/exceptions.py
--rw-rw-rw-   0        0        0    24219 2024-04-21 14:56:48.000000 jenkins_pysdk-1.3/jenkins_pysdk/jenkins.py
--rw-rw-rw-   0        0        0    30659 2024-04-21 14:56:35.000000 jenkins_pysdk-1.3/jenkins_pysdk/jobs.py
--rw-rw-rw-   0        0        0    11239 2024-04-21 09:31:25.000000 jenkins_pysdk-1.3/jenkins_pysdk/nodes.py
--rw-rw-rw-   0        0        0     2581 2024-04-19 19:23:22.000000 jenkins_pysdk-1.3/jenkins_pysdk/objects.py
--rw-rw-rw-   0        0        0    23199 2024-04-21 09:35:25.000000 jenkins_pysdk-1.3/jenkins_pysdk/plugins.py
--rw-rw-rw-   0        0        0     6843 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3/jenkins_pysdk/queues.py
--rw-rw-rw-   0        0        0     9797 2024-04-21 09:41:26.000000 jenkins_pysdk-1.3/jenkins_pysdk/users.py
--rw-rw-rw-   0        0        0     4957 2024-04-20 14:47:01.000000 jenkins_pysdk-1.3/jenkins_pysdk/utils.py
--rw-rw-rw-   0        0        0       88 2024-04-21 14:06:28.000000 jenkins_pysdk-1.3/jenkins_pysdk/version.py
--rw-rw-rw-   0        0        0    12073 2024-04-21 14:55:11.000000 jenkins_pysdk-1.3/jenkins_pysdk/views.py
--rw-rw-rw-   0        0        0     3405 2024-04-21 11:21:38.000000 jenkins_pysdk-1.3/jenkins_pysdk/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:01:27.303436 jenkins_pysdk-1.3/jenkins_pysdk.egg-info/
--rw-rw-rw-   0        0        0     3084 2024-04-21 15:01:27.000000 jenkins_pysdk-1.3/jenkins_pysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      679 2024-04-21 15:01:27.000000 jenkins_pysdk-1.3/jenkins_pysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:01:27.000000 jenkins_pysdk-1.3/jenkins_pysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-21 15:01:27.000000 jenkins_pysdk-1.3/jenkins_pysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 15:01:27.000000 jenkins_pysdk-1.3/jenkins_pysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 15:01:27.304941 jenkins_pysdk-1.3/setup.cfg
--rw-rw-rw-   0        0        0      929 2024-04-21 15:01:22.000000 jenkins_pysdk-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:42:51.797618 jenkins_pysdk-1.3.2/
+-rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3475 2024-05-08 19:42:51.796424 jenkins_pysdk-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2666 2024-04-21 17:59:25.000000 jenkins_pysdk-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 19:42:51.788344 jenkins_pysdk-1.3.2/jenkins_pysdk/
+-rw-rw-rw-   0        0        0        2 2024-04-14 12:07:11.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/__init__.py
+-rw-rw-rw-   0        0        0      842 2024-04-11 20:11:04.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/_logger.py
+-rw-rw-rw-   0        0        0     5431 2024-04-18 19:59:55.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/builders.py
+-rw-rw-rw-   0        0        0    15758 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/builds.py
+-rw-rw-rw-   0        0        0     4242 2024-05-08 18:20:46.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/consts.py
+-rw-rw-rw-   0        0        0     7701 2024-05-08 19:41:50.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/core.py
+-rw-rw-rw-   0        0        0    13349 2024-04-21 09:31:25.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/credentials.py
+-rw-rw-rw-   0        0        0     1869 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/exceptions.py
+-rw-rw-rw-   0        0        0    24815 2024-05-08 19:42:43.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/jenkins.py
+-rw-rw-rw-   0        0        0    30659 2024-04-21 14:56:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/jobs.py
+-rw-rw-rw-   0        0        0    11239 2024-04-21 09:31:25.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/nodes.py
+-rw-rw-rw-   0        0        0     2581 2024-04-19 19:23:22.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/objects.py
+-rw-rw-rw-   0        0        0    24085 2024-05-08 19:19:52.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/plugins.py
+-rw-rw-rw-   0        0        0     6843 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/queues.py
+-rw-rw-rw-   0        0        0     9797 2024-04-21 09:41:26.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/users.py
+-rw-rw-rw-   0        0        0     4813 2024-05-08 19:25:02.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/utils.py
+-rw-rw-rw-   0        0        0       90 2024-05-08 19:35:28.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/version.py
+-rw-rw-rw-   0        0        0    12073 2024-04-21 14:55:11.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/views.py
+-rw-rw-rw-   0        0        0     3405 2024-04-21 11:21:38.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/workspace.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:42:51.795924 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/
+-rw-rw-rw-   0        0        0     3475 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 19:42:51.797618 jenkins_pysdk-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2024-05-08 19:35:28.000000 jenkins_pysdk-1.3.2/setup.py
```

### Comparing `jenkins_pysdk-1.3/LICENSE` & `jenkins_pysdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/PKG-INFO` & `jenkins_pysdk-1.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: jenkins_pysdk
-Version: 1.3
+Version: 1.3.2
 Summary: 2024 Python SDK for Jenkins
 Home-page: https://github.com/KnownZero/JenkinsPythonSDK
 Author: KnownZero
 Author-email: gihjeefs@protonmail.com
 License: MIT
 Keywords: python,Jenkins,SDK,API,REST
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: orjson
+Requires-Dist: pydantic
+Requires-Dist: urllib3
 
 # Jenkins Python SDK (jenkins_pysdk)
 
 [![Documentation Status](https://readthedocs.org/projects/jenkinspythonsdk/badge/?version=latest)](https://jenkinspythonsdk.readthedocs.io/en/latest/?badge=latest) 
+![CodeQL](https://github.com/KnownZero/JenkinsPythonSDK/actions/workflows/github-code-scanning/codeql/badge.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/jenkins-pysdk?style=flat&logo=pypi&logoColor=white&label=Downloads&color=blue)
 
 
 ### Supported for python 3.6+
 
 
 ## Installation
@@ -64,15 +72,15 @@
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2024 KnownZero
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -91,9 +99,7 @@
 [MIT](https://choosealicense.com/licenses/mit/)
 
 This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
 
 ## Contributors
 KnownZero
 
-
-
```

### Comparing `jenkins_pysdk-1.3/README.md` & `jenkins_pysdk-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Jenkins Python SDK (jenkins_pysdk)
 
 [![Documentation Status](https://readthedocs.org/projects/jenkinspythonsdk/badge/?version=latest)](https://jenkinspythonsdk.readthedocs.io/en/latest/?badge=latest) 
+![CodeQL](https://github.com/KnownZero/JenkinsPythonSDK/actions/workflows/github-code-scanning/codeql/badge.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/jenkins-pysdk?style=flat&logo=pypi&logoColor=white&label=Downloads&color=blue)
 
 
 ### Supported for python 3.6+
 
 
 ## Installation
@@ -47,15 +48,15 @@
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2024 KnownZero
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/_logger.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/_logger.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/builders.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/builders.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/builds.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/builds.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/consts.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 FORM_MULTIPART_HEADER = {"Content-Type": "multipart/form-data"}
 
 HOST_MATCH_REGEX_PATTERN = r"^[a-zA-Z0-9.-]+$"
 
 
 class Endpoints:
     class Instance:
-        Crumb = "crumbIssuer/api/json"
+        Crumb = "crumbIssuer"
         Connect = "login"
         Standard = "api/json"
-        About = "about"  # For plugins list etc
-        OverallLoad = "overallLoad/api/json"
+        OverallLoad = "overallLoad"
+        Console = "scriptText"
 
     class Manage:
         Reload = "#"
         CredentialStore = "manage/credentials/store/system"
 
     class Jobs:
         Create = "createItem"
@@ -101,14 +101,15 @@
         Enable = "plugin/{plugin}/makeEnabled"
         Disable = "plugin/{plugin}/makeDisabled"
         Uninstall = "plugin/{plugin}/doUninstall"
 
     class UpdateCenter:
         Iter = "sites[id]"
         Site = "updateCenter/site/{site}"
+        Create = "pluginManager/siteConfigure"
 
     class Nodes:
         Computer = "computer"
         Node = "computer/{name}"
         Delete = "doDelete"
         Disable = "toggleOffline"
         Create = "doCreateItem"
```

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/core.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,16 +99,16 @@
                    params: dict = None,
                    data: Any = None,
                    files: dict = None,
                    username: str = None,
                    passw_or_token: str = None,
                    timeout: int = None,
                    _session: HTTPSessionResponseObject = None,
-                   ) -> Union[Tuple[HTTPRequestObject, HTTPResponseObject],
-                              Tuple[HTTPSessionRequestObject, HTTPSessionResponseObject]]:
+                   ) -> (Tuple[HTTPRequestObject, HTTPResponseObject] or
+                         Tuple[HTTPSessionRequestObject, HTTPSessionResponseObject]):
         """
         Some HTTP interaction function...
         :param url: The url to hit
         :param method: HTTP method
         :param headers: request headers
         :param params: request parameters
         :param data: request data
@@ -132,15 +132,16 @@
                                             timeout=timeout if timeout else self.timeout)
             req, resp = request_obj, interact_http(request_obj)
             if isinstance(resp._raw, Exception):
                 raise JenkinsConnectionException(resp._raw)
             return req, resp
         else:
             crumbed_session_req = HTTPSessionRequestObject(
-                method="GET", url=self._build_url(Endpoints.Instance.Crumb), headers=headers,
+                method="GET", url=self._build_url(Endpoints.Instance.Crumb, suffix=Endpoints.Instance.Standard),
+                headers=headers,
                 username=username if username else self.username,
                 passw_or_token=passw_or_token if passw_or_token else self.passw,
                 verify=self.verify,
                 proxy=self.proxy,
                 timeout=timeout if timeout else self.timeout,
                 keep_session=True
             )
@@ -154,16 +155,7 @@
                                                    username=username if username else self.username,
                                                    passw_or_token=passw_or_token if passw_or_token else self.passw,
                                                    verify=self.verify,
                                                    proxy=self.proxy,
                                                    timeout=timeout if timeout else self.timeout,
                                                    session=crumbed_session.session)
             return request_obj, interact_http_session(request_obj)
-
-
-# class Interact(ABC):
-#     def __init__(self, jenkins):
-#         self._jenkins = jenkins
-#
-#     @property
-#     def config(self):
-#         return
```

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/credentials.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/credentials.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/exceptions.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/jenkins.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/jenkins.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,18 +160,14 @@
 
         :return: Flag for creating FreeStyle jobs
         :rtype: :class:`jenkins_pysdk.objects.Flags.Jobs`
         """
         return r_jobs(value=Class.Freestyle)
 
     # @property
-    # def UsernamePassword(self) -> r_builder.Credential:
-    #     return r_builder.Credential(value=Class.UsernamePassword)
-
-    # @property
     # def enable_logging(self):
     #     """
     #     Get the logging level.
     #     """
     #     return self.Enable_Logging
     #
     # @enable_logging.setter
@@ -307,15 +303,15 @@
 
         :return: Number of available executors
         :rtype: int
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         # TODO: FIX CODE COPY & PASTE BELOW... maybe singledispatch
         _fields = ['_class', 'availableExecutors']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['availableExecutors']
         if not content:
             raise JenkinsGeneralException("No executors are available.")
         return content
 
@@ -325,15 +321,15 @@
         View the executors that are currently being used on the instance.
 
         :return: Information about the executors in use
         :rtype: str
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'busyExecutors']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['busyExecutors']
         if not content:
             raise JenkinsGeneralException("No executors are in-use.")
         return content
 
@@ -343,15 +339,15 @@
         View the number of executors that are about to run on the instance.
 
         :return: Number of pending executors
         :rtype: int
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'connectingExecutors']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['connectingExecutors']
         if not content:
             raise JenkinsGeneralException("No executors are connecting.")
         return content
 
@@ -361,15 +357,15 @@
         View information about the setup executors on the instance.
 
         :return: Information about the setup executors
         :rtype: str
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'definedExecutors']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['definedExecutors']
         if not content:
             raise JenkinsGeneralException("No executors are defined.")
         return content
 
@@ -379,15 +375,15 @@
         View the number of idle executors on the instance.
 
         :return: Number of idle executors
         :rtype: int
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'idleExecutors']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['idleExecutors']
         if not content:
             raise JenkinsGeneralException("No executors are idle.")
         return content
 
@@ -397,15 +393,15 @@
         View the number of executors that are currently online on the instance.
 
         :return: Number of online executors
         :rtype: int
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'onlineExecutors']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['onlineExecutors']
         if not content:
             raise JenkinsGeneralException("No executors are online.")
         return content
 
@@ -415,15 +411,15 @@
         View the current queue size on the instance.
 
         :return: Current queue size
         :rtype: int
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'queueLength']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['queueLength']
         if not content:
             raise JenkinsGeneralException("No work in the queue.")
         return content
 
@@ -433,15 +429,15 @@
         View the total number of executors on the instance.
 
         :return: Total number of executors
         :rtype: int
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'totalExecutors']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['totalExecutors']
         if not content:
             raise JenkinsGeneralException("No executors are setup.")
         return content
 
@@ -452,15 +448,15 @@
 
         :return: Maximum queue size
         :rtype: int
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         # TODO: Fix endpoitn remove api json
         _fields = ['_class', 'totalQueueLength']
-        url = self._build_url(Endpoints.Instance.OverallLoad)
+        url = self._build_url(Endpoints.Instance.OverallLoad, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['totalQueueLength']
         if not content:
             raise JenkinsGeneralException("No executors are setup.")
         return content
 
@@ -627,7 +623,14 @@
         req_obj, resp_obj = self._send_http(method="POST", url=url)
         msg = f"[{resp_obj.status_code}] Successfully reloaded configuration."
         if resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to reload configuration from disk."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
+
+    def script_console(self, commands: str) -> str:
+        url = self._build_url(Endpoints.Instance.Console)
+        req_obj, resp_obj = self._send_http(method="POST", url=url, data={"script": commands}, headers=dict())
+        if resp_obj.status_code != 200:
+            raise JenkinsGeneralException(f"[{resp_obj.status_code}] Failed to send commands to the script console.")
+        return resp_obj.content
```

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/jobs.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/jobs.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/nodes.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/nodes.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/objects.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/objects.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/plugins.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Generator
-from typing import List, Union, Dict
+from typing import List, Union, Dict, BinaryIO
 
 import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.objects import JenkinsActionObject
 from jenkins_pysdk.exceptions import JenkinsGeneralException, JenkinsNotFound
 from jenkins_pysdk.consts import Endpoints, XML_POST_HEADER
@@ -152,22 +152,31 @@
         Get a list of all sites in the update center.
 
         :return: A list of Site objects.
         :rtype: List[:class:`jenkins_pysdk.plugins.Site`]
         """
         return [site for site in self.iter()]
 
-    def create(self) -> JenkinsActionObject:
+    def create(self, site_url: str or HttpUrl) -> JenkinsActionObject:
         """
         Create a new site in the update center.
 
-        :return: JenkinsActionObject representing the create action.
+        :return: JenkinsActionObject representing the create update center operation.
         :rtype: jenkins_pysdk.objects.JenkinsActionObject
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
-        pass
+        url = self._jenkins._build_url(Endpoints.UpdateCenter.Create)
+        params = {"site": site_url}
+        req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, params=params)
+        if resp_obj.status_code != 200:
+            raise JenkinsGeneralException(f"[{resp_obj.status_code}] Failed to add update center ({site_url}).")
+        msg = f"[{resp_obj.status_code}] Successfully added update center ({site_url})."
+        obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
+        obj._raw = resp_obj._raw
+        return obj
 
 
 class Plugin:
     """
     Represents a plugin in Jenkins.
 
     :param jenkins: The Jenkins instance this plugin belongs to.
@@ -548,37 +557,41 @@
         Represents a group of installed plugins in Jenkins.
 
         :return: A PluginGroup instance representing the installed plugins.
         :rtype: jenkins_pysdk.plugins.PluginGroup
         """
         return PluginGroup(self._jenkins, p_type="plugins")
 
-    # def upload(self, filename: str, file_content: bytes) -> JenkinsActionObject:
-    #     """
-    #     Uploads a plugin to Jenkins.
-    #
-    #     :param filename: The name of the plugin file.
-    #     :type filename: str
-    #     :param file_content: The content of the plugin file as bytes.
-    #     :type file_content: bytes
-    #     :return: A JenkinsActionObject representing the upload action.
-    #     :rtype: jenkins_pysdk.objects.JenkinsActionObject
-    #     :raises JenkinsGeneralException: If a general exception occurs.
-    #     """
-    #     url = self._jenkins._build_url(Endpoints.Plugins.Upload)
-    #     req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=None,
-    #                                                  files={"file": (filename, file_content)})
-    #     msg = f"[{resp_obj.status_code}] Successfully uploaded plugin ({filename})."
-    #     if resp_obj.status_code >= 500:
-    #         raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
-    #     elif resp_obj.status_code != 204:
-    #         msg = f"[{resp_obj.status_code}] Failed to upload plugin ({[filename]})."
-    #     obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
-    #     obj._raw = resp_obj._raw
-    #     return obj
+    def upload(self, filename: str, file_content: BinaryIO or bytes) -> JenkinsActionObject:
+        """
+        Uploads a plugin to Jenkins.
+
+        :param filename: The name of the plugin file.
+        :type filename: str
+        :param file_content: The content of the plugin file as bytes.
+        :type file_content: bytes
+        :return: A JenkinsActionObject representing the upload action.
+        :rtype: jenkins_pysdk.objects.JenkinsActionObject
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
+        # Solution: https://issues.jenkins.io/browse/JENKINS-68443
+        # Make it a form submission ^
+        if isinstance(file_content, BinaryIO):
+            file_content = file_content.read()
+        url = self._jenkins._build_url(Endpoints.Plugins.Upload)
+        file = {"file": (filename, file_content, "application/java-archive"), "submit": ""}
+        req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=dict(), files=file)
+        msg = f"[{resp_obj.status_code}] Successfully uploaded plugin ({filename})."
+        if resp_obj.status_code >= 500:
+            raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
+        elif resp_obj.status_code != 200:
+            msg = f"[{resp_obj.status_code}] Failed to upload plugin ({filename})."
+        obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
+        obj._raw = resp_obj._raw
+        return obj
 
     def install(self, name: str, version: str or int or float = "latest", restart: bool = False) -> JenkinsActionObject:
         """
         Installs a plugin in Jenkins.
 
         :param name: The name of the plugin to install.
         :type name: str
```

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/queues.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/queues.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/users.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/users.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/utils.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from httpx import Client, Request, ConnectError, BasicAuth
 from pydantic import HttpUrl
 
 from jenkins_pysdk.consts import HTTP_RETRY_COUNT, HOST_MATCH_REGEX_PATTERN
 from jenkins_pysdk.objects import HTTPRequestObject, HTTPResponseObject, HTTPSessionRequestObject, \
     HTTPSessionResponseObject
 from jenkins_pysdk.exceptions import JenkinsInvalidHost
-# from _logger import logger
+
 
 __all__ = ["validate_connect_host", "validate_http_url", "interact_http", "interact_http_session"]
 
 
 def validate_connect_host(host: str) -> bool:
     """
 
@@ -34,16 +34,14 @@
         result = parse_url(str(url))
         return all([result.scheme, result.netloc])
     except ValueError:
         return False
 
 
 def interact_http(request: HTTPRequestObject) -> HTTPResponseObject:
-    # TODO: Add retry option in HTTPRequestObject and Jenkins __init__??
-    # TODO: should this be in utils :(
     if validate_http_url(request.url) is False:
         raise JenkinsInvalidHost(f"{request.url.host} is not a valid target.")
     req = Request(
         method=request.method,
         url=str(request.url),
         headers=request.headers,
         data=request.data,
@@ -79,15 +77,14 @@
         # logger.debuge(exception)
         return return_object
 
 
 def interact_http_session(request: HTTPSessionRequestObject) -> HTTPSessionResponseObject:
     if validate_http_url(request.url) is False:
         raise JenkinsInvalidHost(f"{request.url.host} is not a valid target.")
-
     req = Request(
         method=request.method,
         url=str(request.url),
         headers=request.headers,
         data=request.data,
         params=request.params,
         files=request.files
```

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/views.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/views.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk/workspace.py` & `jenkins_pysdk-1.3.2/jenkins_pysdk/workspace.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk.egg-info/PKG-INFO` & `jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
-Name: jenkins-pysdk
-Version: 1.3
+Name: jenkins_pysdk
+Version: 1.3.2
 Summary: 2024 Python SDK for Jenkins
 Home-page: https://github.com/KnownZero/JenkinsPythonSDK
 Author: KnownZero
 Author-email: gihjeefs@protonmail.com
 License: MIT
 Keywords: python,Jenkins,SDK,API,REST
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: orjson
+Requires-Dist: pydantic
+Requires-Dist: urllib3
 
 # Jenkins Python SDK (jenkins_pysdk)
 
 [![Documentation Status](https://readthedocs.org/projects/jenkinspythonsdk/badge/?version=latest)](https://jenkinspythonsdk.readthedocs.io/en/latest/?badge=latest) 
+![CodeQL](https://github.com/KnownZero/JenkinsPythonSDK/actions/workflows/github-code-scanning/codeql/badge.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/jenkins-pysdk?style=flat&logo=pypi&logoColor=white&label=Downloads&color=blue)
 
 
 ### Supported for python 3.6+
 
 
 ## Installation
@@ -64,15 +72,15 @@
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2024 KnownZero
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -91,9 +99,7 @@
 [MIT](https://choosealicense.com/licenses/mit/)
 
 This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
 
 ## Contributors
 KnownZero
 
-
-
```

### Comparing `jenkins_pysdk-1.3/jenkins_pysdk.egg-info/SOURCES.txt` & `jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


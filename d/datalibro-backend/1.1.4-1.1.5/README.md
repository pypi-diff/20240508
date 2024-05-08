# Comparing `tmp/datalibro_backend-1.1.4.tar.gz` & `tmp/datalibro_backend-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_backend-1.1.4.tar", last modified: Tue May  7 02:54:26 2024, max compression
+gzip compressed data, was "datalibro_backend-1.1.5.tar", last modified: Wed May  8 10:32:55 2024, max compression
```

## Comparing `datalibro_backend-1.1.4.tar` & `datalibro_backend-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-07 02:54:26.384066 datalibro_backend-1.1.4/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.4/LICENSE.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-07 02:54:26.383780 datalibro_backend-1.1.4/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.4/README.md
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-07 02:54:26.382886 datalibro_backend-1.1.4/datalibro_backend/
--rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.4/datalibro_backend/__init__.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    15308 2024-04-18 06:06:10.000000 datalibro_backend-1.1.4/datalibro_backend/quality_check.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    10986 2024-05-07 02:54:19.000000 datalibro_backend-1.1.4/datalibro_backend/read_file.py
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-07 02:54:26.383583 datalibro_backend-1.1.4/datalibro_backend.egg-info/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-07 02:54:26.000000 datalibro_backend-1.1.4/datalibro_backend.egg-info/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-07 02:54:26.000000 datalibro_backend-1.1.4/datalibro_backend.egg-info/SOURCES.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-07 02:54:26.000000 datalibro_backend-1.1.4/datalibro_backend.egg-info/dependency_links.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-07 02:54:26.000000 datalibro_backend-1.1.4/datalibro_backend.egg-info/top_level.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-07 02:54:26.384135 datalibro_backend-1.1.4/setup.cfg
--rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-07 02:54:17.000000 datalibro_backend-1.1.4/setup.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-08 10:32:55.706574 datalibro_backend-1.1.5/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.5/LICENSE.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-08 10:32:55.706282 datalibro_backend-1.1.5/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.5/README.md
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-08 10:32:55.705229 datalibro_backend-1.1.5/datalibro_backend/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.5/datalibro_backend/__init__.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    15308 2024-04-18 06:06:10.000000 datalibro_backend-1.1.5/datalibro_backend/quality_check.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    11228 2024-05-08 10:31:35.000000 datalibro_backend-1.1.5/datalibro_backend/read_file.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-08 10:32:55.706079 datalibro_backend-1.1.5/datalibro_backend.egg-info/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/top_level.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-08 10:32:55.706634 datalibro_backend-1.1.5/setup.cfg
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-08 10:31:51.000000 datalibro_backend-1.1.5/setup.py
```

### Comparing `datalibro_backend-1.1.4/LICENSE.txt` & `datalibro_backend-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.4/PKG-INFO` & `datalibro_backend-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro_backend
-Version: 1.1.4
+Version: 1.1.5
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.4/README.md` & `datalibro_backend-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.4/datalibro_backend/quality_check.py` & `datalibro_backend-1.1.5/datalibro_backend/quality_check.py`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.4/datalibro_backend/read_file.py` & `datalibro_backend-1.1.5/datalibro_backend/read_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,28 +173,36 @@
         'Authorization': f'Bearer {token}',
         'Content-Type': 'application/json'
     }
 
     # 发送卡片消息
     response = requests.post(message_url, headers=headers, json=card_content)
     return response.json()
-def send_card_message_user(user_id,title,content):
+def send_card_message_user(user_id,content,title,link_url='',content_2=''):
     """Get the access token from Feishu."""
     url = 'https://open.feishu.cn/open-apis/auth/v3/tenant_access_token/internal/'
     headers = {'Content-Type': 'application/json'}
     app_id = 'cli_a5eeb3ad3837100b'
     app_secret = 'ftLZbDJOzDxSx0xiigALNev1tgHTvR4V'
 
     payload = {
         'app_id': app_id,
         'app_secret': app_secret
     }
     response = requests.post(url, headers=headers, json=payload)
     data = response.json()
     token = data.get('tenant_access_token')
+    if link_url != '':
+        if content_2 != '':
+            content_new = f"{content}<a href='{link_url}'></a>{content_2}"
+        else:
+            content_new = f"{content}<a href='{link_url}'></a>"
+    else:
+        content_new = content
+    # 卡片消息内容
     card_content = {
     'user_id': user_id,
     "msg_type": "interactive",
     "card": {
         "config": {
             "wide_screen_mode": True
         },
@@ -202,21 +210,19 @@
             "title": {
                 "tag": "plain_text",
                 "content": f"{title}"
             }
         },
         "elements": [
             {
-                "tag": "div",
-                "text": {
-                    "tag": "plain_text",
-                    "content": f"{content}"
+                "tag": "markdown",
+                "content": f"{content_new}"
+                    
                 }
-            },
-            
+                
             # 其他卡片组件，例如按钮等
         ]
     }
 }
     # 发送消息的API端点
     message_url = 'https://open.feishu.cn/open-apis/message/v4/send/'
```

### Comparing `datalibro_backend-1.1.4/datalibro_backend.egg-info/PKG-INFO` & `datalibro_backend-1.1.5/datalibro_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro-backend
-Version: 1.1.4
+Version: 1.1.5
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.4/setup.py` & `datalibro_backend-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datalibro_backend",
-  version="1.1.4",
+  version="1.1.5",
   author="lucy",
   author_email="lucy@petlibro.com",
   description="A small package for your backend service",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/DesignLibro/datalibro_backend",
   packages=setuptools.find_packages(),
```


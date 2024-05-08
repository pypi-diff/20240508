# Comparing `tmp/pyldk-1.1.4-py3-none-win_amd64.whl.zip` & `tmp/pyldk-1.1.5-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3903329 bytes, number of entries: 9
--rw-r--r--  2.0 unx      245 b- defN 23-May-08 07:49 pyldk/__init__.py
--rw-r--r--  2.0 unx     4344 b- defN 23-May-08 07:49 pyldk/hasp_adapter.py
--rw-r--r--  2.0 unx     2600 b- defN 23-May-08 07:49 pyldk/pyldk.py
--rw-r--r--  2.0 unx       24 b- defN 23-May-08 07:49 pyldk/version.py
--rw-r--r--  2.0 unx  5899264 b- defN 23-May-08 07:49 pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll
--rw-r--r--  2.0 unx      513 b- defN 23-May-08 07:49 pyldk-1.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 07:49 pyldk-1.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 23-May-08 07:49 pyldk-1.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      688 b- defN 23-May-08 07:49 pyldk-1.1.4.dist-info/RECORD
-9 files, 5907798 bytes uncompressed, 3902155 bytes compressed:  34.0%
+Zip file size: 3903354 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      245 b- defN 24-May-08 03:23 pyldk/__init__.py
+-rw-r--r--  2.0 unx     4344 b- defN 24-May-08 03:23 pyldk/hasp_adapter.py
+-rw-r--r--  2.0 unx     2679 b- defN 24-May-08 03:23 pyldk/pyldk.py
+-rw-r--r--  2.0 unx       24 b- defN 24-May-08 03:23 pyldk/version.py
+-rw-r--r--  2.0 unx  5899264 b- defN 24-May-08 03:23 pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll
+-rw-r--r--  2.0 unx      513 b- defN 24-May-08 03:23 pyldk-1.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 03:23 pyldk-1.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-May-08 03:23 pyldk-1.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      688 b- defN 24-May-08 03:23 pyldk-1.1.5.dist-info/RECORD
+9 files, 5907877 bytes uncompressed, 3902180 bytes compressed:  34.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: pyldk/version.py
 Comment: 
 
 Filename: pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll
 Comment: 
 
-Filename: pyldk-1.1.4.dist-info/METADATA
+Filename: pyldk-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pyldk-1.1.4.dist-info/WHEEL
+Filename: pyldk-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyldk-1.1.4.dist-info/top_level.txt
+Filename: pyldk-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyldk-1.1.4.dist-info/RECORD
+Filename: pyldk-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyldk/pyldk.py

```diff
@@ -33,15 +33,15 @@
         else:
             print(msg)
 
     def get_feature_id(self):
         feature_id = self.adapter.get_info()
         return feature_id
 
-    def login(self,feature_id=None):
+    def login(self,feature_id=None,is_mutiple_feature_id=False):
         ## 首先判断加密狗是否存在
         login_status = False
         if feature_id is None:
             feature_id = 0
         haspStruct = self.adapter.login(feature_id)
         if haspStruct.status == 0:
             self.adapter.logout(haspStruct.handle)
@@ -53,15 +53,16 @@
                     login_status = True
                 else:
                     self.adapter.log("加密狗初始化失败,请检查加密狗的授权,或者重新授权")
                     self.adapter.logout(haspStruct.handle)
             else:
                 self.adapter.log("加密狗初始化失败",haspStruct.status)
         else:
-            self.adapter.show_staus("加密狗初始化失败", haspStruct.status,feature_id)
+            if is_mutiple_feature_id is False:
+                self.adapter.show_staus("加密狗初始化失败", haspStruct.status,feature_id)
         return haspStruct,feature_id,login_status
 
 
     def get_ldk(self,feature_id):
         ldk_status = False
         lower_users = self.adapter.bool_lower_users(feature_id)
         if lower_users:
```

## pyldk/version.py

```diff
@@ -1 +1 @@
-full_version  = '1.1.4'
+full_version  = '1.1.5'
```

## Comparing `pyldk-1.1.4.dist-info/METADATA` & `pyldk-1.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyldk
-Version: 1.1.4
+Version: 1.1.5
 Summary: pyldk
 Home-page: https://jadehh@live.com
 Author: jade
 Author-email: jadehh@live.com
 License: MIT Licence
 Keywords: pip,pyldk,
 Platform: any
```

## Comparing `pyldk-1.1.4.dist-info/RECORD` & `pyldk-1.1.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pyldk/__init__.py,sha256=NV5NModdxHlMQ_yOO2fbeO89UuEmkSPQiRcukwU0Ssk,245
 pyldk/hasp_adapter.py,sha256=J7c2Gp2WJR9XFu8Et20DUzdFjCMzupJitXUTa7xcM00,4344
-pyldk/pyldk.py,sha256=l4lh8-OA_Ka02UOaEWneG2fcPyv0xVA2-ZvHYBGJhN0,2600
-pyldk/version.py,sha256=OxsavrrGs22NAvCjmqSmXv_NDIOqPqGGobupg4LG4IM,24
+pyldk/pyldk.py,sha256=RuRjbzN_kud_fYQv9vGJLpM1q-kuAZSVfWXukByTijE,2679
+pyldk/version.py,sha256=uo2YuaqapTMC1MK_opuodPspTYl1sfDhKjgXuUyk5Ng,24
 pyldk/lib/Windows/x64/lib_hasp_adapter_x64.dll,sha256=5F5six-ErdDc9aQqld7LpQ7TlDhLD0C4uwZzLqQcRNA,5899264
-pyldk-1.1.4.dist-info/METADATA,sha256=41Y5Kim6oBe3fC5QHBOSiQ9nfmoRikOWsSO_20tXTnM,513
-pyldk-1.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyldk-1.1.4.dist-info/top_level.txt,sha256=1aCn7AVUNDZFl_MBhuhBcysO6UrkUlIsuKkrsE5eU6o,28
-pyldk-1.1.4.dist-info/RECORD,,
+pyldk-1.1.5.dist-info/METADATA,sha256=-wbB4hv55WTkrTtVcX9p1w3PZAcfJvJAgboVL5nFqnM,513
+pyldk-1.1.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+pyldk-1.1.5.dist-info/top_level.txt,sha256=1aCn7AVUNDZFl_MBhuhBcysO6UrkUlIsuKkrsE5eU6o,28
+pyldk-1.1.5.dist-info/RECORD,,
```


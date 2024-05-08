# Comparing `tmp/nuvla_api-4.0.0-py3-none-any.whl.zip` & `tmp/nuvla_api-4.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 29129 bytes, number of entries: 22
 -rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 nuvla/__init__.py
 -rw-r--r--  2.0 unx      112 b- defN 80-Jan-01 00:00 nuvla/api/__init__.py
--rw-r--r--  2.0 unx    23639 b- defN 80-Jan-01 00:00 nuvla/api/api.py
+-rw-r--r--  2.0 unx    23586 b- defN 80-Jan-01 00:00 nuvla/api/api.py
 -rw-r--r--  2.0 unx     2406 b- defN 80-Jan-01 00:00 nuvla/api/models.py
 -rw-r--r--  2.0 unx      222 b- defN 80-Jan-01 00:00 nuvla/api/resources/__init__.py
 -rw-r--r--  2.0 unx     2351 b- defN 80-Jan-01 00:00 nuvla/api/resources/base.py
 -rw-r--r--  2.0 unx      734 b- defN 80-Jan-01 00:00 nuvla/api/resources/callback.py
 -rw-r--r--  2.0 unx     6410 b- defN 80-Jan-01 00:00 nuvla/api/resources/credential.py
 -rw-r--r--  2.0 unx     3777 b- defN 80-Jan-01 00:00 nuvla/api/resources/data.py
 -rw-r--r--  2.0 unx    19472 b- defN 80-Jan-01 00:00 nuvla/api/resources/deployment.py
@@ -13,12 +13,12 @@
 -rw-r--r--  2.0 unx     2942 b- defN 80-Jan-01 00:00 nuvla/api/resources/infra_service.py
 -rw-r--r--  2.0 unx     7345 b- defN 80-Jan-01 00:00 nuvla/api/resources/module.py
 -rw-r--r--  2.0 unx     1421 b- defN 80-Jan-01 00:00 nuvla/api/resources/notification.py
 -rw-r--r--  2.0 unx     1190 b- defN 80-Jan-01 00:00 nuvla/api/resources/user.py
 -rw-r--r--  2.0 unx       24 b- defN 80-Jan-01 00:00 nuvla/api/util/__init__.py
 -rw-r--r--  2.0 unx      731 b- defN 80-Jan-01 00:00 nuvla/api/util/date.py
 -rw-r--r--  2.0 unx      688 b- defN 80-Jan-01 00:00 nuvla/api/util/filter.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 nuvla_api-4.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2733 b- defN 80-Jan-01 00:00 nuvla_api-4.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 nuvla_api-4.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1819 b- defN 16-Jan-01 00:00 nuvla_api-4.0.0.dist-info/RECORD
-22 files, 91166 bytes uncompressed, 26181 bytes compressed:  71.3%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 nuvla_api-4.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2733 b- defN 80-Jan-01 00:00 nuvla_api-4.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 nuvla_api-4.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1819 b- defN 16-Jan-01 00:00 nuvla_api-4.0.1.dist-info/RECORD
+22 files, 91113 bytes uncompressed, 26181 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: nuvla/api/util/date.py
 Comment: 
 
 Filename: nuvla/api/util/filter.py
 Comment: 
 
-Filename: nuvla_api-4.0.0.dist-info/LICENSE
+Filename: nuvla_api-4.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: nuvla_api-4.0.0.dist-info/METADATA
+Filename: nuvla_api-4.0.1.dist-info/METADATA
 Comment: 
 
-Filename: nuvla_api-4.0.0.dist-info/WHEEL
+Filename: nuvla_api-4.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: nuvla_api-4.0.0.dist-info/RECORD
+Filename: nuvla_api-4.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nuvla/api/api.py

```diff
@@ -484,16 +484,15 @@
         :keyword    select: Cimi select parameter, used to delete an existing attribute from a cimi resource when the
                     selected fields are not present in the data argument (e.g description, value)
         :type       select: str or list of str
 
         :return:    A CimiResponse object which should contain the attributes 'status', 'resource-id' and 'message'
         :rtype:     CimiResource
         """
-        resource = self.get(resource_id=resource_id)
-        return CimiResource(self._cimi_put(resource_id=resource.id, json=data, params=kwargs))
+        return CimiResource(self._cimi_put(resource_id=resource_id, json=data, params=kwargs))
 
     def delete(self, resource_id) -> CimiResponse:
         """ Delete a CIMI resource by it's resource id
 
         :param  resource_id: The id of the resource to delete
         :type   resource_id: str
```

## Comparing `nuvla_api-4.0.0.dist-info/LICENSE` & `nuvla_api-4.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nuvla_api-4.0.0.dist-info/METADATA` & `nuvla_api-4.0.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvla-api
-Version: 4.0.0
+Version: 4.0.1
 Summary: Nuvla APIServer python client library
 Home-page: https://github.com/nuvla/python-library
 License: Apache-2.0
 Author: SixSq SA
 Author-email: support@sixsq.com
 Maintainer: Ignacio Penas
 Maintainer-email: nacho@sixsq.com
```

## Comparing `nuvla_api-4.0.0.dist-info/RECORD` & `nuvla_api-4.0.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 nuvla/__init__.py,sha256=C9Wso9mzB57_KMtYMfZnGqx6lN1jTsNzWQ0UyRtllDA,81
 nuvla/api/__init__.py,sha256=alPddudoqznjse-LuLNhPxfXznHKNIKSE9eS1CVlfeM,112
-nuvla/api/api.py,sha256=vNYzliWG-v9APuqwAuxyTj8jGjxt40i2eiulV6lE2_I,23639
+nuvla/api/api.py,sha256=PrYCVPMFUdiM_BJnaCRJ26273bQSr7DqiMQa96kGRv0,23586
 nuvla/api/models.py,sha256=4ubV01Rb9hOXqJS6V2awTa5ygj_aVNu7sOQTkkUGVzs,2406
 nuvla/api/resources/__init__.py,sha256=2f5cV4q8B58pcFuSghwIsvu-OlX3YMr8dGcOUjAAgJo,222
 nuvla/api/resources/base.py,sha256=DLYRR0AZFR1c6NKujnbF-Jgi_dUp6LvgXKNgDfUpCMw,2351
 nuvla/api/resources/callback.py,sha256=wU8-iZNIDsYENVJgMSx93EIe3vY60igdRtYgNBLzyhY,734
 nuvla/api/resources/credential.py,sha256=Ns44c5cUYTtqajhnvSPo4LebDutqhGtkNC2rxoKX0Ow,6410
 nuvla/api/resources/data.py,sha256=M6G9eHJYDDV2LxKmiE9O1cgqq9NPrGbPjenu61OO500,3777
 nuvla/api/resources/deployment.py,sha256=t4A_9rqFBLBZ88Nc1Imn7rHahnrB4CKr6D5eEALnA_8,19472
@@ -12,11 +12,11 @@
 nuvla/api/resources/infra_service.py,sha256=iyl64nN9_aVlyeBVFT9PtttIAJAf18LZsSI_sANNB-s,2942
 nuvla/api/resources/module.py,sha256=zqfqAN5-tDNONgDCaD2ZS_N03wQZDOpo7EeAVXNjnxY,7345
 nuvla/api/resources/notification.py,sha256=vFKxEVbcsJGlibYmpOsMnQ9ajKP3pVYvsDQjjhTSlTQ,1421
 nuvla/api/resources/user.py,sha256=jW1SApAX8pb75ZXhS0Xdu8QNItFg8lM6Ei30wPQVi9A,1190
 nuvla/api/util/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 nuvla/api/util/date.py,sha256=d2ilqbB0BMpfn-dmjfku7KHbEKEn_7hX1vhkgstLyTE,731
 nuvla/api/util/filter.py,sha256=JKLBwuTs_yu6x0briQCQYoDWXa2N1lIE3yVxM6inK6s,688
-nuvla_api-4.0.0.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-nuvla_api-4.0.0.dist-info/METADATA,sha256=i2terhLDPXPdPq8CY2Q-n73GGIQlVc0Woe-a0EyV8bg,2733
-nuvla_api-4.0.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-nuvla_api-4.0.0.dist-info/RECORD,,
+nuvla_api-4.0.1.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+nuvla_api-4.0.1.dist-info/METADATA,sha256=sK4IfRZJMKn2N2eYZEznfEXF8nJqTVHLvL0ejqWSDAw,2733
+nuvla_api-4.0.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+nuvla_api-4.0.1.dist-info/RECORD,,
```


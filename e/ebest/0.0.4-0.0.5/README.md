# Comparing `tmp/ebest-0.0.4.tar.gz` & `tmp/ebest-0.0.5.tar.gz`

## Comparing `ebest-0.0.4.tar` & `ebest-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,10 @@
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ebest-0.0.4/ebest.pyproj
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/01. 로그인.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/02. 전체업종.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/03. 주식전종목조회.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/04. 주식현재가.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/05. 주식차트.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/06. 주식차트 -연속조회.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/07. 계좌예수금조회.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/08. 지수선물마스터조회.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/10. 서버저장조건 리스트조회.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/11. 서버저장조건 조건검색.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/12. 서버저장조건 실시간검색.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 ebest-0.0.4/samples/21. 웹소켓 실시간 체결시세.py
--rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 ebest-0.0.4/src/ebest/OpenApi.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ebest-0.0.4/src/ebest/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 ebest-0.0.4/src/ebest/code_realtime_account.py
--rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 ebest-0.0.4/src/ebest/tr_code_to_path.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 ebest-0.0.4/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ebest-0.0.4/LICENSE
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 ebest-0.0.4/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ebest-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 ebest-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 ebest-0.0.5/ebest.pyproj
+-rw-r--r--   0        0        0    10305 2020-02-02 00:00:00.000000 ebest-0.0.5/src/ebest/OpenApi.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ebest-0.0.5/src/ebest/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 ebest-0.0.5/src/ebest/code_realtime_account.py
+-rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 ebest-0.0.5/src/ebest/tr_code_to_path.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 ebest-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ebest-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 ebest-0.0.5/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ebest-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ebest-0.0.5/PKG-INFO
```

### Comparing `ebest-0.0.4/src/ebest/OpenApi.py` & `ebest-0.0.5/src/ebest/OpenApi.py`

 * *Files 15% similar despite different names*

```diff
@@ -134,26 +134,21 @@
         httpclient.headers["Authorization"] = f"Bearer {token}";
         httpclient.headers["Content-Type"] = "application/json; charset=UTF-8";
         self._access_token = token;
         self._http = httpclient;
         self._connected = True;
         
         # 모의투자인지 실투자인지 구분한다.
-        CSPAQ12300 = dict();
-        CSPAQ12300['CSPAQ12300InBlock1'] = {
-            "BalCreTp":"0",
-            "CmsnAppTpCode":"0",
-            "D2balBaseQryTp":"0",
-            "UprcTpCode":"0",
-        };
+        FOCCQ33600 = dict();
+        FOCCQ33600['FOCCQ33600InBlock1'] = {};
         
-        response = await self.request("CSPAQ12300", CSPAQ12300);
+        response = await self.request("FOCCQ33600", FOCCQ33600);
         if not response :
             self._connected = False;
-            self._last_message = "Failed to require CSPAQ12300";
+            self._last_message = "Failed to require FOCCQ33600";
             await httpclient.close();
             return False;
     
         rsp_msg:str = response.body["rsp_msg"];
         if rsp_msg.__contains__("모의투자"):
             self._is_simulation = True;
```

### Comparing `ebest-0.0.4/src/ebest/tr_code_to_path.py` & `ebest-0.0.5/src/ebest/tr_code_to_path.py`

 * *Files identical despite different names*

### Comparing `ebest-0.0.4/.gitignore` & `ebest-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ebest-0.0.4/LICENSE` & `ebest-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebest-0.0.4/README.md` & `ebest-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 ```bash
 pip install ebest
 ```
 
 ## Usage
 모든 요청은 비동기로 처리되며, 요청에 대한 응답은 await 키워드를 사용하여 받을 수 있습니다.
+<BR/>
+Samples: https://github.com/teranum/ebest-openapi-samples
 
 ### 로그인 요청은 반드시 먼저 수행되어야 하며, 로그인이 성공하면 다른 요청을 수행할 수 있습니다.
 ```python
 import asyncio
 import ebest
 from app_keys import appkey, appsecretkey # app_keys.py 파일에 appkey, appsecretkey 변수를 정의하고 사용하세요
 
 async def main():
     api=ebest.OpenApi()
     if not await api.login(appkey, appsecretkey): return print(f"연결실패: {api.last_message}")
-    print("연결성공, 접속서버: " + "모의투자" if api.is_simulation else "실투자")
+    print("연결성공, 접속서버: " + ("모의투자" if api.is_simulation else "실투자"))
     
     ... # 다른 작업 수행
 
     await api.close()
 
 asyncio.run(main())
 ```
@@ -98,20 +100,20 @@
     
     sAlertNum:str = response.body["t1860OutBlock"]["sAlertNum"]
     if sAlertNum == "":
         print("실시간검색 등록실패")
     else:
         print("실시간검색 등록성공")
         await api.add_realtime("AFR", sAlertNum) # 실시간검색 등록
-        await asyncio.sleep(3600) # 1시간동안 유효, 후에 중지
+        await asyncio.sleep(60) # 60초동안 유효, 후에 중지
         await api.remove_realtime("AFR", sAlertNum) # 실시간검색 중지
 
 def on_realtime(api:ebest.OpenApi, trcode, key, realtimedata):
     if trcode == "AFR":
-        print(f"실시간조건검색 received: {trcode}, {key}, {realtimedata}")
+        print(f"실시간조건검색: {trcode}, {key}, {realtimedata}")
 
 ```
 
 ### 웹소켓 실시간 요청/응답
 ```python
     api.on_realtime = on_realtime # 실시간 이벤트 핸들러 등록
 
@@ -120,10 +122,10 @@
     
     # 60초후 삼성전자 주식 실시간 시세 중지
     await asyncio.sleep(60)
     await api.remove_realtime("S3_", "005930") # 삼성전자 주식 실시간 시세 중지
 
 def on_realtime(api:ebest.OpenApi, trcode, key, realtimedata):
     if trcode == "S3_":
-        print(f"체결시세 received: {trcode}, {key}, {realtimedata}")
+        print(f"체결시세: {trcode}, {key}, {realtimedata}")
 
 ```
```

### Comparing `ebest-0.0.4/pyproject.toml` & `ebest-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ebest"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="teranum", email="teranum@gmail.com" },
 ]
 description = "package for ebest api"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ebest-0.0.4/PKG-INFO` & `ebest-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ebest
-Version: 0.0.4
+Version: 0.0.5
 Summary: package for ebest api
 Project-URL: Homepage, https://github.com/teranum/python-packages/tree/master/ebest
 Project-URL: Issues, https://github.com/teranum/python-packages/issues
 Author-email: teranum <teranum@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,25 +21,27 @@
 
 ```bash
 pip install ebest
 ```
 
 ## Usage
 모든 요청은 비동기로 처리되며, 요청에 대한 응답은 await 키워드를 사용하여 받을 수 있습니다.
+<BR/>
+Samples: https://github.com/teranum/ebest-openapi-samples
 
 ### 로그인 요청은 반드시 먼저 수행되어야 하며, 로그인이 성공하면 다른 요청을 수행할 수 있습니다.
 ```python
 import asyncio
 import ebest
 from app_keys import appkey, appsecretkey # app_keys.py 파일에 appkey, appsecretkey 변수를 정의하고 사용하세요
 
 async def main():
     api=ebest.OpenApi()
     if not await api.login(appkey, appsecretkey): return print(f"연결실패: {api.last_message}")
-    print("연결성공, 접속서버: " + "모의투자" if api.is_simulation else "실투자")
+    print("연결성공, 접속서버: " + ("모의투자" if api.is_simulation else "실투자"))
     
     ... # 다른 작업 수행
 
     await api.close()
 
 asyncio.run(main())
 ```
@@ -113,20 +115,20 @@
     
     sAlertNum:str = response.body["t1860OutBlock"]["sAlertNum"]
     if sAlertNum == "":
         print("실시간검색 등록실패")
     else:
         print("실시간검색 등록성공")
         await api.add_realtime("AFR", sAlertNum) # 실시간검색 등록
-        await asyncio.sleep(3600) # 1시간동안 유효, 후에 중지
+        await asyncio.sleep(60) # 60초동안 유효, 후에 중지
         await api.remove_realtime("AFR", sAlertNum) # 실시간검색 중지
 
 def on_realtime(api:ebest.OpenApi, trcode, key, realtimedata):
     if trcode == "AFR":
-        print(f"실시간조건검색 received: {trcode}, {key}, {realtimedata}")
+        print(f"실시간조건검색: {trcode}, {key}, {realtimedata}")
 
 ```
 
 ### 웹소켓 실시간 요청/응답
 ```python
     api.on_realtime = on_realtime # 실시간 이벤트 핸들러 등록
 
@@ -135,10 +137,10 @@
     
     # 60초후 삼성전자 주식 실시간 시세 중지
     await asyncio.sleep(60)
     await api.remove_realtime("S3_", "005930") # 삼성전자 주식 실시간 시세 중지
 
 def on_realtime(api:ebest.OpenApi, trcode, key, realtimedata):
     if trcode == "S3_":
-        print(f"체결시세 received: {trcode}, {key}, {realtimedata}")
+        print(f"체결시세: {trcode}, {key}, {realtimedata}")
 
 ```
```


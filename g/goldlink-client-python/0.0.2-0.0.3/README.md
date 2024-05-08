# Comparing `tmp/goldlink_client_python-0.0.2-py3-none-any.whl.zip` & `tmp/goldlink_client_python-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 27611 bytes, number of entries: 21
+Zip file size: 27609 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      222 b- defN 24-May-02 21:33 goldlink/__init__.py
--rw-r--r--  2.0 unx     1943 b- defN 24-May-06 00:05 goldlink/constants.py
+-rw-r--r--  2.0 unx     1943 b- defN 24-May-08 04:16 goldlink/constants.py
 -rw-r--r--  2.0 unx      476 b- defN 24-May-02 21:33 goldlink/errors.py
 -rw-r--r--  2.0 unx     6809 b- defN 24-May-02 21:33 goldlink/goldlink_client.py
 -rw-r--r--  2.0 unx     1482 b- defN 24-May-02 21:33 goldlink/helpers.py
 -rw-r--r--  2.0 unx     5256 b- defN 24-May-02 21:33 goldlink/abi/erc20.json
 -rw-r--r--  2.0 unx     4559 b- defN 24-May-02 21:33 goldlink/abi/gmx-frf-account-getters.json
 -rw-r--r--  2.0 unx    82231 b- defN 24-May-02 21:33 goldlink/abi/gmx-frf-strategy-account.json
 -rw-r--r--  2.0 unx    31076 b- defN 24-May-02 21:33 goldlink/abi/gmx-frf-strategy-manager.json
 -rw-r--r--  2.0 unx    97179 b- defN 24-May-06 00:05 goldlink/abi/gmx_v2_reader.json
 -rw-r--r--  2.0 unx     7411 b- defN 24-May-02 21:33 goldlink/abi/strategy-account.json
 -rw-r--r--  2.0 unx    18013 b- defN 24-May-04 01:19 goldlink/abi/strategy-bank.json
 -rw-r--r--  2.0 unx    28277 b- defN 24-May-02 21:33 goldlink/abi/strategy-reserve.json
 -rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:33 integration_tests/__init__.py
 -rw-r--r--  2.0 unx      199 b- defN 24-May-02 21:33 integration_tests/constants.py
 -rw-r--r--  2.0 unx     1144 b- defN 24-May-02 21:33 integration_tests/test_client.py
--rw-r--r--  2.0 unx    11360 b- defN 24-May-06 00:07 goldlink_client_python-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1859 b- defN 24-May-06 00:07 goldlink_client_python-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-06 00:07 goldlink_client_python-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 24-May-06 00:07 goldlink_client_python-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1847 b- defN 24-May-06 00:07 goldlink_client_python-0.0.2.dist-info/RECORD
-21 files, 301462 bytes uncompressed, 24577 bytes compressed:  91.8%
+-rw-r--r--  2.0 unx    11360 b- defN 24-May-08 04:17 goldlink_client_python-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1859 b- defN 24-May-08 04:17 goldlink_client_python-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 04:17 goldlink_client_python-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 24-May-08 04:17 goldlink_client_python-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1847 b- defN 24-May-08 04:17 goldlink_client_python-0.0.3.dist-info/RECORD
+21 files, 301462 bytes uncompressed, 24575 bytes compressed:  91.8%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: integration_tests/constants.py
 Comment: 
 
 Filename: integration_tests/test_client.py
 Comment: 
 
-Filename: goldlink_client_python-0.0.2.dist-info/LICENSE
+Filename: goldlink_client_python-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: goldlink_client_python-0.0.2.dist-info/METADATA
+Filename: goldlink_client_python-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: goldlink_client_python-0.0.2.dist-info/WHEEL
+Filename: goldlink_client_python-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: goldlink_client_python-0.0.2.dist-info/top_level.txt
+Filename: goldlink_client_python-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: goldlink_client_python-0.0.2.dist-info/RECORD
+Filename: goldlink_client_python-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## goldlink/constants.py

```diff
@@ -30,21 +30,21 @@
 
 CONTRACTS = {
     ASSET_USDC: {
         NETWORK_ID_MAINNET: '0xFF970A61A04b1cA14834A43f5dE4533eBDDB5CC8',
         NETWORK_ID_FUJI: '0x3eBDeaA0DB3FfDe96E7a0DBBAFEC961FC50F725F'
     },
     CONTROLLER: {
-        NETWORK_ID_FUJI: '0xD70e13Ad0C3ba99c09a6130602C30Aac0dF41dA9'
+        NETWORK_ID_FUJI: '0x62be6F58cD141542d3e0d1CB1814e2464cbf3462'
     },
     BANK: {
-        NETWORK_ID_FUJI: '0x7D42836DB1CfAd7898B486B9C8265cE8d9c99D71'
+        NETWORK_ID_FUJI: '0xfc8D0b15999b040A2cF1C6fD4ABF18e6f70E84C7'
     },
     RESERVE: {
-        NETWORK_ID_FUJI: '0x6513dDFE61AE59308B8E3D9483Da4579B3477Ff9'
+        NETWORK_ID_FUJI: '0x4b927EC02cFAB1237eA9e13d5568850Dc0FDFBF5'
     }
 }
 COLLATERAL_TOKEN_DECIMALS = 6
 DEFAULT_GAS_PRICE_ADDITION = 3
 
 # ------------ API Defaults ------------
 DEFAULT_API_TIMEOUT = 3000
```

## Comparing `goldlink_client_python-0.0.2.dist-info/LICENSE` & `goldlink_client_python-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `goldlink_client_python-0.0.2.dist-info/METADATA` & `goldlink_client_python-0.0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goldlink-client-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: GoldLink client for borrowing, lending and active management
 Home-page: https://github.com/GoldLink-Protocol/goldlink-client-python
 Author: GoldLink Protocol Inc.
 Author-email: info@goldlink.io
 License: Apache 2.0
 Keywords: goldlink defi arb arbitrum ethereum eth
 Classifier: Intended Audience :: Developers
```

## Comparing `goldlink_client_python-0.0.2.dist-info/RECORD` & `goldlink_client_python-0.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 goldlink/__init__.py,sha256=Ls1exg62LofT6pA3gmSaMZylaVIZ87YYU-u7Ju3caTE,222
-goldlink/constants.py,sha256=ZQ7pmC16lv8100m7qFthJJXUcwf0mW-xOHeNRadXHK4,1943
+goldlink/constants.py,sha256=9YXmea5Rp7k6AoTcPBsQ8q7iqmtpFxZJOdEWTZPRQOg,1943
 goldlink/errors.py,sha256=bsH_zw9AMARtFpgSFEeIWsJX11T592vqNV0ipi1cEYs,476
 goldlink/goldlink_client.py,sha256=hdsKXesYFJ_6yqrdAmArZJouYr6SulzcqEbnbgE5pCI,6809
 goldlink/helpers.py,sha256=poOkkYySgKpAYRU-8uOGXBWC5eKFcLUUQKNvnzPmRVM,1482
 goldlink/abi/erc20.json,sha256=wrlxVrNgoYZcRbj3BSDFjrUz46TYk-oDdVNyQ0NZR9Y,5256
 goldlink/abi/gmx-frf-account-getters.json,sha256=YAGf4tmMYWyyPofK1yIytXvoHlqdbOU5JWGgbRDbE4A,4559
 goldlink/abi/gmx-frf-strategy-account.json,sha256=weLpkYyKrEl1fIpP8k8kAGCx_vxSiPwAZwZdGzqSF6Q,82231
 goldlink/abi/gmx-frf-strategy-manager.json,sha256=mJtYyEJR_AtS0YqIrb-BiiVYBM5NGwYEUChu-ZXumV0,31076
 goldlink/abi/gmx_v2_reader.json,sha256=AZruBAYmD1k1lMgzGIZQvIwrSqN0C32wP3B5ZRXu900,97179
 goldlink/abi/strategy-account.json,sha256=w15Ufw_xGnHCMbsmkz1u_PJlR_JjM2PRDkuMCulH9l8,7411
 goldlink/abi/strategy-bank.json,sha256=sdZmwlr0-5jtY_DxQd7q4XYH-SoEgvzSI-xTdq6oFeI,18013
 goldlink/abi/strategy-reserve.json,sha256=Q358udTuVEYSPn_RDkkboD41l-wl8I_WnkQxe7gfJ5E,28277
 integration_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 integration_tests/constants.py,sha256=mkw1lcY20chfLiEyspzeHcNPJ4hgkL22ySYnZaY6cmU,199
 integration_tests/test_client.py,sha256=qkQ2wfof2isQz4M17gPfujLvE0P43Q9jAs0k0pTDoCg,1144
-goldlink_client_python-0.0.2.dist-info/LICENSE,sha256=z5DWWd5cHmQYJnq4BDt1bmVQjuXY1Qsp6y0v5ETCw-s,11360
-goldlink_client_python-0.0.2.dist-info/METADATA,sha256=MmLfBAcXtJnNtLgjEzSThSyoDpHltS--NeUnv8XOnoc,1859
-goldlink_client_python-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-goldlink_client_python-0.0.2.dist-info/top_level.txt,sha256=PWbc398Pn1hp5G1SohY9CFFP3wujO0e_ou6bzV3xME0,27
-goldlink_client_python-0.0.2.dist-info/RECORD,,
+goldlink_client_python-0.0.3.dist-info/LICENSE,sha256=z5DWWd5cHmQYJnq4BDt1bmVQjuXY1Qsp6y0v5ETCw-s,11360
+goldlink_client_python-0.0.3.dist-info/METADATA,sha256=7b5bmpYIwEhYsaB_glEiQA_k3DkLlDBzrbth9NvJkt8,1859
+goldlink_client_python-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+goldlink_client_python-0.0.3.dist-info/top_level.txt,sha256=PWbc398Pn1hp5G1SohY9CFFP3wujO0e_ou6bzV3xME0,27
+goldlink_client_python-0.0.3.dist-info/RECORD,,
```


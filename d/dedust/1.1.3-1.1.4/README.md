# Comparing `tmp/dedust-1.1.3.tar.gz` & `tmp/dedust-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedust-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dedust-1.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dedust-1.1.3.tar` & `dedust-1.1.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0       17 2023-09-19 13:32:36.953436 dedust-1.1.3/.gitignore
--rw-r--r--   0        0        0     1077 2023-09-19 12:59:05.189083 dedust-1.1.3/LICENSE.md
--rw-r--r--   0        0        0     2540 2024-04-10 18:26:28.499939 dedust-1.1.3/README.md
--rw-r--r--   0        0        0      164 2023-09-19 13:30:44.402665 dedust-1.1.3/dedust/__init__.py
--rw-r--r--   0        0        0       73 2023-09-19 12:59:05.189372 dedust-1.1.3/dedust/constants.py
--rw-r--r--   0        0        0      178 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/__init__.py
--rw-r--r--   0        0        0      120 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/__init__.py
--rw-r--r--   0        0        0      141 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/common/__init__.py
--rw-r--r--   0        0        0     2311 2023-12-11 14:12:15.397622 dedust-1.1.3/dedust/contracts/dex/common/asset.py
--rw-r--r--   0        0        0       95 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/common/asset_error.py
--rw-r--r--   0        0        0       75 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/common/asset_type.py
--rw-r--r--   0        0        0      133 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/common/readiness_status.py
--rw-r--r--   0        0        0       29 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/factory/__init__.py
--rw-r--r--   0        0        0     4168 2023-12-11 14:12:15.398301 dedust-1.1.3/dedust/contracts/dex/factory/factory.py
--rw-r--r--   0        0        0       48 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/liquidity_deposit/__init__.py
--rw-r--r--   0        0        0     3516 2023-12-11 14:12:15.398483 dedust-1.1.3/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py
--rw-r--r--   0        0        0       55 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/pool/__init__.py
--rw-r--r--   0        0        0     3883 2023-12-11 14:12:15.398660 dedust-1.1.3/dedust/contracts/dex/pool/pool.py
--rw-r--r--   0        0        0       76 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/pool/pool_type.py
--rw-r--r--   0        0        0      123 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/vault/__init__.py
--rw-r--r--   0        0        0     2564 2023-12-11 14:12:15.398801 dedust-1.1.3/dedust/contracts/dex/vault/vault.py
--rw-r--r--   0        0        0     2443 2023-12-11 14:12:15.398943 dedust-1.1.3/dedust/contracts/dex/vault/vault_jetton.py
--rw-r--r--   0        0        0     2530 2023-12-11 14:12:15.399101 dedust-1.1.3/dedust/contracts/dex/vault/vault_native.py
--rw-r--r--   0        0        0       76 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/jettons/__init__.py
--rw-r--r--   0        0        0     1591 2023-12-11 14:12:15.399375 dedust-1.1.3/dedust/contracts/jettons/jetton_root.py
--rw-r--r--   0        0        0     2156 2023-12-11 14:12:15.399510 dedust-1.1.3/dedust/contracts/jettons/jetton_wallet.py
--rw-r--r--   0        0        0     2370 2023-12-11 14:12:15.399665 dedust-1.1.3/examples/deposit_liquidity.py
--rw-r--r--   0        0        0      814 2023-12-11 14:12:15.399803 dedust-1.1.3/examples/get_jetton_price.py
--rw-r--r--   0        0        0     1620 2023-12-11 14:12:15.399938 dedust-1.1.3/examples/multihop.py
--rw-r--r--   0        0        0     1310 2023-12-11 14:12:15.400071 dedust-1.1.3/examples/swap_jetton_to_ton.py
--rw-r--r--   0        0        0     1386 2023-12-11 14:12:15.400208 dedust-1.1.3/examples/swap_ton_to_jetton.py
--rw-r--r--   0        0        0      961 2023-12-11 14:12:15.400349 dedust-1.1.3/examples/withdraw_liquidity.py
--rw-r--r--   0        0        0      323 2024-04-10 18:26:12.514335 dedust-1.1.3/pyproject.toml
--rw-r--r--   0        0        0       32 2023-12-11 14:12:15.400647 dedust-1.1.3/requirements.txt
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 dedust-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-09-19 13:32:36.953436 dedust-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1077 2023-09-19 12:59:05.189083 dedust-1.1.4/LICENSE.md
+-rw-r--r--   0        0        0     2622 2024-05-08 18:43:57.048959 dedust-1.1.4/README.md
+-rw-r--r--   0        0        0      164 2023-09-19 13:30:44.402665 dedust-1.1.4/dedust/__init__.py
+-rw-r--r--   0        0        0       73 2023-09-19 12:59:05.189372 dedust-1.1.4/dedust/constants.py
+-rw-r--r--   0        0        0      178 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/__init__.py
+-rw-r--r--   0        0        0      120 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/dex/__init__.py
+-rw-r--r--   0        0        0      141 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/dex/common/__init__.py
+-rw-r--r--   0        0        0     2311 2023-12-11 14:12:15.397622 dedust-1.1.4/dedust/contracts/dex/common/asset.py
+-rw-r--r--   0        0        0       95 2023-09-19 12:59:05.000000 dedust-1.1.4/dedust/contracts/dex/common/asset_error.py
+-rw-r--r--   0        0        0       75 2023-09-19 12:59:05.000000 dedust-1.1.4/dedust/contracts/dex/common/asset_type.py
+-rw-r--r--   0        0        0      133 2023-09-19 12:59:05.000000 dedust-1.1.4/dedust/contracts/dex/common/readiness_status.py
+-rw-r--r--   0        0        0       29 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/dex/factory/__init__.py
+-rw-r--r--   0        0        0     4168 2024-05-08 18:43:22.160754 dedust-1.1.4/dedust/contracts/dex/factory/factory.py
+-rw-r--r--   0        0        0       48 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/dex/liquidity_deposit/__init__.py
+-rw-r--r--   0        0        0     3516 2023-12-11 14:12:15.398483 dedust-1.1.4/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py
+-rw-r--r--   0        0        0       55 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/dex/pool/__init__.py
+-rw-r--r--   0        0        0     3886 2024-05-08 18:41:49.503048 dedust-1.1.4/dedust/contracts/dex/pool/pool.py
+-rw-r--r--   0        0        0       76 2023-09-19 12:59:05.000000 dedust-1.1.4/dedust/contracts/dex/pool/pool_type.py
+-rw-r--r--   0        0        0      123 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/dex/vault/__init__.py
+-rw-r--r--   0        0        0     2557 2024-05-08 18:43:22.160954 dedust-1.1.4/dedust/contracts/dex/vault/vault.py
+-rw-r--r--   0        0        0     2443 2023-12-11 14:12:15.398943 dedust-1.1.4/dedust/contracts/dex/vault/vault_jetton.py
+-rw-r--r--   0        0        0     2553 2024-05-08 18:43:22.161130 dedust-1.1.4/dedust/contracts/dex/vault/vault_native.py
+-rw-r--r--   0        0        0       76 2023-09-19 13:30:44.000000 dedust-1.1.4/dedust/contracts/jettons/__init__.py
+-rw-r--r--   0        0        0     1591 2023-12-11 14:12:15.399375 dedust-1.1.4/dedust/contracts/jettons/jetton_root.py
+-rw-r--r--   0        0        0     2156 2023-12-11 14:12:15.399510 dedust-1.1.4/dedust/contracts/jettons/jetton_wallet.py
+-rw-r--r--   0        0        0     2388 2024-05-08 18:43:22.161465 dedust-1.1.4/examples/deposit_liquidity.py
+-rw-r--r--   0        0        0      846 2024-05-08 18:43:22.161712 dedust-1.1.4/examples/get_jetton_price.py
+-rw-r--r--   0        0        0     1679 2024-05-08 18:43:22.161822 dedust-1.1.4/examples/jetton_multihop.py
+-rw-r--r--   0        0        0     1342 2024-05-08 18:43:22.162596 dedust-1.1.4/examples/swap_jetton_to_ton.py
+-rw-r--r--   0        0        0     1418 2024-05-08 18:43:22.162864 dedust-1.1.4/examples/swap_ton_to_jetton.py
+-rw-r--r--   0        0        0     1575 2024-05-08 18:43:22.162974 dedust-1.1.4/examples/ton_multihop.py
+-rw-r--r--   0        0        0      926 2024-05-08 18:43:22.163140 dedust-1.1.4/examples/withdraw_liquidity.py
+-rw-r--r--   0        0        0      302 2024-05-08 18:43:38.419421 dedust-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       17 2024-05-08 18:43:22.163630 dedust-1.1.4/requirements.txt
+-rw-r--r--   0        0        0     2810 1970-01-01 00:00:00.000000 dedust-1.1.4/PKG-INFO
```

### Comparing `dedust-1.1.3/LICENSE.md` & `dedust-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dedust-1.1.3/README.md` & `dedust-1.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 You can swap tokens, deposit liquidity and many more.
 
 ## Getting Started
 
 ### Dependencies
 
-* httpx
 * pytoniq
 
 ### Installing
 
 ```
 pip install dedust
 ```
@@ -66,20 +65,20 @@
 ## Authors
 
 [@shibdev](https://t.me/dogpy)
 [@VladPavly](https://t.me/dalvpv)
 
 ## Version History
 
-* 1.1.3
-    * Bug fix
+* 1.1.4
+    * Fixed `estimate_deposit_out` get method
 * 1.1.2
-    * Bug fix
+    * Update examples, fix bug with VaultNative
 * 1.1.1
-    * Bug fix
+    * Removed httpx from dependencies
 * 1.1.0
     * Change tonsdk to pytoniq
 * 1.0.5
     * Changes
 * 1.0.4
     * Bug fix
 * 1.0.3
```

### Comparing `dedust-1.1.3/dedust/contracts/dex/common/asset.py` & `dedust-1.1.4/dedust/contracts/dex/common/asset.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.3/dedust/contracts/dex/factory/factory.py` & `dedust-1.1.4/dedust/contracts/dex/factory/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         assets: [Asset, Asset],
         query_id: int = 0
     ) -> Cell:
         return begin_cell()\
             .store_uint(0x97d51f2f, 32)\
             .store_uint(query_id, 64)\
             .store_slice(assets[0].to_slice())\
-            .store_slice(assets[0].to_slice())\
+            .store_slice(assets[1].to_slice())\
             .end_cell()
     
     @staticmethod
     async def get_pool_address(
         pool_type: PoolType,
         assets: [Asset, Asset],
         provider: LiteBalancer
```

### Comparing `dedust-1.1.3/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py` & `dedust-1.1.4/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.3/dedust/contracts/dex/pool/pool.py` & `dedust-1.1.4/dedust/contracts/dex/pool/pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     
     async def get_estimate_deposit_out(
         self,
         amounts: [int, int],
         provider: LiteBalancer
     ) -> list:
         stack = await provider.run_get_method(address=self.address,
-                                              method="estimate_swap_out",
+                                              method="estimate_deposit_out",
                                               stack=amounts)
 
         return {
             "deposits": [stack[0], stack[1]],
             "fair_supply": stack[2]
         }
```

### Comparing `dedust-1.1.3/dedust/contracts/dex/vault/vault.py` & `dedust-1.1.4/dedust/contracts/dex/vault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,10 +65,10 @@
         if _next is None:
             return None
 
         return begin_cell()\
             .store_address(_next.pool_address)\
             .store_uint(0, 1)\
             .store_coins(_next.limit)\
-            .store_maybe_ref(Vault.pack_swap_step(_next.pool_address) if _next._next else None)\
+            .store_maybe_ref(Vault.pack_swap_step(_next._next) if _next._next else None)\
             .end_cell()
```

### Comparing `dedust-1.1.3/dedust/contracts/dex/vault/vault_jetton.py` & `dedust-1.1.4/dedust/contracts/dex/vault/vault_jetton.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.3/dedust/contracts/dex/vault/vault_native.py` & `dedust-1.1.4/dedust/contracts/dex/vault/vault_native.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,10 @@
         return begin_cell()\
             .store_uint(0xea06185d, 32)\
             .store_uint(query_id, 64)\
             .store_coins(amount)\
             .store_address(pool_address)\
             .store_uint(0, 1)\
             .store_coins(limit)\
-            .store_maybe_ref(None)\
+            .store_maybe_ref(Vault.pack_swap_step(_next))\
             .store_ref(Vault.pack_swap_params(swap_params))\
             .end_cell()
```

### Comparing `dedust-1.1.3/dedust/contracts/jettons/jetton_root.py` & `dedust-1.1.4/dedust/contracts/jettons/jetton_root.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.3/dedust/contracts/jettons/jetton_wallet.py` & `dedust-1.1.4/dedust/contracts/jettons/jetton_wallet.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.3/examples/deposit_liquidity.py` & `dedust-1.1.4/examples/deposit_liquidity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dedust import Asset, Factory, PoolType, JettonRoot, JettonWallet, VaultJetton
+from dedust import Asset, Factory, PoolType, JettonRoot, VaultJetton
 import asyncio
 from pytoniq import WalletV4R2, LiteBalancer
 
 mnemonics = ["your", "mnemonics", "here"]
 
 async def main():
     provider = LiteBalancer.from_mainnet_config(1)
@@ -51,8 +51,10 @@
                                                                      target_balances=target_balances)
     )
 
     await wallet.transfer(destination=scale_wallet.address,
                           amount=int(0.5*1e9),
                           body=scale_payload)
 
+    await provider.close_all()
+
 asyncio.run(main())
```

### Comparing `dedust-1.1.3/examples/get_jetton_price.py` & `dedust-1.1.4/examples/get_jetton_price.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,8 +16,10 @@
                                   provider=provider)
                                     
     price = (await pool.get_estimated_swap_out(asset_in=TON,
                                                amount_in=int(10*1e9),
                                                provider=provider))["amount_out"]
     print(f"10 TON = {price / 1e9} SCALE")
 
+    await provider.close_all()
+
 asyncio.run(main())
```

### Comparing `dedust-1.1.3/examples/multihop.py` & `dedust-1.1.4/examples/jetton_multihop.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     SCALE_ADDRESS = "EQBlqsm144Dq6SjbPI4jjZvA1hqTIP3CvHovbIfW_t-SCALE"
     BOLT_ADDRESS = "EQD0vdSA_NedR9uvbgN9EikRX-suesDxGeFg69XQMavfLqIw"
 
     SCALE = Asset.jetton(SCALE_ADDRESS)
     TON = Asset.native()
     BOLT = Asset.jetton(BOLT_ADDRESS)
 
-    TON_SCALE = await Factory.get_pool(PoolType.VOLATILE, [TON, SCALE], provider)
+    # SCALE -> TON -> BOLT
+    TON_SCALE = await Factory.get_pool(PoolType.VOLATILE, [SCALE, TON], provider)
     TON_BOLT = await Factory.get_pool(PoolType.VOLATILE, [TON, BOLT], provider)
 
     scale_vault = await Factory.get_jetton_vault(SCALE_ADDRESS, provider)
     scale_root = JettonRoot.create_from_address(SCALE_ADDRESS)
     scale_wallet = await scale_root.get_wallet(wallet.address, provider)
 
     swap_amount = int(float(input("Enter swap amount(SCALE): ")) * 1e9)
@@ -34,8 +35,10 @@
                                                         _next=SwapStep(pool_address=TON_BOLT.address))
     )
 
     await wallet.transfer(destination=scale_wallet.address,
                           amount=int(0.3*1e9),
                           body=swap)
 
+    await provider.close_all()
+
 asyncio.run(main())
```

### Comparing `dedust-1.1.3/examples/swap_jetton_to_ton.py` & `dedust-1.1.4/examples/swap_jetton_to_ton.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,8 +30,10 @@
         forward_payload=VaultJetton.create_swap_payload(pool_address=pool.address)
     )
 
     await wallet.transfer(destination=scale_wallet.address,
                           amount=int(0.3*1e9),
                           body=swap)
 
+    await provider.close_all()
+
 asyncio.run(main())
```

### Comparing `dedust-1.1.3/examples/swap_ton_to_jetton.py` & `dedust-1.1.4/examples/swap_ton_to_jetton.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,8 +30,10 @@
 
     swap_amount = int(swap_amount + (0.25*1e9)) # 0.25 = gas_value
 
     await wallet.transfer(destination="EQDa4VOnTYlLvDJ0gZjNYm5PXfSmmtL6Vs6A_CZEtXCNICq_", # native vault
                           amount=swap_amount,
                           body=swap)
 
+    await provider.close_all()
+
 asyncio.run(main())
```

### Comparing `dedust-1.1.3/examples/withdraw_liquidity.py` & `dedust-1.1.4/examples/withdraw_liquidity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dedust import Asset, Factory, PoolType, SwapParams, SwapStep, JettonRoot, JettonWallet, VaultJetton, Pool
+from dedust import Asset, Factory, PoolType
 import asyncio
 from pytoniq import WalletV4R2, LiteBalancer
 
 mnemonics = ["your", "mnemonics", "here"]
 
 async def main():
     provider = LiteBalancer.from_mainnet_config(1)
@@ -21,8 +21,10 @@
     burn_payload = lp_wallet.create_burn_payload(
         amount=(await lp_wallet.get_balance(provider))
     )
     await wallet.transfer(destination=lp_wallet.address,
                           amount=int(0.5*1e9),
                           body=burn_payload)
 
+    await provider.close_all()
+
 asyncio.run(main())
```

### Comparing `dedust-1.1.3/PKG-INFO` & `dedust-1.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: dedust
-Version: 1.1.3
+Version: 1.1.4
 Summary: DeDust - DeDust SDK for Python.
 Author: Shibdev, Dalvpv
 Description-Content-Type: text/markdown
-Requires-Dist: httpx==0.19.0
 Requires-Dist: pytoniq>=0.1.19
 
 # DeDust SDK for Python
 
 Analogue of DeDust SDK for Python.
 
 ## Description
 
 You can swap tokens, deposit liquidity and many more.
 
 ## Getting Started
 
 ### Dependencies
 
-* httpx
 * pytoniq
 
 ### Installing
 
 ```
 pip install dedust
 ```
@@ -75,20 +73,20 @@
 ## Authors
 
 [@shibdev](https://t.me/dogpy)
 [@VladPavly](https://t.me/dalvpv)
 
 ## Version History
 
-* 1.1.3
-    * Bug fix
+* 1.1.4
+    * Fixed `estimate_deposit_out` get method
 * 1.1.2
-    * Bug fix
+    * Update examples, fix bug with VaultNative
 * 1.1.1
-    * Bug fix
+    * Removed httpx from dependencies
 * 1.1.0
     * Change tonsdk to pytoniq
 * 1.0.5
     * Changes
 * 1.0.4
     * Bug fix
 * 1.0.3
```


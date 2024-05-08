# Comparing `tmp/unione-0.4.tar.gz` & `tmp/unione-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unione-0.4.tar", last modified: Thu May  2 08:56:30 2024, max compression
+gzip compressed data, was "unione-0.5.tar", last modified: Wed May  8 04:39:23 2024, max compression
```

## Comparing `unione-0.4.tar` & `unione-0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-02 08:56:30.853366 unione-0.4/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-02 08:56:30.853366 unione-0.4/PKG-INFO
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       38 2024-05-02 08:56:30.853366 unione-0.4/setup.cfg
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      213 2024-05-02 08:56:12.000000 unione-0.4/setup.py
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-02 08:56:30.833366 unione-0.4/unilite/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       35 2024-04-29 13:17:00.000000 unione-0.4/unilite/__init__.py
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)     3707 2024-05-01 11:25:04.000000 unione-0.4/unilite/constants.py
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)   108670 2024-05-01 11:28:29.000000 unione-0.4/unilite/contract_maker.py
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-02 08:56:30.853366 unione-0.4/unione.egg-info/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/PKG-INFO
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      224 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/SOURCES.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        1 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/dependency_links.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        5 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/requires.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        8 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/top_level.txt
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-08 04:39:23.590853 unione-0.5/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-08 04:39:23.590853 unione-0.5/PKG-INFO
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       38 2024-05-08 04:39:23.590853 unione-0.5/setup.cfg
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      213 2024-05-08 04:39:21.000000 unione-0.5/setup.py
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-08 04:39:23.587520 unione-0.5/unilite/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       35 2024-04-29 13:17:00.000000 unione-0.5/unilite/__init__.py
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)     3894 2024-05-04 09:26:38.000000 unione-0.5/unilite/constants.py
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)   109121 2024-05-03 05:13:26.000000 unione-0.5/unilite/contract_maker.py
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      652 2024-05-08 04:39:04.000000 unione-0.5/unilite/w3.py
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-08 04:39:23.590853 unione-0.5/unione.egg-info/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-08 04:39:23.000000 unione-0.5/unione.egg-info/PKG-INFO
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      238 2024-05-08 04:39:23.000000 unione-0.5/unione.egg-info/SOURCES.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        1 2024-05-08 04:39:23.000000 unione-0.5/unione.egg-info/dependency_links.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        5 2024-05-08 04:39:23.000000 unione-0.5/unione.egg-info/requires.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        8 2024-05-08 04:39:23.000000 unione-0.5/unione.egg-info/top_level.txt
```

### Comparing `unione-0.4/unilite/constants.py` & `unione-0.5/unilite/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 ETH_MAINNET_RPC = 'https://eth.llamarpc.com'
 CONTRACT_ADDRESS = '0x9DAEa35A922492BE23941De2433D3FD88b3e7cAE'
 UNISWAP_V2_FACTORY = '0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f'
 UNISWAP_V2_ROUTER = '0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D'
 UNISWAP_V3_FACTORY = '0x1F98431c8aD98523631AE4a59f267346ea31F984'
 UNISWAP_V3_ROUTER = '0xE592427A0AEce92De3Edee1F18E0157C05861564'
 UNISWAP_V3_QUOTER = '0xb27308f9F90D607463bb33eA1BeBb41C27CE5AB6'
+SUSHISWAP_V2_FACTORY = '0xC0AEe478e3658e2610c5F7A4A2E1777cE9e4f2Ac'
+SUSHISWAP_V2_ROUTER = '0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F'
 
 NATIVE = "0x0000000000000000000000000000000000000000"
 EEFI = "0x857FfC55B1Aa61A7fF847C82072790cAE73cd883"
 USDC = "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"
+ELON = "0x69420E3A3aa9E17Dea102Bb3a9b3B73dcDDB9528"
 OHM = "0x64aa3364F17a4D01c6f1751Fd97C2BD3D7e7f1D5"
 WETH = "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"
 GDT = "0xc67B12049c2D0CF6e476BC64c7F82fc6C63cFFc5"
 USDT = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 BNB = "0xB8c77482e45F1F44dE1745F52C74426C631bDD52"
 WBTC = "0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599"
 UNI = "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984"
@@ -48,25 +51,25 @@
 DINGER = "0x9e5BD9D9fAd182ff0A93bA8085b664bcab00fA68"
 FLRBRG = "0x9138C8779A0Ac8a84D69617D5715BD8AFa23C650"
 puppies = "0xCF91b70017eABDE82c9671E30e5502D312eA6eb2"
 AIUS = "0x8AFE4055Ebc86Bd2AFB3940c0095C9aca511d852"
 EMRLD = "0xeBB1AFb0A4ddC9b1f84D9Aa72FF956cD1c1Eb4be"
 MFERS = "0xaD913DCD987fE54cE823E4b755F90598Cd62bb15"
 SHIV = "0xEb51B8dC2d43469c0F0b7365c8a18438907BDf21"
-SEXY = "0xc52FaFDc900cB92Ae01E6E4F8979aF7f436e2EB2"
 NXRA = "0x644192291cc835A93d6330b24EA5f5FEdD0eEF9e"
 FLT = "0x236501327e701692a281934230AF0b6BE8Df3353"
 WMC = "0x7Fd4d7737597E7b4ee22AcbF8D94362343ae0a79"
 SBEE = "0x7Ae0f19D2aE2f490e710579284A58000d4E8C85f"
 BEPRO = "0xCF3C8Be2e2C42331Da80EF210e9B1b307C03d36A"
 LMEOW = "0x1aE7e1d0ce06364CED9aD58225a1705b3e5DB92b"
 CLOSEDAI = "0x50B0696468F42CaB1ddc76413A1312Aff3cAbdf6"
 PEPE = "0x6982508145454Ce325dDbE47a25d4ec3d2311933"
 CSWAP = "0xae41b275aaAF484b541A5881a2dDED9515184CCA"
 ZYN = "0x58cB30368ceB2d194740b144EAB4c2da8a917Dcb"
+SEXY = "0xc52FaFDc900cB92Ae01E6E4F8979aF7f436e2EB2"
 HEX = "0x2b591e99afE9f32eAA6214f7B7629768c40Eeb39"
 
 
 HAY_WETH_FEE = 10000
 NODE_URL = "https://eth.llamarpc.com"
 NODE_URL2 = "https://eth.drpc.org"
 NODE_URL3 = "https://api.securerpc.com/v1"
```

### Comparing `unione-0.4/unilite/contract_maker.py` & `unione-0.5/unilite/contract_maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -4223,7 +4223,20 @@
 
 def get_bot_contract():
     return w3.eth.contract(address=constants.CONTRACT_ADDRESS, abi=contract_abi)
 
 
 def get_uniswap_v3_quoter():
     return w3.eth.contract(address=constants.UNISWAP_V3_QUOTER, abi=uniswap_v3_quoter_abi)
+
+
+def get_sushiswap_v2_factory():
+    return w3.eth.contract(address=constants.SUSHISWAP_V2_FACTORY, abi=uniswap_v2_factory_abi)
+
+
+def get_sushiswap_v2_router():
+    return w3.eth.contract(address=constants.SUSHISWAP_V2_ROUTER, abi=uniswap_v2_router_abi)
+
+
+def get_sushiswap_v2_pool(token0, token1):
+    address = get_sushiswap_v2_factory().functions.getPair(token0, token1).call()
+    return w3.eth.contract(address=address, abi=uniswap_v2_pool_abi)
```


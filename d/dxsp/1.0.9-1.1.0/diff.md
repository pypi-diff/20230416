# Comparing `tmp/dxsp-1.0.9.tar.gz` & `tmp/dxsp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.0.9.tar", max compression
+gzip compressed data, was "dxsp-1.1.0.tar", max compression
```

## Comparing `dxsp-1.0.9.tar` & `dxsp-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-13 14:38:11.405686 dxsp-1.0.9/LICENSE
--rw-r--r--   0        0        0     2877 2023-04-13 14:38:11.405686 dxsp-1.0.9/README.md
--rw-r--r--   0        0        0      137 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8589 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    16065 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/main.py
--rw-r--r--   0        0        0      678 2023-04-13 14:38:12.053685 dxsp-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-16 10:14:29.297165 dxsp-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-16 10:14:29.297165 dxsp-1.1.0/README.md
+-rw-r--r--   0        0        0      136 2023-04-16 10:14:30.049179 dxsp-1.1.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-16 10:14:29.297165 dxsp-1.1.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-16 10:14:29.297165 dxsp-1.1.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    22794 2023-04-16 10:14:29.297165 dxsp-1.1.0/dxsp/main.py
+-rw-r--r--   0        0        0      916 2023-04-16 10:14:30.049179 dxsp-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 dxsp-1.1.0/PKG-INFO
```

### Comparing `dxsp-1.0.9/LICENSE` & `dxsp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.9/README.md` & `dxsp-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # DXSP (DeX SwaP)
-A python defi swap helper package. Swap made easy.
 
-<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">
 
+|<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy. |
+| ------------- | ------------- |
+|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![🐍Build](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml) ![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
-- 7 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
+
+
+Key features:
+
+- 24 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
 - 2 swap protocol type supported:
 	- 1inch API v5
 	- Uniswap version 2 router protocol type
 
 Other features:
 - Translate token symbol to contract address via user defined tokenlist format or coingecko api 
 - Connect to web3  if no web3 object or no rpc provided
 - Able to approve contract and sign transaction
 - Quote for a given token
 - Use Base symbol like stablecoin
 
-[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/)
-![Pypi](https://img.shields.io/pypi/dm/dxsp) ![Version](https://img.shields.io/pypi/v/dxsp)
-
-[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko) 
 
-[![🐍Build](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml)
 
 # Install
 `pip install dxsp`
 
 # How to use it
 ```
 from dxsp import DexSwap
```

### Comparing `dxsp-1.0.9/dxsp/assets/blockchains.py` & `dxsp-1.1.0/dxsp/assets/blockchains.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,19 @@
         "rpc": "https://rpc.ankr.com/eth_goerli",
         "uniswap_v2": "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D",
         "uniswap_v3": "",
         "1inch": "",
         "1inch_limit": "",
         "0x": "https://goerli.api.0x.org/"
     },
-    # Optimism
-    10: {
-        "block_explorer_url": "https://api-optimistic.etherscan.io/api?",
-        "rpc": "https://rpc.ankr.com/optimism",
-        "uniswap_v2": "0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f",
-        "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
-        "1inch": "https://api.1inch.exchange/v5.0/10",
-        "1inch_limit": "https://limit-orders.1inch.io/v3.0/10",
-        "0x": "https://optimism.api.0x.org/"
-    },
     # ETHEREUM Sepolia
     11155111: {
         "block_explorer_url": "https://api-Sepolia.etherscan.io/api?",
         "rpc": "https://rpc.ankr.com/eth_sepolia",
-        "uniswap_v2": "",
+        "uniswap_v2": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
         "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
         "1inch": "",
         "1inch_limit": "",
         "0x": "https://sepolia.api.0x.org/"
         },
     # Binance Smart Chain
     56: {
@@ -77,15 +67,15 @@
         "uniswap_v3": "",
         "1inch": "",
         "1inch_limit": "",
         "0x": ""
         },
     # Polygon
     137: {
-        "url": "https://api.polygonscan.com/api?",
+        "block_explorer_url": "https://api.polygonscan.com/api?",
         "rpc": "https://rpc.ankr.com/polygon",
         "uniswap_v2": "0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f",
         "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
         "1inch": "https://api.1inch.exchange/v5.0/137",
         "1inch_limit": "https://api.1inch.exchange/v5.0/137",
         "0x": "https://polygon.api.0x.org/"
     },
@@ -97,33 +87,42 @@
         "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
         "1inch": "",
         "1inch_limit": "",
         "0x": "https://mumbai.api.0x.org/"
         },
     # Polygon zkEVM
     1101: {
-        "url": "",
+        "block_explorer_url": "",
         "rpc": "https://rpc.ankr.com/polygon_zkevm",
         "uniswap_v2": "",
         "uniswap_v3": "",
         "1inch": "",
         "1inch_limit": "h",
         "0x": ""
     },
     # Polygon zkEVM testnet
     1442: {
-        "url": "",
+        "block_explorer_url": "",
         "rpc": "https://rpc.ankr.com/polygon_zkevm_testnet",
         "uniswap_v2": "",
         "uniswap_v3": "",
         "1inch": "",
         "1inch_limit": "h",
         "0x": ""
     },
-
+    # Optimism
+    10: {
+        "block_explorer_url": "https://api-optimistic.etherscan.io/api?",
+        "rpc": "https://rpc.ankr.com/optimism",
+        "uniswap_v2": "0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f",
+        "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
+        "1inch": "https://api.1inch.exchange/v5.0/10",
+        "1inch_limit": "https://limit-orders.1inch.io/v3.0/10",
+        "0x": "https://optimism.api.0x.org/"
+    },
     # Optimism goerli
     69: {
         "block_explorer_url": "https://api-Goerli.etherscan.io/api? ne",
         "rpc": "https://rpc.ankr.com/optimism_testnet",
         "uniswap_v2": "",
         "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
         "1inch": "",
```


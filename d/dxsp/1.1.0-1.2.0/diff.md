# Comparing `tmp/dxsp-1.1.0.tar.gz` & `tmp/dxsp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.1.0.tar", max compression
+gzip compressed data, was "dxsp-1.2.0.tar", max compression
```

## Comparing `dxsp-1.1.0.tar` & `dxsp-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-16 10:14:29.297165 dxsp-1.1.0/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-16 10:14:29.297165 dxsp-1.1.0/README.md
--rw-r--r--   0        0        0      136 2023-04-16 10:14:30.049179 dxsp-1.1.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-16 10:14:29.297165 dxsp-1.1.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-16 10:14:29.297165 dxsp-1.1.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    22794 2023-04-16 10:14:29.297165 dxsp-1.1.0/dxsp/main.py
--rw-r--r--   0        0        0      916 2023-04-16 10:14:30.049179 dxsp-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 dxsp-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-16 12:53:25.232962 dxsp-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-16 12:53:25.232962 dxsp-1.2.0/README.md
+-rw-r--r--   0        0        0      136 2023-04-16 12:53:26.152967 dxsp-1.2.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-16 12:53:25.232962 dxsp-1.2.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-16 12:53:25.232962 dxsp-1.2.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    26954 2023-04-16 12:53:25.236962 dxsp-1.2.0/dxsp/main.py
+-rw-r--r--   0        0        0      929 2023-04-16 12:53:26.152967 dxsp-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 dxsp-1.2.0/PKG-INFO
```

### Comparing `dxsp-1.1.0/LICENSE` & `dxsp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.1.0/README.md` & `dxsp-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.1.0/dxsp/assets/blockchains.py` & `dxsp-1.2.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.1.0/dxsp/main.py` & `dxsp-1.2.0/dxsp/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 import asyncio
 
 import logging
 
 from dotenv import load_dotenv
 
 from web3 import Web3
+from datetime import datetime
 from pycoingecko import CoinGeckoAPI
 
 from dxsp.assets.blockchains import blockchains
 
+from ping3 import ping
+
 class DexSwap:
 
 
     def __init__(self,
                  chain_id: int = 1, 
                  wallet_address: str = None,
                  private_key: str = None,
                  block_explorer_api: str = None,
                  block_explorer_url: str = None,
                  rpc: str = None,
                  w3: Web3 = None,
                  protocol_type: str = None,
                  dex_exchange: str = None,
+                 dex_router: str = None,
                  base_trading_symbol: str = None,
                  amount_trading_option: int = 1,
                  ):
 
         self.logger =  logging.getLogger(__name__)
         self.logger.debug(f"DXSP Logger:  {self.logger} on {__name__}")
         self.logger.info(f"Initializing DexSwap object for {wallet_address} on {chain_id}")
@@ -56,18 +60,28 @@
         self.logger.debug(f"self.block_explorer_url {self.block_explorer_url}")
 
         self.rpc = rpc
         if self.rpc is None:
             self.rpc = blockchain["rpc"]
         self.logger.debug(f"self.rpc {self.rpc}")
 
+        self.latency = round(ping(self.rpc, unit='ms'), 3)
+        self.logger.debug(f"self.latency {self.latency}")    
+
         self.w3 = w3
         if self.w3 is None:
             self.w3 = Web3(Web3.HTTPProvider(self.rpc))
+            try:
+                self.w3.net.listening
+                logger.info(msg=f"connected to {w3}")
+            except Exception as e:
+                logger.error(msg=f"connectivity failed using {rpc}")
+                return
         self.logger.debug(f"self.w3 {self.w3}")
+            logger.info(msg=f"connected to {ex}")
 
         self.protocol_type = protocol_type
         if self.protocol_type is None:
             if self.protocol_type == "0x":
                 base_url = blockchain["0x"]
             elif self.protocol_type == "1inch_limit":
                 base_url = blockchain["1inch_limit"]
@@ -77,37 +91,45 @@
             self.dex_url = f"{base_url}"
 
         self.logger.debug(f"self.dex_url {self.dex_url}")
         self.logger.debug(f"self.protocol_type {self.protocol_type}")
 
         self.dex_exchange = dex_exchange
         self.logger.debug(f"self.dex_exchange {self.dex_exchange}")
-        if (
-            self.dex_exchange is None
-            or self.dex_exchange != blockchain["uniswap_v3"]
-        ):
-            self.router = blockchain["uniswap_v2"]
-        else:
-            self.router = blockchain["uniswap_v3"]
+
+        self.dex_router = dex_router
+        if self.dex_router is None:
+            if (
+                self.dex_exchange is None
+                or self.dex_exchange != blockchain["uniswap_v3"]
+            ):
+                self.router = blockchain["uniswap_v2"]
+            else:
+                self.router = blockchain["uniswap_v3"]
         self.logger.debug(f"self.router {self.router}")
 
+        self.logger.debug(f"self.name {self.name}")        
+
         self.base_trading_symbol = base_trading_symbol
         if self.base_trading_symbol is None:
             self.base_trading_symbol= 'USDC'
         self.logger.debug(f"self.base_trading_symbol {self.base_trading_symbol}")
 
         self.amount_trading_option = amount_trading_option
         self.logger.debug(f"self.amount_trading_option {self.amount_trading_option}")
 
         self.gecko_api = CoinGeckoAPI() # llama_api = f"https://api.llama.fi/" maybe as backup to be reviewed
         assetplatform = self.gecko_api.get_asset_platforms()
         output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
         self.gecko_platform = output_dict[0]['id']
         self.logger.debug(f"self.gecko_platform {self.gecko_platform}")
 
+        # global gasPrice
+        # global gasLimit
+
     async def _get(self, url, params=None, headers=None):
         headers = { "User-Agent": "Mozilla/5.0" }
         #self.logger.debug(f"_get url {url}")
         response = requests.get(url,params =params,headers=headers)
         #self.logger.debug(f"response _get {response}")
         return response.json()
 
@@ -198,24 +220,24 @@
                 'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
                 }
                 tx = tx.build_transaction(tx_params)
             elif self.protocol_type in ['uniswap_v3']:
                 tx_params = {
                 'from': self.wallet_address,
                 'gas': await estimate_gas(tx),
-                'gasPrice': self.w3.to_wei(gasPrice,'gwei'),
+                'gasPrice': await self.get_gasPrice(tx),
                 'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
                 }
                 tx = tx.build_transaction(tx_params)
             elif self.protocol_type in ["1inch","1inch_limit"]:
                 tx = tx['tx']
                 tx['gas'] = await estimate_gas(tx)
                 tx['nonce'] = self.w3.eth.get_transaction_count(self.wallet_address)
                 tx['value'] = int(tx['value'])
-                tx['gasPrice'] = int(ex.to_wei(gasPrice,'gwei'))
+                tx['gasPrice'] = await self.get_gasPrice(tx)
             signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
             raw_tx = signed.rawTransaction
             return self.w3.eth.send_raw_transaction(raw_tx)
         except Exception as e:
             self.logger.debug(f"error get_sign {e}")
             return
 
@@ -225,32 +247,41 @@
         return int(self.w3.to_wei(gasestimate,'wei'))
 
     async def get_gasPrice(self, tx):
         self.logger.debug(f"get_gasPrice {tx}")
         gasprice= self.w3.eth.generate_gas_price()
         return self.w3.to_wei(gasPrice,'gwei')
 
-    async def execute_order(self,direction,symbol,stoploss=10000,takeprofit=10000,quantity=1,amount_trading_option=1):
-        self.logger.debug(f"execute_order {direction} {symbol}")
-        try:
-            asset_out_symbol = self.base_trading_symbol if direction=="BUY" else symbol
-            asset_in_symbol = symbol if direction=="BUY" else self.base_trading_symbol
-            asset_out_contract = await self.get_token_contract(asset_out_symbol)
-            asset_out_decimals = asset_out_contract.functions.decimals().call()
-            asset_out_balance = await self.get_token_balance(asset_out_symbol)
-            if amount_trading_option == 1:
-                asset_out_amount = ((asset_out_balance)/(10 ** asset_out_decimals))*(float(quantity)/100) #buy or sell %p percentage DEFAULT OPTION
-            if amount_trading_option == 2:
-                asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals) #SELL all token in case of sell order for example
-      
-            swap = self.get_swap(asset_out_symbol,asset_in_symbol,asset_out_amount)
+    async def execute_order(self,direction,symbol,stoploss=10000,takeprofit=10000,quantity=1,amount_trading_option=1,order_type='swap'):
+        self.logger.debug(f"execute_order {direction} {symbol} {order_type}")
+        if order_type == 'swap'
+            self.logger.debug(f"execute_order {order_type}")
+            try:
+                asset_out_symbol = self.base_trading_symbol if direction=="BUY" else symbol
+                asset_in_symbol = symbol if direction=="BUY" else self.base_trading_symbol
+                asset_out_contract = await self.get_token_contract(asset_out_symbol)
+                asset_out_decimals = asset_out_contract.functions.decimals().call()
+                asset_out_balance = await self.get_token_balance(asset_out_symbol)
+                if amount_trading_option == 1:
+                    asset_out_amount = ((asset_out_balance)/(10 ** asset_out_decimals))*(float(quantity)/100) #buy or sell %p percentage DEFAULT OPTION
+                if amount_trading_option == 2:
+                    asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals) #SELL all token in case of sell order for example
+          
+                swap = self.get_swap(asset_out_symbol,asset_in_symbol,asset_out_amount)
 
-        except Exception as e:
-            self.logger.debug(f"error execute_order {e}")
-            return  
+            except Exception as e:
+                self.logger.debug(f"error execute_order {e}")
+                return
+
+        if order_type == 'market'
+            self.logger.debug(f"execute_order {order_type}")
+            return
+        if order_type == 'limit'
+            self.logger.debug(f"execute_order {order_type}")
+            return
 
     async def get_swap(self, 
             asset_out_symbol: str, 
             asset_in_symbol: str,
             amount: int, 
             slippage_tolerance_percentage = 2 
         ):
@@ -325,14 +356,21 @@
             if swap_TX:
                 self.logger.debug(f"swap_TX {swap_TX}")
                 signed_TX = await self.get_sign(swap_TX)
                 txHash = str(self.w3.to_hex(signed_TX))
                 txResult = await self.get_block_explorer_status(txHash)
                 txHashDetail= self.w3.wait_for_transaction_receipt(txHash, timeout=120, poll_latency=0.1)
                 if(txResult == "1"):
+                    order={}
+                    d['id'] = '15222'
+                    d['datetime'] = datetime.now()
+                    d['gasUsed'] = txHashDetail['gasUsed']
+                    d['id'] = '15222'
+                    d['amount'] = 'host name'
+                    d['price'] = '15222'
                     return txHash
         except Exception as e:
             self.logger.debug(f"error get_swap {e}")
             return
 
     async def get_block_explorer_status(self,txHash):
         self.logger.debug(f"get_block_explorer_status {txHash}")
@@ -411,15 +449,14 @@
                 coin_info['platforms'][f'{self.gecko_platform}']
                 self.logger.debug(f"🦎search_gecko_coin_info {coin_info} {token}")
                 return coin_info['platforms'][f'{self.gecko_platform}']
         except Exception as e:
             self.logger.debug(f"error search_gecko_contract {e}")
             return
 
-
     async def get_contract_address(self,token_list_url, symbol):
         self.logger.debug(f"get_contract_address {token_list_url} {symbol}")
         try: 
             token_list = await self._get(token_list_url)
             #self.logger.debug(f"token_list {token_list}")
             token_search = token_list['tokens']
             for keyval in token_search:
@@ -428,43 +465,98 @@
         except Exception as e:
             self.logger.debug(f"error get_contract_address {e}")
             return
 
     async def get_token_contract(self, token):
         self.logger.debug(f"get_token_contract {token}")
         try:
-            token_address= await self.search_contract(token)
-            token_abi= await self.get_abi(token_address)
+            token_address = await self.search_contract(token)
+            token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
-            self.logger.debug(f"error  get_token_contract {e}")
+            self.logger.error(f"error  get_token_contract {e}")
             return
 
     async def get_token_balance(self, token):
         self.logger.debug(f"get_token_balance {token}")
         try:
-            token_contract = await self.get_token_contract(token)
+            token_address = await self.search_contract(token)
+            token_abi =  await self.get_abi(token_address)
+            token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
             token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
+            logger.debug(msg=f"token_address {token_address} token_balance {token_balance}")
+            # (ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
             return 0 if token_balance <=0 or token_balance is None else token_balance
         except Exception as e:
-            self.logger.debug(f"error get_token_balance {e}")
+            logger.error(msg=f"{token} get_token_balance error: {e}")
             return 0
 
+    async def get_basecoin_balance(self):
+        bal_base_trading_symbol = await self.get_token_balance(self.base_trading_symbol)
+            # return round(ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
+        return bal_base_trading_symbol
+        # bal = round(ex.from_wei(bal,'ether'),5)
+
     async def get_stablecoin_balance(self):
         toptokens = ["USDT","USDC","BUSD","DAI"]
         for i in toptokens:
-            bal_toptoken = await get_token_balance(i)
+            bal_toptoken = await self.get_token_balance(i)
             if bal_toptoken:
                 msg += f"\n💵{bal_toptoken} {i}"
             # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_balance(self):
         toptokens = ["WBTC","ETH","BNB","UNI"]
         for i in toptokens:
-            bal_toptoken = await get_token_balance(i)
+            bal_toptoken = await self.get_token_balance(i)
             if bal_toptoken:
                 msg += f"\n💵{bal_toptoken} {i}"
             # bal = round(ex.from_wei(bal,'ether'),5)
 
+    async def get_account_position(self):
+        self.logger.debug(f"get_account_position")
+        try:
+            # asset_position_address= await search_contract(asset_out_symbol)
+            # asset_position_abi= await fetch_abi_dex(asset_out_address)
+            # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
+            # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
+            return
+        except Exception as e:
+            logger.error(msg=f"get_account_position error: {e}")
+            return 0
 
 
+    # async def fetch_account_dex(addr):
+    #     url = block_explorer_url
+    #     query = {'module':'account',
+    #             'action':'tokenbalance',
+    #             'contractaddress':addr,
+    #             'address':walletaddress,
+    #             'tag':'latest',
+    #             'apikey':block_explorer_api}
+    #     r = requests.get(url, params=query)
+    #     try:
+    #         d = json.loads(r.text)
+    #     except:
+    #         return None
+    #     return int(d['result']) / self.zeroes
+
+
+#     async def fetch_gecko_asset_price(token):
+#     try:
+#         asset_in_address = ex.to_checksum_address(await search_contract(token))
+#         fetch_tokeninfo = gecko_api.get_coin_info_from_contract_address_by_id(id=f'{coin_platform}',contract_address=asset_in_address)
+#         return fetch_tokeninfo['market_data']['current_price']['usd']
+#     except Exception:
+#         return
+
+# async def fetch_gecko_quote(token):
+#     try:
+#         asset_in_address = ex.to_checksum_address(await search_contract(token))
+#         fetch_tokeninfo = gecko_api.get_coin_info_from_contract_address_by_id(id=f'{coin_platform}',contract_address=asset_in_address)
+#         logger.debug(msg=f"fetch_tokeninfo {fetch_tokeninfo}")
+#         asset_out_cg_quote = fetch_tokeninfo['market_data']['current_price']['usd']
+#         asset_out_cg_name = fetch_tokeninfo['name']
+#         return f"{asset_out_cg_name}\n🦎{asset_out_cg_quote} USD"
+#     except Exception:
+#         return
```

### Comparing `dxsp-1.1.0/pyproject.toml` & `dxsp-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.1.0"
+version = "1.2.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
+asyncio = "*"
+python-dotenv = "*"
 web3 = ">=6.*"
 pycoingecko = "*"
-python-dotenv = "*"
-asyncio ="*"
+ping3 = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dxsp-1.1.0/PKG-INFO` & `dxsp-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.1.0
+Version: 1.2.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio
+Requires-Dist: ping3
 Requires-Dist: pycoingecko
 Requires-Dist: python-dotenv
 Requires-Dist: web3 (>=6)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
```


# Comparing `tmp/dxsp-3.1.3.tar.gz` & `tmp/dxsp-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.1.3.tar", max compression
+gzip compressed data, was "dxsp-3.1.4.tar", max compression
```

## Comparing `dxsp-3.1.3.tar` & `dxsp-3.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-02 20:01:58.405334 dxsp-3.1.3/LICENSE
--rw-r--r--   0        0        0     2378 2023-07-02 20:01:58.405334 dxsp-3.1.3/README.md
--rw-r--r--   0        0        0      114 2023-07-02 20:01:59.369343 dxsp-3.1.3/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-02 20:01:58.405334 dxsp-3.1.3/dxsp/config.py
--rw-r--r--   0        0        0     8093 2023-07-02 20:01:58.405334 dxsp-3.1.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    15424 2023-07-02 20:01:58.405334 dxsp-3.1.3/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-02 20:01:58.405334 dxsp-3.1.3/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-02 20:01:58.405334 dxsp-3.1.3/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     2645 2023-07-02 20:01:58.405334 dxsp-3.1.3/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-02 20:01:58.405334 dxsp-3.1.3/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2144 2023-07-02 20:01:59.369343 dxsp-3.1.3/pyproject.toml
--rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 dxsp-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-03 00:29:11.034198 dxsp-3.1.4/LICENSE
+-rw-r--r--   0        0        0     2378 2023-07-03 00:29:11.034198 dxsp-3.1.4/README.md
+-rw-r--r--   0        0        0      114 2023-07-03 00:29:11.842202 dxsp-3.1.4/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/config.py
+-rw-r--r--   0        0        0     8093 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    15255 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     4000 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2144 2023-07-03 00:29:11.838201 dxsp-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 dxsp-3.1.4/PKG-INFO
```

### Comparing `dxsp-3.1.3/LICENSE` & `dxsp-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.3/README.md` & `dxsp-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.3/dxsp/default_settings.toml` & `dxsp-3.1.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.3/dxsp/main.py` & `dxsp-3.1.4/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,72 +24,68 @@
                 self.logger.info("connected %s",self.w3)
         except Exception as error:
             raise error
 
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
-        self.account = f"{str(self.chain_id)} - {str(self.wallet_address[-8:])}"
+        self.account = f"{str(self.w3.net.version)} - {str(self.wallet_address[-8:])}"
         self.private_key = settings.dex_private_key
         self.trading_asset_address = self.w3.to_checksum_address(
             settings.trading_asset_address)
         self.cg = CoinGeckoAPI()
                     
         self.protocol_type = settings.dex_protocol_type
         self.dex_swap = None
         self.router = None
         self.quoter = None
 
-
     async def get_protocol(self):
         """ protocol init """
         from dxsp.protocols import DexSwapUniswap, DexSwapZeroX, DexSwapOneInch
         if self.protocol_type == "0x":
             self.dex_swap = DexSwapZeroX()
         elif self.protocol_type == "1inch":
             self.dex_swap = DexSwapOneInch()
         else:
             self.dex_swap = DexSwapUniswap()
 
-
     async def execute_order(self, order_params):
         """ Execute swap function. """
         try:
             action = order_params.get('action')
             instrument = order_params.get('instrument')
             quantity = order_params.get('quantity', 1)
             sell_token, buy_token = (
                 (self.trading_asset_address, instrument)
                 if action == 'BUY'
                 else (instrument, self.trading_asset_address))
             order = await self.get_swap(sell_token, buy_token, quantity)
             if order:
-                    trade_confirmation = (
-                        f"⬇️ {instrument}" if (action == "SELL") else f"⬆️ {instrument}\n")
-                    trade_confirmation += order
-                    return trade_confirmation
+                trade_confirmation = (
+                    f"⬇️ {instrument}" if (action == "SELL") else f"⬆️ {instrument}\n")
+                trade_confirmation += order
+                return trade_confirmation
 
         except Exception as error:
             return f"⚠️ order execution: {error}"
 
     async def get_swap(self, sell_token: str, buy_token: str, quantity: int) -> None:
         """ Main swap function """
         try:
             await self.get_protocol()
             sell_token_address = sell_token
             if not sell_token.startswith("0x"):
                 sell_token_address = await self.search_contract_address(sell_token)
-            sell_token_balance = await self.get_token_balance(sell_token_address)
             buy_token_address = buy_token
             if not buy_token_address.startswith("0x"):   
                 buy_token_address = await self.search_contract_address(buy_token)
             sell_amount = await self.calculate_sell_amount(sell_token_address, quantity)
-            sell_token_amount_wei = self.w3.to_wei(
-                sell_amount * 10 ** (await self.get_token_decimals(sell_token_address)), "ether")
-
+            sell_token_amount_wei = sell_amount * (10 ** (
+                await self.get_token_decimals(sell_token_address)))
             await self.get_approve(sell_token_address)
 
             order_amount = int(sell_token_amount_wei * (settings.dex_trading_slippage / 100))
             order = await self.dex_swap.get_swap(sell_token_address, buy_token_address, order_amount)
 
             if not order:
                 raise ValueError("swap order not executed")
@@ -102,90 +98,93 @@
                 raise ValueError("receipt failed")
 
             return await self.get_confirmation(receipt['transactionHash'])
 
         except ValueError as error:
             raise error
 
-
     async def get_quote(self, sell_token):
         """ gets a quote for a token """
         try:
             await self.get_protocol()
             buy_address = self.trading_asset_address
             sell_address = await self.search_contract_address(sell_token)
             quote = await self.dex_swap.get_quote(buy_address, sell_address)
             return f"🦄 {quote} {settings.trading_asset}"
         except Exception as error:
             return f"⚠️: {error}"
 
-
     async def get_approve(self, token_address):
         """ approve a token """
         try:
             contract = await self.get_token_contract(token_address)
             if contract is None:
                 return
             approved_amount = self.w3.to_wei(2 ** 64 - 1, 'ether')
             owner_address = self.w3.to_checksum_address(self.wallet_address)
-            dex_router_address = self.w3.to_checksum_address(settings.dex_router_contract_addr)
-            allowance = contract.functions.allowance(owner_address, dex_router_address).call()
+            dex_router_address = self.w3.to_checksum_address(
+                settings.dex_router_contract_addr)
+            allowance = contract.functions.allowance(
+                owner_address, dex_router_address).call()
             if allowance == 0:
-                approval_tx = contract.functions.approve(dex_router_address, approved_amount)
+                approval_tx = contract.functions.approve(
+                    dex_router_address, approved_amount)
                 approval_tx_hash = await self.get_sign(approval_tx.transact())
-                return self.w3.eth.wait_for_transaction_receipt(approval_tx_hash)
+                return self.w3.eth.wait_for_transaction_receipt(
+                    approval_tx_hash)
         except Exception as error:
             raise ValueError(f"Approval failed {error}") 
 
-
     async def get_sign(self, transaction):
         """ sign a transaction """
         try:
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 transaction_params = {
                     'from': self.wallet_address,
                     'gas': await self.get_gas(transaction),
                     'gasPrice': await self.get_gas_price(),
                     'nonce': self.w3.eth.get_transaction_count(
                         self.wallet_address),
                 }
                 transaction = transaction.build_transaction(transaction_params)
             signed_tx = self.w3.eth.account.sign_transaction(
                 transaction, self.private_key)
-            raw_tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
+            raw_tx_hash = self.w3.eth.send_raw_transaction(
+                signed_tx.rawTransaction)
             return self.w3.to_hex(raw_tx_hash)
         except Exception as error:
             raise error
 
 ### ------🛠️ W3 UTILS ---------
     async def get(self, url, params=None, headers=None):
         """ gets a url payload """
         try:
             self.logger.debug(f"Requesting URL: {url}")
-            response = requests.get(url, params=params, headers=headers, timeout=10)
+            response = requests.get(
+                url, params=params, headers=headers, timeout=10)
             if response.status_code == 200:
                 return response.json()
 
         except Exception as error:
             raise error
 
-    async def router_contract(self):
-        """ create a router contract """
-        try:
-            router_abi = await self.get(settings.dex_router_abi_url)
-            self.router = self.w3.eth.contract(
-                address=self.w3.to_checksum_address(
-                    settings.dex_router_contract_addr
-                ),
-                abi=router_abi,
-            )
-            if self.router.functions is None:
-                raise ValueError("Router/Chain setup incorrect")
-        except Exception as error:
-            raise error
+    # async def router_contract(self):
+    #     """ create a router contract """
+    #     try:
+    #         router_abi = await self.get(settings.dex_router_abi_url)
+    #         self.router = self.w3.eth.contract(
+    #             address=self.w3.to_checksum_address(
+    #                 settings.dex_router_contract_addr
+    #             ),
+    #             abi=router_abi,
+    #         )
+    #         if self.router.functions is None:
+    #             raise ValueError("Router/Chain setup incorrect")
+    #     except Exception as error:
+    #         raise error
 
     # async def quoter_contract(self):
     #     """ create a quoter contract """
     #     try:
     #         quoter_abi = await self.get(settings.dex_quoter_abi_url)
     #         self.quoter = self.w3.eth.contract(
     #             address=self.w3.to_checksum_address(
@@ -253,15 +252,14 @@
                 return self.w3.to_checksum_address(token_address)
 
         token_address = await self.search_cg_contract(token)
         if token_address is None:
             raise ValueError("Invalid Token")
         return self.w3.to_checksum_address(token_address)
 
-
     async def search_cg_platform(self):
         """search coingecko platform"""
         asset_platforms = self.cg.get_asset_platforms()
         output_dict = next(
             x for x in asset_platforms
             if x["chain_identifier"] == int(self.chain_id)
         )
@@ -310,15 +308,14 @@
         token_abi = await self.get_explorer_abi(token_address)
         if token_abi is None:
             token_abi = await self.get(settings.dex_erc20_abi_url)
         return self.w3.eth.contract(
             address=token_address,
             abi=token_abi)
 
-
     async def get_token_decimals(self, token_address: str) -> Optional[int]:
         """Get token decimals"""
         contract = await self.get_token_contract(token_address)
         return 18 if not contract else contract.functions.decimals().call()
 
     async def get_token_balance(self, token_address: str) -> Optional[int]:
         """Get token balance"""
@@ -326,63 +323,54 @@
         if contract is None or contract.functions is None:
             raise ValueError("No Balance")
         balance = contract.functions.balanceOf(self.wallet_address).call()
         if balance is None:
             raise ValueError("No Balance")
         return balance
 
-
     async def get_explorer_abi(self, address):
         if not settings.dex_block_explorer_api:
             return None
 
         params = {
             "module": "contract",
             "action": "getabi",
             "address": address,
             "apikey": settings.dex_block_explorer_api
         }
-        try:
-            resp = await self.get(
-                url=settings.dex_block_explorer_url, params=params)
-            if resp['status'] == "1":
-                self.logger.debug("ABI found %s", resp)
-                return resp["result"]
-            else:
-                return None
-        except Exception as error:
+        resp = await self.get(
+            url=settings.dex_block_explorer_url, params=params)
+        if resp['status'] == "1":
+            self.logger.debug("ABI found %s", resp)
+            return resp["result"]
+        else:
             return None
 
-
 # 🔒 USER RELATED
-
     async def get_name(self):
         return settings.dex_router_contract_addr[-8:]
         
     async def get_info(self):
         return f"💱 {await self.get_name()}\n🪪 {self.account}"
 
     async def get_account_balance(self):
-        try:
-            account_balance = self.w3.eth.get_balance(
-                self.w3.to_checksum_address(self.wallet_address))
-            account_balance = self.w3.from_wei(account_balance, 'ether')
-            trading_asset_balance = await self.get_trading_asset_balance()
-            if trading_asset_balance:
-                account_balance += f"💵{trading_asset_balance}"
-            return round(account_balance, 5)
-        except Exception:
-            return 0
+        account_balance = self.w3.eth.get_balance(
+            self.w3.to_checksum_address(self.wallet_address))
+        account_balance = self.w3.from_wei(account_balance, 'ether')
+        trading_asset_balance = await self.get_trading_asset_balance()
+        if trading_asset_balance:
+            account_balance += f"💵{trading_asset_balance}"
+        return round(account_balance, 5)
 
     async def get_trading_asset_balance(self):
         trading_asset_balance = await self.get_token_balance(
             self.trading_asset_address)
         return trading_asset_balance if trading_asset_balance else 0
 
     async def get_account_position(self):
-        #position = "📊 Position\n" + str(open_positions)
-        #position += str(await self.get_account_margin())
-        #return position
-        return 0
+        open_positions = 0
+        position = "📊 Position\n" + str(open_positions)
+        position += str(await self.get_account_margin())
+        return position
 
     async def get_account_margin(self):
         return 0
```

### Comparing `dxsp-3.1.3/dxsp/protocols/oneinch.py` & `dxsp-3.1.4/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.3/dxsp/protocols/zerox.py` & `dxsp-3.1.4/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.3/pyproject.toml` & `dxsp-3.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "3.1.3"
+version = "3.1.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.1.3/PKG-INFO` & `dxsp-3.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.1.3
+Version: 3.1.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/dxsp-3.1.4.tar.gz` & `tmp/dxsp-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.1.4.tar", max compression
+gzip compressed data, was "dxsp-3.2.0.tar", max compression
```

## Comparing `dxsp-3.1.4.tar` & `dxsp-3.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-03 00:29:11.034198 dxsp-3.1.4/LICENSE
--rw-r--r--   0        0        0     2378 2023-07-03 00:29:11.034198 dxsp-3.1.4/README.md
--rw-r--r--   0        0        0      114 2023-07-03 00:29:11.842202 dxsp-3.1.4/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/config.py
--rw-r--r--   0        0        0     8093 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0    15255 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     4000 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-03 00:29:11.034198 dxsp-3.1.4/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2144 2023-07-03 00:29:11.838201 dxsp-3.1.4/pyproject.toml
--rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 dxsp-3.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-03 15:28:45.419052 dxsp-3.2.0/LICENSE
+-rw-r--r--   0        0        0     2395 2023-07-03 15:28:45.419052 dxsp-3.2.0/README.md
+-rw-r--r--   0        0        0      114 2023-07-03 15:28:46.371094 dxsp-3.2.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/config.py
+-rw-r--r--   0        0        0    10489 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    14284 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-03 15:28:45.419052 dxsp-3.2.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2144 2023-07-03 15:28:46.371094 dxsp-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 dxsp-3.2.0/PKG-INFO
```

### Comparing `dxsp-3.1.4/LICENSE` & `dxsp-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.4/README.md` & `dxsp-3.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
 |[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) <br>[![👷Flow](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%91%B7Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml)<br>[![codebeat badge](https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a)](https://codebeat.co/projects/github-com-mraniki-dxsp-main)<br>[![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko) [![uniswap](https://badgen.net/badge/icon/unipy/black?icon=libraries&label)](https://github.com/uniswap-python/uniswap-python)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (Uni and 0x)
 
 Key features:
 
-- Any blockchains mainnet or testnet supported by web3py, uniswap type router (uniswap, pancakeswap) or 0x.
-
+- Any blockchains mainnet or testnet supported by web3py, for uniswap based router (e.g uniswap, pancakeswap) or 0x protocol.
 
 Other features:
 
 - Translate token symbol to contract address via user defined tokenlist format or coingecko API
 - Connect to web3 automatically or use your own w3
 - Approve contract and sign transaction
 - Quote a given token
@@ -24,15 +23,15 @@
 
 ## How to use it
 
 ```
 from dxsp import DexSwap
 
  dex = DexSwap()
- #BUY 10 USDC to SWAP with BITCOIN
+ #BUY 10 USDT to SWAP with BITCOIN
  demo_tx = await dex.get_swap('USDT','wBTC',10)
  print("demo_tx ", demo_tx)
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
```

### Comparing `dxsp-3.1.4/dxsp/default_settings.toml` & `dxsp-3.2.0/dxsp/default_settings.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [default]
 VALUE = "On default"
 dxsp_enabled = true
 loglevel = "INFO"
 dex_wallet_address = "0x1234567890123456789012345678901234567890"
 dex_private_key = "0xdeadbeef45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
-dex_protocol_type = "uniswap_v2" #0x
-dex_chain_id = 1
+dex_protocol_type = "uniswap"
+dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_0x_url = "https://api.0x.org/mainnet"
 dex_0x_api_key = "" 
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e"
-dex_quoter_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v3/quoter.abi"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 trading_asset = "USDT"
@@ -32,98 +30,147 @@
 
 
 
 ##############
 ## SETTINGS ##
 ## FOR TEST ##
 ##############
-[test_uniswap_chain_1]
+[uniswap]
 VALUE = "On Testing"
 dxsp_enabled = true
 loglevel = "DEBUG"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
-dex_protocol_type = "uniswap_v2"
-dex_chain_id = 1
+dex_protocol_type = "uniswap"
+dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
+dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e"
-dex_quoter_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v3/quoter.abi"
 trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
-[test_zerox_chain_1]
+[zerox]
 VALUE = "test_zerox"
 loglevel = "DEBUG"
 dxsp_enabled = true
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "0x"
-dex_chain_id = 1
+dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_0x_url = "https://api.0x.org/"
 dex_router_contract_addr = "0xdef1c0ded9bec7f1a1670819833240f027b25eff"
+dex_factory_contract_addr = ""
 dex_router_abi_url = "https://raw.githubusercontent.com/0xProject/protocol/development/packages/contract-artifacts/artifacts/Exchange.json"
-dex_erc20_abi_url = "https://raw.githubusercontent.com/0xProject/protocol/development/packages/contract-artifacts/artifacts/ERC20Token.json"
+dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10
 dex_trading_slippage = 2
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
-
-[test_uniswap_chain5]
+[testnet]
 VALUE = "On Testnet"
 loglevel = "DEBUG"
 dxsp_enabled = true
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
-dex_protocol_type = "uniswap_v2"
-dex_chain_id = 5
+dex_protocol_type = "uniswap"
+dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth_goerli"
-# dex_block_explorer_url = "https://api-Goerli.etherscan.io/api?"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
+dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-trading_asset = "USDT"
-trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
+trading_asset = "USDC"
+trading_asset_address = "0xa3726f2e6423caF1824cD7721B543B29b621fB4f"
 trading_risk_amount = 10
 dex_trading_slippage = 2
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
-[test_chain_56]
+[bsc]
 VALUE = "chain_56"
-dex_chain_id = 56
 dxsp_enabled = true
 dex_wallet_address = "0xf977814e90da44bfa03b6295a0616a897441acec"
-dex_protocol_type = "0x"
+dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
+dex_protocol_type = "uniswap"
+dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/bsc"
-dex_0x_url = "https://bsc.api.0x.org/"
 dex_router_contract_addr = "0x10ED43C718714eb63d5aA57B78B54704E256024E"
-dex_block_explorer_url = "https://api.bscscan.com/api?"
-dex_block_explorer_api =  ""
+dex_factory_contract_addr = "0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73"
 trading_asset = "BUSD"
 trading_asset_address = "0xe9e7cea3dedca5984780bafc599bd69add087d56"
+trading_risk_amount = 10 
+dex_trading_slippage = 2
+headers = {User-Agent= 'Mozilla/5.0'}
+token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
+token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
+token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
+
+[uniswap3]
+VALUE = "On uniswap3"
+dxsp_enabled = true
+loglevel = "DEBUG"
+dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
+dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
+dex_protocol_type = "uniswap"
+dex_protocol_version = 3
+dex_rpc = "https://rpc.ankr.com/eth"
+dex_router_contract_addr = "0x1F98431c8aD98523631AE4a59f267346ea31F984"
+dex_factory_contract_addr = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45"
+dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
+dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
+trading_asset = "USDT"
+trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
+trading_risk_amount = 10 
+dex_trading_slippage = 2
+headers = {User-Agent= 'Mozilla/5.0'}
+token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
+token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
+token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
+
+[pancake3]
+VALUE = "On pancake3"
+dxsp_enabled = true
+loglevel = "DEBUG"
+dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
+dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
+dex_protocol_type = "uniswap"
+dex_protocol_version = 3
+dex_rpc = "https://rpc.ankr.com/bsc"
+dex_router_contract_addr = "0x1F98431c8aD98523631AE4a59f267346ea31F984"
+dex_factory_contract_addr = "0x13f4EA83D0bd40E75C8222255bc855a974568Dd4"
+dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
+dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
+trading_asset = "BUSD"
+trading_asset_address = "0xe9e7cea3dedca5984780bafc599bd69add087d56"
+trading_risk_amount = 10 
+dex_trading_slippage = 2
+headers = {User-Agent= 'Mozilla/5.0'}
+token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
+token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
+token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
+
 
 
-# [test_oneinch_chain_1]
+# [oneinch]
 # VALUE = "1inchtesting"
 # loglevel = "DEBUG"
 # dxsp_enabled = true
 # headers = {User-Agent= 'Mozilla/5.0'}
 # token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 # token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 # token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
@@ -138,35 +185,35 @@
 # dex_protocol_type = "1inch"
 # dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 # dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
 # dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" #UNI_V2
 # dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 # dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 
-# [test_uniswap_chain_11155111]
+# [sepolia]
 # VALUE = "SEPOLIA"
 # loglevel = "DEBUG"
 # dxsp_enabled = true
 # dex_chain_id = 11155111
 # dex_rpc = "https://rpc.ankr.com/eth_sepolia"
 # dex_block_explorer_url = "https://api-Sepolia.etherscan.io/api?"
 # dex_protocol_type = "0x"
 # dex_router_contract_addr = "0x1f98431c8ad98523631ae4a59f267346ea31f984"
 # dex_0x_url = "https://sepolia.api.0x.org/"
 
-# [test_pancake_chain_97]
+# [bsctesnet]
 # VALUE = "DEX chain_97"
 # loglevel = "DEBUG"
 # dxsp_enabled = true
 # dex_chain_id = 97
 # dex_rpc = "https://rpc.ankr.com/bsc_testnet_chapel"
 # dex_block_explorer_url = "https://api-testnet.bscscan.com/api?"
 # dex_router_contract_addr = ""
 
-# [test_chain_42161]
+# [arbitrum]
 # VALUE = "DEX chain_42161"
 # loglevel = "DEBUG"
 # dex_chain_id = 42161
 # dex_rpc = "https://rpc.ankr.com/arbitrum"
 # dex_block_explorer_url = "https://api-testnet.bscscan.com/api?"
 # dex_router_contract_addr = "0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f"
 # dex_0x_url = "https://arbitrum.api.0x.org/"
```

### Comparing `dxsp-3.1.4/dxsp/main.py` & `dxsp-3.2.0/dxsp/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,34 +14,34 @@
 
 
 class DexSwap:
     """swap  class"""
     def __init__(self, w3: Optional[Web3] = None):
         self.logger = logging.getLogger(name="DexSwap")
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
-        self.w3.eth.set_gas_price_strategy(medium_gas_price_strategy)
-        try:
-            if self.w3.net.listening:
-                self.logger.info("connected %s",self.w3)
-        except Exception as error:
-            raise error
+        if self.w3.net.listening:
+            self.logger.info("connected %s", self.w3)
+            self.w3.eth.set_gas_price_strategy(medium_gas_price_strategy)
+            self.chain_id = self.w3.net.version
+            self.wallet_address = self.w3.to_checksum_address(
+                settings.dex_wallet_address)
+            self.account = f"{str(self.w3.net.version)} - {str(self.wallet_address[-8:])}"
+            self.private_key = settings.dex_private_key
+            self.trading_asset_address = self.w3.to_checksum_address(
+                settings.trading_asset_address)
+
+            self.protocol_type = settings.dex_protocol_type
+            self.protocol_version = settings.dex_protocol_version
+            self.dex_swap = None
+            self.router = None
+            self.quoter = None
+        else:
+            raise ValueError("w3 not connected")
 
-        self.chain_id = settings.dex_chain_id
-        self.wallet_address = self.w3.to_checksum_address(
-            settings.dex_wallet_address)
-        self.account = f"{str(self.w3.net.version)} - {str(self.wallet_address[-8:])}"
-        self.private_key = settings.dex_private_key
-        self.trading_asset_address = self.w3.to_checksum_address(
-            settings.trading_asset_address)
         self.cg = CoinGeckoAPI()
-                    
-        self.protocol_type = settings.dex_protocol_type
-        self.dex_swap = None
-        self.router = None
-        self.quoter = None
 
     async def get_protocol(self):
         """ protocol init """
         from dxsp.protocols import DexSwapUniswap, DexSwapZeroX, DexSwapOneInch
         if self.protocol_type == "0x":
             self.dex_swap = DexSwapZeroX()
         elif self.protocol_type == "1inch":
@@ -73,15 +73,15 @@
         """ Main swap function """
         try:
             await self.get_protocol()
             sell_token_address = sell_token
             if not sell_token.startswith("0x"):
                 sell_token_address = await self.search_contract_address(sell_token)
             buy_token_address = buy_token
-            if not buy_token_address.startswith("0x"):   
+            if not buy_token_address.startswith("0x"):
                 buy_token_address = await self.search_contract_address(buy_token)
             sell_amount = await self.calculate_sell_amount(sell_token_address, quantity)
             sell_token_amount_wei = sell_amount * (10 ** (
                 await self.get_token_decimals(sell_token_address)))
             await self.get_approve(sell_token_address)
 
             order_amount = int(sell_token_amount_wei * (settings.dex_trading_slippage / 100))
@@ -128,20 +128,20 @@
             if allowance == 0:
                 approval_tx = contract.functions.approve(
                     dex_router_address, approved_amount)
                 approval_tx_hash = await self.get_sign(approval_tx.transact())
                 return self.w3.eth.wait_for_transaction_receipt(
                     approval_tx_hash)
         except Exception as error:
-            raise ValueError(f"Approval failed {error}") 
+            raise ValueError(f"Approval failed {error}")
 
     async def get_sign(self, transaction):
         """ sign a transaction """
         try:
-            if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
+            if self.protocol_type == 'uniswap':
                 transaction_params = {
                     'from': self.wallet_address,
                     'gas': await self.get_gas(transaction),
                     'gasPrice': await self.get_gas_price(),
                     'nonce': self.w3.eth.get_transaction_count(
                         self.wallet_address),
                 }
@@ -150,71 +150,45 @@
                 transaction, self.private_key)
             raw_tx_hash = self.w3.eth.send_raw_transaction(
                 signed_tx.rawTransaction)
             return self.w3.to_hex(raw_tx_hash)
         except Exception as error:
             raise error
 
-### ------🛠️ W3 UTILS ---------
+# ------🛠️ W3 UTILS ---------
     async def get(self, url, params=None, headers=None):
         """ gets a url payload """
         try:
             self.logger.debug(f"Requesting URL: {url}")
             response = requests.get(
                 url, params=params, headers=headers, timeout=10)
             if response.status_code == 200:
                 return response.json()
 
         except Exception as error:
             raise error
 
-    # async def router_contract(self):
-    #     """ create a router contract """
-    #     try:
-    #         router_abi = await self.get(settings.dex_router_abi_url)
-    #         self.router = self.w3.eth.contract(
-    #             address=self.w3.to_checksum_address(
-    #                 settings.dex_router_contract_addr
-    #             ),
-    #             abi=router_abi,
-    #         )
-    #         if self.router.functions is None:
-    #             raise ValueError("Router/Chain setup incorrect")
-    #     except Exception as error:
-    #         raise error
-
-    # async def quoter_contract(self):
-    #     """ create a quoter contract """
-    #     try:
-    #         quoter_abi = await self.get(settings.dex_quoter_abi_url)
-    #         self.quoter = self.w3.eth.contract(
-    #             address=self.w3.to_checksum_address(
-    #                 settings.dex_quoter_contract_addr),
-    #             abi=quoter_abi)
-    #     except Exception as error:
-    #         raise error
-
     async def calculate_sell_amount(self, sell_token_address, quantity):
         """Returns amount based on risk percentage."""
         sell_balance = await self.get_token_balance(sell_token_address)
         sell_contract = await self.get_token_contract(sell_token_address)
         sell_decimals = sell_contract.functions.decimals().call() if sell_contract is not None else 18
         risk_percentage = settings.trading_risk_amount
-        return (sell_balance / (risk_percentage ** sell_decimals)) * (float(quantity) / 100)
+        return (sell_balance / (risk_percentage * 10 ** sell_decimals)) * (float(quantity) / 100)
 
     async def get_confirmation(self, transactionHash):
         """Returns trade confirmation."""
         try:
             transaction = self.w3.eth.get_transaction(transactionHash)
             block = self.w3.eth.get_block(transaction["blockNumber"])
             return {
                 "timestamp": block["timestamp"],
                 "id": transactionHash,
                 "instrument": transaction["to"],
-                "contract": transaction["to"], # TBD To be determined.
+                "contract": transaction["to"],   # TBD To be determined.
                 "amount": transaction["value"],
                 "price": transaction["value"],  # TBD To be determined.
                 "fee": transaction["gas"],
                 "confirmation": (
                     f"➕ Size: {round(transaction['value'], 4)}\n"
                     f"⚫️ Entry: {round(transaction['value'], 4)}\n"
                     f"ℹ️ {transactionHash}\n"
@@ -230,15 +204,15 @@
         gas_limit = self.w3.eth.estimate_gas(transaction) * 1.25
         return int(self.w3.to_wei(gas_limit, 'wei'))
 
     async def get_gas_price(self):
         """search get gas price"""
         return round(self.w3.from_wei(self.w3.eth.generate_gas_price(), 'gwei'), 2)
 
-### ------✍️ CONTRACT ---------
+# ## ------✍️ CONTRACT ---------
     async def search_contract_address(self, token):
         """search a contract function"""
 
         contract_lists = [
             settings.token_personal_list,
             settings.token_testnet_list,
             settings.token_mainnet_list,
@@ -344,33 +318,31 @@
             return resp["result"]
         else:
             return None
 
 # 🔒 USER RELATED
     async def get_name(self):
         return settings.dex_router_contract_addr[-8:]
-        
+
     async def get_info(self):
-        return f"💱 {await self.get_name()}\n🪪 {self.account}"
+        return f"{__class__.__name__} {__version__}\n💱 {await self.get_name()}\n🪪 {self.account}"
 
     async def get_account_balance(self):
         account_balance = self.w3.eth.get_balance(
             self.w3.to_checksum_address(self.wallet_address))
-        account_balance = self.w3.from_wei(account_balance, 'ether')
-        trading_asset_balance = await self.get_trading_asset_balance()
-        if trading_asset_balance:
-            account_balance += f"💵{trading_asset_balance}"
-        return round(account_balance, 5)
+        account_balance = self.w3.from_wei(account_balance, 'ether') or 0
+        trading_asset_balance = await self.get_trading_asset_balance() or 0
+        return f"₿ {account_balance}\n💵 {trading_asset_balance}"
 
     async def get_trading_asset_balance(self):
         trading_asset_balance = await self.get_token_balance(
             self.trading_asset_address)
         return trading_asset_balance if trading_asset_balance else 0
 
     async def get_account_position(self):
         open_positions = 0
         position = "📊 Position\n" + str(open_positions)
-        position += str(await self.get_account_margin())
+        position += "\n" + str(await self.get_account_margin())
         return position
 
     async def get_account_margin(self):
         return 0
```

### Comparing `dxsp-3.1.4/dxsp/protocols/oneinch.py` & `dxsp-3.2.0/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.4/dxsp/protocols/zerox.py` & `dxsp-3.2.0/dxsp/protocols/zerox.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 0️⃣x
 """
 from dxsp.config import settings
 from dxsp.main import DexSwap
 
 class DexSwapZeroX(DexSwap):
     async def get_quote(self, buy_address, sell_address, amount=1):
-        #pass
         try:
             out_amount = amount * (10 ** await self.get_token_decimals(sell_address)) ##1000000000
             url = f"{settings.dex_0x_url}/swap/v1/quote?buyToken={str(buy_address)}&sellToken={str(sell_address)}&sellAmount={str(out_amount)}"
             headers = {"0x-api-key": settings.dex_0x_api_key}
             response = await self.get(url, params=None, headers=headers)
-            print(response)
             if response:
-                raw_amount = round(float(response['guaranteedPrice']), 6)
+                quote = float(response['guaranteedPrice'])
+                print(quote)
+                return quote
         except Exception as error:
             raise ValueError(f"Quote failed {error}") 
 
-
     async def get_swap(self, buy_address, sell_address, amount):
         swap_order = await self.get_quote(buy_address, sell_address, amount)
         return await self.get_sign(swap_order)
```

### Comparing `dxsp-3.1.4/pyproject.toml` & `dxsp-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "3.1.4"
+version = "3.2.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.1.4/PKG-INFO` & `dxsp-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.1.4
+Version: 3.2.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,15 @@
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
 |[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) <br>[![👷Flow](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%91%B7Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml)<br>[![codebeat badge](https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a)](https://codebeat.co/projects/github-com-mraniki-dxsp-main)<br>[![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko) [![uniswap](https://badgen.net/badge/icon/unipy/black?icon=libraries&label)](https://github.com/uniswap-python/uniswap-python)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (Uni and 0x)
 
 Key features:
 
-- Any blockchains mainnet or testnet supported by web3py, uniswap type router (uniswap, pancakeswap) or 0x.
-
+- Any blockchains mainnet or testnet supported by web3py, for uniswap based router (e.g uniswap, pancakeswap) or 0x protocol.
 
 Other features:
 
 - Translate token symbol to contract address via user defined tokenlist format or coingecko API
 - Connect to web3 automatically or use your own w3
 - Approve contract and sign transaction
 - Quote a given token
@@ -45,15 +44,15 @@
 
 ## How to use it
 
 ```
 from dxsp import DexSwap
 
  dex = DexSwap()
- #BUY 10 USDC to SWAP with BITCOIN
+ #BUY 10 USDT to SWAP with BITCOIN
  demo_tx = await dex.get_swap('USDT','wBTC',10)
  print("demo_tx ", demo_tx)
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
```


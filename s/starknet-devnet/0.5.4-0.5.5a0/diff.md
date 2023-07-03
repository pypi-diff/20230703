# Comparing `tmp/starknet_devnet-0.5.4.tar.gz` & `tmp/starknet_devnet-0.5.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_devnet-0.5.4.tar", max compression
+gzip compressed data, was "starknet_devnet-0.5.5a0.tar", max compression
```

## Comparing `starknet_devnet-0.5.4.tar` & `starknet_devnet-0.5.5a0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-06-16 12:50:09.375941 starknet_devnet-0.5.4/LICENSE
--rw-r--r--   0        0        0     1054 2023-06-16 12:50:09.375941 starknet_devnet-0.5.4/README.md
--rw-r--r--   0        0        0     1818 2023-06-16 12:50:09.387941 starknet_devnet-0.5.4/pyproject.toml
--rw-r--r--   0        0        0   208485 2023-06-16 12:50:09.387941 starknet_devnet-0.5.4/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
--rw-r--r--   0        0        0    32739 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/MockStarknetMessaging.json
--rw-r--r--   0        0        0    35645 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/UDC_OZ_0.5.0.json
--rw-r--r--   0        0        0     2958 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/__init__.py
--rw-r--r--   0        0        0     2595 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/account.py
--rw-r--r--   0        0        0     3784 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/account_util.py
--rw-r--r--   0        0        0     2511 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/accounts.py
--rw-r--r--   0        0        0   118818 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
--rw-r--r--   0        0        0     1784 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
--rw-r--r--   0        0        0     1866 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/block_info_generator.py
--rw-r--r--   0        0        0    12337 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blocks.py
--rw-r--r--   0        0        0        0 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/__init__.py
--rw-r--r--   0        0        0     7585 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/base.py
--rw-r--r--   0        0        0    14072 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/feeder_gateway.py
--rw-r--r--   0        0        0     2256 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/gateway.py
--rw-r--r--   0        0        0     3959 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/postman.py
--rw-r--r--   0        0        0        0 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/blocks.py
--rw-r--r--   0        0        0     2120 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/call.py
--rw-r--r--   0        0        0     2195 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/classes.py
--rw-r--r--   0        0        0     6257 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/misc.py
--rw-r--r--   0        0        0     4953 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/routes.py
--rw-r--r--   0        0        0   116673 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec.py
--rw-r--r--   0        0        0     6049 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec_write.py
--rw-r--r--   0        0        0    16310 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_trace_spec.py
--rw-r--r--   0        0        0     7135 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/schema.py
--rw-r--r--   0        0        0     1144 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/state.py
--rw-r--r--   0        0        0      929 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/storage.py
--rw-r--r--   0        0        0        0 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/__init__.py
--rw-r--r--   0        0        0    31253 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/payloads.py
--rw-r--r--   0        0        0     6544 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/responses.py
--rw-r--r--   0        0        0     3457 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/types.py
--rw-r--r--   0        0        0     8789 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/transactions.py
--rw-r--r--   0        0        0     3542 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/utils.py
--rw-r--r--   0        0        0      899 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/shared.py
--rw-r--r--   0        0        0    24763 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/cairo_rs_py_patch.py
--rw-r--r--   0        0        0     1038 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/chargeable_account.py
--rw-r--r--   0        0        0     5310 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/compiler.py
--rw-r--r--   0        0        0     1239 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/constants.py
--rw-r--r--   0        0        0      646 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/contract_class_wrapper.py
--rw-r--r--   0        0        0    16387 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/devnet_config.py
--rw-r--r--   0        0        0      784 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/dump.py
--rw-r--r--   0        0        0     6119 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/fee_token.py
--rw-r--r--   0        0        0     8161 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/forked_state.py
--rw-r--r--   0        0        0     1640 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/general_config.py
--rw-r--r--   0        0        0     9005 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/origin.py
--rw-r--r--   0        0        0    10015 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/postman_wrapper.py
--rw-r--r--   0        0        0     2237 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/predeployed_contract_wrapper.py
--rw-r--r--   0        0        0     4353 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/server.py
--rw-r--r--   0        0        0    40357 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/starknet_wrapper.py
--rw-r--r--   0        0        0     1988 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/state.py
--rw-r--r--   0        0        0     2573 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/state_archive.py
--rw-r--r--   0        0        0    11617 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/transactions.py
--rw-r--r--   0        0        0     1822 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/udc.py
--rw-r--r--   0        0        0    10902 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/util.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 starknet_devnet-0.5.4/setup.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 starknet_devnet-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-03 11:45:14.809619 starknet_devnet-0.5.5a0/LICENSE
+-rw-r--r--   0        0        0     1054 2023-07-03 11:45:14.809619 starknet_devnet-0.5.5a0/README.md
+-rw-r--r--   0        0        0     1822 2023-07-03 11:45:14.821619 starknet_devnet-0.5.5a0/pyproject.toml
+-rw-r--r--   0        0        0   208485 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
+-rw-r--r--   0        0        0    32739 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/MockStarknetMessaging.json
+-rw-r--r--   0        0        0    35645 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/UDC_OZ_0.5.0.json
+-rw-r--r--   0        0        0     2960 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/__init__.py
+-rw-r--r--   0        0        0     2779 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/account.py
+-rw-r--r--   0        0        0     4161 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/account_util.py
+-rw-r--r--   0        0        0     2511 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/accounts.py
+-rw-r--r--   0        0        0   118818 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
+-rw-r--r--   0        0        0     1784 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
+-rw-r--r--   0        0        0     1866 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/block_info_generator.py
+-rw-r--r--   0        0        0    12483 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blocks.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/__init__.py
+-rw-r--r--   0        0        0     7585 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/base.py
+-rw-r--r--   0        0        0    14072 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/feeder_gateway.py
+-rw-r--r--   0        0        0     2256 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/gateway.py
+-rw-r--r--   0        0        0     3959 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/postman.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/__init__.py
+-rw-r--r--   0        0        0     2138 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/blocks.py
+-rw-r--r--   0        0        0     2120 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/call.py
+-rw-r--r--   0        0        0     2195 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/classes.py
+-rw-r--r--   0        0        0     6257 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/misc.py
+-rw-r--r--   0        0        0     4953 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/routes.py
+-rw-r--r--   0        0        0   116673 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec.py
+-rw-r--r--   0        0        0     6049 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py
+-rw-r--r--   0        0        0    16310 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py
+-rw-r--r--   0        0        0     7135 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/schema.py
+-rw-r--r--   0        0        0     1144 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/state.py
+-rw-r--r--   0        0        0      929 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/storage.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/__init__.py
+-rw-r--r--   0        0        0    32879 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/payloads.py
+-rw-r--r--   0        0        0     6494 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/responses.py
+-rw-r--r--   0        0        0     3457 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/types.py
+-rw-r--r--   0        0        0     8789 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/transactions.py
+-rw-r--r--   0        0        0     3542 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/utils.py
+-rw-r--r--   0        0        0      899 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/shared.py
+-rw-r--r--   0        0        0    24763 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/cairo_rs_py_patch.py
+-rw-r--r--   0        0        0     1038 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/chargeable_account.py
+-rw-r--r--   0        0        0     5310 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/compiler.py
+-rw-r--r--   0        0        0     1239 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/constants.py
+-rw-r--r--   0        0        0      646 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/contract_class_wrapper.py
+-rw-r--r--   0        0        0    16332 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/devnet_config.py
+-rw-r--r--   0        0        0      784 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/dump.py
+-rw-r--r--   0        0        0     6558 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/fee_token.py
+-rw-r--r--   0        0        0     8332 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/forked_state.py
+-rw-r--r--   0        0        0     1640 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/general_config.py
+-rw-r--r--   0        0        0     9005 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/origin.py
+-rw-r--r--   0        0        0    10015 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/postman_wrapper.py
+-rw-r--r--   0        0        0     2237 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/predeployed_contract_wrapper.py
+-rw-r--r--   0        0        0     4353 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/server.py
+-rw-r--r--   0        0        0    41451 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/starknet_wrapper.py
+-rw-r--r--   0        0        0     1988 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/state.py
+-rw-r--r--   0        0        0     2573 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/state_archive.py
+-rw-r--r--   0        0        0    11947 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/transactions.py
+-rw-r--r--   0        0        0     1822 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/udc.py
+-rw-r--r--   0        0        0    11174 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/util.py
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5a0/setup.py
+-rw-r--r--   0        0        0     2193 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5a0/PKG-INFO
```

### Comparing `starknet_devnet-0.5.4/LICENSE` & `starknet_devnet-0.5.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/README.md` & `starknet_devnet-0.5.5a0/README.md`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/pyproject.toml` & `starknet_devnet-0.5.5a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "starknet_devnet"
-version = "0.5.4"
+version = "0.5.5a0"
 description = "A local testnet for Starknet"
 authors = ["FabijanC <fabijan.corak@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/0xSpaceShard/starknet-devnet"
 homepage = "https://github.com/0xSpaceShard/starknet-devnet"
 keywords = ["starknet", "cairo", "testnet", "local", "server"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 Flask = {extras = ["async"], version = "~2.0.3"}
 flask-cors = "~3.0.10"
-cairo-lang = "0.11.2"
+cairo-lang = "0.12.0a0"
 Werkzeug = "~2.0.3"
 cloudpickle = "~2.1.0"
 crypto-cpp-py = "~1.4.0"
 marshmallow = "~3.17.0"
 typing-extensions = "~4.3.0"
 gunicorn = "~20.1.0"
 marshmallow-dataclass = "~8.4"
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json` & `starknet_devnet-0.5.5a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/MockStarknetMessaging.json` & `starknet_devnet-0.5.5a0/starknet_devnet/MockStarknetMessaging.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/UDC_OZ_0.5.0.json` & `starknet_devnet-0.5.5a0/starknet_devnet/UDC_OZ_0.5.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/__init__.py` & `starknet_devnet-0.5.5a0/starknet_devnet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # pylint: disable=unused-import
 # pylint: disable=import-outside-toplevel
 
 import os
 import sys
 
-__version__ = "0.5.4"
+__version__ = "0.5.5a0"
 
 
 def _patch_pedersen_hash():
     """
     Improves performance by substituting the default Python implementation of Pedersen hash
     with Software Mansion's Python wrapper of C++ implementation.
     """
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/account.py` & `starknet_devnet-0.5.5a0/starknet_devnet/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Account class and its predefined constants.
 """
 
 from typing import Optional
 
+from starkware.starknet.business_logic.state.storage_domain import StorageDomain
 from starkware.starknet.core.os.contract_address.contract_address import (
     calculate_contract_address_from_hash,
 )
 from starkware.starknet.public.abi import get_selector_from_name
 from starkware.starknet.testing.starknet import Starknet
 
 from starknet_devnet.account_util import set_balance
@@ -57,15 +58,18 @@
             "address": hex(self.address),
         }
 
     async def _mimic_constructor(self):
         starknet: Starknet = self.starknet_wrapper.starknet
 
         await starknet.state.state.set_storage_at(
-            self.address, get_selector_from_name("Account_public_key"), self.public_key
+            storage_domain=StorageDomain.ON_CHAIN,
+            contract_address=self.address,
+            key=get_selector_from_name("Account_public_key"),
+            value=self.public_key,
         )
 
         await set_balance(starknet.state, self.address, self.initial_balance)
 
     def print(self):
         print(f"Account #{self.__index}:")
         print(f"Address: {hex(self.address)}")
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/account_util.py` & `starknet_devnet-0.5.5a0/starknet_devnet/account_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Latest changes based on https://github.com/OpenZeppelin/nile/pull/184
 """
 
 from typing import List, NamedTuple, Sequence, Tuple
 
 from starkware.cairo.lang.vm.crypto import pedersen_hash
 from starkware.crypto.signature.signature import sign
+from starkware.starknet.business_logic.state.storage_domain import StorageDomain
 from starkware.starknet.core.os.transaction_hash.transaction_hash import (
     TransactionHashPrefix,
     calculate_transaction_hash_common,
 )
 from starkware.starknet.definitions.general_config import StarknetChainId
 from starkware.starknet.public.abi import get_selector_from_name
 from starkware.starknet.testing.starknet import StarknetState
@@ -116,16 +117,24 @@
 
 
 async def set_balance(state: StarknetState, address: int, balance: int):
     """Modify `state` so that `address` has `balance`"""
 
     fee_token_address = state.general_config.fee_token_address
 
-    balance_address = pedersen_hash(get_selector_from_name("ERC20_balances"), address)
+    balance_key = pedersen_hash(get_selector_from_name("ERC20_balances"), address)
     balance_uint256 = Uint256.from_felt(balance)
 
     await state.state.set_storage_at(
-        fee_token_address, balance_address, balance_uint256.low
+        storage_domain=StorageDomain.ON_CHAIN,
+        contract_address=fee_token_address,
+        key=balance_key,
+        value=balance_uint256.low,
     )
     await state.state.set_storage_at(
-        fee_token_address, balance_address + 1, balance_uint256.high
+        storage_domain=StorageDomain.ON_CHAIN,
+        contract_address=fee_token_address,
+        # uint256 takes up two memory places, uint256.high is in
+        # the memory address after uint256.low, hence the +1
+        key=balance_key + 1,
+        value=balance_uint256.high,
     )
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/accounts.py` & `starknet_devnet-0.5.5a0/starknet_devnet/accounts.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json` & `starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json` & `starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/block_info_generator.py` & `starknet_devnet-0.5.5a0/starknet_devnet/block_info_generator.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blocks.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,18 @@
         """Returns the last block stored so far."""
         return await self.get_by_number(self.get_number_of_accepted_blocks() - 1)
 
     def get_number_of_accepted_blocks(self) -> int:
         """Returns the number of not aborted blocks."""
         return len(self.__num2hash) + self.origin.get_number_of_blocks()
 
+    def get_next_block_number(self) -> int:
+        """Returns the block_number of the next block"""
+        return self.get_number_of_accepted_blocks()
+
     def __assert_block_number_in_range(self, block_number: BlockIdentifier):
         if block_number < 0:
             message = (
                 f"Block number must be a non-negative integer; got: {block_number}."
             )
             raise StarknetDevnetException(
                 code=StarkErrorCode.MALFORMED_REQUEST, message=message
@@ -267,15 +271,15 @@
 
         block_dict = self.__pending_block.dump()
 
         block_dict["status"] = BlockStatus.ACCEPTED_ON_L2.name
         state_root = DUMMY_STATE_ROOT
         block_dict["state_root"] = state_root.hex()
 
-        block_number = self.get_number_of_accepted_blocks()
+        block_number = self.get_next_block_number()
         block_dict["block_number"] = block_number
 
         if self.lite or is_empty_block:
             block_hash = block_number
         elif block_hash is None:
             block_hash = await self.__calculate_pending_block_hash(
                 state, block_number, state_root
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/base.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/feeder_gateway.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/feeder_gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/gateway.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/postman.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/postman.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,9 +97,9 @@
             from_address, to_address, payload
         )
         return jsonify({"message_hash": result})
     except AssertionError as err:
         raise StarknetDevnetException(
             code=StarknetErrorCode.L1_TO_L2_MESSAGE_ZEROED_COUNTER,
             message="Message is fully consumed or does not exist.",
-            status_code=500,
+            status_code=400,
         ) from err
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/blocks.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/call.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/call.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/classes.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/classes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/misc.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/misc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/routes.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/routes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec_write.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_trace_spec.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/schema.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/schema.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/state.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/storage.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/storage.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/payloads.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/payloads.py`

 * *Files 4% similar despite different names*

```diff
@@ -1002,37 +1002,99 @@
             )
 
         result.append(trace)
 
     return result
 
 
+def gateway_to_rpc_invocation(
+    invocation_dict: Optional[dict],
+) -> Optional[Dict[str, Dict]]:
+    """
+    Convert function invocation result from gateway to RPC.
+    """
+    if invocation_dict is None:
+        return invocation_dict
+
+    # All unnecessary properties should be removed except these mentioned here.
+    accepted_properties = {
+        "contract_address",
+        "entry_point_selector",
+        "calldata",
+        "call_type",
+        "caller_address",
+        "entry_point_type",
+        "class_hash",
+        "result",
+        "calls",
+        "events",
+        "messages",
+    }
+
+    # Map calls from internal_calls and process recursively
+    invocation_dict["calls"] = [
+        gateway_to_rpc_invocation(nested_call)
+        for nested_call in invocation_dict["internal_calls"]
+    ]
+
+    for event in invocation_dict["events"]:
+        del event["order"]
+
+    for message in invocation_dict["messages"]:
+        del message["order"]
+        message["from_address"] = invocation_dict["caller_address"]
+
+    invocation_dict["entry_point_selector"] = invocation_dict["selector"]
+
+    return {
+        key: invocation_dict[key]
+        for key in invocation_dict
+        if key in accepted_properties
+    }
+
+
 def rpc_invoke_txn_trace(trace_dict: dict) -> Dict[str, Dict]:
     """
     Mapping for the execution trace of a invoke transaction.
     """
     return {
-        "validate_invocation": trace_dict.get("validate_invocation"),
-        "execute_invocation": trace_dict.get("function_invocation"),
-        "fee_transfer_invocation": trace_dict.get("fee_transfer_invocation"),
+        "validate_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("validate_invocation")
+        ),
+        "execute_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("function_invocation")
+        ),
+        "fee_transfer_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("fee_transfer_invocation")
+        ),
     }
 
 
 def rpc_declare_txn_trace(trace_dict: dict) -> Dict[str, Dict]:
     """
     Mapping for the execution trace of a declare transaction.
     """
     return {
-        "validate_invocation": trace_dict.get("validate_invocation"),
-        "fee_transfer_invocation": trace_dict.get("fee_transfer_invocation"),
+        "validate_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("validate_invocation")
+        ),
+        "fee_transfer_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("fee_transfer_invocation")
+        ),
     }
 
 
 def rpc_deploy_account_txn_trace(trace_dict: dict) -> Dict[str, Dict]:
     """
     Mapping for the execution trace of a deploy account transaction.
     """
     return {
-        "validate_invocation": trace_dict.get("validate_invocation"),
-        "constructor_invocation": trace_dict.get("function_invocation"),
-        "fee_transfer_invocation": trace_dict.get("fee_transfer_invocation"),
+        "validate_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("validate_invocation")
+        ),
+        "constructor_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("function_invocation")
+        ),
+        "fee_transfer_invocation": gateway_to_rpc_invocation(
+            trace_dict.get("fee_transfer_invocation")
+        ),
     }
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/responses.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         return _events
 
     def status() -> TxnStatus:
         mapping: Dict[TransactionStatus, TxnStatus] = {
             TransactionStatus.ACCEPTED_ON_L2: "ACCEPTED_ON_L2",
             TransactionStatus.ACCEPTED_ON_L1: "ACCEPTED_ON_L1",
             TransactionStatus.RECEIVED: "PENDING",
-            TransactionStatus.PENDING: "PENDING",
             TransactionStatus.REJECTED: "REJECTED",
         }
         return mapping[txr.status]
 
     async def txn_type() -> RpcTxnType:
         transaction = await state.starknet_wrapper.transactions.get_transaction(
             hex(txr.transaction_hash)
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/types.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/types.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/transactions.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/transactions.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/utils.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/blueprints/shared.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/shared.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/cairo_rs_py_patch.py` & `starknet_devnet-0.5.5a0/starknet_devnet/cairo_rs_py_patch.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/chargeable_account.py` & `starknet_devnet-0.5.5a0/starknet_devnet/chargeable_account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/compiler.py` & `starknet_devnet-0.5.5a0/starknet_devnet/compiler.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/constants.py` & `starknet_devnet-0.5.5a0/starknet_devnet/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 OLD_SUPPORTED_VERSIONS = [0]
 
 # account used by Starknet CLI; calculated using
 # poetry run python scripts/compute_compiled_class_hash.py \
 #   ~/.cache/pypoetry/virtualenvs/<YOUR_VENV>/lib/python3.9/site-packages/starkware/starknet/third_party/open_zeppelin/account.json
 STARKNET_CLI_ACCOUNT_CLASS_HASH = (
-    0x7AB95E820D92B974797C8F139AD72F8550ADAA068FEBE4E38DA9A4A9539A81D
+    0x2AF01407D426B1FFF03A6982813EA9F3E9467B2B19EDCC9FB612C3B5B6FFCEB
 )
 
 # starkware.starknet.public.abi.get_selector_from_name("replace_class")
 REPLACE_CLASS_SELECTOR = (
     0x217DF192877EED2921E241046523F8D8DA7981F0A3DDAFE0E7517F6523276D2
 )
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/contract_class_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/contract_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/devnet_config.py` & `starknet_devnet-0.5.5a0/starknet_devnet/devnet_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,14 @@
 }
 NETWORK_NAMES = ", ".join(NETWORK_TO_URL.keys())
 CHAIN_IDS = ", ".join([member.name for member in StarknetChainId])
 DEFAULT_CHAIN_ID = StarknetChainId.TESTNET
 
 DEFAULT_COMPILER_ARGS = [
     "--add-pythonic-hints",
-    "--allowed-libfuncs-list-name",
-    "experimental_v0.1.0",
 ]
 
 
 def _fork_network(network_id: str):
     """
     Return the URL corresponding to the provided name.
     If it's not one of predefined names, assumes it is already a URL.
@@ -270,15 +268,15 @@
         sys.exit("Error: The argument of --sierra-compiler-path must be an executable")
 
     _assert_valid_compiler([compiler_path, "--version"])
     return compiler_path
 
 
 def _parse_compiler_args(compiler_args: str):
-    return compiler_args.split()
+    return compiler_args.strip().split()
 
 
 def parse_args(raw_args: List[str]):
     """
     Parses CLI arguments.
     """
     parser = argparse.ArgumentParser(
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/dump.py` & `starknet_devnet-0.5.5a0/starknet_devnet/dump.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/fee_token.py` & `starknet_devnet-0.5.5a0/starknet_devnet/fee_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Fee token and its predefined constants.
 """
 import pprint
 import sys
 
 from starkware.solidity.utils import load_nearby_contract
+from starkware.starknet.business_logic.state.storage_domain import StorageDomain
 from starkware.starknet.business_logic.transaction.objects import InternalInvokeFunction
 from starkware.starknet.compiler.compile import get_selector_from_name
 from starkware.starknet.services.api.contract_class.contract_class import (
     CompiledClassBase,
     DeprecatedCompiledClass,
 )
 from starkware.starknet.services.api.gateway.transaction import InvokeFunction
@@ -54,32 +55,36 @@
     def contract_class(self) -> DeprecatedCompiledClass:
         """Same as `get_contract_class`, used by `PredeployedContractWrapper` parent"""
         return self.get_contract_class()
 
     async def _mimic_constructor(self):
         starknet: Starknet = self.starknet_wrapper.starknet
         await starknet.state.state.set_storage_at(
-            FeeToken.ADDRESS,
-            get_selector_from_name("ERC20_name"),
-            str_to_felt(FeeToken.NAME),
+            storage_domain=StorageDomain.ON_CHAIN,
+            contract_address=FeeToken.ADDRESS,
+            key=get_selector_from_name("ERC20_name"),
+            value=str_to_felt(FeeToken.NAME),
         )
         await starknet.state.state.set_storage_at(
-            FeeToken.ADDRESS,
-            get_selector_from_name("ERC20_symbol"),
-            str_to_felt(FeeToken.SYMBOL),
+            storage_domain=StorageDomain.ON_CHAIN,
+            contract_address=FeeToken.ADDRESS,
+            key=get_selector_from_name("ERC20_symbol"),
+            value=str_to_felt(FeeToken.SYMBOL),
         )
         await starknet.state.state.set_storage_at(
-            FeeToken.ADDRESS,
-            get_selector_from_name("ERC20_decimals"),
-            18,
+            storage_domain=StorageDomain.ON_CHAIN,
+            contract_address=FeeToken.ADDRESS,
+            key=get_selector_from_name("ERC20_decimals"),
+            value=18,
         )
         await starknet.state.state.set_storage_at(
-            FeeToken.ADDRESS,
-            get_selector_from_name("Ownable_owner"),
-            ChargeableAccount.ADDRESS,
+            storage_domain=StorageDomain.ON_CHAIN,
+            contract_address=FeeToken.ADDRESS,
+            key=get_selector_from_name("Ownable_owner"),
+            value=ChargeableAccount.ADDRESS,
         )
 
     async def get_balance(self, address: int) -> int:
         """Return the balance of the contract under `address`."""
         response = await self.contract.balanceOf(address).call()
 
         balance = Uint256(
@@ -98,15 +103,17 @@
         ]
 
         version = SUPPORTED_TX_VERSION
         max_fee = int(1e18)  # big enough
 
         # we need a funded account for this since the tx has to be signed and a fee will be charged
         # a user-intedded predeployed account cannot be used for this
-        nonce = await starknet.state.state.get_nonce_at(ChargeableAccount.ADDRESS)
+        nonce = await starknet.state.state.get_nonce_at(
+            StorageDomain.ON_CHAIN, ChargeableAccount.ADDRESS
+        )
         chargeable_address = hex(ChargeableAccount.ADDRESS)
         signature, execute_calldata = get_execute_args(
             calls=[(hex(FeeToken.ADDRESS), "mint", calldata)],
             account_address=chargeable_address,
             private_key=ChargeableAccount.PRIVATE_KEY,
             nonce=nonce,
             version=version,
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/forked_state.py` & `starknet_devnet-0.5.5a0/starknet_devnet/forked_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Forked state"""
 
 import json
 
 from services.external_api.client import BadRequest
 from starkware.starknet.business_logic.state.state import BlockInfo, CachedState
 from starkware.starknet.business_logic.state.state_api import StateReader
+from starkware.starknet.business_logic.state.storage_domain import StorageDomain
 from starkware.starknet.core.os.contract_class.compiled_class_hash import (
     compute_compiled_class_hash,
 )
 from starkware.starknet.definitions.constants import UNINITIALIZED_CLASS_HASH
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.definitions.general_config import StarknetChainId
 from starkware.starknet.services.api.contract_class.contract_class import (
@@ -158,21 +159,25 @@
                 )
             return int(class_hash_hex, 16)
         except BadRequest as bad_request:
             if is_originally_starknet_exception(bad_request):
                 return int.from_bytes(UNINITIALIZED_CLASS_HASH, "big")
             raise
 
-    async def get_nonce_at(self, contract_address: int) -> int:
+    async def get_nonce_at(
+        self, storage_domain: StorageDomain, contract_address: int
+    ) -> int:
         return await self.__feeder_gateway_client.get_nonce(
             contract_address=contract_address,
             block_number=self.__block_number,
         )
 
-    async def get_storage_at(self, contract_address: int, key: int) -> int:
+    async def get_storage_at(
+        self, storage_domain: StorageDomain, contract_address: int, key: int
+    ) -> int:
         storage_hex = await self.__feeder_gateway_client.get_storage_at(
             contract_address=contract_address,
             key=key,
             block_number=self.__block_number,
         )
         return int(storage_hex, 16)
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/general_config.py` & `starknet_devnet-0.5.5a0/starknet_devnet/general_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/origin.py` & `starknet_devnet-0.5.5a0/starknet_devnet/origin.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/postman_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/postman_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/predeployed_contract_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/predeployed_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/server.py` & `starknet_devnet-0.5.5a0/starknet_devnet/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 @app.errorhandler(json.decoder.JSONDecodeError)
 def handle_json_decode_error(error: json.decoder.JSONDecodeError):
     """Handles json error"""
     return {
         "message": f"Error while decoding JSON: {error}",
         "code": str(StarkErrorCode.MALFORMED_REQUEST),
-    }, 500
+    }, 400
 
 
 @app.route("/api", methods=["GET"])
 def api():
     """Return available endpoints."""
     routes = {}
     for url in app.url_map.iter_rules():
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/starknet_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/starknet_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pprint
 from copy import deepcopy
 from types import TracebackType
 from typing import Dict, List, Optional, Set, Tuple, Type, Union
 
 import cloudpickle as pickle
 from starkware.starknet.business_logic.state.state import BlockInfo, CachedState
+from starkware.starknet.business_logic.state.storage_domain import StorageDomain
 from starkware.starknet.business_logic.transaction.fee import calculate_tx_fee
 from starkware.starknet.business_logic.transaction.objects import (
     CallInfo,
     InternalDeclare,
     InternalDeploy,
     InternalDeployAccount,
     InternalInvokeFunction,
@@ -182,27 +183,32 @@
             self.__initialized = True
 
     async def __create_genesis_block(self):
         """Create genesis block"""
         transactions: List[DevnetTransaction] = []
         transaction_hash = 1
 
+        self.genesis_block_number = self.blocks.get_next_block_number()
+
         # Declare transactions
         declare_hashes = [
             FeeToken.HASH,
             UDC.HASH,
             self.config.account_class.hash,
             STARKNET_CLI_ACCOUNT_CLASS_HASH,
         ]
         for class_hash in declare_hashes:
             internal_declare = create_empty_internal_declare(
                 transaction_hash, class_hash
             )
             declare_transaction = create_genesis_block_transaction(
-                internal_declare, TransactionType.DECLARE
+                internal_declare,
+                TransactionType.DECLARE,
+                block_number=self.genesis_block_number,
+                transaction_index=len(transactions),
             )
             transactions.append(declare_transaction)
             transaction_hash += 1
 
         # Deploy transactions
         deploy_data = [
             (FeeToken.HASH, FeeToken.ADDRESS),
@@ -214,30 +220,29 @@
 
         for class_hash, contract_address in deploy_data:
             # this might be the only place where DEPLOY tx is used
             internal_deploy = create_empty_internal_deploy(
                 transaction_hash, class_hash, contract_address
             )
             deploy_transaction = create_genesis_block_transaction(
-                internal_deploy, TransactionType.DEPLOY
+                internal_deploy,
+                TransactionType.DEPLOY,
+                block_number=self.genesis_block_number,
+                transaction_index=len(transactions),
             )
             transactions.append(deploy_transaction)
             transaction_hash += 1
 
         self._update_block_number()
         state = self.get_state()
         state_update = await self.update_pending_state()
         await self.blocks.generate_pending(transactions, state, state_update)
-        block = await self.generate_latest_block(block_hash=0)
-
-        # Set the genesis block number
-        self.genesis_block_number = block.block_number
+        await self.generate_latest_block(block_hash=0)
 
         for transaction in transactions:
-            transaction.set_block(block=block)
             self.transactions.store(transaction.transaction_hash, transaction)
 
     async def create_empty_block(self) -> StarknetBlock:
         """Create empty block."""
         self._update_block_number()
         state_update = await self.update_pending_state()
         self.__latest_state = self.get_state().copy()
@@ -473,20 +478,22 @@
                     )
 
                     transaction = DevnetTransaction(
                         internal_tx=self.internal_tx,
                         status=status,
                         execution_info=TransactionExecutionInfo.empty(),
                         transaction_hash=tx_hash,
+                        block_number=None,  # Rejected txs have no block number
+                        transaction_index=None,  # Rejected txs have no tx index
                     )
                     self.starknet_wrapper._store_transaction(
                         transaction, error_message=exc.message
                     )
                 else:
-                    status = TransactionStatus.PENDING
+                    status = TransactionStatus.ACCEPTED_ON_L2
 
                     assert self.execution_info is not None
                     if self.execution_info.call_info:
                         await self.starknet_wrapper._register_new_contracts(
                             self.internal_calls,
                             tx_hash,
                             self.deployed_contracts,
@@ -495,19 +502,25 @@
                     state_update = await self.starknet_wrapper.update_pending_state(
                         deployed_contracts=self.deployed_contracts,
                         explicitly_declared=self.explicitly_declared,
                         explicitly_declared_old=self.explicitly_declared_old,
                         visited_storage_entries=self.visited_storage_entries,
                     )
 
+                    next_block_number = (
+                        self.starknet_wrapper.blocks.get_next_block_number()
+                    )
+
                     transaction = DevnetTransaction(
                         internal_tx=self.internal_tx,
                         status=status,
                         execution_info=self.execution_info,
                         transaction_hash=tx_hash,
+                        block_number=next_block_number,
+                        transaction_index=len(self.starknet_wrapper.pending_txs),
                     )
                     self.starknet_wrapper.pending_txs.append(transaction)
                     self.starknet_wrapper._store_transaction(transaction)
 
                     await self.starknet_wrapper.update_pending_block(state_update)
 
                     if not self.starknet_wrapper.config.blocks_on_demand:
@@ -660,28 +673,32 @@
         Return compiled class given the class hash (sierra hash).
         Should report an undeclared class if given the hash of a deprecated class
         """
         state = self.get_state().state
 
         # first handle the case of artifact being locally present
         if class_hash in self._contract_classes:
+            contract_class = self._contract_classes[class_hash]
+            if isinstance(contract_class, DeprecatedCompiledClass):
+                # should raise if class hash does not belong to sierra of a cairo 1 contract
+                raise UndeclaredClassDevnetException(class_hash)
+
             compiled_class_hash = await state.get_compiled_class_hash(class_hash)
             return await state.get_compiled_class(compiled_class_hash)
 
         try:
             # directly on state_reader to ensure overridden method is called if forking
             compiled_class = await state.state_reader.get_compiled_class_by_class_hash(
                 class_hash
             )
             if isinstance(compiled_class, CompiledClass):
                 return compiled_class
         except AssertionError:
             # the received hash is compiled_class_hash of a cairo1 class
             pass
-
         raise UndeclaredClassDevnetException(class_hash)
 
     async def get_class_hash_at(
         self, contract_address: int, block_id: BlockId = DEFAULT_BLOCK_ID
     ) -> int:
         """Return class hash given the contract address"""
         state = await self.__get_query_state(block_id)
@@ -730,15 +747,19 @@
         key: int,
         block_id: BlockId = DEFAULT_BLOCK_ID,
     ) -> Felt:
         """
         Returns the storage identified by `key` from the contract at `contract_address`.
         """
         state = await self.__get_query_state(block_id)
-        return hex(await state.state.get_storage_at(contract_address, key))
+        return hex(
+            await state.state.get_storage_at(
+                StorageDomain.ON_CHAIN, contract_address, key
+            )
+        )
 
     async def load_messaging_contract_in_l1(
         self, network_url: str, contract_address: str, network_id: str
     ) -> dict:
         """Loads the messaging contract at `contract_address`"""
         return self.l1l2.load_l1_messaging_contract(
             self.starknet, network_url, contract_address, network_id
@@ -940,15 +961,15 @@
         self.block_info_generator.set_gas_price(gas_price)
 
     async def get_nonce(
         self, contract_address: int, block_id: BlockId = DEFAULT_BLOCK_ID
     ):
         """Returns nonce of contract with `contract_address`"""
         state = await self.__get_query_state(block_id)
-        return await state.state.get_nonce_at(contract_address)
+        return await state.state.get_nonce_at(StorageDomain.ON_CHAIN, contract_address)
 
     async def __predeclare_starknet_cli_account(self):
         """Predeclares the account class used by Starknet CLI"""
         state = self.get_state().state
         state.compiled_classes[STARKNET_CLI_ACCOUNT_CLASS_HASH] = oz_account_class
         if self.config.verbose or not self.config.hide_predeployed_contracts:
             print("Predeclared Starknet CLI account: ", flush=True)
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/state.py` & `starknet_devnet-0.5.5a0/starknet_devnet/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/state_archive.py` & `starknet_devnet-0.5.5a0/starknet_devnet/state_archive.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/transactions.py` & `starknet_devnet-0.5.5a0/starknet_devnet/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Classes for storing and handling transactions.
 """
 
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 from services.everest.business_logic.transaction_execution_objects import (
     TransactionFailureReason,
 )
 from starkware.python.utils import to_bytes
 from starkware.starknet.business_logic.execution.objects import TransactionExecutionInfo
 from starkware.starknet.business_logic.transaction.objects import (
     InternalDeclare,
     InternalDeploy,
     InternalTransaction,
 )
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
+from starkware.starknet.definitions.transaction_type import TransactionType
 from starkware.starknet.services.api.feeder_gateway.response_objects import (
     Event,
     FunctionInvocation,
     L2ToL1Message,
     StarknetBlock,
     TransactionExecution,
     TransactionInfo,
@@ -34,31 +35,35 @@
 from .util import StarknetDevnetException
 
 
 # pylint: disable=too-many-instance-attributes
 class DevnetTransaction:
     """Represents the devnet transaction"""
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         internal_tx: InternalTransaction,
         status: TransactionStatus,
         execution_info: TransactionExecutionInfo,
-        transaction_hash: int = None,
+        block_number: Optional[int],
+        transaction_index: Optional[int],
+        transaction_hash: Optional[int] = None,
     ):
-        self.block = None
+        self.block: Optional[StarknetBlock] = None
         self.execution_info = execution_info
         if status != TransactionStatus.REJECTED and execution_info.call_info:
             self.execution_resources = execution_info.call_info.execution_resources
         else:
             self.execution_resources = None
         self.internal_tx = internal_tx
         self.status = status
         self.transaction_failure_reason = None
-        self.transaction_index = 0
+        self.transaction_index = transaction_index
+        self.__block_number = block_number
         self.transaction_hash = transaction_hash
 
         if transaction_hash is None:
             self.transaction_hash = internal_tx.hash_value
 
     def __get_actual_fee(self) -> int:
         """Returns the actual fee"""
@@ -97,18 +102,14 @@
 
         return l2_to_l1_messages
 
     def __get_block_hash(self) -> int:
         """Returns the block hash"""
         return self.block.block_hash if self.block else None
 
-    def __get_block_number(self) -> int:
-        """Returns the block number"""
-        return self.block.block_number if self.block else None
-
     def set_block(self, block: StarknetBlock):
         """Sets the block hash and number of the transaction"""
         self.block = block
 
     def set_failure_reason(self, error_message: str):
         """Sets the failure reason of the transaction"""
         self.transaction_failure_reason = TransactionFailureReason(
@@ -124,15 +125,15 @@
     def get_tx_info(self) -> TransactionInfo:
         """Returns the transaction info"""
         return TransactionInfo.create(
             status=self.status,
             transaction=self.internal_tx,
             transaction_index=self.transaction_index,
             block_hash=self.__get_block_hash(),
-            block_number=self.__get_block_number(),
+            block_number=self.__block_number,
             transaction_failure_reason=self.transaction_failure_reason,
         )
 
     def get_receipt(self) -> TransactionReceipt:
         """Returns the transaction receipt"""
         tx_info = self.get_tx_info()
 
@@ -322,15 +323,20 @@
         contract_address_salt=0,
         hash_value=tx_hash,
         version=0,
         constructor_calldata=[],
     )
 
 
-def create_genesis_block_transaction(internal_tx, tx_type) -> DevnetTransaction:
+def create_genesis_block_transaction(
+    internal_tx: InternalTransaction,
+    tx_type: TransactionType,
+    block_number: int,
+    transaction_index: int,
+) -> DevnetTransaction:
     "Create DevnetTransaction used in the genesis block"
     execution_info = TransactionExecutionInfo(
         validate_info=None,
         call_info=None,
         fee_transfer_info=None,
         actual_fee=0,
         actual_resources={
@@ -341,9 +347,11 @@
         },
         tx_type=tx_type,
     )
     return DevnetTransaction(
         internal_tx=internal_tx,
         status=TransactionStatus.ACCEPTED_ON_L2,
         execution_info=execution_info,
+        block_number=block_number,
+        transaction_index=transaction_index,
         transaction_hash=internal_tx.hash_value,
     )
```

### Comparing `starknet_devnet-0.5.4/starknet_devnet/udc.py` & `starknet_devnet-0.5.5a0/starknet_devnet/udc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.4/starknet_devnet/util.py` & `starknet_devnet-0.5.5a0/starknet_devnet/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pprint
 import sys
 from dataclasses import dataclass
 from typing import Dict, List, Set, Tuple
 
 from flask import request
 from starkware.starknet.business_logic.state.state import CachedState
+from starkware.starknet.business_logic.state.storage_domain import StorageDomain
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.services.api.feeder_gateway.response_objects import (
     ClassHashPair,
     ContractAddressHashPair,
     FeeEstimationInfo,
     StorageEntry,
 )
@@ -70,25 +71,26 @@
 
 class StarknetDevnetException(StarkException):
     """
     Exception raised across the project.
     Indicates the raised issue is devnet-related.
     """
 
-    def __init__(self, code: StarknetErrorCode, status_code=500, message=None):
+    def __init__(self, code: StarknetErrorCode, status_code=400, message=None):
         super().__init__(code=code, message=message)
         self.status_code = status_code
 
 
 class UndeclaredClassDevnetException(StarknetDevnetException):
     """Exception raised when Devnet has to return an undeclared class"""
 
     def __init__(self, class_hash: int):
         super().__init__(
             code=StarknetErrorCode.UNDECLARED_CLASS,
+            status_code=400,
             message=f"Class with hash {class_hash:#x} is not declared.",
         )
 
 
 def enable_pickling():
     """
     Extends the `StarknetContract` class to enable pickling.
@@ -192,23 +194,29 @@
 ):
     """Returns storages modified from change"""
     assert previous_state is not current_state
 
     storage_diffs: Dict[int, List[StorageEntry]] = {}
 
     for address, key in visited_storage_entries or {}:
-        old_storage_value = await previous_state.get_storage_at(address, key)
-        new_storage_value = await current_state.get_storage_at(address, key)
+        old_storage_value = await previous_state.get_storage_at(
+            StorageDomain.ON_CHAIN, address, key
+        )
+        new_storage_value = await current_state.get_storage_at(
+            StorageDomain.ON_CHAIN, address, key
+        )
         if old_storage_value != new_storage_value:
             if address not in storage_diffs:
                 storage_diffs[address] = []
             storage_diffs[address].append(
                 StorageEntry(
                     key=key,
-                    value=await current_state.get_storage_at(address, key),
+                    value=await current_state.get_storage_at(
+                        StorageDomain.ON_CHAIN, address, key
+                    ),
                 )
             )
 
     return storage_diffs
 
 
 async def assert_not_declared(class_hash: int, compiled_class_hash: int):
```

### Comparing `starknet_devnet-0.5.4/setup.py` & `starknet_devnet-0.5.5a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 package_data = \
 {'': ['*'],
  'starknet_devnet': ['accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/*']}
 
 install_requires = \
 ['Flask[async]>=2.0.3,<2.1.0',
  'Werkzeug>=2.0.3,<2.1.0',
- 'cairo-lang==0.11.2',
+ 'cairo-lang==0.12.0a0',
  'cloudpickle>=2.1.0,<2.2.0',
  'crypto-cpp-py>=1.4.0,<1.5.0',
  'flask-cors>=3.0.10,<3.1.0',
  'gunicorn>=20.1.0,<20.2.0',
  'jsonschema>=4.17.0,<4.18.0',
  'marshmallow-dataclass>=8.4,<8.5',
  'marshmallow>=3.17.0,<3.18.0',
@@ -27,15 +27,15 @@
  'web3>=6.0.0,<6.1.0']
 
 entry_points = \
 {'console_scripts': ['starknet-devnet = starknet_devnet.server:main']}
 
 setup_kwargs = {
     'name': 'starknet-devnet',
-    'version': '0.5.4',
+    'version': '0.5.5a0',
     'description': 'A local testnet for Starknet',
     'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!\n',
     'author': 'FabijanC',
     'author_email': 'fabijan.corak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xSpaceShard/starknet-devnet',
```

### Comparing `starknet_devnet-0.5.4/PKG-INFO` & `starknet_devnet-0.5.5a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: starknet-devnet
-Version: 0.5.4
+Version: 0.5.5a0
 Summary: A local testnet for Starknet
 Home-page: https://github.com/0xSpaceShard/starknet-devnet
 License: MIT
 Keywords: starknet,cairo,testnet,local,server
 Author: FabijanC
 Author-email: fabijan.corak@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask[async] (>=2.0.3,<2.1.0)
 Requires-Dist: Werkzeug (>=2.0.3,<2.1.0)
-Requires-Dist: cairo-lang (==0.11.2)
+Requires-Dist: cairo-lang (==0.12.0a0)
 Requires-Dist: cloudpickle (>=2.1.0,<2.2.0)
 Requires-Dist: crypto-cpp-py (>=1.4.0,<1.5.0)
 Requires-Dist: flask-cors (>=3.0.10,<3.1.0)
 Requires-Dist: gunicorn (>=20.1.0,<20.2.0)
 Requires-Dist: jsonschema (>=4.17.0,<4.18.0)
 Requires-Dist: marshmallow (>=3.17.0,<3.18.0)
 Requires-Dist: marshmallow-dataclass (>=8.4,<8.5)
```


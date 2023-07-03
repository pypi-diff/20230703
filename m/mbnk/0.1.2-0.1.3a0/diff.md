# Comparing `tmp/mbnk-0.1.2.tar.gz` & `tmp/mbnk-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.1.2.tar", max compression
+gzip compressed data, was "mbnk-0.1.3a0.tar", max compression
```

## Comparing `mbnk-0.1.2.tar` & `mbnk-0.1.3a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1799 2023-07-02 23:48:44.152523 mbnk-0.1.2/README.md
--rw-r--r--   0        0        0      275 2023-07-03 02:00:50.620267 mbnk-0.1.2/mbnk/__init__.py
--rw-r--r--   0        0        0    17863 2023-07-03 00:30:56.330813 mbnk-0.1.2/mbnk/api.py
--rw-r--r--   0        0        0      127 2023-07-02 23:03:02.426763 mbnk-0.1.2/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0      496 2023-07-03 01:58:35.864712 mbnk-0.1.2/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     1347 2023-07-02 22:17:52.460089 mbnk-0.1.2/mbnk/enums.py
--rw-r--r--   0        0        0      576 2023-07-03 00:10:27.269164 mbnk-0.1.2/mbnk/exceptions.py
--rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.2/mbnk/instances.py
--rw-r--r--   0        0        0      385 2023-07-03 01:59:23.280557 mbnk-0.1.2/mbnk/mbnk.py
--rw-r--r--   0        0        0     2262 2023-07-03 01:57:36.488901 mbnk-0.1.2/mbnk/responses.py
--rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.1.2/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.1.2/mbnk/utils/webhook.py
--rw-r--r--   0        0        0      313 2023-07-03 02:01:29.632134 mbnk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 mbnk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-02 23:48:44.152523 mbnk-0.1.3a0/README.md
+-rw-r--r--   0        0        0      275 2023-07-03 02:00:50.620267 mbnk-0.1.3a0/mbnk/__init__.py
+-rw-r--r--   0        0        0    18631 2023-07-03 20:39:34.795786 mbnk-0.1.3a0/mbnk/api.py
+-rw-r--r--   0        0        0      140 2023-07-03 20:40:21.439433 mbnk-0.1.3a0/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0     1031 2023-07-03 20:39:56.655610 mbnk-0.1.3a0/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     1347 2023-07-02 22:17:52.460089 mbnk-0.1.3a0/mbnk/enums.py
+-rw-r--r--   0        0        0      576 2023-07-03 00:10:27.269164 mbnk-0.1.3a0/mbnk/exceptions.py
+-rw-r--r--   0        0        0     2231 2023-07-03 20:43:41.014672 mbnk-0.1.3a0/mbnk/instances.py
+-rw-r--r--   0        0        0     1001 2023-07-03 20:42:01.586927 mbnk-0.1.3a0/mbnk/mbnk.py
+-rw-r--r--   0        0        0     2286 2023-07-03 20:44:17.082624 mbnk-0.1.3a0/mbnk/responses.py
+-rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.1.3a0/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.1.3a0/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      315 2023-07-03 20:49:16.142760 mbnk-0.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0     2332 1970-01-01 00:00:00.000000 mbnk-0.1.3a0/PKG-INFO
```

### Comparing `mbnk-0.1.2/README.md` & `mbnk-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.2/mbnk/api.py` & `mbnk-0.1.3a0/mbnk/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+__all__ = [
+    'MonobankOpenAPIModel',
+    'MonobankCorporateOpenAPIModel',
+    'MonoAcquiringAPIModel'
+]
+
 import re
 import json
 import requests
 
 from requests import Response
 from aiohttp import (
     ClientSession,
@@ -149,15 +155,15 @@
 
                 if self.__is_exception(response):
                     return MonoPayAPIException(**response_data)
 
                 return response_data
 
     @staticmethod
-    def request(
+    def _request(
             request_method: str,
             path: str
     ):
         def outer(func):
             def inner(*args, **kwargs):
                 self = args[0]
                 args = args[1:]
@@ -189,29 +195,29 @@
 
         return outer
 
 
 # Monobank Open API
 class Public(APIMethod):
 
-    @APIMethod.request("get", path=APIPaths.currencies_list)
+    @APIMethod._request("get", path=APIPaths.currencies_list)
     def currency(self, **kwargs) -> Union[CurrencyRatesResponse, MonobankAPIException]:
 
         return CurrencyRatesResponse(
             list=[
                 CurrencyListItem(
                     **item
                 ) for item in kwargs['response_data']
             ]
         )
 
 
 class Personal(APIMethod):
 
-    @APIMethod.request("get", path=APIPaths.personal_info)
+    @APIMethod._request("get", path=APIPaths.personal_info)
     def info(self, **kwargs) -> Union[ClientInfoResponse, MonobankAPIException]:
         """
         Source: https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1client-info/get
 
         :return:
         """
 
@@ -228,40 +234,62 @@
             jars=[
                 Jar(
                     **jar
                 ) for jar in kwargs['response_data']['jars']
             ]
         )
 
-    @APIMethod.request("post", path=APIPaths.personal_webhook)
+    @APIMethod._request("post", path=APIPaths.personal_webhook)
     def set_webhook(self, web_hook_url: str) -> Union[EmptyResponse, MonobankAPIException]:
         """
         Source: https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1webhook/post
 
         :param web_hook_url:
         :return:
         """
         return EmptyResponse()
 
-    @APIMethod.request("get", path=APIPaths.personal_statement)
+    @APIMethod._request("get", path=APIPaths.personal_statement)
     def statement(self, **kwargs) -> Union[StatementResponse, MonobankAPIException]:
 
         return StatementResponse(
             list=[
                 Transaction(
                     **transaction
                 ) for transaction in kwargs['response_data']
             ]
         )
 
 
-class Corporate(APIMethod):
+class MonobankOpenAPIModel:
+
+    __base_url = "https://api.monobank.ua"
+    __api_token = None
+    __headers = {}
+
+    def __init__(self, api_token: str, _async: bool):
+        self.__is_async = _async
+
+        self.__api_token__ = api_token
+        self.__headers["X-Token"] = self.__api_token__
 
-    __base_url__ = None
-    __headers__ = {}
+        self.public: Public = Public(
+            api_token=self.__api_token,
+            base_url=self.__base_url,
+            _async=self.__is_async
+        )
+
+        self.personal: Personal = Personal(
+            api_token=self.__api_token,
+            base_url=self.__base_url,
+            _async=self.__is_async
+        )
+
+
+class Corporate(APIMethod):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.auth: Authorization = Authorization(*args, **kwargs)
 
         self.client: Client = Client(*args, **kwargs)
@@ -271,83 +299,74 @@
 
     def info(self):
         pass
 
 
 class Client(APIMethod):
 
-    @APIMethod.request("post", path=APIPaths.init_access)
+    @APIMethod._request("post", path=APIPaths.init_access)
     def init_access(self):
         pass
 
-    @APIMethod.request("get", path=APIPaths.check_access)
+    @APIMethod._request("get", path=APIPaths.check_access)
     def check_access(self):
         pass
 
 
 class Authorization(APIMethod):
 
-    @APIMethod.request("post", path=APIPaths.auth_registration)
+    @APIMethod._request("post", path=APIPaths.auth_registration)
     def registration(self):
         pass
 
-    @APIMethod.request("post", path=APIPaths.auth_status)
+    @APIMethod._request("post", path=APIPaths.auth_status)
     def status(self):
         pass
 
 
-class MonobankOpenAPI:
+class MonobankCorporateOpenAPIModel:
 
-    __base_url = "https://api.monobank.ua"
-    __api_token = None
-    __headers = {}
+    __base_url: str = "https://api.monobank.ua"
+    __api_token: str = None
+    __headers: dict = {}
 
     def __init__(self, api_token: str, _async: bool):
-        self.__is_async = _async
+        self.__is_async: bool = _async
 
-        self.__api_token__ = api_token
+        self.__api_token: str = api_token
         self.__headers["X-Token"] = self.__api_token__
 
         self.public: Public = Public(
             api_token=self.__api_token,
             base_url=self.__base_url,
             _async=self.__is_async
         )
 
-        self.personal: Personal = Personal(
-            api_token=self.__api_token,
-            base_url=self.__base_url,
-            _async=self.__is_async
-        )
-
         self.corporate: Corporate = Corporate(
             api_token=self.__api_token,
             base_url=self.__base_url,
             _async=self.__is_async
         )
 
 
-class MonobankCorpAPI:
-    pass
-
 
 # MonoPay
 class Merchant(APIMethod):
 
-    @APIMethod.request("get", path=APIPaths.merchant_details)
+    @APIMethod._request("get", path=APIPaths.merchant_details)
     def details(self, **kwargs) -> Union[MerchantDetailsResponse, MonoPayAPIException]:
         """
         Mono Acquiring API: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1details/get
 
         :return: MerchantDetailsResponse
         """
 
         return MerchantDetailsResponse(**kwargs["response_data"])
 
-    @APIMethod.request("get", path=APIPaths.merchant_statement)
+    @APIMethod._request("get", path=APIPaths.merchant_statement)
     def statement(
             self,
             from_timestamp: int,
             to_timestamp: Optional[int] = None,
             **kwargs
     ) -> Union[MerchantStatementResponse, MonoPayAPIException]:
         """
@@ -368,28 +387,28 @@
                             **cancel_item
                         ) for cancel_item in statement_item['cancel_list']
                     ] if "cancel_list" in statement_item else None
                 ) for statement_item in kwargs['response_data']['list']
             ]
         )
 
-    @APIMethod.request("get", path=APIPaths.merchant_pubkey)
+    @APIMethod._request("get", path=APIPaths.merchant_pubkey)
     def pubkey(self, **kwargs) -> Union[MerchantPubKeyResponse, MonoPayAPIException]:
         """
         Mono Acquiring API Docs: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1pubkey/get
 
         :return: MerchantPubKeyResponse
         """
 
         return MerchantPubKeyResponse(**kwargs["response_data"])
 
 
 class Invoice(APIMethod):
 
-    @APIMethod.request("post", path=APIPaths.invoice_create)
+    @APIMethod._request("post", path=APIPaths.invoice_create)
     def create(
             self,
             amount: int,
             ccy: Optional[int] = None,
             merchant_paym_info: Optional = None,
             redirect_url: Optional[str] = None,
             web_hook_url: Optional[str] = None,
@@ -412,15 +431,15 @@
         :param qr_id:
         :param save_card_data:
         :return:
         """
 
         return InvoiceCreatedResponse(**kwargs['response_data'])
 
-    @APIMethod.request("post", path=APIPaths.invoice_split)
+    @APIMethod._request("post", path=APIPaths.invoice_split)
     def split(
             self,
             invoice_id: str,
             **kwargs
     ) -> Union[SplitInvoiceResponse, MonoPayAPIException]:
         """
         Mono Acquiring API:
@@ -428,15 +447,15 @@
         :param invoice_id:
         :param kwargs:
         :return:
         """
 
         return SplitInvoiceResponse(**kwargs['response_data'])
 
-    @APIMethod.request("post", path=APIPaths.invoice_cancel)
+    @APIMethod._request("post", path=APIPaths.invoice_cancel)
     def cancel(
             self,
             invoice_id: str,
             ext_ref: str = None,
             amount: int = None,
             items=None,
             **kwargs
@@ -464,15 +483,15 @@
         :param invoice_id:
         :param kwargs:
         :return:
         """
 
         return kwargs["response_data"]
 
-    @APIMethod.request("post", path=APIPaths.invoice_invalidation)
+    @APIMethod._request("post", path=APIPaths.invoice_invalidation)
     def invalidation(
             self,
             invoice_id: str,
             **kwargs
     ) -> Union[EmptyResponse, MonoPayAPIException]:
         """
         Source: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1invoice~1remove/post
@@ -480,14 +499,15 @@
         :param invoice_id:
         :param kwargs:
         :return:
         """
 
         return EmptyResponse()
 
+    @APIMethod._request("get", path=APIPaths.invoice_info)
     async def info(
             self,
             invoice_id: str,
             **kwargs
     ) -> Union[InvoiceInfoResponse, MonoPayAPIException]:
         """
         Source: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1invoice~1payment-info?invoiceId=%7BinvoiceId%7D/get
@@ -495,14 +515,15 @@
         :param invoice_id:
         :param kwargs:
         :return:
         """
 
         return kwargs['response_data']
 
+    @APIMethod._request("get", path=APIPaths.invoice_finalize)
     def finalize(
             self,
             invoice_id: str,
             amount: int,
             **kwargs
     ) -> Union[FinalizeInvoiceResponse, MonoPayAPIException]:
         """
@@ -516,74 +537,75 @@
         return FinalizeInvoiceResponse(
             **kwargs['response_data']
         )
 
 
 class Qr(APIMethod):
 
-    @APIMethod.request("get", path=APIPaths.qr_list)
+    @APIMethod._request("get", path=APIPaths.qr_list)
     def list(self, **kwargs) -> Union[QrListResponse, MonoPayAPIException]:
         return QrListResponse(
             list=[
                 QrListItem(
                     **qr
                 ) for qr in kwargs['response']['list']
             ]
         )
 
-    @APIMethod.request("post", path=APIPaths.qr_details)
+    @APIMethod._request("post", path=APIPaths.qr_details)
     def details(
             self,
             qr_id: str,
             **kwargs
     ) -> Union[QrDetailsResponse, MonoPayAPIException]:
         """
         :param qr_id:
         :return:
         """
         return QrDetailsResponse(**kwargs['response_data'])
 
-    @APIMethod.request("post", path=APIPaths.qr_reset_amount)
+    @APIMethod._request("post", path=APIPaths.qr_reset_amount)
     def reset_amount(
             self,
             qr_id: str,
             **kwargs
     ) -> Union[EmptyResponse, MonoPayAPIException]:
         """
         :param qr_id:
         :return:
         """
         return EmptyResponse()
 
 
 class Wallet(APIMethod):
 
-    @APIMethod.request("get", path=APIPaths.wallet_cards)
+    @APIMethod._request("get", path=APIPaths.wallet_cards)
     async def cards(
             self,
             wallet_id: str,
             **kwargs
     ):
         """
         Source: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1wallet/get
 
         :param wallet_id:
         :param kwargs:
         :return:
         """
         return kwargs["response_data"]
 
+    @APIMethod._request("post", path=APIPaths.wallet_payment)
     async def payment(self):
         """
         Source: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1wallet~1payment/post
         :return:
         """
         pass
 
-    @APIMethod.request("delete", path=APIPaths.wallet_delete_card)
+    @APIMethod._request("delete", path=APIPaths.wallet_delete_card)
     def delete_card(
             self,
             card_token: str,
             **kwargs
     ):
         """
         This method delete tokenized card from wallet
@@ -592,23 +614,23 @@
         :param card_token:
         :param kwargs:
         :return:
         """
         return kwargs["response_data"]
 
 
-class MonoPayAPI:
+class MonoAcquiringAPIModel:
 
-    __base_url = "https://api.monobank.ua/api"
-    __is_async = None
+    __base_url: str = "https://api.monobank.ua/api"
+    __is_async: bool = False
 
     def __init__(self, api_token: str, _async: bool):
 
-        self.__is_async = _async
-        self.__api_token = api_token
+        self.__is_async: bool = _async
+        self.__api_token: str = api_token
 
         self.merchant: Merchant = Merchant(
             api_token=self.__api_token,
             base_url=self.__base_url,
             _async=self.__is_async
         )
```

### Comparing `mbnk-0.1.2/mbnk/enums.py` & `mbnk-0.1.3a0/mbnk/enums.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.2/mbnk/exceptions.py` & `mbnk-0.1.3a0/mbnk/exceptions.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.2/mbnk/instances.py` & `mbnk-0.1.3a0/mbnk/instances.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 __all__ = [
-    # Monobank API Instances
+    # Monobank Open API Instances
     'CurrencyListItem',
     'Account',
     'Jar',
     'Transaction',
-    # MonoPay API Instances
+    # Monobank Corporate Open API Instances
+
+    # Mono Acquiring API Instances
     'QrListItem',
     'WalletItem',
     'CancelListItem',
     'MerchantStatementItem'
 ]
 
 
 from typing import List, Optional
 from dataclasses import dataclass
 
 
-# Monobank API Instances
+# Monobank Open API Instances
 @dataclass
 class CurrencyListItem:
     currency_code_a: int
     currency_code_b: int
     date: int
     rate_sell: float
     rate_buy: float
@@ -69,17 +71,15 @@
     receipt_id: Optional[str] = None
     invoice_id: Optional[str] = None
     counter_edrpou: Optional[str] = None
     counter_iban: Optional[str] = None
     counter_name: Optional[str] = None
 
 
-# MonoPay API Instances
-
-
+# Mono Acquiring API Instances
 @dataclass
 class QrListItem:
     short_qr_id: str
     qr_id: str
     amount_type: str
     page_url: str
```

### Comparing `mbnk-0.1.2/mbnk/responses.py` & `mbnk-0.1.3a0/mbnk/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
     'EmptyResponse',
 
     # Monobank Open API Responses
     'CurrencyRatesResponse',
     'ClientInfoResponse',
     'StatementResponse',
 
-    # Monobank Corp Open API Responses
+    # Monobank Corporate Open API Responses
 
-    # MonoPay API Responses
+    # Mono Acquiring API Responses
     'InvoiceCreatedResponse',
     'InvoiceCanceledResponse',
     'InvoiceStatusResponse',
     'InvoiceInfoResponse',
     'SplitInvoiceResponse',
     'FinalizeInvoiceResponse',
     'QrListResponse',
@@ -40,15 +40,15 @@
 
 
 @dataclass
 class EmptyResponse:
     pass
 
 
-# Monobank API Responses
+# Monobank Open API Responses
 @dataclass
 class CurrencyRatesResponse:
     list: List[CurrencyListItem]
 
 
 @dataclass
 class ClientInfoResponse:
@@ -61,15 +61,15 @@
 
 
 @dataclass
 class StatementResponse:
     list: List[Transaction]
 
 
-# MonoPay API Responses
+# Mono Acquiring API Responses
 @dataclass
 class InvoiceCreatedResponse:
     invoice_id: str
     page_url: str
 
 
 @dataclass
```

### Comparing `mbnk-0.1.2/PKG-INFO` & `mbnk-0.1.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.1.2
+Version: 0.1.3a0
 Summary: Sync/Async version monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


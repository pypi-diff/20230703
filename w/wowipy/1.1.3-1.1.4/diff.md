# Comparing `tmp/wowipy-1.1.3.tar.gz` & `tmp/wowipy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-1.1.3.tar", last modified: Tue Jun 27 14:19:54 2023, max compression
+gzip compressed data, was "wowipy-1.1.4.tar", last modified: Mon Jul  3 14:23:09 2023, max compression
```

## Comparing `wowipy-1.1.3.tar` & `wowipy-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 14:19:54.879138 wowipy-1.1.3/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.3/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-06-27 14:19:54.879138 wowipy-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-27 14:19:54.879138 wowipy-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-06-27 13:46:21.000000 wowipy-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:19:54.859192 wowipy-1.1.3/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.3/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.3/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    38772 2023-06-27 12:49:00.000000 wowipy-1.1.3/wowipy/models.py
--rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.3/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    41565 2023-06-27 14:00:21.000000 wowipy-1.1.3/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:19:54.878143 wowipy-1.1.3/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 14:23:09.090977 wowipy-1.1.4/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.4/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-07-03 14:23:09.090977 wowipy-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:23:09.090977 wowipy-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-03 14:23:07.000000 wowipy-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:23:09.073994 wowipy-1.1.4/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.4/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.4/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    49213 2023-06-30 09:34:21.000000 wowipy-1.1.4/wowipy/models.py
+-rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.4/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    43528 2023-06-30 09:41:11.000000 wowipy-1.1.4/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:23:09.089979 wowipy-1.1.4/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 14:23:08.000000 wowipy-1.1.4/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-1.1.3/COPYING` & `wowipy-1.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.3/LICENSE` & `wowipy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.3/PKG-INFO` & `wowipy-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.3
+Version: 1.1.4
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-1.1.3/setup.py` & `wowipy-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='1.1.3',
+    version='1.1.4',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
```

### Comparing `wowipy-1.1.3/wowipy/models.py` & `wowipy-1.1.4/wowipy/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,131 @@
 class Result:
     def __init__(self, status_code: int, message: str = '', data: List[Dict] = None):
         self.status_code = int(status_code)
         self.message = str(message)
         self.data = data if data else []
 
 
+class CraftActivity:
+    id_: int
+    code: str
+
+    def __init__(self, id_: int, code: str) -> None:
+        self.id_ = id_
+        self.code = code
+
+
+class PaymentFileStatus:
+    id_: int
+    code: str
+
+    def __init__(self, id_: int, code: str) -> None:
+        self.id_ = id_
+        self.code = code
+
+
+class SalesTax:
+    id_: int
+    code: str
+
+    def __init__(self, id_: int, code: str) -> None:
+        self.id_ = id_
+        self.code = code
+
+
+class CommissionType:
+    id_: int
+    code: str
+
+    def __init__(self, id_: int, code: str) -> None:
+        self.id_ = id_
+        self.code = code
+
+
+class CommissionStatus:
+    id_: int
+    code: str
+
+    def __init__(self, id_: int, code: str) -> None:
+        self.id_ = id_
+        self.code = code
+
+
+class Commission:
+    id_: int
+    id_num: str
+    code: str
+    recording_date: datetime
+    release_date: datetime
+    placing_date: Optional[datetime]
+    acceptance_date: Optional[datetime]
+    completion_date: Optional[datetime]
+    commission_type: CommissionType
+    commission_status: CommissionStatus
+
+    def __init__(self, id_: int,
+                 id_num: str,
+                 code: str,
+                 recording_date: str,
+                 release_date: str,
+                 placing_date: str,
+                 acceptance_date: str,
+                 completion_date: str,
+                 commission_type: Dict,
+                 commission_status: Dict) -> None:
+        self.id_ = id_
+        self.id_num = id_num
+        self.code = code
+        self.recording_date = datetime.strptime(recording_date, "%Y-%m-%dT%H:%M:%S%z")
+        if '.' in release_date:
+            self.release_date = datetime.strptime(release_date, "%Y-%m-%dT%H:%M:%S.%f%z")
+        else:
+            self.release_date = datetime.strptime(release_date, "%Y-%m-%dT%H:%M:%S%z")
+        if placing_date is not None:
+            if '.' in placing_date:
+                self.placing_date = datetime.strptime(placing_date, "%Y-%m-%dT%H:%M:%S.%f%z")
+            else:
+                self.placing_date = datetime.strptime(placing_date, "%Y-%m-%dT%H:%M:%S%z")
+        else:
+            self.placing_date = None
+        if acceptance_date is not None:
+            self.acceptance_date = datetime.strptime(acceptance_date, "%Y-%m-%dT%H:%M:%S.%f%z")
+        else:
+            self.acceptance_date = None
+        if completion_date is not None:
+            if '.' in completion_date:
+                self.completion_date = datetime.strptime(completion_date, "%Y-%m-%dT%H:%M:%S.%f%z")
+            else:
+                self.completion_date = datetime.strptime(completion_date, "%Y-%m-%dT%H:%M:%S%z")
+        else:
+            self.completion_date = None
+        commission_type["id_"] = commission_type.pop("id")
+        self.commission_type = CommissionType(**commission_type)
+        commission_status["id_"] = commission_status.pop("id")
+        self.commission_status = CommissionStatus(**commission_status)
+
+
+class Component:
+    id_: int
+    name: str
+
+    def __init__(self, id_: int, name: str) -> None:
+        self.id_ = id_
+        self.name = name
+
+
+class Facility:
+    id_: int
+    name: str
+
+    def __init__(self, id_: int, name: str) -> None:
+        self.id_ = id_
+        self.name = name
+
+
 class IdNameCombination:
     id_: int
     name: str
 
     def __init__(self, name: str, id_: int = None, **kwargs) -> None:
         if id_ is not None:
             self.id_ = id_
@@ -315,14 +432,215 @@
     def __init__(self, id_: int, name: str, code: str, arge_code: str = None) -> None:
         self.id_ = id_
         self.name = name
         self.code = code
         self.arge_code = arge_code
 
 
+class QuantityType:
+    id_: int
+    name: str
+    code: str
+    arge_code: Optional[str]
+
+    def __init__(self, id_: int, name: str, code: str, arge_code: str = None) -> None:
+        self.id_ = id_
+        self.name = name
+        self.code = code
+        self.arge_code = arge_code
+
+
+class ServiceCatalogue:
+    id_: int
+    id_num: str
+    description: str
+    quantity_type: Optional[QuantityType]
+
+    def __init__(self, id_: int, id_num: str, description: str, quantity_type: Dict) -> None:
+        self.id_ = id_
+        self.id_num = id_num
+        self.description = description
+        if quantity_type is not None:
+            self.quantity_type = QuantityType(**quantity_type)
+        else:
+            self.quantity_type = None
+
+
+class CommissionItem:
+    id_: int
+    code: str
+    unit_price: int
+    gross_amount: int
+    net_amount: int
+    units: int
+    commission_text: str
+    internal_description: str
+    position_number: int
+    sales_tax: SalesTax
+    service_catalogue: ServiceCatalogue
+    craft_activity: CraftActivity
+    quantity_type: Optional[QuantityType]
+    component: Optional[Component]
+    facility: Optional[Facility]
+    approved_net_amount: int
+    commission: Commission
+
+    def __init__(self, id_: int,
+                 code: str,
+                 unit_price: int,
+                 gross_amount: int,
+                 net_amount: int,
+                 units: int,
+                 commission_text: str,
+                 internal_description: str,
+                 position_number: int,
+                 sales_tax: Dict,
+                 service_catalogue: Dict,
+                 craft_activity: Dict,
+                 quantity_type: Dict,
+                 component: Dict,
+                 facility: Dict,
+                 approved_net_amount: int,
+                 commission: Dict) -> None:
+        self.id_ = id_
+        self.code = code
+        self.unit_price = unit_price
+        self.gross_amount = gross_amount
+        self.net_amount = net_amount
+        self.units = units
+        self.commission_text = commission_text
+        self.internal_description = internal_description
+        self.position_number = position_number
+        sales_tax["id_"] = sales_tax.pop("id")
+        self.sales_tax = SalesTax(**sales_tax)
+        service_catalogue["id_"] = service_catalogue.pop("id")
+        self.service_catalogue = ServiceCatalogue(**service_catalogue)
+        craft_activity["id_"] = craft_activity.pop("id")
+        self.craft_activity = CraftActivity(**craft_activity)
+        if quantity_type is not None:
+            quantity_type["id_"] = quantity_type.pop("id")
+            self.quantity_type = QuantityType(**quantity_type)
+        else:
+            self.quantity_type = None
+        if component is not None:
+            component["id_"] = component.pop("id")
+            self.component = Component(**component)
+        else:
+            self.component = None
+        if facility is not None:
+            facility["id_"] = facility.pop("id")
+            self.facility = Facility(**facility)
+        else:
+            self.facility = None
+        self.approved_net_amount = approved_net_amount
+        commission["id_"] = commission.pop("id")
+        self.commission = Commission(**commission)
+
+
+class PaymentOrderElement:
+    payment_order_number: str
+    maturity: datetime
+    transfer_date: datetime
+    payment_file_status: PaymentFileStatus
+
+    def __init__(self,
+                 payment_order_number: str,
+                 maturity: str,
+                 transfer_date: str,
+                 payment_file_status: Dict) -> None:
+        self.payment_order_number = payment_order_number
+        self.maturity = datetime.strptime(maturity, "%Y-%m-%d")
+        self.transfer_date = datetime.strptime(transfer_date, "%Y-%m-%d")
+        payment_file_status["id_"] = payment_file_status.pop("id")
+        self.payment_file_status = PaymentFileStatus(**payment_file_status)
+
+
+class TaxSubtotal:
+    net: int
+    vat: int
+    tax: CraftActivity
+
+    def __init__(self, net: int, vat: int, tax: CraftActivity) -> None:
+        self.net = net
+        self.vat = vat
+        self.tax = tax
+
+
+class TaxTotal:
+    tax_amount: int
+    tax_subtotal: List[TaxSubtotal]
+
+    def __init__(self, tax_amount: int, tax_subtotal: List[TaxSubtotal]) -> None:
+        self.tax_amount = tax_amount
+        self.tax_subtotal = tax_subtotal
+
+
+class MonetaryTotal:
+    tax_exclusive_amount: int
+    tax_inclusive_amount: int
+    labor_cost: int
+    material_cost: int
+
+    def __init__(self, tax_exclusive_amount: int, tax_inclusive_amount: int, labor_cost: int,
+                 material_cost: int) -> None:
+        self.tax_exclusive_amount = tax_exclusive_amount
+        self.tax_inclusive_amount = tax_inclusive_amount
+        self.labor_cost = labor_cost
+        self.material_cost = material_cost
+
+
+class InvoiceReceipt:
+    id_: int
+    number: str
+    company_code: CompanyCode
+    payment_orders: List[PaymentOrderElement]
+    invoice_date: datetime
+    maturity_date: datetime
+    monetary_total: MonetaryTotal
+    tax_total: TaxTotal
+    commission_items: List[CommissionItem]
+
+    def __init__(self, id_: int,
+                 number: str,
+                 company_code: Dict,
+                 invoice_date: str,
+                 maturity_date: str,
+                 monetary_total: Dict,
+                 tax_total: Dict,
+                 payment_orders: List[Dict],
+                 commission_items: List[Dict]) -> None:
+        self.id_ = id_
+        self.number = number
+        company_code["id_"] = company_code.pop("id")
+        self.company_code = CompanyCode(**company_code)
+        if '.' in invoice_date:
+            self.invoice_date = datetime.strptime(invoice_date, "%Y-%m-%dT%H:%M:%S.%f%z")
+        else:
+            self.invoice_date = datetime.strptime(invoice_date, "%Y-%m-%dT%H:%M:%S%z")
+        if '.' in maturity_date:
+            self.maturity_date = datetime.strptime(maturity_date, "%Y-%m-%dT%H:%M:%S.%f%z")
+        else:
+            self.maturity_date = datetime.strptime(maturity_date, "%Y-%m-%dT%H:%M:%S%z")
+        self.monetary_total = MonetaryTotal(**monetary_total)
+        self.tax_total = TaxTotal(**tax_total)
+        tpayment_orders = []
+        if payment_orders is not None:
+            for payment_order in payment_orders:
+                payment_order_obj = PaymentOrderElement(**payment_order)
+                tpayment_orders.append(payment_order_obj)
+        self.payment_orders = tpayment_orders
+        tcommission_items = []
+        if commission_items is not None:
+            for commission_item in commission_items:
+                commission_item["id_"] = commission_item.pop("id")
+                commission_item_obj = CommissionItem(**commission_item)
+                tcommission_items.append(commission_item_obj)
+        self.commission_items = tcommission_items
+
+
 class Address:
     id_: int
     zip_: str
     town: str
     street: str
     house_number: str
     house_number_addition: str
```

### Comparing `wowipy-1.1.3/wowipy/rest_adapter.py` & `wowipy-1.1.4/wowipy/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.3/wowipy/wowipy.py` & `wowipy-1.1.4/wowipy/wowipy.py`

 * *Files 4% similar despite different names*

```diff
@@ -674,14 +674,58 @@
             data['id_'] = data.pop('id')
             if data.get('estate_address') is not None:
                 data.get('estate_address')['zip_'] = data.get('estate_address').pop('zip')
             ret_la = Owner(**data)
             retlist.append(ret_la)
         return retlist
 
+    def get_commissioning_invoice_receipts(self,
+                                           limit: int = None,
+                                           offset: int = 0,
+                                           add_args: Dict = None,
+                                           fetch_all: bool = False) -> List[InvoiceReceipt]:
+        filter_params = {}
+        if limit is not None:
+            filter_params['limit'] = limit
+        filter_params['offset'] = offset
+
+        # Ein paar Standardwerte, können aber durch add_args überschrieben werden
+        filter_params['showNullValues'] = 'true'
+        filter_params['includePaymentOrder'] = 'true'
+
+        if add_args is not None:
+            filter_params.update(add_args)
+        retlist = []
+
+        if not fetch_all:
+            result = self._rest_adapter.get(endpoint='Commissioning/InvoiceReceipt/CommissionItems',
+                                            ep_params=filter_params)
+        else:
+            result = Result(0, "", [])
+            merge_schema = {"mergeStrategy": "append"}
+            merger = Merger(schema=merge_schema)
+            filter_params['offset'] = 0
+            filter_params['limit'] = 100
+            response_count = 100
+            while response_count == 100:
+                part_result = self._rest_adapter.get(endpoint='Commissioning/InvoiceReceipt/CommissionItems',
+                                                     ep_params=filter_params)
+                result.data = merger.merge(result.data, part_result.data)
+                filter_params['offset'] += 100
+                response_count = len(part_result.data)
+                print(f"Receipt-Count: {len(result.data)}")
+
+        for entry in result.data:
+            data = dict(humps.decamelize(entry))
+            data['id_'] = data.pop('id')
+            ret_la = InvoiceReceipt(**data)
+            retlist.append(ret_la)
+
+        return retlist
+
     def get_use_units(self,
                       use_unit_idnum: str = None,
                       building_land_idnum: str = None,
                       economic_unit_idnum: str = None,
                       management_idnum: str = None,
                       owner_number: str = None,
                       limit: int = None,
```

### Comparing `wowipy-1.1.3/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.4/wowipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.3
+Version: 1.1.4
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


# Comparing `tmp/octodns-dnsmadeeasy-0.0.3.tar.gz` & `tmp/octodns-dnsmadeeasy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-dnsmadeeasy-0.0.3.tar", last modified: Mon Jun 26 17:53:59 2023, max compression
+gzip compressed data, was "octodns-dnsmadeeasy-0.0.4.tar", last modified: Mon Jul  3 17:10:45 2023, max compression
```

## Comparing `octodns-dnsmadeeasy-0.0.3.tar` & `octodns-dnsmadeeasy-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.284079 octodns-dnsmadeeasy-0.0.3/
--rw-r--r--   0 yzguy      (501) staff       (20)     2193 2023-06-26 17:53:59.283924 octodns-dnsmadeeasy-0.0.3/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)     1854 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.3/README.md
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.282984 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy/
--rw-r--r--   0 yzguy      (501) staff       (20)    14740 2023-06-26 17:47:00.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy/__init__.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.283503 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/
--rw-r--r--   0 yzguy      (501) staff       (20)     2193 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)      322 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/SOURCES.txt
--rw-r--r--   0 yzguy      (501) staff       (20)        1 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/dependency_links.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      238 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/requires.txt
--rw-r--r--   0 yzguy      (501) staff       (20)       20 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/top_level.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      312 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.3/pyproject.toml
--rw-r--r--   0 yzguy      (501) staff       (20)       38 2023-06-26 17:53:59.284114 octodns-dnsmadeeasy-0.0.3/setup.cfg
--rw-r--r--   0 yzguy      (501) staff       (20)     1830 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.3/setup.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.283607 octodns-dnsmadeeasy-0.0.3/tests/
--rw-r--r--   0 yzguy      (501) staff       (20)    16135 2023-06-26 17:37:39.000000 octodns-dnsmadeeasy-0.0.3/tests/test_octodns_provider_dnsmadeeasy.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.333033 octodns-dnsmadeeasy-0.0.4/
+-rw-r--r--   0 yzguy      (501) staff       (20)     2331 2023-07-03 17:10:45.332912 octodns-dnsmadeeasy-0.0.4/PKG-INFO
+-rw-r--r--   0 yzguy      (501) staff       (20)     1992 2023-07-03 17:05:24.000000 octodns-dnsmadeeasy-0.0.4/README.md
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.331988 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy/
+-rw-r--r--   0 yzguy      (501) staff       (20)    15380 2023-07-03 17:10:07.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy/__init__.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.332541 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/
+-rw-r--r--   0 yzguy      (501) staff       (20)     2331 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/PKG-INFO
+-rw-r--r--   0 yzguy      (501) staff       (20)      322 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)        1 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)      246 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/requires.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)       20 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/top_level.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)      312 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.4/pyproject.toml
+-rw-r--r--   0 yzguy      (501) staff       (20)       38 2023-07-03 17:10:45.333068 octodns-dnsmadeeasy-0.0.4/setup.cfg
+-rw-r--r--   0 yzguy      (501) staff       (20)     2090 2023-07-03 17:05:24.000000 octodns-dnsmadeeasy-0.0.4/setup.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.332660 octodns-dnsmadeeasy-0.0.4/tests/
+-rw-r--r--   0 yzguy      (501) staff       (20)    22023 2023-07-03 17:05:24.000000 octodns-dnsmadeeasy-0.0.4/tests/test_octodns_provider_dnsmadeeasy.py
```

### Comparing `octodns-dnsmadeeasy-0.0.3/PKG-INFO` & `octodns-dnsmadeeasy-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-dnsmadeeasy
-Version: 0.0.3
+Version: 0.0.4
 Summary:  DNS Made Easy provider for octoDNS
 Home-page: https://github.com/octodns/octodns-dnsmadeeasy
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -52,14 +52,17 @@
     # Your DnsMadeEasy api key (required)
     api_key: env/DNSMADEEASY_API_KEY
     # Your DnsMadeEasy secret key (required)
     secret_key: env/DNSMADEEASY_SECRET_KEY
     # Whether or not to use Sandbox environment
     # (optional, default is false)
     #sandbox: true
+    # The maximum number of records to submit in one request to the DnsMadeEasy API
+    # (optional, default is 200)
+    #batch_size: 100
 ```
 
 ### Support Information
 
 #### Records
 
 DnsMadeEasyProvider supports A, AAAA, ALIAS (ANAME), CAA, CNAME, MX, NS, PTR, SPF, SRV, and TXT. There are some restrictions on CAA tags.
```

### Comparing `octodns-dnsmadeeasy-0.0.3/README.md` & `octodns-dnsmadeeasy-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,17 @@
     # Your DnsMadeEasy api key (required)
     api_key: env/DNSMADEEASY_API_KEY
     # Your DnsMadeEasy secret key (required)
     secret_key: env/DNSMADEEASY_SECRET_KEY
     # Whether or not to use Sandbox environment
     # (optional, default is false)
     #sandbox: true
+    # The maximum number of records to submit in one request to the DnsMadeEasy API
+    # (optional, default is 200)
+    #batch_size: 100
 ```
 
 ### Support Information
 
 #### Records
 
 DnsMadeEasyProvider supports A, AAAA, ALIAS (ANAME), CAA, CNAME, MX, NS, PTR, SPF, SRV, and TXT. There are some restrictions on CAA tags.
```

### Comparing `octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy/__init__.py` & `octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from requests import Session
 
 from octodns import __VERSION__ as octodns_version
 from octodns.provider import ProviderException
 from octodns.provider.base import BaseProvider
 from octodns.record import Record
 
-__VERSION__ = '0.0.3'
+__VERSION__ = '0.0.4'
 
 
 class DnsMadeEasyClientException(ProviderException):
     pass
 
 
 class DnsMadeEasyClientBadRequest(DnsMadeEasyClientException):
@@ -38,19 +38,27 @@
         super().__init__('Not Found')
 
 
 class DnsMadeEasyClient(object):
     PRODUCTION = 'https://api.dnsmadeeasy.com/V2.0/dns/managed'
     SANDBOX = 'https://api.sandbox.dnsmadeeasy.com/V2.0/dns/managed'
 
-    def __init__(self, api_key, secret_key, sandbox=False, ratelimit_delay=0.0):
+    def __init__(
+        self,
+        api_key,
+        secret_key,
+        sandbox=False,
+        ratelimit_delay=0.0,
+        batch_size=200,
+    ):
         self.api_key = api_key
         self.secret_key = secret_key
         self._base = self.SANDBOX if sandbox else self.PRODUCTION
         self.ratelimit_delay = ratelimit_delay
+        self.batch_size = batch_size
         self._sess = Session()
         self._sess.headers.update(
             {
                 'x-dnsme-apiKey': self.api_key,
                 'User-Agent': f'octodns/{octodns_version} octodns-dnsmadeasy/{__VERSION__}',
             }
         )
@@ -131,26 +139,36 @@
                     record['value'] = f'{value}.{zone_name}'
 
         return ret
 
     def record_multi_delete(self, zone_name, record_ids):
         zone_id = self.domains.get(zone_name, False)
         path = f'/{zone_id}/records'
-        self._request('DELETE', path, params={'ids': record_ids})
+
+        # there is a maximum batch size for bulk actions, batch the records based on our batch size
+        for batch in self._batch_records(record_ids):
+            self._request('DELETE', path, params={'ids': batch})
 
     def record_multi_create(self, zone_name, records):
         zone_id = self.domains.get(zone_name, False)
         path = f'/{zone_id}/records/createMulti'
 
-        # Change ALIAS records to ANAME
+        # change ALIAS records to ANAME
         for record in records:
             if record['type'] == 'ALIAS':
                 record['type'] = 'ANAME'
             record['gtdLocation'] = 'DEFAULT'
-        self._request('POST', path, data=records)
+
+        # there is a maximum batch size for bulk actions, batch the records based on our batch size
+        for batch in self._batch_records(records):
+            self._request('POST', path, data=batch)
+
+    def _batch_records(self, records):
+        for i in range(0, len(records), self.batch_size):
+            yield records[i : i + self.batch_size]
 
 
 class DnsMadeEasyProvider(BaseProvider):
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = False
     SUPPORTS_ROOT_NS = True
     SUPPORTS = set(
@@ -172,26 +190,28 @@
     def __init__(
         self,
         id,
         api_key,
         secret_key,
         sandbox=False,
         ratelimit_delay=0.0,
+        batch_size=200,
         *args,
         **kwargs,
     ):
         self.log = logging.getLogger(f'DnsMadeEasyProvider[{id}]')
         self.log.debug(
-            '__init__: id=%s, api_key=***, secret_key=***, sandbox=%s',
+            '__init__: id=%s, api_key=***, secret_key=***, sandbox=%s, batch_size=%s',
             id,
             sandbox,
+            batch_size,
         )
         super().__init__(id, *args, **kwargs)
         self._client = DnsMadeEasyClient(
-            api_key, secret_key, sandbox, ratelimit_delay
+            api_key, secret_key, sandbox, ratelimit_delay, batch_size
         )
 
         self._zone_records = {}
 
     def _data_for_multiple(self, _type, records):
         return {
             'ttl': records[0]['ttl'],
```

### Comparing `octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/PKG-INFO` & `octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-dnsmadeeasy
-Version: 0.0.3
+Version: 0.0.4
 Summary:  DNS Made Easy provider for octoDNS
 Home-page: https://github.com/octodns/octodns-dnsmadeeasy
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -52,14 +52,17 @@
     # Your DnsMadeEasy api key (required)
     api_key: env/DNSMADEEASY_API_KEY
     # Your DnsMadeEasy secret key (required)
     secret_key: env/DNSMADEEASY_SECRET_KEY
     # Whether or not to use Sandbox environment
     # (optional, default is false)
     #sandbox: true
+    # The maximum number of records to submit in one request to the DnsMadeEasy API
+    # (optional, default is 200)
+    #batch_size: 100
 ```
 
 ### Support Information
 
 #### Records
 
 DnsMadeEasyProvider supports A, AAAA, ALIAS (ANAME), CAA, CNAME, MX, NS, PTR, SPF, SRV, and TXT. There are some restrictions on CAA tags.
```

### Comparing `octodns-dnsmadeeasy-0.0.3/setup.py` & `octodns-dnsmadeeasy-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,18 +38,21 @@
 setup(
     author='Ross McFarland',
     author_email='rwmcfa1@gmail.com',
     description=description,
     extras_require={
         'dev': tests_require
         + (
-            'black>=22.3.0',
+            # we need to manually/explicitely bump major versions as they're
+            # likely to result in formatting changes that should happen in their
+            # own PR. This will basically happen yearly
+            # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
+            'black>=23.1.0,<24.0.0',
             'build>=0.7.0',
-            # >=5.12.0 does not support python 3.7, we still do
-            'isort==5.11.5',
+            'isort>=5.11.5',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         ),
         'test': tests_require,
     },
     install_requires=('octodns>=0.9.14', 'requests>=2.27.0'),
```

### Comparing `octodns-dnsmadeeasy-0.0.3/tests/test_octodns_provider_dnsmadeeasy.py` & `octodns-dnsmadeeasy-0.0.4/tests/test_octodns_provider_dnsmadeeasy.py`

 * *Files 13% similar despite different names*

```diff
@@ -440,7 +440,179 @@
 
         # recreate for update, and deletes for the 2 parts of the other
         provider._client._request.assert_has_calls(
             [call('DELETE', '/123123/records', params={'ids': [11189897]})],
             any_order=True,
         )
         self.assertEqual(2, provider._client._request.call_count)
+
+    def test_batching_requests(self):
+        # Create our provider with a batch size of 2
+        provider = DnsMadeEasyProvider(
+            'test', 'api', 'secret', True, batch_size=2, strict_supports=False
+        )
+
+        resp = Mock()
+        resp.json = Mock()
+        provider._client._request = Mock(return_value=resp)
+
+        provider._client.records = Mock(
+            return_value=[
+                {
+                    'id': 11189897,
+                    'name': 'www',
+                    'value': '1.2.3.4',
+                    'ttl': 300,
+                    'type': 'A',
+                },
+                {
+                    'id': 11189898,
+                    'name': 'www',
+                    'value': '2.2.3.4',
+                    'ttl': 300,
+                    'type': 'A',
+                },
+                {
+                    'id': 11189899,
+                    'name': 'ttl',
+                    'value': '3.2.3.4',
+                    'ttl': 600,
+                    'type': 'A',
+                },
+            ]
+        )
+
+        # Domain exists, we don't care about return
+
+        with open('tests/fixtures/dnsmadeeasy-domains.json') as fh:
+            domains = json.load(fh)
+
+        with open('tests/fixtures/dnsmadeeasy-domain-create.json') as fh:
+            created_domain = json.load(fh)
+
+        # non-existent domain, create everything
+        resp.json.side_effect = [
+            created_domain,  # GET /id/unit.tests during plan
+            domains,  # domains during plan
+            domains,  # domains during apply
+        ]
+
+        wanted = Zone('unit.tests.', [])
+        for i in range(1, 10):
+            wanted.add_record(
+                Record.new(
+                    wanted,
+                    f'www{i}',
+                    {'ttl': 300, 'type': 'A', 'value': f'3.2.3.{i}'},
+                )
+            )
+
+        plan = provider.plan(wanted)
+        self.assertEqual(11, len(plan.changes))
+        self.assertEqual(11, provider.apply(plan))
+
+        # recreate for update, and deletes for the 2 parts of the other
+        provider._client._request.assert_has_calls(
+            [
+                call(
+                    'DELETE',
+                    '/123123/records',
+                    params={'ids': [11189899, 11189897]},
+                ),
+                call('DELETE', '/123123/records', params={'ids': [11189898]}),
+                call(
+                    'POST',
+                    '/123123/records/createMulti',
+                    data=[
+                        {
+                            'value': '3.2.3.1',
+                            'type': 'A',
+                            'name': 'www1',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                        {
+                            'value': '3.2.3.2',
+                            'type': 'A',
+                            'name': 'www2',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                    ],
+                ),
+                call(
+                    'POST',
+                    '/123123/records/createMulti',
+                    data=[
+                        {
+                            'value': '3.2.3.3',
+                            'type': 'A',
+                            'name': 'www3',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                        {
+                            'value': '3.2.3.4',
+                            'type': 'A',
+                            'name': 'www4',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                    ],
+                ),
+                call(
+                    'POST',
+                    '/123123/records/createMulti',
+                    data=[
+                        {
+                            'value': '3.2.3.5',
+                            'type': 'A',
+                            'name': 'www5',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                        {
+                            'value': '3.2.3.6',
+                            'type': 'A',
+                            'name': 'www6',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                    ],
+                ),
+                call(
+                    'POST',
+                    '/123123/records/createMulti',
+                    data=[
+                        {
+                            'value': '3.2.3.7',
+                            'type': 'A',
+                            'name': 'www7',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                        {
+                            'value': '3.2.3.8',
+                            'type': 'A',
+                            'name': 'www8',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        },
+                    ],
+                ),
+                call(
+                    'POST',
+                    '/123123/records/createMulti',
+                    data=[
+                        {
+                            'value': '3.2.3.9',
+                            'type': 'A',
+                            'name': 'www9',
+                            'ttl': 300,
+                            'gtdLocation': 'DEFAULT',
+                        }
+                    ],
+                ),
+            ],
+            any_order=True,
+        )
+        self.assertEqual(9, provider._client._request.call_count)
```


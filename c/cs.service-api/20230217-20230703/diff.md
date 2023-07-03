# Comparing `tmp/cs.service_api-20230217.tar.gz` & `tmp/cs.service_api-20230703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.service_api-20230217.tar", last modified: Fri Feb 17 00:48:25 2023, max compression
+gzip compressed data, was "cs.service_api-20230703.tar", last modified: Mon Jul  3 10:10:01 2023, max compression
```

## Comparing `cs.service_api-20230217.tar` & `cs.service_api-20230703.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:48:25.866700 cs.service_api-20230217/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-02-17 00:48:16.000000 cs.service_api-20230217/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     2050 2023-02-17 00:48:25.866831 cs.service_api-20230217/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     2343 2023-02-17 00:48:17.000000 cs.service_api-20230217/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:48:25.862528 cs.service_api-20230217/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:48:25.862950 cs.service_api-20230217/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:48:25.864972 cs.service_api-20230217/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)     6415 2023-02-17 00:48:08.000000 cs.service_api-20230217/lib/python/cs/service_api.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:48:25.866486 cs.service_api-20230217/lib/python/cs.service_api.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     2050 2023-02-17 00:48:25.000000 cs.service_api-20230217/lib/python/cs.service_api.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      328 2023-02-17 00:48:25.000000 cs.service_api-20230217/lib/python/cs.service_api.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-02-17 00:48:25.000000 cs.service_api-20230217/lib/python/cs.service_api.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      178 2023-02-17 00:48:25.000000 cs.service_api-20230217/lib/python/cs.service_api.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-02-17 00:48:25.000000 cs.service_api-20230217/lib/python/cs.service_api.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     2433 2023-02-17 00:48:18.000000 cs.service_api-20230217/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1042 2023-02-17 00:48:25.867381 cs.service_api-20230217/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-02-17 00:48:17.000000 cs.service_api-20230217/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:10:01.203894 cs.service_api-20230703/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-07-03 10:09:49.000000 cs.service_api-20230703/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2106 2023-07-03 10:10:01.204026 cs.service_api-20230703/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2399 2023-07-03 10:09:50.000000 cs.service_api-20230703/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:10:01.198261 cs.service_api-20230703/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:10:01.198800 cs.service_api-20230703/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:10:01.201547 cs.service_api-20230703/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)     6845 2023-07-03 10:09:36.000000 cs.service_api-20230703/lib/python/cs/service_api.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:10:01.203591 cs.service_api-20230703/lib/python/cs.service_api.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2106 2023-07-03 10:10:01.000000 cs.service_api-20230703/lib/python/cs.service_api.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      328 2023-07-03 10:10:01.000000 cs.service_api-20230703/lib/python/cs.service_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-07-03 10:10:01.000000 cs.service_api-20230703/lib/python/cs.service_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      178 2023-07-03 10:10:01.000000 cs.service_api-20230703/lib/python/cs.service_api.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-07-03 10:10:01.000000 cs.service_api-20230703/lib/python/cs.service_api.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2489 2023-07-03 10:09:52.000000 cs.service_api-20230703/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1042 2023-07-03 10:10:01.204660 cs.service_api-20230703/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-07-03 10:09:50.000000 cs.service_api-20230703/setup.py
```

### Comparing `cs.service_api-20230217/PKG-INFO` & `cs.service_api-20230703/lib/python/cs.service_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cs.service_api
-Version: 20230217
+Name: cs.service-api
+Version: 20230703
 Summary: ServiceAPI, a base class for APIs which talk to a service, typically a web service via HTTP.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,16 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 ServiceAPI, a base class for APIs which talk to a service,
 typically a web service via HTTP.
 
-*Latest release 20230217*:
-Initial release.
+*Latest release 20230703*:
+Retry logic for requests.
 
 An instance of a `ServiceAPI` embodies some basic features
 that feel common to web based services:
 - a notion of a login
 - local state, an `SQLTags` for data about entities of the service
 - downloads, if that is a thing, with `FSTags` for file annotations
 
@@ -48,9 +48,12 @@
 
 `SewrviceAPI` base class for other APIs talking to services.
 
 # Release Log
 
 
 
+*Release 20230703*:
+Retry logic for requests.
+
 *Release 20230217*:
 Initial release.
```

### Comparing `cs.service_api-20230217/README.md` & `cs.service_api-20230703/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ServiceAPI, a base class for APIs which talk to a service,
 typically a web service via HTTP.
 
-*Latest release 20230217*:
-Initial release.
+*Latest release 20230703*:
+Retry logic for requests.
 
 An instance of a `ServiceAPI` embodies some basic features
 that feel common to web based services:
 - a notion of a login
 - local state, an `SQLTags` for data about entities of the service
 - downloads, if that is a thing, with `FSTags` for file annotations
 
@@ -60,9 +60,12 @@
 *Method `ServiceAPI.startup_shutdown(self)`*:
 Start up: open and init the `SQLTags`, open the `FSTags`.
 
 # Release Log
 
 
 
+*Release 20230703*:
+Retry logic for requests.
+
 *Release 20230217*:
 Initial release.
```

### Comparing `cs.service_api-20230217/lib/python/cs/service_api.py` & `cs.service_api-20230703/lib/python/cs/service_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from cs.fstags import FSTags
 from cs.logutils import warning
 from cs.pfx import pfx_call
 from cs.resources import MultiOpenMixin
 from cs.sqltags import SQLTags, SQLTagSet
 from cs.upd import uses_upd
 
-__version__ = '20230217'
+__version__ = '20230703'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
@@ -52,14 +52,16 @@
 }
 
 class ServiceAPI(MultiOpenMixin):
   ''' `SewrviceAPI` base class for other APIs talking to services.
   '''
 
   API_AUTH_GRACETIME = None
+  API_RETRY_COUNT = 3  # number of request attempts
+  API_RETRY_DELAY = 5  # interval between request retries
 
   @promote
   def __init__(self, *, sqltags: SQLTags):
     self.sqltags = sqltags
     self.fstags = None
     self._lock = RLock()
     self.login_state_mapping = None
@@ -177,15 +179,24 @@
       cookies = self.cookies
     url = _base_url + suburl
     rq_headers = {}
     rq_headers.update(self.default_headers)
     if headers is not None:
       rq_headers.update(headers)
     with upd.run_task(f'{_method} {url}'):
-      rsp = pfx_call(rqm, url, cookies=cookies, headers=rq_headers, **rqkw)
+      for retry in range(self.API_RETRY_COUNT, 0, -1):
+        try:
+          rsp = pfx_call(rqm, url, cookies=cookies, headers=rq_headers, **rqkw)
+          break
+        except requests.ConnectionError as e:
+          if retry <= 1:
+            # last retry
+            raise
+          warning("%s: %s, retrying in %ds", url, e, self.API_RETRY_DELAY)
+          time.sleep(self.API_RETRY_DELAY)
     if not _no_raise_for_status:
       rsp.raise_for_status()
     return rsp
 
   def json(self, suburl, _response_encoding=None, **kw):
     ''' Request `suburl` from the service, by default using a `GET`.
         Return the result decoded as JSON.
```

### Comparing `cs.service_api-20230217/lib/python/cs.service_api.egg-info/PKG-INFO` & `cs.service_api-20230703/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cs.service-api
-Version: 20230217
+Name: cs.service_api
+Version: 20230703
 Summary: ServiceAPI, a base class for APIs which talk to a service, typically a web service via HTTP.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,16 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 ServiceAPI, a base class for APIs which talk to a service,
 typically a web service via HTTP.
 
-*Latest release 20230217*:
-Initial release.
+*Latest release 20230703*:
+Retry logic for requests.
 
 An instance of a `ServiceAPI` embodies some basic features
 that feel common to web based services:
 - a notion of a login
 - local state, an `SQLTags` for data about entities of the service
 - downloads, if that is a thing, with `FSTags` for file annotations
 
@@ -48,9 +48,12 @@
 
 `SewrviceAPI` base class for other APIs talking to services.
 
 # Release Log
 
 
 
+*Release 20230703*:
+Retry logic for requests.
+
 *Release 20230217*:
 Initial release.
```

### Comparing `cs.service_api-20230217/setup.cfg` & `cs.service_api-20230703/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.service_api
-version = 20230217
+version = 20230703
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = ServiceAPI, a base class for APIs which talk to a service, typically a web service via HTTP.
 keywords = python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -18,22 +18,22 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
-	cs.context>=20230212
-	cs.deco>=20230212
-	cs.fstags>=20230217
+	cs.context>=20230331
+	cs.deco>=20230331
+	cs.fstags>=20230407
 	cs.logutils>=20230212
-	cs.pfx>=20221118
-	cs.resources>=20230217
-	cs.sqltags>=20230217
-	cs.upd>=20230217
+	cs.pfx>=20230604
+	cs.resources>=20230503
+	cs.sqltags>=20230612
+	cs.upd>=20230401
 	icontract
 	requests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


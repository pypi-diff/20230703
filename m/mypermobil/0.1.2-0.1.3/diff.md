# Comparing `tmp/mypermobil-0.1.2.tar.gz` & `tmp/mypermobil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypermobil-0.1.2.tar", last modified: Fri Jun 30 08:49:01 2023, max compression
+gzip compressed data, was "mypermobil-0.1.3.tar", last modified: Mon Jul  3 09:41:26 2023, max compression
```

## Comparing `mypermobil-0.1.2.tar` & `mypermobil-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 08:49:01.144258 mypermobil-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-06-26 13:05:01.000000 mypermobil-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      599 2023-06-30 08:49:01.145251 mypermobil-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-27 12:19:10.000000 mypermobil-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 08:49:01.118252 mypermobil-0.1.2/mypermobil/
--rw-rw-rw-   0        0        0      196 2023-06-28 08:53:52.000000 mypermobil-0.1.2/mypermobil/__init__.py
--rw-rw-rw-   0        0        0     3397 2023-06-27 11:58:00.000000 mypermobil-0.1.2/mypermobil/const.py
--rw-rw-rw-   0        0        0    10945 2023-06-30 08:46:21.000000 mypermobil-0.1.2/mypermobil/mypermobil.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:49:01.140252 mypermobil-0.1.2/mypermobil.egg-info/
--rw-rw-rw-   0        0        0      599 2023-06-30 08:49:01.000000 mypermobil-0.1.2/mypermobil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-30 08:49:01.000000 mypermobil-0.1.2/mypermobil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 08:49:01.000000 mypermobil-0.1.2/mypermobil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 08:49:01.000000 mypermobil-0.1.2/mypermobil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 08:49:01.000000 mypermobil-0.1.2/mypermobil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-06-27 12:17:06.000000 mypermobil-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      627 2023-06-30 08:49:01.148254 mypermobil-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      467 2023-06-30 08:46:45.000000 mypermobil-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:41:26.826207 mypermobil-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-26 13:05:01.000000 mypermobil-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      599 2023-07-03 09:41:26.827207 mypermobil-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-27 12:19:10.000000 mypermobil-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 09:41:26.791206 mypermobil-0.1.3/mypermobil/
+-rw-rw-rw-   0        0        0      196 2023-07-03 09:39:33.000000 mypermobil-0.1.3/mypermobil/__init__.py
+-rw-rw-rw-   0        0        0     3397 2023-06-27 11:58:00.000000 mypermobil-0.1.3/mypermobil/const.py
+-rw-rw-rw-   0        0        0    11236 2023-07-03 09:40:12.000000 mypermobil-0.1.3/mypermobil/mypermobil.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:41:26.822204 mypermobil-0.1.3/mypermobil.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-03 09:41:26.000000 mypermobil-0.1.3/mypermobil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-07-03 09:41:26.000000 mypermobil-0.1.3/mypermobil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:41:26.000000 mypermobil-0.1.3/mypermobil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 09:41:26.000000 mypermobil-0.1.3/mypermobil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-03 09:41:26.000000 mypermobil-0.1.3/mypermobil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-06-27 12:17:06.000000 mypermobil-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      627 2023-07-03 09:41:26.833212 mypermobil-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      467 2023-07-03 09:39:13.000000 mypermobil-0.1.3/setup.py
```

### Comparing `mypermobil-0.1.2/LICENSE` & `mypermobil-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypermobil-0.1.2/PKG-INFO` & `mypermobil-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypermobil
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python wrapper for the MyPermobil API
 Home-page: https://github.com/IsakNyberg/MyPermobil-API
 Author: Isak Nyberg
 Author-email: isak@nyberg.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IsakNyberg/MyPermobil-API/issues
 Project-URL: repository, https://github.com/IsakNyberg/MyPermobil-API
```

### Comparing `mypermobil-0.1.2/mypermobil/const.py` & `mypermobil-0.1.3/mypermobil/const.py`

 * *Files identical despite different names*

### Comparing `mypermobil-0.1.2/mypermobil/mypermobil.py` & `mypermobil-0.1.3/mypermobil/mypermobil.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """Validates an code."""
     try:
         _ = int(code)
     except ValueError as err:
         raise MyPermobilClientException("Code must be a number") from err
     if len(code) != 6:
         # the code must be 6 digits long
-        raise MyPermobilClientException("Invalid code")
+        raise MyPermobilClientException("Code must be 6 digits long")
     return code
 
 
 def validate_token(token: str) -> str:
     """Validates an token."""
     if not token or len(token) != 256:
         # the token must be 256 characters long
@@ -134,15 +134,17 @@
         self.request_timeout = request_timeout
 
         self.authenticated = False
 
     # Magic methods
     def __str__(self) -> str:
         """str."""
-        return f"MyPermobil({self.application}, {self.email}, {self.region}, {self.code}, {self.token}, {self.headers}, {self.expiration_date})"
+        app, email, region = self.application, self.email, self.region
+        code, token, exp = self.code, self.token, self.expiration_date
+        return f"Permobil({app}, {email}, {region}, {code}, {token}, {exp})"
 
     # Selectors
     @property
     def headers(self):
         """headers."""
         assert self.authenticated is True
         return {"Authorization": f"Bearer {self.token}"}
@@ -290,16 +292,19 @@
             self.authenticated = True
             if expiration_date is None:
                 # set expiration date to 1 year from now
                 time_delta = datetime.timedelta(days=365)
                 date = datetime.datetime.now() + time_delta
                 expiration_date = date.strftime("%Y-%m-%d")
             self.expiration_date = expiration_date
-
-        elif response.status in (400, 401, 403, 500):
+        elif response.status == 401:
+            raise MyPermobilAPIException("Email not registered for region")
+        elif response.status == 403:
+            raise MyPermobilAPIException("Incorrect code")
+        elif response.status in (400, 500):
             resp = await response.json()
             raise MyPermobilAPIException(resp.get("error", resp))
         else:
             text = await response.text()
             raise MyPermobilAPIException(text)
 
         return self.token, self.expiration_date
```

### Comparing `mypermobil-0.1.2/mypermobil.egg-info/PKG-INFO` & `mypermobil-0.1.3/mypermobil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypermobil
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python wrapper for the MyPermobil API
 Home-page: https://github.com/IsakNyberg/MyPermobil-API
 Author: Isak Nyberg
 Author-email: isak@nyberg.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IsakNyberg/MyPermobil-API/issues
 Project-URL: repository, https://github.com/IsakNyberg/MyPermobil-API
```

### Comparing `mypermobil-0.1.2/setup.cfg` & `mypermobil-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7970 6572 6d6f 6269 6c0d 0a76   = mypermobil..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e32 0d0a  ersion = 0.1.2..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e33 0d0a  ersion = 0.1.3..
 00000030: 6175 7468 6f72 203d 2049 7361 6b20 4e79  author = Isak Ny
 00000040: 6265 7267 0d0a 6175 7468 6f72 5f65 6d61  berg..author_ema
 00000050: 696c 203d 2069 7361 6b40 6e79 6265 7267  il = isak@nyberg
 00000060: 2e64 6576 0d0a 6465 7363 7269 7074 696f  .dev..descriptio
 00000070: 6e20 3d20 4120 7079 7468 6f6e 2077 7261  n = A python wra
 00000080: 7070 6572 2066 6f72 2061 2073 7562 7365  pper for a subse
 00000090: 7420 6f66 2074 6865 204d 7950 6572 6d6f  t of the MyPermo
```


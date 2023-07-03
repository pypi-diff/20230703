# Comparing `tmp/lhp-0.0.3.tar.gz` & `tmp/lhp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lhp-0.0.3.tar", max compression
+gzip compressed data, was "lhp-0.0.4.tar", max compression
```

## Comparing `lhp-0.0.3.tar` & `lhp-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-06-26 21:17:02.336231 lhp-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     5205 2023-06-26 21:17:02.336231 lhp-0.0.3/README.md
--rw-r--r--   0        0        0     2756 2023-06-26 21:17:26.068385 lhp-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      302 2023-06-26 21:17:02.340231 lhp-0.0.3/src/lhp/__init__.py
--rw-r--r--   0        0        0      221 2023-06-26 21:17:02.340231 lhp-0.0.3/src/lhp/exceptions.py
--rw-r--r--   0        0        0     4099 2023-06-26 21:17:02.340231 lhp-0.0.3/src/lhp/lhp.py
--rw-r--r--   0        0        0      366 2023-06-26 21:17:02.340231 lhp-0.0.3/src/lhp/models.py
--rw-r--r--   0        0        0        0 2023-06-26 21:17:02.340231 lhp-0.0.3/src/lhp/py.typed
--rw-r--r--   0        0        0     2201 2023-06-26 21:17:02.340231 lhp-0.0.3/src/lhp/util.py
--rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 lhp-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-03 11:09:21.826927 lhp-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     5205 2023-07-03 11:09:21.826927 lhp-0.0.4/README.md
+-rw-r--r--   0        0        0     2756 2023-07-03 11:09:37.150793 lhp-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      302 2023-07-03 11:09:21.826927 lhp-0.0.4/src/lhp/__init__.py
+-rw-r--r--   0        0        0      221 2023-07-03 11:09:21.826927 lhp-0.0.4/src/lhp/exceptions.py
+-rw-r--r--   0        0        0     4499 2023-07-03 11:09:21.826927 lhp-0.0.4/src/lhp/lhp.py
+-rw-r--r--   0        0        0      366 2023-07-03 11:09:21.826927 lhp-0.0.4/src/lhp/models.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:09:21.826927 lhp-0.0.4/src/lhp/py.typed
+-rw-r--r--   0        0        0     2201 2023-07-03 11:09:21.826927 lhp-0.0.4/src/lhp/util.py
+-rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 lhp-0.0.4/PKG-INFO
```

### Comparing `lhp-0.0.3/LICENSE.md` & `lhp-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lhp-0.0.3/README.md` & `lhp-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lhp-0.0.3/pyproject.toml` & `lhp-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lhp"
-version = "0.0.3"
+version = "0.0.4"
 description = "Asynchronous client for the Länderübergreifendes Hochwasserportal (LHP) API."
 authors = ["Karsten Bade <karsten@bade.dev>"]
 maintainers = ["Karsten Bade <karsten@bade.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/embeddedfiedel/python-lhp"
 repository = "https://github.com/embeddedfiedel/python-lhp"
```

### Comparing `lhp-0.0.3/src/lhp/lhp.py` & `lhp-0.0.4/src/lhp/lhp.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,23 +93,36 @@
         """Get current water level.
 
         Args:
             pgnr: The name of the water level measurement station.
 
         Returns:
             A CurrentWaterLevel object.
+
+        Raises:
+            LHPError: Received an unexpected response from the LHP
+                API.
         """
         url = URL(
             "https://hochwasserzentralen.api.proxy.bund.dev/"
             "webservices/get_infospegel.php"
         )
         data = {"pgnr": pgnr}
         result = await self._request(url=url, data=data)
 
         # Separate value from unit.
+        if result is None:
+            raise LHPError(
+                "Unexpected empty response from the LHP API",
+            )
+        if "W" not in result:
+            raise LHPError(
+                "Unexpected response from the LHP API",
+                {"Result": result},
+            )
         result["W_float"] = float(result["W"].split()[0])
 
         return CurrentWaterLevel.parse_obj(result)
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
```

### Comparing `lhp-0.0.3/src/lhp/util.py` & `lhp-0.0.4/src/lhp/util.py`

 * *Files identical despite different names*

### Comparing `lhp-0.0.3/PKG-INFO` & `lhp-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lhp
-Version: 0.0.3
+Version: 0.0.4
 Summary: Asynchronous client for the Länderübergreifendes Hochwasserportal (LHP) API.
 Home-page: https://github.com/embeddedfiedel/python-lhp
 License: MIT
 Keywords: lhp,lhp-api,api,async,client
 Author: Karsten Bade
 Author-email: karsten@bade.dev
 Maintainer: Karsten Bade
```


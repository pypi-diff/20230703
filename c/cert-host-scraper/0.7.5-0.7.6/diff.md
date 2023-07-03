# Comparing `tmp/cert_host_scraper-0.7.5.tar.gz` & `tmp/cert_host_scraper-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert_host_scraper-0.7.5.tar", max compression
+gzip compressed data, was "cert_host_scraper-0.7.6.tar", max compression
```

## Comparing `cert_host_scraper-0.7.5.tar` & `cert_host_scraper-0.7.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/LICENSE
--rw-r--r--   0        0        0     1187 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/README.md
--rw-r--r--   0        0        0      142 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/__init__.py
--rw-r--r--   0        0        0     3077 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/cli.py
--rw-r--r--   0        0        0     1723 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/scraper.py
--rw-r--r--   0        0        0      337 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/cert_host_scraper/utils.py
--rw-r--r--   0        0        0      697 2023-04-18 21:31:55.092769 cert_host_scraper-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 cert_host_scraper-0.7.5/setup.py
--rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 cert_host_scraper-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-03 19:30:48.873962 cert_host_scraper-0.7.6/LICENSE
+-rw-r--r--   0        0        0     1187 2023-07-03 19:30:48.873962 cert_host_scraper-0.7.6/README.md
+-rw-r--r--   0        0        0      142 2023-07-03 19:30:48.873962 cert_host_scraper-0.7.6/cert_host_scraper/__init__.py
+-rw-r--r--   0        0        0     3069 2023-07-03 19:30:48.873962 cert_host_scraper-0.7.6/cert_host_scraper/cli.py
+-rw-r--r--   0        0        0     1723 2023-07-03 19:30:48.873962 cert_host_scraper-0.7.6/cert_host_scraper/scraper.py
+-rw-r--r--   0        0        0      337 2023-07-03 19:30:48.873962 cert_host_scraper-0.7.6/cert_host_scraper/utils.py
+-rw-r--r--   0        0        0      697 2023-07-03 19:31:02.938072 cert_host_scraper-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 cert_host_scraper-0.7.6/PKG-INFO
```

### Comparing `cert_host_scraper-0.7.5/LICENSE` & `cert_host_scraper-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cert_host_scraper-0.7.5/README.md` & `cert_host_scraper-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `cert_host_scraper-0.7.5/cert_host_scraper/cli.py` & `cert_host_scraper-0.7.6/cert_host_scraper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def validate_status_code(
     _ctx: click.core.Context, _param: click.core.Option, value: str
 ):
     try:
         status_code = int(value)
         if not (100 <= status_code <= 599):
             raise click.BadParameter("status code must be between 100 and 599")
-        
+
         return status_code
     except ValueError:
         raise click.BadParameter("must be an integer")
     except TypeError:
         return NO_STATUS_CODE_FILTER
```

### Comparing `cert_host_scraper-0.7.5/cert_host_scraper/scraper.py` & `cert_host_scraper-0.7.6/cert_host_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `cert_host_scraper-0.7.5/pyproject.toml` & `cert_host_scraper-0.7.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cert-host-scraper"
-version = "0.7.5"
+version = "0.7.6"
 description = ""
 authors = ["Malachi Soord <inverse.chi@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/inverse/cert-host-scraper"
 homepage = "https://github.com/inverse/cert-host-scraper"
@@ -17,17 +17,17 @@
 python = "^3.10"
 requests = "^2.27.1"
 click = "^8.0.3"
 rich = ">=11,<14"
 single-source = "^0.3.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.1"
+pytest = "^7.4.0"
 pytest-socket = "^0.6.0"
-vcrpy = "^4.2.1"
+vcrpy = "^5.0.0"
 
 [tool.ruff]
 ignore = ["E501"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cert_host_scraper-0.7.5/PKG-INFO` & `cert_host_scraper-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cert-host-scraper
-Version: 0.7.5
+Version: 0.7.6
 Summary: 
 Home-page: https://github.com/inverse/cert-host-scraper
 License: MIT
 Author: Malachi Soord
 Author-email: inverse.chi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


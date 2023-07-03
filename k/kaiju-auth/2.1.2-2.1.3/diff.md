# Comparing `tmp/kaiju_auth-2.1.2-py3-none-any.whl.zip` & `tmp/kaiju_auth-2.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18870 bytes, number of entries: 14
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-30 16:23 kaiju_auth/__init__.py
--rw-r--r--  2.0 unx    39376 b- defN 23-Jun-30 16:23 kaiju_auth/services.py
--rw-r--r--  2.0 unx       55 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/__init__.py
--rw-r--r--  2.0 unx     3228 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/models.py
--rw-r--r--  2.0 unx    18327 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/service.py
--rw-r--r--  2.0 unx     1212 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/validators.py
--rw-r--r--  2.0 unx       42 b- defN 23-Jun-30 16:23 kaiju_auth/tests/__init__.py
--rw-r--r--  2.0 unx     1516 b- defN 23-Jun-30 16:23 kaiju_auth/tests/fixtures.py
--rw-r--r--  2.0 unx     7957 b- defN 23-Jun-30 16:23 kaiju_auth/tests/test_auth.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2987 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1189 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/RECORD
-14 files, 76695 bytes uncompressed, 16876 bytes compressed:  78.0%
+Zip file size: 18863 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-03 14:46 kaiju_auth/__init__.py
+-rw-r--r--  2.0 unx    39328 b- defN 23-Jul-03 14:46 kaiju_auth/services.py
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-03 14:46 kaiju_auth/permissions_gui/__init__.py
+-rw-r--r--  2.0 unx     3228 b- defN 23-Jul-03 14:46 kaiju_auth/permissions_gui/models.py
+-rw-r--r--  2.0 unx    18327 b- defN 23-Jul-03 14:46 kaiju_auth/permissions_gui/service.py
+-rw-r--r--  2.0 unx     1212 b- defN 23-Jul-03 14:46 kaiju_auth/permissions_gui/validators.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-03 14:46 kaiju_auth/tests/__init__.py
+-rw-r--r--  2.0 unx     1516 b- defN 23-Jul-03 14:46 kaiju_auth/tests/fixtures.py
+-rw-r--r--  2.0 unx     7957 b- defN 23-Jul-03 14:46 kaiju_auth/tests/test_auth.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-03 14:46 kaiju_auth-2.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2875 b- defN 23-Jul-03 14:46 kaiju_auth-2.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 14:46 kaiju_auth-2.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-03 14:46 kaiju_auth-2.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Jul-03 14:46 kaiju_auth-2.1.3.dist-info/RECORD
+14 files, 76535 bytes uncompressed, 16869 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: kaiju_auth/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_auth/tests/test_auth.py
 Comment: 
 
-Filename: kaiju_auth-2.1.2.dist-info/LICENSE
+Filename: kaiju_auth-2.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_auth-2.1.2.dist-info/METADATA
+Filename: kaiju_auth-2.1.3.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_auth-2.1.2.dist-info/WHEEL
+Filename: kaiju_auth-2.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_auth-2.1.2.dist-info/top_level.txt
+Filename: kaiju_auth-2.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_auth-2.1.2.dist-info/RECORD
+Filename: kaiju_auth-2.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_auth/__init__.py

```diff
@@ -1,4 +1,4 @@
 from kaiju_auth.services import *
 
-__version__ = '2.1.2'
+__version__ = '2.1.3'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_auth/services.py

```diff
@@ -14,15 +14,15 @@
 from jwcrypto import jwk, jwt  # noqa: pycharm
 
 import kaiju_tools.jsonschema as j
 from kaiju_tools.exceptions import ValidationError, Conflict, NotAuthorized
 from kaiju_tools.encoding import load, loads, dumps
 from kaiju_tools.interfaces import PublicInterface, UserInterface, Cache, TokenInterface
 from kaiju_tools.sessions import TokenClientService
-from kaiju_tools.app import ContextableService, service_class_registry, Scheduler
+from kaiju_tools.app import ContextableService, SERVICE_CLASS_REGISTRY, Scheduler
 from kaiju_db.services import DatabaseService, SQLService
 from kaiju_tools.types import Session
 
 __all__ = (
     'PermissionService',
     'GroupService',
     'UserService',
@@ -1039,15 +1039,15 @@
     @staticmethod
     def load_file(path: Path):
         if path.exists():
             with open(path) as f:
                 return load(f)
 
 
-service_class_registry.register_class(PermissionService)
-service_class_registry.register_class(GroupService)
-service_class_registry.register_class(UserService)
-service_class_registry.register_class(JWTClientService)
-service_class_registry.register_class(SessionStore)
-service_class_registry.register_class(UserFixtureService)
-service_class_registry.register_class(KeystoreService)
-service_class_registry.register_class(JWTService)
+SERVICE_CLASS_REGISTRY.register(PermissionService)
+SERVICE_CLASS_REGISTRY.register(GroupService)
+SERVICE_CLASS_REGISTRY.register(UserService)
+SERVICE_CLASS_REGISTRY.register(JWTClientService)
+SERVICE_CLASS_REGISTRY.register(SessionStore)
+SERVICE_CLASS_REGISTRY.register(UserFixtureService)
+SERVICE_CLASS_REGISTRY.register(KeystoreService)
+SERVICE_CLASS_REGISTRY.register(JWTService)
```

## Comparing `kaiju_auth-2.1.2.dist-info/LICENSE` & `kaiju_auth-2.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_auth-2.1.2.dist-info/METADATA` & `kaiju_auth-2.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-auth
-Version: 2.1.2
+Version: 2.1.3
 Summary: Authentication services.
 Home-page: https://gitlab.com/kaiju-python/kaiju-auth
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -35,17 +35,14 @@
 Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
 Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
 Requires-Dist: tox (==3.28.*) ; extra == 'dev'
 Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
 Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
-Provides-Extra: docs
-Requires-Dist: sphinx ; extra == 'docs'
-Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest (>=7.2) ; extra == 'test'
 Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
 Requires-Dist: docker (>=6.0) ; extra == 'test'
 Requires-Dist: pytest-timeout (>=2.1) ; extra == 'test'
```

## Comparing `kaiju_auth-2.1.2.dist-info/RECORD` & `kaiju_auth-2.1.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-kaiju_auth/__init__.py,sha256=VBf253I3z5cw6XpoKpU5hNZcomt-91rxPnFq1GUkmQI,93
-kaiju_auth/services.py,sha256=fZdTWqMku3t_JcjMGLhPxbtSZUHTWrJhvAAkjtwUVsY,39376
+kaiju_auth/__init__.py,sha256=UmjLXRj-Fwsr0E3RH6iurzbyE_qA5ckZgXXirDcKD4g,93
+kaiju_auth/services.py,sha256=0ttu54H0-5p7q8682Ueo8RUc40vC71CC8DoGBcwmC_k,39328
 kaiju_auth/permissions_gui/__init__.py,sha256=8Bxbwkjqk5QjDlZyXQ7R8dWLajhggp8of-yeZPz_pN0,55
 kaiju_auth/permissions_gui/models.py,sha256=JJFA7O1W-TaiJjVG1XgRKlhm92c0RRi4KJzFqKCXcWQ,3228
 kaiju_auth/permissions_gui/service.py,sha256=-zq5O6XhkF5wV7cRHHZBvpbdNZwOGyrzdkzlxWk2GOY,18327
 kaiju_auth/permissions_gui/validators.py,sha256=sytK30UHT8fg_SI5DaQRlsp1dEuyAholiOgF7fICp1I,1212
 kaiju_auth/tests/__init__.py,sha256=WlPruePOcaMi5ikqn6GheE1Z-zYcysb9M1dj6SteWGY,42
 kaiju_auth/tests/fixtures.py,sha256=VY2tGCDQuh6eVKsMw7k09utiaExEqHYOkcJ3j-9H6gg,1516
 kaiju_auth/tests/test_auth.py,sha256=h2RQCYjxJn2MCuHK0y2e4eMnmPk2QMrzslEIWaHejFI,7957
-kaiju_auth-2.1.2.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_auth-2.1.2.dist-info/METADATA,sha256=kDrkCxMuqKpPu2N8hRmlv7OxBsjQrg9pyAAN80o9YNU,2987
-kaiju_auth-2.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_auth-2.1.2.dist-info/top_level.txt,sha256=5F9g7EZLuzcI4ioeLmgI2Pp_r2yuzykkUc5L7lcUl2I,11
-kaiju_auth-2.1.2.dist-info/RECORD,,
+kaiju_auth-2.1.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_auth-2.1.3.dist-info/METADATA,sha256=jC_aioZQolFLJ70_iqEoXxLF17upgxd0iD8d2X0MZus,2875
+kaiju_auth-2.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_auth-2.1.3.dist-info/top_level.txt,sha256=5F9g7EZLuzcI4ioeLmgI2Pp_r2yuzykkUc5L7lcUl2I,11
+kaiju_auth-2.1.3.dist-info/RECORD,,
```


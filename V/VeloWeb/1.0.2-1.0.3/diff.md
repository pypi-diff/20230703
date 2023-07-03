# Comparing `tmp/VeloWeb-1.0.2.tar.gz` & `tmp/VeloWeb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VeloWeb-1.0.2.tar", last modified: Sun Jul  2 14:30:48 2023, max compression
+gzip compressed data, was "VeloWeb-1.0.3.tar", last modified: Mon Jul  3 18:02:19 2023, max compression
```

## Comparing `VeloWeb-1.0.2.tar` & `VeloWeb-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 14:30:48.602010 VeloWeb-1.0.2/
--rw-rw-rw-   0        0        0      910 2023-07-02 14:30:48.600009 VeloWeb-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-02 14:30:48.554007 VeloWeb-1.0.2/VeloWeb.egg-info/
--rw-rw-rw-   0        0        0      910 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 14:30:48.603010 VeloWeb-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-07-02 14:30:12.000000 VeloWeb-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:30:48.596008 VeloWeb-1.0.2/veloweb/
--rw-rw-rw-   0        0        0     3900 2023-07-02 13:06:35.000000 VeloWeb-1.0.2/veloweb/VeloHasher.py
--rw-rw-rw-   0        0        0     6403 2023-07-02 13:16:09.000000 VeloWeb-1.0.2/veloweb/VeloJWT.py
--rw-rw-rw-   0        0        0     2847 2023-07-01 16:49:03.000000 VeloWeb-1.0.2/veloweb/VeloMailer.py
--rw-rw-rw-   0        0        0     2594 2023-07-01 16:49:12.000000 VeloWeb-1.0.2/veloweb/VeloWTF.py
--rw-rw-rw-   0        0        0       27 2023-07-01 20:25:18.000000 VeloWeb-1.0.2/veloweb/__init__.py
--rw-rw-rw-   0        0        0      221 2023-07-02 12:55:02.000000 VeloWeb-1.0.2/veloweb/test.py
--rw-rw-rw-   0        0        0    12889 2023-07-02 14:29:43.000000 VeloWeb-1.0.2/veloweb/veloweb.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:02:19.759226 VeloWeb-1.0.3/
+-rw-rw-rw-   0        0        0      910 2023-07-03 18:02:19.756225 VeloWeb-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 18:02:19.714220 VeloWeb-1.0.3/VeloWeb.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 18:02:19.759226 VeloWeb-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-07-03 18:02:15.000000 VeloWeb-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:02:19.752225 VeloWeb-1.0.3/veloweb/
+-rw-rw-rw-   0        0        0     3648 2023-07-03 07:50:31.000000 VeloWeb-1.0.3/veloweb/VeloHasher.py
+-rw-rw-rw-   0        0        0     7776 2023-07-03 18:01:44.000000 VeloWeb-1.0.3/veloweb/VeloJWT.py
+-rw-rw-rw-   0        0        0     2847 2023-07-01 16:49:03.000000 VeloWeb-1.0.3/veloweb/VeloMailer.py
+-rw-rw-rw-   0        0        0     2594 2023-07-01 16:49:12.000000 VeloWeb-1.0.3/veloweb/VeloWTF.py
+-rw-rw-rw-   0        0        0       27 2023-07-01 20:25:18.000000 VeloWeb-1.0.3/veloweb/__init__.py
+-rw-rw-rw-   0        0        0    14356 2023-07-03 17:58:50.000000 VeloWeb-1.0.3/veloweb/veloweb.py
```

### Comparing `VeloWeb-1.0.2/PKG-INFO` & `VeloWeb-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-1.0.2/VeloWeb.egg-info/PKG-INFO` & `VeloWeb-1.0.3/VeloWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-1.0.2/setup.py` & `VeloWeb-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="VeloWeb",
-    version="1.0.2",
+    version="1.0.3",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/veloweb",
```

### Comparing `VeloWeb-1.0.2/veloweb/VeloHasher.py` & `VeloWeb-1.0.3/veloweb/VeloHasher.py`

 * *Files 16% similar despite different names*

```diff
@@ -107,16 +107,8 @@
 def RouterID5(namespace, name):
     namespace_bytes = namespace if isinstance(namespace, bytes) else namespace.encode()
     name_bytes = name.encode() if isinstance(name, str) else name
 
     hash_value = hashlib.sha1(namespace_bytes + name_bytes).digest()
     hash_value = hash_value[:16]
 
-    return bytes(hash_value)
-
-# Encrypting and decrypting data
-data = "Hello, World!"
-key = generate_key()
-encrypted_data = encrypt_data(data, key)
-print("Encrypted Data:", encrypted_data)
-decrypted_data = decrypt_data(encrypted_data, key)
-print("Decrypted Data:", decrypted_data)
+    return bytes(hash_value)
```

### Comparing `VeloWeb-1.0.2/veloweb/VeloJWT.py` & `VeloWeb-1.0.3/veloweb/VeloJWT.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import os
 import platform
 import datetime
 import jwt
 import uuid
 import json
-import pyaes
+import binascii
+from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives.asymmetric import rsa, padding
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.primitives.ciphers.aead import AESCCM
 
 class TokenExpiredError(Exception):
     pass
 
 class InvalidTokenError(Exception):
     pass
 
@@ -28,35 +34,47 @@
             return os.path.join(os.path.expanduser('~'), '.GoRouteJWT')
         elif system == 'Darwin':
             return os.path.join(os.path.expanduser('~'), 'Library', 'Application Support', 'GoRouteJWT')
         else:
             raise Exception('Unsupported platform')
 
     def generate_key_pair(self):
-        private_key = jwt.encode({'kid': 'private'}, key=self.encryption_key, algorithm=self.algorithm)
-        public_key = jwt.encode({'kid': 'public'}, key=self.encryption_key, algorithm=self.algorithm)
+        private_key = rsa.generate_private_key(
+            public_exponent=65537,
+            key_size=2048,
+            backend=default_backend()
+        )
+        public_key = private_key.public_key()
         return private_key, public_key
 
     def get_or_generate_keys(self):
         system_directory = self.get_system_directory()
-        private_key_file = os.path.join(system_directory, 'private_key.pem')
-        public_key_file = os.path.join(system_directory, 'public_key.pem')
+        private_key_file = os.path.join(system_directory, 'key', 'private_key.pem')
+        public_key_file = os.path.join(system_directory, 'key', 'public_key.pem')
+
         if os.path.exists(private_key_file) and os.path.exists(public_key_file):
             with open(private_key_file, 'rb') as f:
-                private_key = f.read()
+                private_key = serialization.load_pem_private_key(f.read(), password=None, backend=default_backend())
             with open(public_key_file, 'rb') as f:
-                public_key = f.read()
+                public_key = serialization.load_pem_public_key(f.read(), backend=default_backend())
             return private_key, public_key
         else:
             private_key, public_key = self.generate_key_pair()
-            os.makedirs(system_directory, exist_ok=True)
+            os.makedirs(os.path.join(system_directory, 'key'), exist_ok=True)
             with open(private_key_file, 'wb') as f:
-                f.write(private_key)
+                f.write(private_key.private_bytes(
+                    encoding=serialization.Encoding.PEM,
+                    format=serialization.PrivateFormat.PKCS8,
+                    encryption_algorithm=serialization.NoEncryption()
+                ))
             with open(public_key_file, 'wb') as f:
-                f.write(public_key)
+                f.write(public_key.public_bytes(
+                    encoding=serialization.Encoding.PEM,
+                    format=serialization.PublicFormat.SubjectPublicKeyInfo
+                ))
             return private_key, public_key
 
     def get_blacklist_file(self):
         system_directory = self.get_system_directory()
         blacklist_file = os.path.join(system_directory, 'token_blacklist.json')
         return blacklist_file
 
@@ -67,15 +85,15 @@
 
         if expires_delta:
             expires = datetime.datetime.utcnow() + expires_delta
         else:
             expires = datetime.datetime.utcnow() + datetime.timedelta(minutes=30)
 
         payload['exp'] = expires.timestamp()
-        access_token = jwt.encode(payload, self.private_key, algorithm=self.algorithm).decode('utf-8')
+        access_token = jwt.encode(payload, self.private_key, algorithm=self.algorithm)
         encrypted_access_token = self.encrypt_token(access_token)
         return encrypted_access_token
 
     def decode_access_token(self, encrypted_access_token):
         if not self.public_key or not self.encryption_key:
             raise Exception('Public key and encryption key are required for token decoding')
 
@@ -125,25 +143,31 @@
                     tokens_to_revoke.append(token_id)
 
         with open(self.blacklist_file, 'w') as f:
             for token_id in tokens_to_revoke:
                 del blacklist[token_id]
             json.dump(blacklist, f)
 
+
     def generate_token_id(self):
         return str(uuid.uuid4())
 
     def encrypt_token(self, token):
-        aes = pyaes.AESModeOfOperationCTR(self.encryption_key.encode('utf-8'))
-        encrypted_token = aes.encrypt(token.encode('utf-8'))
-        return encrypted_token.hex()
+        encryption_key = self.encryption_key.ljust(32)[:32].encode('utf-8')  # Pad or truncate to 32 bytes
+        nonce = os.urandom(16)  # Generate a random nonce
+        cipher = Cipher(algorithms.AES(encryption_key), modes.CTR(nonce))
+        encryptor = cipher.encryptor()
+        encrypted_token = encryptor.update(token.encode('utf-8')) + encryptor.finalize()
+        return binascii.hexlify(nonce + encrypted_token).decode('utf-8')
 
     def decrypt_token(self, encrypted_token):
-        aes = pyaes.AESModeOfOperationCTR(self.encryption_key.encode('utf-8'))
-        decrypted_token = aes.decrypt(bytes.fromhex(encrypted_token))
+        encryption_key = self.encryption_key.ljust(32)[:32].encode('utf-8')  # Pad or truncate to 32 bytes
+        cipher = Cipher(algorithms.AES(encryption_key), modes.CTR())
+        decryptor = cipher.decryptor()
+        decrypted_token = decryptor.update(bytes.fromhex(encrypted_token)) + decryptor.finalize()
         return decrypted_token.decode('utf-8')
 
     def blacklist_token(self, token_id):
         with open(self.blacklist_file, 'r') as f:
             blacklist = json.load(f)
         blacklist[token_id] = datetime.datetime.utcnow().isoformat()
         with open(self.blacklist_file, 'w') as f:
```

### Comparing `VeloWeb-1.0.2/veloweb/VeloMailer.py` & `VeloWeb-1.0.3/veloweb/VeloMailer.py`

 * *Files identical despite different names*

### Comparing `VeloWeb-1.0.2/veloweb/VeloWTF.py` & `VeloWeb-1.0.3/veloweb/VeloWTF.py`

 * *Files identical despite different names*

### Comparing `VeloWeb-1.0.2/veloweb/veloweb.py` & `VeloWeb-1.0.3/veloweb/veloweb.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 from jinja2 import Environment, FileSystemLoader
 from itsdangerous import URLSafeTimedSerializer, BadSignature
 from werkzeug.exceptions import HTTPException, MethodNotAllowed, NotFound
 from werkzeug.routing import Map, Rule
 from werkzeug.wrappers import Request, Response
+from werkzeug.urls import url_encode
 from werkzeug.serving import run_simple
 import asyncio
 import importlib
 
 class velo:
     def __init__(self):
         self.url_map = Map()
@@ -42,20 +43,49 @@
 
     def add_route(self, path, methods, func):
         options = {"methods": methods}
         rule = Rule(path, endpoint=func, **options)
         self.url_map.add(rule)
         self.routes[func] = path
 
+    def add_api_route(self, path, methods=['GET'], secure=False):
+        """
+        A decorator for adding API routes.
+        """
+        def decorator(func):
+            self.add_route(path, methods, func)
+            func.secure = secure
+            func.is_api_route = True  # Mark the function as an API route handler
+            return func
+        return decorator
+
     def route(self, path, methods=['GET'], secure=False):
         def decorator(func):
             self.add_route(path, methods, func)
             func.secure = secure
             return func
+
         return decorator
+    
+    async def parse_json_data(self, request):
+        """
+        Helper method to parse JSON data from the request body.
+        """
+        try:
+            data = await request.get_json()
+            return data
+        except Exception as e:
+            return None
+        
+    def redirect_args(self, location, **kwargs):
+        url = location
+        if kwargs:
+            query_params = url_encode(kwargs)
+            url += f'?{query_params}'
+        return Response(status=302, headers={'Location': url})
 
     def jsonify(self, data):
         return Response(json.dumps(data), mimetype='application/json')
 
     def make_response(self, response):
         if isinstance(response, Response):
             return response
@@ -173,17 +203,25 @@
     def url_for(self, endpoint):
         return self.routes.get(endpoint)
 
     async def process_request(self, request):
         try:
             endpoint, values = self.url_map.bind_to_environ(request.environ).match()
             handler = endpoint
+
             for middleware in self.middlewares:
                 request, values = await middleware.before_request(request, values)
-            response = await handler(request, **values)
+
+            if hasattr(handler, 'is_api_route') and request.content_type == 'application/json':
+                # For API routes, parse JSON data from the request body
+                data = await self.parse_json_data(request)
+                response = await handler(request, data, **values)
+            else:
+                response = await handler(request, **values)
+
             for middleware in reversed(self.middlewares):
                 response = await middleware.after_request(request, response)
             return response
         except MethodNotAllowed as e:
             return self.handle_method_not_allowed(e.valid_methods)
         except NotFound:
             return self.handle_not_found()
@@ -275,20 +313,29 @@
 
         loop = asyncio.new_event_loop()
         response = loop.run_until_complete(process_request_async())
         loop.close()
         return response
 
     def runserver(self, host=None, port=None, debug=None):
-        settings = importlib.import_module('settings', None)
-        host = host or (getattr(settings, 'HOST', '127.0.0.1') if settings else '127.0.0.1')
-        port = port or (getattr(settings, 'PORT', 8000) if settings else 8000)
-        debug = debug or (getattr(settings, 'DEBUG', True) if settings else True)
+        try:
+            settings = importlib.import_module('settings')
+        except ModuleNotFoundError:
+            # If settings.py is not available, use default values
+            host = host or '127.0.0.1'
+            port = port or 8000
+            debug = debug or True
+        else:
+            host = host or getattr(settings, 'HOST', '127.0.0.1')
+            port = port or getattr(settings, 'PORT', 8000)
+            debug = debug or getattr(settings, 'DEBUG', True)
+
         run_simple(host, port, self.wsgi_app, use_reloader=debug, threaded=True)
 
+
     def use(self, middleware):
         self.middlewares.append(middleware)
 
     def session_middleware(self):
         class SessionMiddleware:
             def __init__(self, app):
                 self.app = app
```


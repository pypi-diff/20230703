# Comparing `tmp/Cryptem-0.1.0.tar.gz` & `tmp/Cryptem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cryptem-0.1.0.tar", last modified: Sun May 21 10:19:54 2023, max compression
+gzip compressed data, was "Cryptem-0.1.1.tar", last modified: Mon Jul  3 11:11:55 2023, max compression
```

## Comparing `Cryptem-0.1.0.tar` & `Cryptem-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-21 10:19:54.334720 Cryptem-0.1.0/
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-21 10:19:54.334720 Cryptem-0.1.0/Cryptem.egg-info/
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6578 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/PKG-INFO
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      199 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/SOURCES.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        1 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/dependency_links.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       31 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/requires.txt
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       16 2023-05-21 10:19:54.000000 Cryptem-0.1.0/Cryptem.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     4437 2023-05-21 10:00:39.000000 Cryptem-0.1.0/Cryptem.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6578 2023-05-21 10:19:54.334720 Cryptem-0.1.0/PKG-INFO
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7447 2023-05-21 09:21:02.000000 Cryptem-0.1.0/cryptem.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 Cryptem-0.1.0/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-05-21 10:19:54.334720 Cryptem-0.1.0/setup.cfg
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1182 2023-05-21 10:10:07.000000 Cryptem-0.1.0/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-07-03 11:11:55.082133 Cryptem-0.1.1/
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-07-03 11:11:55.082133 Cryptem-0.1.1/Cryptem.egg-info/
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6641 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/PKG-INFO
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      199 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/SOURCES.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        1 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/dependency_links.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       31 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/requires.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       16 2023-07-03 11:11:54.000000 Cryptem-0.1.1/Cryptem.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     4437 2023-05-21 10:00:39.000000 Cryptem-0.1.1/Cryptem.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6641 2023-07-03 11:11:55.082133 Cryptem-0.1.1/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7940 2023-07-03 11:09:54.000000 Cryptem-0.1.1/cryptem.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 Cryptem-0.1.1/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-07-03 11:11:55.082133 Cryptem-0.1.1/setup.cfg
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1245 2023-05-21 10:24:10.000000 Cryptem-0.1.1/setup.py
```

### Comparing `Cryptem-0.1.0/Cryptem.egg-info/PKG-INFO` & `Cryptem-0.1.1/Cryptem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
 License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
+Project-URL: Github, https://github.com/emendir/Cryptem-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.
```

### Comparing `Cryptem-0.1.0/Cryptem.py` & `Cryptem-0.1.1/Cryptem.py`

 * *Files identical despite different names*

### Comparing `Cryptem-0.1.0/PKG-INFO` & `Cryptem-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
 License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
+Project-URL: Github, https://github.com/emendir/Cryptem-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.
```

### Comparing `Cryptem-0.1.0/cryptem.py` & `Cryptem-0.1.1/cryptem.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,24 +65,28 @@
             codec2 = Crypt("my_password")
             plaintext = codec2.decrypt(cipher).decode('utf-8')
     """
 
     public_key = ""  # string
     __private_key = ""  # coincurve.keys.coincurve.PrivateKey
 
-    def __init__(self, password=None):
-        if password == None:
+    def __init__(self, password=None, private_key=None):
+        if not password and not private_key:
             key = generate_key()    # generate new random key
-        else:
+        elif password:
             # creating a cryptographic hash from the password, to create a larger encryption key from it
             hashGen = hashlib.sha256()
             hashGen.update(password.encode())
             hash = hashGen.hexdigest()
 
             key = coincurve.PrivateKey.from_hex(hash)
+        elif private_key:
+            key = coincurve.PrivateKey.from_hex(private_key)
+        else:
+            raise Exception("Specify a password or a private_key, not both.")
 
         self.__private_key = key
         self.public_key = key.public_key.format(False).hex()
 
     def encrypt(self, data_to_encrypt: bytearray):
         return encrypt(data_to_encrypt, self.public_key)
 
@@ -123,14 +127,22 @@
 
     def sign(self, data: bytes):
         return self.__private_key.sign(data)
 
     def verify_signature(self, data: bytes, signature: bytes):
         return verify_signature(data, self.public_key, signature)
 
+    def get_private_key(self):
+        """Returns the private key in hexadecimal format."""
+        return self.__private_key.to_hex()
+
+    def get_public_key(self):
+        """Returns the private key in hexadecimal format."""
+        return self.__private_key.to_hex()
+
 
 class Encryptor:
     def __init__(self, public_key):
         self.public_key = public_key
 
     def encrypt(self, data):
         return encrypt(data, self.public_key)
```

### Comparing `Cryptem-0.1.0/setup.py` & `Cryptem-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     description="Cryptographic applications library based on elliptic curve cryptography",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83",
 
     project_urls={
         "Source Code on IPFS": "https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83",
+        "Github": 'https://github.com/emendir/Cryptem-Python',
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     # 'package_dir={"": "."},
     packages=setuptools.find_packages(),
```


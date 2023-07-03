# Comparing `tmp/ts_auth0-0.0.11.tar.gz` & `tmp/ts_auth0-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_auth0-0.0.11.tar", last modified: Wed Jun 28 16:02:40 2023, max compression
+gzip compressed data, was "ts_auth0-0.0.14.tar", last modified: Mon Jul  3 21:22:37 2023, max compression
```

## Comparing `ts_auth0-0.0.11.tar` & `ts_auth0-0.0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-06-28 16:02:40.437027 ts_auth0-0.0.11/
--rw-r--r--   0 jon        (501) staff       (20)     1068 2023-06-22 15:47:27.000000 ts_auth0-0.0.11/LICENSE
--rw-r--r--   0 jon        (501) staff       (20)     5830 2023-06-28 16:02:40.436767 ts_auth0-0.0.11/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)     5314 2023-06-28 16:01:57.000000 ts_auth0-0.0.11/README.md
--rw-r--r--   0 jon        (501) staff       (20)      623 2023-06-28 15:59:48.000000 ts_auth0-0.0.11/pyproject.toml
--rw-r--r--   0 jon        (501) staff       (20)       38 2023-06-28 16:02:40.437110 ts_auth0-0.0.11/setup.cfg
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-06-28 16:02:40.434177 ts_auth0-0.0.11/src/
--rw-r--r--   0 jon        (501) staff       (20)        0 2023-06-28 15:31:14.000000 ts_auth0-0.0.11/src/__init__.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-06-28 16:02:40.436367 ts_auth0-0.0.11/src/ts_auth0.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)     5830 2023-06-28 16:02:40.000000 ts_auth0-0.0.11/src/ts_auth0.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      243 2023-06-28 16:02:40.000000 ts_auth0-0.0.11/src/ts_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2023-06-28 16:02:40.000000 ts_auth0-0.0.11/src/ts_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)        9 2023-06-28 16:02:40.000000 ts_auth0-0.0.11/src/ts_auth0.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       18 2023-06-28 16:02:40.000000 ts_auth0-0.0.11/src/ts_auth0.egg-info/top_level.txt
--rw-r--r--   0 jon        (501) staff       (20)    12552 2023-06-28 16:00:30.000000 ts_auth0-0.0.11/src/ts_auth0.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-03 21:22:37.511223 ts_auth0-0.0.14/
+-rw-r--r--   0 jon        (501) staff       (20)     1068 2023-06-22 15:47:27.000000 ts_auth0-0.0.14/LICENSE
+-rw-r--r--   0 jon        (501) staff       (20)     6877 2023-07-03 21:22:37.510615 ts_auth0-0.0.14/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)     6361 2023-07-03 21:20:57.000000 ts_auth0-0.0.14/README.md
+-rw-r--r--   0 jon        (501) staff       (20)      623 2023-07-03 21:12:07.000000 ts_auth0-0.0.14/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)       38 2023-07-03 21:22:37.511448 ts_auth0-0.0.14/setup.cfg
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-03 21:22:37.505556 ts_auth0-0.0.14/src/
+-rw-r--r--   0 jon        (501) staff       (20)        0 2023-06-28 15:31:14.000000 ts_auth0-0.0.14/src/__init__.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-03 21:22:37.509734 ts_auth0-0.0.14/src/ts_auth0.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)     6877 2023-07-03 21:22:37.000000 ts_auth0-0.0.14/src/ts_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      243 2023-07-03 21:22:37.000000 ts_auth0-0.0.14/src/ts_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2023-07-03 21:22:37.000000 ts_auth0-0.0.14/src/ts_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)        9 2023-07-03 21:22:37.000000 ts_auth0-0.0.14/src/ts_auth0.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)       18 2023-07-03 21:22:37.000000 ts_auth0-0.0.14/src/ts_auth0.egg-info/top_level.txt
+-rw-r--r--   0 jon        (501) staff       (20)    14318 2023-07-03 21:12:22.000000 ts_auth0-0.0.14/src/ts_auth0.py
```

### Comparing `ts_auth0-0.0.11/LICENSE` & `ts_auth0-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_auth0-0.0.11/PKG-INFO` & `ts_auth0-0.0.14/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ts_auth0
-Version: 0.0.11
-Summary: Simple Python Auth0 login for Tradestation API v3
-Author-email: Jon Richards <jrseti@gmail.com>
-Project-URL: Homepage, https://github.com/jrseti/ts_auth0
-Project-URL: Bug Tracker, https://github.com/jrseti/ts_auth0/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ts_auth0
 Simple Python Auth0 login for Tradestation API v3
 
 This package is purely for experimental purposes and is not supported by Tradestation https://www.tradestation.com/. Use at your own risk - trading is risky!
 
 I found the Tradestation authentication process to be complicated, so once I figured out the correct procedure and was able to authenicate and get an access token, I wrapped it all into this easy to use Python class for all to enjoy!
 
@@ -28,15 +14,15 @@
 
 To start, you provide your API Key and Secret API Key. A simple function call is all that is required to log in and obtain an access token. The access token is then used for all API calls to get market updates, account information, etc.
 
 Please note that this package only addresses authentication. Making API calls for market data and trading is a seperate task and not addresses in this package. But, see the example code below for an example of making an API once you pass authentication and are able to obtain the access token needed for all Tradestation API calls.
  
 - Works with Python >= 3.8
 - Tested on MacOS
-- Not tested yet on Windows 
+- Tested on Windows 11 
 
 To start, you will need to request API access from Tradestation. See  https://api.tradestation.com/docs/faq#how-do-i-get-an-api-key. Baically you need to do the following:
 
 - Deposit at least $10,000 into Tradestation (!). It may take over a week to get confirmation that the money was deposited and available. Without this deposit your requests for API access will be declined.
 - After requesting API access you will receive via email a PDF file that requres a password to view. This file contains your API Key and Secret API Key.
 
 ## Getting Started
@@ -128,13 +114,20 @@
   - Default: http://localhost
 - SCOPE (str): The scope for the auth server
   - Default: "openid profile MarketData ReadAccount Trade Matrix OptionSpreads offline_access"
 - TOKEN_REQUEST_URL (str): The URL for the token request
   - Default: https://signin.tradestation.com/oauth/token
 - SHOW_KEYS_IN_STR (bool): Show the API keys in the string representation of the class
   - Default: False
+- REFRESH_TOKEN_CACHE_FILE (str): The file to cache the refresh token.
+  - Default: refresh_token_cache.txt
+
+# Headless
+
+I tried implementing headless login, where the user name and password would be used automatically to log in without requiring interaction with a browser. I ran into difficulty with the two-factor authentication, you still need to enter the code received in email or on your phone. So for now I have not implemented headless mode. Maybe I will in the future if I move my trading projects over to a server in the cloud. I could automate everything except the two-factor authenication. TBD.
+
+# Refresh Token
 
+The refresh token is assigned as a result of the authentication process. This token string is stored in a text file. The next time start_auth0() is called, the authentication is skipped and the previous refresh token is used to obtain an access token needed for your first API call. Via the Tradestation Forum one of the engineers said that the refresh token remains valid indefinately. So in theory this code should only need to perform the login and two-factor authentication once, and the refresh token will be re-used on subsequent re-starts of the code.
 
-# TODO
 
-Next, I need to make the Tradestation login to be headless so you do not have to manually log in via the browser. Stay tuned.
```

### Comparing `ts_auth0-0.0.11/README.md` & `ts_auth0-0.0.14/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: ts_auth0
+Version: 0.0.14
+Summary: Simple Python Auth0 login for Tradestation API v3
+Author-email: Jon Richards <jrseti@gmail.com>
+Project-URL: Homepage, https://github.com/jrseti/ts_auth0
+Project-URL: Bug Tracker, https://github.com/jrseti/ts_auth0/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ts_auth0
 Simple Python Auth0 login for Tradestation API v3
 
 This package is purely for experimental purposes and is not supported by Tradestation https://www.tradestation.com/. Use at your own risk - trading is risky!
 
 I found the Tradestation authentication process to be complicated, so once I figured out the correct procedure and was able to authenicate and get an access token, I wrapped it all into this easy to use Python class for all to enjoy!
 
@@ -14,15 +28,15 @@
 
 To start, you provide your API Key and Secret API Key. A simple function call is all that is required to log in and obtain an access token. The access token is then used for all API calls to get market updates, account information, etc.
 
 Please note that this package only addresses authentication. Making API calls for market data and trading is a seperate task and not addresses in this package. But, see the example code below for an example of making an API once you pass authentication and are able to obtain the access token needed for all Tradestation API calls.
  
 - Works with Python >= 3.8
 - Tested on MacOS
-- Not tested yet on Windows 
+- Tested on Windows 11 
 
 To start, you will need to request API access from Tradestation. See  https://api.tradestation.com/docs/faq#how-do-i-get-an-api-key. Baically you need to do the following:
 
 - Deposit at least $10,000 into Tradestation (!). It may take over a week to get confirmation that the money was deposited and available. Without this deposit your requests for API access will be declined.
 - After requesting API access you will receive via email a PDF file that requres a password to view. This file contains your API Key and Secret API Key.
 
 ## Getting Started
@@ -114,13 +128,20 @@
   - Default: http://localhost
 - SCOPE (str): The scope for the auth server
   - Default: "openid profile MarketData ReadAccount Trade Matrix OptionSpreads offline_access"
 - TOKEN_REQUEST_URL (str): The URL for the token request
   - Default: https://signin.tradestation.com/oauth/token
 - SHOW_KEYS_IN_STR (bool): Show the API keys in the string representation of the class
   - Default: False
+- REFRESH_TOKEN_CACHE_FILE (str): The file to cache the refresh token.
+  - Default: refresh_token_cache.txt
+
+# Headless
+
+I tried implementing headless login, where the user name and password would be used automatically to log in without requiring interaction with a browser. I ran into difficulty with the two-factor authentication, you still need to enter the code received in email or on your phone. So for now I have not implemented headless mode. Maybe I will in the future if I move my trading projects over to a server in the cloud. I could automate everything except the two-factor authenication. TBD.
+
+# Refresh Token
 
+The refresh token is assigned as a result of the authentication process. This token string is stored in a text file. The next time start_auth0() is called, the authentication is skipped and the previous refresh token is used to obtain an access token needed for your first API call. Via the Tradestation Forum one of the engineers said that the refresh token remains valid indefinately. So in theory this code should only need to perform the login and two-factor authentication once, and the refresh token will be re-used on subsequent re-starts of the code.
 
-# TODO
 
-Next, I need to make the Tradestation login to be headless so you do not have to manually log in via the browser. Stay tuned.
```

### Comparing `ts_auth0-0.0.11/pyproject.toml` & `ts_auth0-0.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ts_auth0"
-version = "0.0.11"
+version = "0.0.14"
 authors = [
   { name="Jon Richards", email="jrseti@gmail.com" },
 ]
 description = "Simple Python Auth0 login for Tradestation API v3"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ts_auth0-0.0.11/src/ts_auth0.egg-info/PKG-INFO` & `ts_auth0-0.0.14/src/ts_auth0.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-auth0
-Version: 0.0.11
+Version: 0.0.14
 Summary: Simple Python Auth0 login for Tradestation API v3
 Author-email: Jon Richards <jrseti@gmail.com>
 Project-URL: Homepage, https://github.com/jrseti/ts_auth0
 Project-URL: Bug Tracker, https://github.com/jrseti/ts_auth0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 
 To start, you provide your API Key and Secret API Key. A simple function call is all that is required to log in and obtain an access token. The access token is then used for all API calls to get market updates, account information, etc.
 
 Please note that this package only addresses authentication. Making API calls for market data and trading is a seperate task and not addresses in this package. But, see the example code below for an example of making an API once you pass authentication and are able to obtain the access token needed for all Tradestation API calls.
  
 - Works with Python >= 3.8
 - Tested on MacOS
-- Not tested yet on Windows 
+- Tested on Windows 11 
 
 To start, you will need to request API access from Tradestation. See  https://api.tradestation.com/docs/faq#how-do-i-get-an-api-key. Baically you need to do the following:
 
 - Deposit at least $10,000 into Tradestation (!). It may take over a week to get confirmation that the money was deposited and available. Without this deposit your requests for API access will be declined.
 - After requesting API access you will receive via email a PDF file that requres a password to view. This file contains your API Key and Secret API Key.
 
 ## Getting Started
@@ -128,13 +128,20 @@
   - Default: http://localhost
 - SCOPE (str): The scope for the auth server
   - Default: "openid profile MarketData ReadAccount Trade Matrix OptionSpreads offline_access"
 - TOKEN_REQUEST_URL (str): The URL for the token request
   - Default: https://signin.tradestation.com/oauth/token
 - SHOW_KEYS_IN_STR (bool): Show the API keys in the string representation of the class
   - Default: False
+- REFRESH_TOKEN_CACHE_FILE (str): The file to cache the refresh token.
+  - Default: refresh_token_cache.txt
 
+# Headless
+
+I tried implementing headless login, where the user name and password would be used automatically to log in without requiring interaction with a browser. I ran into difficulty with the two-factor authentication, you still need to enter the code received in email or on your phone. So for now I have not implemented headless mode. Maybe I will in the future if I move my trading projects over to a server in the cloud. I could automate everything except the two-factor authenication. TBD.
+
+# Refresh Token
+
+The refresh token is assigned as a result of the authentication process. This token string is stored in a text file. The next time start_auth0() is called, the authentication is skipped and the previous refresh token is used to obtain an access token needed for your first API call. Via the Tradestation Forum one of the engineers said that the refresh token remains valid indefinately. So in theory this code should only need to perform the login and two-factor authentication once, and the refresh token will be re-used on subsequent re-starts of the code.
 
-# TODO
 
-Next, I need to make the Tradestation login to be headless so you do not have to manually log in via the browser. Stay tuned.
```

### Comparing `ts_auth0-0.0.11/src/ts_auth0.py` & `ts_auth0-0.0.14/src/ts_auth0.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # -*- coding: utf-8 -*-
 """
 Script: ts_auth0
 Description: This script handles the authentication process for the Tradestation API
 Author: Jon Richards, jrseti@gmail.com
 Copyrite: 2023, Jon Richards
 Licence: MIT
-Version: 0.0.11
 """
-
-import json
 import requests
 import webbrowser
 from http.server import HTTPServer, BaseHTTPRequestHandler
 import urllib.parse
 import string
 import random
 import time
 import copy
+import os
 
 __author__ = "Jon Richards"
 __copyright__ = "Copyright 2023, Jon Richards"
 __credits__ = ["Jon Richards"]
 __license__ = "MIT"
-__version__ = "0.0.11"
+__version__ = "0.0.14"
 __maintainer__ = "Jon Richards"
 __email__ = "jrseti@gmail.com"
 __status__ = "Dev"
 
 class TS_Auth: 
 
     """This class handles the authentication process for the Tradestation API"""
@@ -34,15 +32,16 @@
     _DEFAULT_PARAMETERS = {
         "BASE_URL" : "https://signin.tradestation.com/authorize",
         "AUDIENCE" : "https://api.tradestation.com",
         "REDIRECT_PORT" : 3000,
         "REDIRECT_URI" : "http://localhost",
         "SCOPE" : "openid profile MarketData ReadAccount Trade Matrix OptionSpreads offline_access",
         "TOKEN_REQUEST_URL" : "https://signin.tradestation.com/oauth/token",
-        "SHOW_KEYS_IN_STR" : False
+        "SHOW_KEYS_IN_STR" : False,
+        "REFRESH_TOKEN_CACHE_FILE" : "refresh_token_cache.txt"
     }
 
     def __init__(self, 
                  api_key, api_secret_key, 
                  **parameters):  
         """Initialize the TS_Auth class
         Args:
@@ -59,14 +58,16 @@
                     Default: http://localhost
                 SCOPE (str): The scope for the auth server
                     Default: "openid profile MarketData ReadAccount Trade Matrix OptionSpreads offline_access"
                 TOKEN_REQUEST_URL (str): The URL for the token request
                     Default: https://signin.tradestation.com/oauth/token
                 SHOW_KEYS_IN_STR (bool): Show the API keys in the string representation of the class
                     Default: False
+                REFRESH_TOKEN_CACHE_FILE (str): The file to cache the refresh token
+                    Default: refresh_token_cache.txt
 
         Raises:
             Auth_Error: Invalid parameter
         """
 
         # Make sure all the parameters are valid.
         for key in parameters:
@@ -87,17 +88,18 @@
         if "REDIRECT_URI" not in parameters:
             self._parameters["REDIRECT_URI"] = TS_Auth._DEFAULT_PARAMETERS["REDIRECT_URI"]
         if "SCOPE" not in parameters:
             self._parameters["SCOPE"] = TS_Auth._DEFAULT_PARAMETERS["SCOPE"]
         if "TOKEN_REQUEST_URL" not in parameters:
             self._parameters["TOKEN_REQUEST_URL"] = TS_Auth._DEFAULT_PARAMETERS["TOKEN_REQUEST_URL"]
         if "SHOW_KEYS_IN_STR" not in parameters:
-            self._parameters["SHOW_KEYS_IN_STR"] = TS_Auth._DEFAULT_PARAMETERS["SHOW_KEYS_IN_STR"]  
-
-        
+            self._parameters["SHOW_KEYS_IN_STR"] = TS_Auth._DEFAULT_PARAMETERS["SHOW_KEYS_IN_STR"] 
+        if "REFRESH_TOKEN_CACHE_FILE" not in parameters:
+            self._parameters["REFRESH_TOKEN_CACHE_FILE"] = TS_Auth._DEFAULT_PARAMETERS["REFRESH_TOKEN_CACHE_FILE"]
+     
         # Initialize the class variables.
         self._code = None
         self._access_end_of_life = 0
         self._access_token = None
         self._refresh_token = None
         self._keep_running = False;
 
@@ -162,14 +164,18 @@
         """Start the auth0 process
         Args:
             timeout_secs (int): The number of seconds to wait for the auth server to respond. Default: 10
         Raises:
             Auth_Error: The auth server did not respond within the specified timeout period.
         """
 
+        if self._attempt_getting_access_token() is True:
+            print("Access token already exists and is valid, skipping login")
+            return;
+
         self._returned_code = None
         self._keep_running = True;
 
         server_address = ('localhost', self._parameters["REDIRECT_PORT"])
    
         # Create an HTTP server and a handler class
         # Tell the request handler class who its parent is so the received code can be
@@ -190,15 +196,15 @@
             'audience': self._parameters["AUDIENCE"],
             'redirect_uri': self._constructRedirectURI(),
             'scope': self._parameters["SCOPE"],
             'state': self.state_string
         }
         url = f'{self._parameters["BASE_URL"]}?{urllib.parse.urlencode(url_params)}'
         
-        # Open the browser and request the url
+        # Open the browser and request the url, requiring the user to manually login
         webbrowser.open(url)
         
         # Wait for the auth server to report the code. _RequestHandler do_Get() will set self._code
         count_for_timeout = timeout_secs
         while self._keep_running:
             if(count_for_timeout == 0):
                 raise self.Auth_Error(f'{timeout_secs} second Timeout waiting for auth response using request: {url}')
@@ -259,14 +265,37 @@
             self._access_end_of_life = int(response_data['expires_in']) + int(time.time()) - 30
             self._access_token = response_data['access_token']
         except:
             raise self.Auth_Error("Error getting access token, try again")
 
         return response_data['access_token']
     
+    def _attempt_getting_access_token(self):
+        """Attempt to get an access token using the previous refresh token
+        Args:
+            previous_refresh_token (str): The previous refresh token
+        Returns:
+            str: The access token, None if there was an error
+        """
+        token_cache_file = self._parameters["REFRESH_TOKEN_CACHE_FILE"]
+        if os.path.exists(token_cache_file) == False:
+            return False;
+    
+        with open(token_cache_file, 'r') as f:
+            previous_refresh_token = f.read()
+            self._refresh_token = previous_refresh_token
+            print(f"Attempting to get access token using previous refresh token {self._refresh_token}")
+            try:
+                self.get_access_token()
+                print("Got access token using previous refresh token")
+                return True
+            except:
+                print("Error getting access token using previous refresh token")
+                return False
+    
     def _constructRedirectURI(self):
         """Construct the actual redirect URI from the server name and port.
         If the server port is None, then the port is not included in the URI
         Returns:
             str: The redirect URI
         """ 
         return f'{self._parameters["REDIRECT_URI"]}:{self._parameters["REDIRECT_PORT"]}'      
@@ -292,11 +321,15 @@
         'Content-Type': 'application/x-www-form-urlencoded'
         }
 
         try:
             response = requests.request("POST", url, headers=headers, data=payload)
             response_data = response.json()
             self._refresh_token = response_data['refresh_token']
+            # Save the refresh token to a file
+            token_cache_file = self._parameters["REFRESH_TOKEN_CACHE_FILE"]
+            with open(token_cache_file, 'w') as f:
+                f.write(self._refresh_token)
             return
         except:
             raise self.Auth_Error("Error getting refresh token, try again")
-
+
```


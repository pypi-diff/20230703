# Comparing `tmp/self-discover-1.0.tar.gz` & `tmp/self-discover-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "self-discover-1.0.tar", last modified: Sun Jul  2 21:00:29 2023, max compression
+gzip compressed data, was "self-discover-1.0.1.tar", last modified: Sun Jul  2 23:10:37 2023, max compression
```

## Comparing `self-discover-1.0.tar` & `self-discover-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:00:29.149120 self-discover-1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 19:11:24.000000 self-discover-1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1230 2023-07-02 21:00:29.149120 self-discover-1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-07-02 19:29:21.000000 self-discover-1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 19:11:24.000000 self-discover-1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:00:29.145120 self-discover-1.0/self_discover/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 19:11:24.000000 self-discover-1.0/self_discover/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-07-02 20:51:58.000000 self-discover-1.0/self_discover/main.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-02 19:11:24.000000 self-discover-1.0/self_discover/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4453 2023-07-02 19:27:51.000000 self-discover-1.0/self_discover/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:00:29.149120 self-discover-1.0/self_discover.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1230 2023-07-02 21:00:29.000000 self-discover-1.0/self_discover.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-02 21:00:29.000000 self-discover-1.0/self_discover.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 21:00:29.000000 self-discover-1.0/self_discover.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-02 21:00:29.000000 self-discover-1.0/self_discover.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 21:00:29.000000 self-discover-1.0/self_discover.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-02 21:00:29.149120 self-discover-1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1214 2023-07-02 19:15:14.000000 self-discover-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:10:37.550544 self-discover-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 19:11:24.000000 self-discover-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-07-02 23:10:37.554544 self-discover-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-07-02 19:29:21.000000 self-discover-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 19:11:24.000000 self-discover-1.0.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:10:37.550544 self-discover-1.0.1/self_discover/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 19:11:24.000000 self-discover-1.0.1/self_discover/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2023-07-02 23:04:36.000000 self-discover-1.0.1/self_discover/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-02 19:11:24.000000 self-discover-1.0.1/self_discover/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4455 2023-07-02 23:04:36.000000 self-discover-1.0.1/self_discover/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:10:37.550544 self-discover-1.0.1/self_discover.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-02 23:10:37.554544 self-discover-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1216 2023-07-02 23:09:00.000000 self-discover-1.0.1/setup.py
```

### Comparing `self-discover-1.0/LICENSE` & `self-discover-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `self-discover-1.0/PKG-INFO` & `self-discover-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-discover
-Version: 1.0
+Version: 1.0.1
 Summary: Self Discover serves autodiscover (Outlook) and autoconfig (Thunderbird) XML files for mail auto-configuration.
 Home-page: https://github.com/CyberfusionIO/Self-Discover
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,fastapi,mail,email,outlook,thunderbird,autodiscover,autoconfig
 Platform: linux
```

### Comparing `self-discover-1.0/README.md` & `self-discover-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `self-discover-1.0/self_discover/main.py` & `self-discover-1.0.1/self_discover/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,23 +24,35 @@
             content=f"URL must start with '{PREFIX_AUTODISCOVER}'",
             status_code=status.HTTP_400_BAD_REQUEST,
         )
 
     body = await request.body()
 
     try:
-        email_address = SafeET.fromstring(body).find(
-            ".//{https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006}EMailAddress"
-        )
+        parsed_body = SafeET.fromstring(body)
     except SafeET.ParseError:
         return Response(
             content="Payload must be valid XML",
             status_code=status.HTTP_400_BAD_REQUEST,
         )
 
+    # 'xmlns' includes http or https. Example with https on #1, with http on #2.
+    #
+    # 1: https://learn.microsoft.com/en-us/exchange/client-developer/web-service-reference/pox-autodiscover-request-for-exchange
+    # 2: https://learn.microsoft.com/en-us/openspecs/exchange_server_protocols/ms-oxdscli/fc420a31-5180-4a28-8397-8db8977861c6
+
+    email_address = parsed_body.find(
+        ".//{http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006}EMailAddress"
+    )
+
+    if email_address is None:
+        email_address = parsed_body.find(
+            ".//{https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006}EMailAddress"
+        )
+
     if email_address is None:
         return Response(
             content="Email address must be present in XML payload",
             status_code=status.HTTP_400_BAD_REQUEST,
         )
 
     data = get_pox_autodiscover_response(
```

### Comparing `self-discover-1.0/self_discover/utilities.py` & `self-discover-1.0.1/self_discover/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 ) -> str:
     """Get POX ('plain old XML') autodiscover response.
 
     See: https://learn.microsoft.com/en-us/exchange/client-developer/web-service-reference/pox-autodiscover-response-for-exchange
     """
     root = ET.Element(
         "Autodiscover",
-        xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006",
+        xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006",
     )
 
     Response = ET.SubElement(
         root,
         "Response",
-        xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a",
+        xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a",
     )
 
     Account = ET.SubElement(Response, "Account")
     ET.SubElement(Account, "AccountType").text = "email"
     ET.SubElement(Account, "Action").text = "settings"
 
     Protocol = ET.SubElement(Account, "Protocol")
@@ -100,20 +100,20 @@
     )
     ET.SubElement(incomingServer, "hostname").text = imap_server_hostname
     ET.SubElement(incomingServer, "port").text = "993"
     ET.SubElement(incomingServer, "socketType").text = "SSL"
     ET.SubElement(incomingServer, "username").text = "%EMAILADDRESS%"
     ET.SubElement(incomingServer, "authentication").text = "password-cleartext"
 
-    incomingServer = ET.SubElement(
-        emailProvider, "incomingServer", type="smtp"
+    outgoingServer = ET.SubElement(
+        emailProvider, "outgoingServer", type="smtp"
     )
-    ET.SubElement(incomingServer, "hostname").text = smtp_server_hostname
-    ET.SubElement(incomingServer, "port").text = "587"
-    ET.SubElement(incomingServer, "socketType").text = "STARTTLS"
-    ET.SubElement(incomingServer, "username").text = "%EMAILADDRESS%"
-    ET.SubElement(incomingServer, "authentication").text = "password-cleartext"
+    ET.SubElement(outgoingServer, "hostname").text = smtp_server_hostname
+    ET.SubElement(outgoingServer, "port").text = "587"
+    ET.SubElement(outgoingServer, "socketType").text = "STARTTLS"
+    ET.SubElement(outgoingServer, "username").text = "%EMAILADDRESS%"
+    ET.SubElement(outgoingServer, "authentication").text = "password-cleartext"
 
     tree = ET.ElementTree(root)
     ET.indent(tree, space="    ", level=0)
 
     return ET.tostring(root, encoding="unicode", xml_declaration=True) + "\n"
```

### Comparing `self-discover-1.0/self_discover.egg-info/PKG-INFO` & `self-discover-1.0.1/self_discover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-discover
-Version: 1.0
+Version: 1.0.1
 Summary: Self Discover serves autodiscover (Outlook) and autoconfig (Thunderbird) XML files for mail auto-configuration.
 Home-page: https://github.com/CyberfusionIO/Self-Discover
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,fastapi,mail,email,outlook,thunderbird,autodiscover,autoconfig
 Platform: linux
```

### Comparing `self-discover-1.0/setup.py` & `self-discover-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="self-discover",
-    version="1.0",
+    version="1.0.1",
     description="Self Discover serves autodiscover (Outlook) and autoconfig (Thunderbird) XML files for mail auto-configuration.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     author="William Edwards",
     author_email="support@cyberfusion.nl",
     url="https://github.com/CyberfusionIO/Self-Discover",
```


# Comparing `tmp/whatsapp-api-client-python-0.0.37.tar.gz` & `tmp/whatsapp-api-client-python-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-client-python-0.0.37.tar", last modified: Wed Jun 14 05:53:45 2023, max compression
+gzip compressed data, was "whatsapp-api-client-python-0.0.38.tar", last modified: Mon Jul  3 08:55:20 2023, max compression
```

## Comparing `whatsapp-api-client-python-0.0.37.tar` & `whatsapp-api-client-python-0.0.38.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 05:53:45.866652 whatsapp-api-client-python-0.0.37/
--rw-rw-rw-   0        0        0    18132 2023-06-14 05:52:26.000000 whatsapp-api-client-python-0.0.37/LICENSE
--rw-rw-rw-   0        0        0    21364 2023-06-14 05:53:45.866652 whatsapp-api-client-python-0.0.37/PKG-INFO
--rw-rw-rw-   0        0        0    20328 2023-06-14 05:52:26.000000 whatsapp-api-client-python-0.0.37/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 05:53:45.866652 whatsapp-api-client-python-0.0.37/setup.cfg
--rw-rw-rw-   0        0        0     1398 2023-06-14 05:52:26.000000 whatsapp-api-client-python-0.0.37/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:53:45.843774 whatsapp-api-client-python-0.0.37/tests/
--rw-rw-rw-   0        0        0     3879 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/tests/test_methods.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:53:45.846783 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/
--rw-rw-rw-   0        0        0     2822 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/API.py
--rw-rw-rw-   0        0        0        0 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/__init__.py
--rw-rw-rw-   0        0        0      336 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/response.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:53:45.864647 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/
--rw-rw-rw-   0        0        0        0 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/account.py
--rw-rw-rw-   0        0        0      517 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/device.py
--rw-rw-rw-   0        0        0     4671 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/groups.py
--rw-rw-rw-   0        0        0     2174 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/journals.py
--rw-rw-rw-   0        0        0      598 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/marking.py
--rw-rw-rw-   0        0        0      865 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/queues.py
--rw-rw-rw-   0        0        0     3354 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/receiving.py
--rw-rw-rw-   0        0        0     7412 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/sending.py
--rw-rw-rw-   0        0        0     4254 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/serviceMethods.py
--rw-rw-rw-   0        0        0     1257 2023-06-04 05:34:22.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/webhooks.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:53:45.852913 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/
--rw-rw-rw-   0        0        0    21364 2023-06-14 05:53:45.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      902 2023-06-14 05:53:45.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 05:53:45.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 05:53:45.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-14 05:53:45.000000 whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 08:55:20.009895 whatsapp-api-client-python-0.0.38/
+-rw-rw-rw-   0        0        0    18132 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/LICENSE
+-rw-rw-rw-   0        0        0    21313 2023-07-03 08:55:20.009895 whatsapp-api-client-python-0.0.38/PKG-INFO
+-rw-rw-rw-   0        0        0    20328 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:55:20.010898 whatsapp-api-client-python-0.0.38/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:55:19.992850 whatsapp-api-client-python-0.0.38/tests/
+-rw-rw-rw-   0        0        0     3965 2023-07-03 08:51:05.000000 whatsapp-api-client-python-0.0.38/tests/test_methods.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:55:19.995859 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/
+-rw-rw-rw-   0        0        0     2058 2023-07-03 08:41:02.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/API.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/__init__.py
+-rw-rw-rw-   0        0        0      363 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/response.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:55:20.008892 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-07-01 10:03:15.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/account.py
+-rw-rw-rw-   0        0        0      595 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/device.py
+-rw-rw-rw-   0        0        0     4518 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/groups.py
+-rw-rw-rw-   0        0        0     2174 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/journals.py
+-rw-rw-rw-   0        0        0      743 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/marking.py
+-rw-rw-rw-   0        0        0      928 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/queues.py
+-rw-rw-rw-   0        0        0     1238 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/receiving.py
+-rw-rw-rw-   0        0        0     8002 2023-07-03 08:50:13.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/sending.py
+-rw-rw-rw-   0        0        0     3599 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/serviceMethods.py
+-rw-rw-rw-   0        0        0     2640 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/webhooks.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:55:19.999868 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/
+-rw-rw-rw-   0        0        0    21313 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      902 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-03 08:55:19.000000 whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/top_level.txt
```

### Comparing `whatsapp-api-client-python-0.0.37/LICENSE` & `whatsapp-api-client-python-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.37/PKG-INFO` & `whatsapp-api-client-python-0.0.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-client-python
-Version: 0.0.37
+Version: 0.0.38
 Summary: This library helps you easily create a Python application with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-api-client-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿# whatsapp-api-client-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-api-client-python)
```

### Comparing `whatsapp-api-client-python-0.0.37/README.md` & `whatsapp-api-client-python-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.37/setup.py` & `whatsapp-api-client-python-0.0.38/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-api-client-python",
-    version="0.0.37",
+    version="0.0.38",
     description=(
         "This library helps you easily create"
         " a Python application with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -18,21 +18,20 @@
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
     install_requires=["requests==2.31.0"],
-    python_requires=">=3.7"
+    python_requires=">=3.8"
 )
```

### Comparing `whatsapp-api-client-python-0.0.37/tests/test_methods.py` & `whatsapp-api-client-python-0.0.38/tests/test_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import unittest
-from unittest.mock import patch, Mock
+from unittest.mock import Mock, patch
 
 from whatsapp_api_client_python.API import GreenApi
 
 api = GreenApi("", "")
 
+path = "examples/data/green-api-logo_2.png"
+
 
 class MethodsTestCase(unittest.TestCase):
-    @patch("whatsapp_api_client_python.API.requests.request")
+    @patch("whatsapp_api_client_python.API.Session.request")
     def test_methods(self, mock_request):
         mock_request.return_value = Mock(
             status_code=200, text="{\"example\": {\"key\": \"value\"}}"
         )
 
         methods = [
             *self.account_methods,
@@ -37,15 +39,15 @@
             api.account.getSettings(),
             api.account.setSettings({}),
             api.account.getStateInstance(),
             api.account.getStatusInstance(),
             api.account.reboot(),
             api.account.logout(),
             api.account.qr(),
-            # api.account.setProfilePicture("")
+            api.account.setProfilePicture(path)
         ]
 
     @property
     def device_methods(self):
         return [api.device.getDeviceInfo()]
 
     @property
@@ -54,15 +56,15 @@
             api.groups.createGroup("", []),
             api.groups.updateGroupName("", ""),
             api.groups.getGroupData(""),
             api.groups.addGroupParticipant("", ""),
             api.groups.removeGroupParticipant("", ""),
             api.groups.setGroupAdmin("", ""),
             api.groups.removeAdmin("", ""),
-            # api.groups.setGroupPicture("", ""),
+            api.groups.setGroupPicture("", path),
             api.groups.leaveGroup("")
         ]
 
     @property
     def log_methods(self):
         return [
             api.journals.getChatHistory(""),
@@ -76,33 +78,34 @@
         return [
             api.queues.showMessagesQueue(),
             api.queues.clearMessagesQueue()
         ]
 
     @property
     def read_mark_methods(self):
-        return [api.marking.readChat("", "")]
+        return [api.marking.readChat("")]
 
     @property
     def receiving_methods(self):
         return [
             api.receiving.receiveNotification(),
             api.receiving.deleteNotification(0),
-            api.receiving.downloadFile("")
+            api.receiving.downloadFile("", "")
         ]
 
     @property
     def sending_methods(self):
         return [
             api.sending.sendMessage("", ""),
             api.sending.sendButtons("", "", []),
             api.sending.sendTemplateButtons("", "", []),
             api.sending.sendListMessage("", "", "", []),
-            # api.sending.sendFileByUpload("", ""),
+            api.sending.sendFileByUpload("", path),
             api.sending.sendFileByUrl("", "", ""),
+            api.sending.uploadFile(path),
             api.sending.sendLocation("", 0.0, 0.0),
             api.sending.sendContact("", {}),
             api.sending.sendLink("", ""),
             api.sending.forwardMessages("", "", [])
         ]
 
     @property
@@ -111,13 +114,13 @@
             api.serviceMethods.checkWhatsapp(0),
             api.serviceMethods.getAvatar(""),
             api.serviceMethods.getContacts(),
             api.serviceMethods.getContactInfo(""),
             api.serviceMethods.deleteMessage("", ""),
             api.serviceMethods.archiveChat(""),
             api.serviceMethods.unarchiveChat(""),
-            api.serviceMethods.setDisappearingChat("", 0)
+            api.serviceMethods.setDisappearingChat("")
         ]
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/account.py` & `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/account.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/groups.py` & `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,148 @@
-import os.path
-from array import array
+from pathlib import Path
+from typing import List, TYPE_CHECKING
 
-from whatsapp_api_client_python.response import Response
+from ..response import Response
+
+if TYPE_CHECKING:
+    from ..API import GreenApi
 
 
 class Groups:
-    def __init__(self, greenApi) -> None:
-        self.greenApi = greenApi
-        
-    def addGroupParticipant(self, 
-            groupId: str, 
-            participantChatId: str) -> Response:
-            'The method adds a participant to a group chat.'
-
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId,
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/AddGroupParticipant/{{apiTokenInstance}}',
-                requestBody)
-
-    def createGroup(self, groupName: str, chatIds: array) -> Response:
-            'The method is aimed for creating a group chat.'
-            
-            requestBody = {
-                'groupName': groupName,
-                'chatIds': chatIds
-            }
-
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/CreateGroup/{{apiTokenInstance}}',
-                requestBody)
+    def __init__(self, api: "GreenApi"):
+        self.api = api
 
-    def getGroupData(self, groupId: str) -> Response:
-            'The method gets group chat data.'
+    def createGroup(self, groupName: str, chatIds: List[str]) -> Response:
+        """The method is aimed for creating a group chat."""
 
-            requestBody = {
-                'groupId': groupId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/GetGroupData/{{apiTokenInstance}}',
-                requestBody)
+        request_body = self.__handle_parameters(locals())
 
-    def leaveGroup(self, groupId: str) -> Response:
-            'The method makes the current account user leave the group chat.'
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "createGroup/{{apiTokenInstance}}"
+            ), request_body
+        )
+
+    def updateGroupName(self, groupId: str, groupName: str) -> Response:
+        """The method changes a group chat name."""
+
+        request_body = self.__handle_parameters(locals())
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "updateGroupName/{{apiTokenInstance}}"
+            ), request_body
+        )
+
+    def getGroupData(self, groupId: str) -> Response:
+        """The method gets group chat data."""
+
+        request_body = self.__handle_parameters(locals())
 
-            requestBody = {
-                'groupId': groupId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/LeaveGroup/{{apiTokenInstance}}',
-                requestBody)
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "getGroupData/{{apiTokenInstance}}"
+            ), request_body
+        )
+
+    def addGroupParticipant(
+            self, groupId: str, participantChatId: str
+    ) -> Response:
+        """The method adds a participant to a group chat."""
+
+        request_body = self.__handle_parameters(locals())
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "addGroupParticipant/{{apiTokenInstance}}"
+            ), request_body
+        )
+
+    def removeGroupParticipant(
+            self, groupId: str, participantChatId: str
+    ) -> Response:
+        """The method removes a participant from a group chat."""
+
+        request_body = self.__handle_parameters(locals())
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "removeGroupParticipant/{{apiTokenInstance}}"
+            ), request_body
+        )
+
+    def setGroupAdmin(self, groupId: str, participantChatId: str) -> Response:
+        """
+        The method sets a group chat participant as an administrator.
+        """
+
+        request_body = self.__handle_parameters(locals())
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "setGroupAdmin/{{apiTokenInstance}}"
+            ), request_body
+        )
 
     def removeAdmin(self, groupId: str, participantChatId: str) -> Response:
-            'The method removes a participant from group chat '\
-            'administartion rights.'
+        """
+        The method removes a participant from group chat administration
+        rights.
+        """
+
+        request_body = self.__handle_parameters(locals())
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "removeAdmin/{{apiTokenInstance}}"
+            ), request_body
+        )
+
+    def setGroupPicture(self, groupId: str, path: str) -> Response:
+        """The method sets a group picture."""
+
+        request_body = self.__handle_parameters(locals())
+
+        file_name = Path(path).name
+        files = {"file": (file_name, open(path, "rb"), "image/jpeg")}
+
+        request_body.pop("path")
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "setGroupPicture/{{apiTokenInstance}}"
+            ), request_body, files
+        )
+
+    def leaveGroup(self, groupId: str) -> Response:
+        """
+        The method makes the current account user leave the group chat.
+        """
+
+        request_body = self.__handle_parameters(locals())
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "leaveGroup/{{apiTokenInstance}}"
+            ), request_body
+        )
+
+    @classmethod
+    def __handle_parameters(cls, parameters: dict) -> dict:
+        handled_parameters = parameters.copy()
+
+        handled_parameters.pop("self")
+
+        for key, value in parameters.items():
+            if value is None:
+                handled_parameters.pop(key)
 
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/RemoveAdmin/{{apiTokenInstance}}',
-                requestBody)
-
-    def removeGroupParticipant(self, 
-        groupId: str, 
-        participantChatId: str) -> Response:
-            'The method removes a participant from a group chat.'
-
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/RemoveGroupParticipant/{{apiTokenInstance}}',
-                requestBody)
-
-    def setGroupAdmin(self, 
-        groupId: str, 
-        participantChatId: str) -> Response:
-            'The method sets a group chat participant as an administrator.'
-
-            requestBody = {
-                'groupId': groupId,
-                'participantChatId': participantChatId
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/SetGroupAdmin/{{apiTokenInstance}}',
-                requestBody)
-
-    def setGroupPicture(self, 
-        groupId: str, 
-        path: str) -> Response:
-            'The method sets a group picture.'
-
-            requestBody = {
-                'groupId': groupId
-            }
-
-            pathParts = os.path.split(path)
-            file = pathParts[1]
-
-            files = [
-                ('file',(file, open(path,'rb'),'image/jpeg'))
-            ]
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/SetGroupPicture/{{apiTokenInstance}}',
-                requestBody, files)
-
-    def updateGroupName(self, 
-        groupId: str, 
-        groupName: str) -> Response:
-            'The method changes a group chat name.'
-
-            requestBody = {
-                'groupId': groupId,
-                'groupName': groupName
-            }
-            
-            return self.greenApi.request('POST', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/UpdateGroupName/{{apiTokenInstance}}',
-                requestBody)
+        return handled_parameters
```

### Comparing `whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/journals.py` & `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/journals.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,29 @@
     def getChatHistory(
             self, chatId: str, count: Optional[int] = None
     ) -> Response:
         """The method returns the chat message history."""
 
         request_body = locals()
         if count is None:
-            del request_body["count"]
-        del request_body["self"]
+            request_body.pop("count")
+        request_body.pop("self")
 
         return self.api.request(
             "POST", (
                 "{{host}}/waInstance{{idInstance}}/"
                 "getChatHistory/{{apiTokenInstance}}"
             ), request_body
         )
 
     def getMessage(self, chatId: str, idMessage: str) -> Response:
         """The method returns the chat message."""
 
         request_body = locals()
-        del request_body["self"]
+        request_body.pop("self")
 
         return self.api.request(
             "POST", (
                 "{{host}}/waInstance{{idInstance}}/"
                 "getMessage/{{apiTokenInstance}}"
             ), request_body
         )
```

### Comparing `whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/queues.py` & `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/queues.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,37 @@
-from whatsapp_api_client_python.response import Response
+from typing import TYPE_CHECKING
 
+from ..response import Response
 
-class Queues:
-    def __init__(self, greenApi) -> None:
-        self.greenApi = greenApi
-        
-    def clearMessagesQueue(self) -> Response:
-            'The method is aimed for clearing the queue of messages to be sent.'
+if TYPE_CHECKING:
+    from ..API import GreenApi
 
-            return self.greenApi.request('GET', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/ClearMessagesQueue/{{apiTokenInstance}}')
+
+class Queues:
+    def __init__(self, api: "GreenApi"):
+        self.api = api
 
     def showMessagesQueue(self) -> Response:
-            'The method is aimed for getting a list of messages in the queue '\
-            'to be sent. Messages sending rate is managed by Messages sending '\
-            'delay parameter.'
-
-            return self.greenApi.request('GET', 
-                '{{host}}/waInstance{{idInstance}}'
-                '/ShowMessagesQueue/{{apiTokenInstance}}')
+        """
+        The method is aimed for getting a list of messages in the queue
+        to be sent.
+        """
+
+        return self.api.request(
+            "GET", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "showMessagesQueue/{{apiTokenInstance}}"
+            )
+        )
+
+    def clearMessagesQueue(self) -> Response:
+        """
+        The method is aimed for clearing the queue of messages to be
+        sent.
+        """
+
+        return self.api.request(
+            "GET", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "clearMessagesQueue/{{apiTokenInstance}}"
+            )
+        )
```

### Comparing `whatsapp-api-client-python-0.0.37/whatsapp_api_client_python/tools/sending.py` & `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python/tools/sending.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         request_body = self.__handle_parameters(locals())
 
         file_name = pathlib.Path(path).name
         content_type = mimetypes.guess_type(file_name)[0]
 
         files = {"file": (file_name, open(path, "rb"), content_type)}
 
-        del request_body["path"]
+        request_body.pop("path")
 
         return self.api.request(
             "POST", (
                 "{{host}}/waInstance{{idInstance}}/"
                 "sendFileByUpload/{{apiTokenInstance}}"
             ), request_body, files
         )
@@ -150,14 +150,32 @@
         return self.api.request(
             "POST", (
                 "{{host}}/waInstance{{idInstance}}/"
                 "sendFileByUrl/{{apiTokenInstance}}"
             ), request_body
         )
 
+    def uploadFile(self, path: str) -> Response:
+        """
+        The method is designed to upload a file to the cloud storage,
+        which can be sent using the sendFileByUrl method.
+        """
+
+        file_name = pathlib.Path(path).name
+        content_type = mimetypes.guess_type(file_name)[0]
+
+        files = {"file": (file_name, open(path, "rb"), content_type)}
+
+        return self.api.request(
+            "POST", (
+                "{{host}}/waInstance{{idInstance}}/"
+                "uploadFile/{{apiTokenInstance}}"
+            ), files=files
+        )
+
     def sendLocation(
             self,
             chatId: str,
             latitude: float,
             longitude: float,
             nameLocation: Optional[str] = None,
             address: Optional[str] = None,
```

### Comparing `whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/PKG-INFO` & `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-client-python
-Version: 0.0.37
+Version: 0.0.38
 Summary: This library helps you easily create a Python application with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-api-client-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿# whatsapp-api-client-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-api-client-python)
```

### Comparing `whatsapp-api-client-python-0.0.37/whatsapp_api_client_python.egg-info/SOURCES.txt` & `whatsapp-api-client-python-0.0.38/whatsapp_api_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*


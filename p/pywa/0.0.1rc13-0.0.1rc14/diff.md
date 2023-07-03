# Comparing `tmp/pywa-0.0.1rc13-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25031 bytes, number of entries: 15
+Zip file size: 26427 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-02 08:23 pywa/__version__.py
--rw-rw-r--  2.0 unx    14991 b- defN 23-Jul-02 07:58 pywa/api.py
--rw-rw-r--  2.0 unx    26847 b- defN 23-Jul-02 08:19 pywa/client.py
--rw-rw-r--  2.0 unx     2322 b- defN 23-Jul-02 08:19 pywa/errors.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-03 08:44 pywa/__version__.py
+-rw-rw-r--  2.0 unx    14991 b- defN 23-Jul-03 08:35 pywa/api.py
+-rw-rw-r--  2.0 unx    26847 b- defN 23-Jul-03 08:42 pywa/client.py
+-rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
 -rw-rw-r--  2.0 unx    15854 b- defN 23-Jul-02 08:19 pywa/filters.py
 -rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-02 08:19 pywa/handlers.py
 -rw-rw-r--  2.0 unx    34447 b- defN 23-Jul-02 08:21 pywa/types.py
 -rw-rw-r--  2.0 unx      991 b- defN 23-Jun-20 16:58 pywa/utils.py
--rw-rw-r--  2.0 unx     4399 b- defN 23-Jun-30 09:01 pywa/webhook.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4399 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/RECORD
-15 files, 108456 bytes uncompressed, 23249 bytes compressed:  78.6%
+-rw-rw-r--  2.0 unx     4613 b- defN 23-Jul-03 08:35 pywa/webhook.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-03 08:45 pywa-0.0.1rc14.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-03 08:45 pywa-0.0.1rc14.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-03 08:45 pywa-0.0.1rc14.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-03 08:45 pywa-0.0.1rc14.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-03 08:45 pywa-0.0.1rc14.dist-info/RECORD
+15 files, 113527 bytes uncompressed, 24645 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pywa/utils.py
 Comment: 
 
 Filename: pywa/webhook.py
 Comment: 
 
-Filename: pywa-0.0.1rc13.dist-info/LICENSE
+Filename: pywa-0.0.1rc14.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc13.dist-info/METADATA
+Filename: pywa-0.0.1rc14.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc13.dist-info/WHEEL
+Filename: pywa-0.0.1rc14.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc13.dist-info/top_level.txt
+Filename: pywa-0.0.1rc14.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc13.dist-info/RECORD
+Filename: pywa-0.0.1rc14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc13"
+__version__ = "0.0.1rc14"
```

## pywa/api.py

```diff
@@ -47,15 +47,15 @@
         Returns:
             The response JSON.
 
         Raises:
             WhatsAppError: If the request failed.
         """
         res = self._session.request(method=method, url=f"{self._base_url}{endpoint}", **kwargs)
-        if res.status_code != 200:
+        if res.status_code >= 400:
             raise WhatsAppError.from_response(status_code=res.status_code, error=res.json()["error"])
         return res.json()
 
     def send_text_message(
             self,
             to: str | int,
             text: str,
```

## pywa/errors.py

```diff
@@ -1,73 +1,232 @@
 """
 This module contains the errors that can be raised by the WhatsApp Cloud API or incoming error from the webhook.
 """
 
-__all__ = ("WhatsAppError",)
+import functools
+from typing import Type
 
 
 class WhatsAppError(Exception):
     """
-    Represents an error that happened while making a request to the WhatsApp Cloud API or incoming error from the webhook.
+    Base exception for all WhatsApp errors.
 
     - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/support/error-codes
 
     Attributes:
-        status_code: The status code (in case of response, else None).
         error_code: The error code.
         message: The error message.
         details: The error details (optional).
         fbtrace_id: The Facebook trace ID (optional).
         href: The href to the documentation (optional).
+        status_code: The status code (in case of response, else None).
     """
+    __error_codes__ = ()
+
     def __init__(
             self,
-            status_code: int | None,
             error_code: int,
             message: str,
             details: str | None,
             fbtrace_id: str | None,
-            href: str | None
+            href: str | None,
+            status_code: int | None,
     ) -> None:
-        self.status_code = status_code
         self.error_code = error_code
         self.message = message
         self.details = details
         self.fbtrace_id = fbtrace_id
         self.href = href
+        self.status_code = status_code
 
     @classmethod
     def from_response(
             cls,
             status_code: int,
             error: dict
     ) -> "WhatsAppError":
         """Create an error from a response."""
-        return cls(
+        return cls._get_exception(error["code"])(
             status_code=status_code,
             error_code=error["code"],
             message=error["message"],
             details=error.get("error_data", {}).get("details", None),
             fbtrace_id=error.get("fbtrace_id"),
             href=error.get('href')
         )
 
     @classmethod
     def from_incoming_error(
             cls,
             error: dict
     ) -> "WhatsAppError":
         """Create an error from an incoming error."""
-        return cls(
+        return cls._get_exception(error["code"])(
             status_code=None,
             error_code=error["code"],
             message=error["message"],
             details=error.get("error_data", {}).get("details", None),
             fbtrace_id=error.get("fbtrace_id"),
             href=error.get('href')
         )
 
+    @staticmethod
+    @functools.cache
+    def _all_exceptions() -> tuple[Type["WhatsAppError"], ...]:
+        """Get all exceptions that can be raised from this error."""
+        return tuple(ss for s in WhatsAppError.__subclasses__() for ss in s.__subclasses__())
+
+    @staticmethod
+    @functools.cache
+    def _get_exception(code: int) -> Type["WhatsAppError"]:
+        """Get the exception class from the error code."""
+        return next((e for e in WhatsAppError._all_exceptions() if code in e.__error_codes__), WhatsAppError)
+
     def __str__(self) -> str:
-        return f"WhatsAppError(message={self.message!r}, details={self.details!r}, error_code={self.error_code!r})"
+        return f"{self.__class__.__name__}(message={self.message!r}, details={self.details!r}, code={self.error_code!r})"
 
     def __repr__(self) -> str:
         return self.__str__()
+
+
+class AuthorizationError(WhatsAppError):
+    """Base exception for all authorization errors."""
+    __error_codes__ = None
+
+
+class AuthException(AuthorizationError):
+    """We were unable to authenticate the app user"""
+    __error_codes__ = (0,)
+
+
+class APIMethod(AuthorizationError):
+    """Capability or permissions issue."""
+    __error_codes__ = (3,)
+
+
+class PermissionDenied(AuthorizationError):
+    """Permission is either not granted or has been removed."""
+    __error_codes__ = (10,)
+
+
+class ExpiredAccessToken(AuthorizationError):
+    """Your access token has expired."""
+    __error_codes__ = (190,)
+
+
+class APIPermission(AuthorizationError):
+    """Permission is either not granted or has been removed."""
+    __error_codes__ = range(200, 300)
+
+
+# ====================================================================================================
+
+
+class ThrottlingError(WhatsAppError):
+    """Base exception for all rate limit errors."""
+    __error_codes__ = None
+
+
+class ToManyAPICalls(ThrottlingError):
+    """The app has reached its API call rate limit."""
+    __error_codes__ = (4,)
+
+
+class RateLimitIssues(ThrottlingError):
+    """The WhatsApp Business Account has reached its rate limit."""
+    __error_codes__ = (80007,)
+
+
+class RateLimitHit(ThrottlingError):
+    """Cloud API message throughput has been reached."""
+    __error_codes__ = (130429,)
+
+
+class SpamRateLimitHit(ThrottlingError):
+    """
+    Message failed to send because there are restrictions on how many messages can be sent from this phone number.
+    This may be because too many previous messages were blocked or flagged as spam.
+    """
+    __error_codes__ = (131048,)
+
+
+class ToManyMessages(ThrottlingError):
+    """
+    Too many messages sent from the sender phone number to the same recipient phone number in a short period of time.
+    """
+    __error_codes__ = (131056,)
+
+
+# ====================================================================================================
+
+
+class IntegrityError(WhatsAppError):
+    """Base exception for all integrity errors."""
+    __error_codes__ = None
+
+
+class TemporarilyBlocked(IntegrityError):
+    """
+    The WhatsApp Business Account associated with the app has been restricted or disabled for violating a platform policy.
+    """
+    __error_codes__ = (368,)
+
+
+class AccountLocked(IntegrityError):
+    """
+    The WhatsApp Business Account associated with the app has been restricted or disabled for violating a platform
+    policy, or we were unable to verify data included in the request against data set on the WhatsApp Business
+    Account (e.g, the two-step pin included in the request is incorrect).
+    """
+    __error_codes__ = (131031,)
+
+
+# ====================================================================================================
+
+
+class SendMessageError(WhatsAppError):
+    """Base exception for all message errors."""
+    __error_codes__ = None
+
+
+class MessageUndeliverable(SendMessageError):
+    """Unable to deliver message. Reasons can include:
+
+        - The recipient phone number is not a WhatsApp phone number.
+        - Recipient has not accepted our new Terms of Service and Privacy Policy.
+        - Recipient using an old WhatsApp version; must use the following WhatsApp version or greater:
+            Android: 2.21.15.15
+            SMBA: 2.21.15.15
+            iOS: 2.21.170.4
+            SMBI: 2.21.170.4
+            KaiOS: 2.2130.10
+            Web: 2.2132.6
+    """
+    __error_codes__ = (131026,)
+
+
+class ReEngagementMessage(SendMessageError):
+    """More than 24 hours have passed since the recipient last replied to the sender number."""
+    __error_codes__ = (131047,)
+
+
+class UnsupportedMessageType(SendMessageError):
+    """The message type is not supported."""
+    __error_codes__ = (131051,)
+
+
+class RecipientNotInAllowedList(SendMessageError):
+    """
+    When using test numbers, you can add up to 5 numbers that can receive messages. This error is raised when the
+    recipient is not in the list.
+    """
+    __error_codes__ = (131030,)
+
+
+class InvalidParameter(SendMessageError):
+    """The parameter you passed is invalid."""
+    __error_codes__ = (131009,)
+
+
+class MissingRequiredParameter(SendMessageError):
+    """You must provide a value for the required parameter."""
+    __error_codes__ = (131008,)
```

## pywa/webhook.py

```diff
@@ -67,32 +67,37 @@
                 return await call_next(request)
 
         else:
             raise ValueError("The app must be a Flask or FastAPI app.")
 
     def call_handlers(self, update: dict) -> None:
         """Call the handlers for the given update."""
-        if not self.filter_updates or (
-                update["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] == self.wa_client.phone_id):
-            for raw_update_handler in self.handlers["raw_update"]:
-                raw_update_handler(self.wa_client, update)
-            update, key = self.convert_dict_to_update(client=self.wa_client, d=update)
-            for handler in self.handlers[key]:  # TODO execute in parallel
-                handler(self.wa_client, update)
+        try:
+            if not self.filter_updates or (
+                    update["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] == self.wa_client.phone_id):
+                for raw_update_handler in self.handlers["raw_update"]:
+                    raw_update_handler(self.wa_client, update)
+                update, key = self.convert_dict_to_update(client=self.wa_client, d=update)
+                if key is None:
+                    return
+                for handler in self.handlers[key]:  # TODO execute in parallel
+                    handler(self.wa_client, update)
+        except (KeyError, IndexError):  # the update not send to this phone and filter_updates is True
+            pass
 
     @staticmethod
-    def convert_dict_to_update(client: WhatsApp, d: dict) -> tuple[BaseUpdate, str]:
+    def convert_dict_to_update(client: WhatsApp, d: dict) -> tuple[BaseUpdate | None, str | None]:
         """Convert a webhook dict to a BaseUpdate object."""
         value = d["entry"][0]["changes"][0]["value"]
         if 'messages' in value:
             if value["messages"][0]["type"] != "interactive":
                 return Message.from_dict(client=client, value=value), "message"
             else:
                 if value["messages"][0]["interactive"]["type"] == "button_reply":
                     return CallbackButton.from_dict(client=client, value=value), "button"
                 elif value["messages"][0]["interactive"]["type"] == "list_reply":
                     return CallbackSelection.from_dict(client=client, value=value), "selection"
 
         elif 'statuses' in value:
             return MessageStatus.from_dict(client=client, value=value), "message_status"
-        else:
-            raise ValueError("Invalid webhook data: " + str(d))
+        return None, None  # the update is not supported
+
```

## Comparing `pywa-0.0.1rc13.dist-info/LICENSE` & `pywa-0.0.1rc14.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc13.dist-info/METADATA` & `pywa-0.0.1rc14.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc13
+Version: 0.0.1rc14
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
@@ -21,15 +21,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Provides-Extra: fastapi
 Requires-Dist: fastapi ; extra == 'fastapi'
-Requires-Dist: uvicorn[standard] ; extra == 'fastapi'
+Requires-Dist: uvicorn ; extra == 'fastapi'
 Provides-Extra: flask
 Requires-Dist: flask ; extra == 'flask'
 
 .. image:: https://i.imgur.com/hbGP0rW.png
   :width: 200
   :alt: PyWa Logo
 .. end-logo
@@ -119,28 +119,28 @@
     wa = WhatsApp(
         phone_id='1234567890',
         token='xxxxxxxxxxxxxxx',
         server=flask_app,
         verify_token='XYZXYZ',
     )
 
-    @wa.on_message(TextFilter.equals('Hello', 'Hi'))
+    @wa.on_message(TextFilter.match('Hello', 'Hi'))
     def hello(client: WhatsApp, message: Message):
         message.react('👋')
         message.reply_text(
             text='Hello from PyWa!',
             keyboard=[
                 InlineButton(
                     title='Click me!',
                     callback_data='id:123'
                 )
             ]
         )
 
-    @wa.on_callback_button(CallbackFilter.data_startswith('id:'))
+    @wa.on_callback_button(CallbackFilter.data_startswith('id'))
     def click_me(client: WhatsApp, clb: CallbackButton):
         clb.reply_text('You clicked me!')
 
     flask_app.run()  # Run the flask app to start the webhook
 
 
 💾 **Requirements**
```

## Comparing `pywa-0.0.1rc13.dist-info/RECORD` & `pywa-0.0.1rc14.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=pbauRs5Hqw_IKLlJ8yVG-JwWzqmGTpAEv2LPEWxqin8,26
-pywa/api.py,sha256=P6cXCxFjVbx7i8Ty5MGWbWsYqcv_Z7Ez-Oqz99GeHCs,14991
+pywa/__version__.py,sha256=NGwXVoQ6SdNPhkhKG-2C-o1hfqUZq-Rgs0nLUhpgb1c,26
+pywa/api.py,sha256=G3NL2PKhGO7YhrVeEz2bfJhGNfD7j1lGwgKnhsZpAuU,14991
 pywa/client.py,sha256=ita4mY7UfM8xwjvEV_a60-3W4frC3uAJP-xumP5oYdM,26847
-pywa/errors.py,sha256=aoAMLuWcLGgMQICN-YdnrRbSJi2LrbKzwxznQ2XO2-s,2322
+pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
 pywa/filters.py,sha256=UveMHCSjbAT5xR6JccQWOtC02kHN6mpU3COlmzc0Z-U,15854
 pywa/handlers.py,sha256=DTlKr-yvVKpTgh3F0Gsq78gT5XhBIo_VVnYHz3lu25w,1794
 pywa/types.py,sha256=1eSkFpuq-nntPe3-jjrbjIVfkkBWuRTrGQcyxQ39rv8,34447
 pywa/utils.py,sha256=GRTfSvmsuOBd1_Yw2c90XoALqVPuy6HzyvJuqg3xjtI,991
-pywa/webhook.py,sha256=5Yc4OAtcYvumcguf22od-lg4VYEWLFadYJou-h_Rbwk,4399
-pywa-0.0.1rc13.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc13.dist-info/METADATA,sha256=efBjKWQCdrWELM1h0JbpRciT7MYPhsMcsq55lNgtL3E,4399
-pywa-0.0.1rc13.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc13.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc13.dist-info/RECORD,,
+pywa/webhook.py,sha256=UFsV3UyltYLj3MYjURG6YImjU4hYVHkDffweyEe1Jdc,4613
+pywa-0.0.1rc14.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc14.dist-info/METADATA,sha256=tQoHoCaXoak4kISu3-xecF9sSYSGaMaau0zxf3sO1V4,4387
+pywa-0.0.1rc14.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc14.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc14.dist-info/RECORD,,
```


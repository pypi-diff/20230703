# Comparing `tmp/context_python-0.2.1.tar.gz` & `tmp/context_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "context_python-0.2.1.tar", max compression
+gzip compressed data, was "context_python-0.3.0.tar", max compression
```

## Comparing `context_python-0.2.1.tar` & `context_python-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2023-06-01 15:29:28.188846 context_python-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2899 2023-06-01 16:09:16.093724 context_python-0.2.1/README.md
--rw-r--r--   0        0        0       43 2023-06-01 14:40:09.995595 context_python-0.2.1/getcontext/__init__.py
--rw-r--r--   0        0        0      709 2023-06-01 14:36:11.780194 context_python-0.2.1/getcontext/generated/__init__.py
--rw-r--r--   0        0        0     3290 2023-06-01 14:36:11.780203 context_python-0.2.1/getcontext/generated/_client.py
--rw-r--r--   0        0        0     2643 2023-06-01 14:36:11.780222 context_python-0.2.1/getcontext/generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780394 context_python-0.2.1/getcontext/generated/_patch.py
--rw-r--r--   0        0        0    78836 2023-06-01 14:36:11.780239 context_python-0.2.1/getcontext/generated/_serialization.py
--rw-r--r--   0        0        0      709 2023-06-01 14:36:11.780251 context_python-0.2.1/getcontext/generated/aio/__init__.py
--rw-r--r--   0        0        0     3426 2023-06-01 14:36:11.780275 context_python-0.2.1/getcontext/generated/aio/_client.py
--rw-r--r--   0        0        0     2685 2023-06-01 14:36:11.780268 context_python-0.2.1/getcontext/generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780179 context_python-0.2.1/getcontext/generated/aio/_patch.py
--rw-r--r--   0        0        0      665 2023-06-01 14:36:11.780283 context_python-0.2.1/getcontext/generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     6598 2023-06-01 14:36:11.780301 context_python-0.2.1/getcontext/generated/aio/operations/_operations.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780424 context_python-0.2.1/getcontext/generated/aio/operations/_patch.py
--rw-r--r--   0        0        0      973 2023-06-01 14:36:11.780337 context_python-0.2.1/getcontext/generated/models/__init__.py
--rw-r--r--   0        0        0      794 2023-06-01 14:36:11.780328 context_python-0.2.1/getcontext/generated/models/_enums.py
--rw-r--r--   0        0        0     4130 2023-06-01 14:36:11.780320 context_python-0.2.1/getcontext/generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780310 context_python-0.2.1/getcontext/generated/models/_patch.py
--rw-r--r--   0        0        0      665 2023-06-01 14:36:11.780259 context_python-0.2.1/getcontext/generated/operations/__init__.py
--rw-r--r--   0        0        0     7263 2023-06-01 14:36:11.780290 context_python-0.2.1/getcontext/generated/operations/_operations.py
--rw-r--r--   0        0        0      674 2023-06-01 14:36:11.780357 context_python-0.2.1/getcontext/generated/operations/_patch.py
--rw-r--r--   0        0        0       26 2023-06-01 14:36:10.592708 context_python-0.2.1/getcontext/generated/py.typed
--rw-r--r--   0        0        0      449 2023-06-01 15:50:20.326267 context_python-0.2.1/getcontext/token.py
--rw-r--r--   0        0        0      481 2023-06-01 16:11:17.537642 context_python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 context_python-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-01 15:29:28.188846 context_python-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2899 2023-06-01 16:09:16.093724 context_python-0.3.0/README.md
+-rw-r--r--   0        0        0       43 2023-06-01 14:40:09.995595 context_python-0.3.0/getcontext/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-03 14:46:15.177633 context_python-0.3.0/getcontext/generated/__init__.py
+-rw-r--r--   0        0        0     3289 2023-07-03 14:46:15.177620 context_python-0.3.0/getcontext/generated/_client.py
+-rw-r--r--   0        0        0     2642 2023-07-03 14:46:15.177821 context_python-0.3.0/getcontext/generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-07-03 14:46:15.177744 context_python-0.3.0/getcontext/generated/_patch.py
+-rw-r--r--   0        0        0    78836 2023-07-03 14:46:15.177674 context_python-0.3.0/getcontext/generated/_serialization.py
+-rw-r--r--   0        0        0      708 2023-07-03 14:46:15.177688 context_python-0.3.0/getcontext/generated/aio/__init__.py
+-rw-r--r--   0        0        0     3425 2023-07-03 14:46:15.177719 context_python-0.3.0/getcontext/generated/aio/_client.py
+-rw-r--r--   0        0        0     2684 2023-07-03 14:46:15.177865 context_python-0.3.0/getcontext/generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-07-03 14:46:15.177601 context_python-0.3.0/getcontext/generated/aio/_patch.py
+-rw-r--r--   0        0        0      664 2023-07-03 14:46:15.177761 context_python-0.3.0/getcontext/generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0    11464 2023-07-03 14:46:15.177780 context_python-0.3.0/getcontext/generated/aio/operations/_operations.py
+-rw-r--r--   0        0        0      674 2023-07-03 14:46:15.177642 context_python-0.3.0/getcontext/generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     1162 2023-07-03 14:46:15.177888 context_python-0.3.0/getcontext/generated/models/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-03 14:46:15.177961 context_python-0.3.0/getcontext/generated/models/_enums.py
+-rw-r--r--   0        0        0     4829 2023-07-03 14:46:15.177803 context_python-0.3.0/getcontext/generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-07-03 14:46:15.177794 context_python-0.3.0/getcontext/generated/models/_patch.py
+-rw-r--r--   0        0        0      664 2023-07-03 14:46:15.177705 context_python-0.3.0/getcontext/generated/operations/__init__.py
+-rw-r--r--   0        0        0    12762 2023-07-03 14:46:15.177771 context_python-0.3.0/getcontext/generated/operations/_operations.py
+-rw-r--r--   0        0        0      674 2023-07-03 14:46:15.177920 context_python-0.3.0/getcontext/generated/operations/_patch.py
+-rw-r--r--   0        0        0       26 2023-07-03 14:46:13.903709 context_python-0.3.0/getcontext/generated/py.typed
+-rw-r--r--   0        0        0      691 2023-07-03 17:14:16.935162 context_python-0.3.0/getcontext/token.py
+-rw-r--r--   0        0        0      482 2023-07-03 17:01:09.264758 context_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 context_python-0.3.0/PKG-INFO
```

### Comparing `context_python-0.2.1/LICENSE.md` & `context_python-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/README.md` & `context_python-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/getcontext/generated/__init__.py` & `context_python-0.3.0/getcontext/generated/aio/operations/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._client import ContextAPI
+from ._operations import LogOperations
 
-try:
-    from ._patch import __all__ as _patch_all
-    from ._patch import *  # pylint: disable=unused-wildcard-import
-except ImportError:
-    _patch_all = []
+from ._patch import __all__ as _patch_all
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "ContextAPI",
+    "LogOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
-
 _patch_sdk()
```

### Comparing `context_python-0.2.1/getcontext/generated/_client.py` & `context_python-0.3.0/getcontext/generated/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
 from azure.core import PipelineClient
```

### Comparing `context_python-0.2.1/getcontext/generated/_configuration.py` & `context_python-0.3.0/getcontext/generated/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

### Comparing `context_python-0.2.1/getcontext/generated/_patch.py` & `context_python-0.3.0/getcontext/generated/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/getcontext/generated/_serialization.py` & `context_python-0.3.0/getcontext/generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/getcontext/generated/aio/__init__.py` & `context_python-0.3.0/getcontext/generated/operations/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._client import ContextAPI
+from ._operations import LogOperations
 
-try:
-    from ._patch import __all__ as _patch_all
-    from ._patch import *  # pylint: disable=unused-wildcard-import
-except ImportError:
-    _patch_all = []
+from ._patch import __all__ as _patch_all
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "ContextAPI",
+    "LogOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
-
 _patch_sdk()
```

### Comparing `context_python-0.2.1/getcontext/generated/aio/_client.py` & `context_python-0.3.0/getcontext/generated/aio/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core import AsyncPipelineClient
```

### Comparing `context_python-0.2.1/getcontext/generated/aio/_configuration.py` & `context_python-0.3.0/getcontext/generated/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

### Comparing `context_python-0.2.1/getcontext/generated/aio/_patch.py` & `context_python-0.3.0/getcontext/generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/getcontext/generated/aio/operations/__init__.py` & `context_python-0.3.0/getcontext/generated/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._operations import LogOperations
+from ._client import ContextAPI
 
-from ._patch import __all__ as _patch_all
-from ._patch import *  # pylint: disable=unused-wildcard-import
+try:
+    from ._patch import __all__ as _patch_all
+    from ._patch import *  # pylint: disable=unused-wildcard-import
+except ImportError:
+    _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "LogOperations",
+    "ContextAPI",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
+
 _patch_sdk()
```

### Comparing `context_python-0.2.1/getcontext/generated/aio/operations/_operations.py` & `context_python-0.3.0/getcontext/generated/aio/operations/_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -18,15 +18,15 @@
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 
 from ... import models as _models
-from ...operations._operations import build_log_conversation_request
+from ...operations._operations import build_log_conversation_request, build_log_conversation_upsert_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class LogOperations:
     """
@@ -158,14 +158,145 @@
             authorization=authorization,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [201]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    async def conversation_upsert(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Ingests or updates conversation.
+
+        Ingests or updates conversation.
+
+        :param body: Default value is None.
+        :type body:
+         ~context_api.models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def conversation_upsert(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[IO] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Ingests or updates conversation.
+
+        Ingests or updates conversation.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def conversation_upsert(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[
+            Union[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema, IO]
+        ] = None,
+        *,
+        authorization: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """Ingests or updates conversation.
+
+        Ingests or updates conversation.
+
+        :param body: Is either a
+         PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema type or a IO
+         type. Default value is None.
+        :type body:
+         ~context_api.models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
+         or IO
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(
+                    body, "PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema"
+                )
+            else:
+                _json = None
+
+        request = build_log_conversation_upsert_request(
+            authorization=authorization,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
```

### Comparing `context_python-0.2.1/getcontext/generated/aio/operations/_patch.py` & `context_python-0.3.0/getcontext/generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/getcontext/generated/models/__init__.py` & `context_python-0.3.0/getcontext/generated/models/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models import Conversation
 from ._models import Message
 from ._models import PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema
+from ._models import PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
 
 from ._enums import MessageRole
 from ._enums import Rating
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Conversation",
     "Message",
     "PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema",
+    "PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema",
     "MessageRole",
     "Rating",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `context_python-0.2.1/getcontext/generated/models/_enums.py` & `context_python-0.3.0/getcontext/generated/models/_enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
```

### Comparing `context_python-0.2.1/getcontext/generated/models/_models.py` & `context_python-0.3.0/getcontext/generated/models/_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
 import sys
 from typing import Any, List, Optional, TYPE_CHECKING, Union
 
@@ -108,14 +108,34 @@
 
     :ivar conversation:
     :vartype conversation: ~context_api.models.Conversation
     """
 
     _attribute_map = {
         "conversation": {"key": "conversation", "type": "Conversation"},
+    }
+
+    def __init__(self, *, conversation: Optional["_models.Conversation"] = None, **kwargs: Any) -> None:
+        """
+        :keyword conversation:
+        :paramtype conversation: ~context_api.models.Conversation
+        """
+        super().__init__(**kwargs)
+        self.conversation = conversation
+
+
+class PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema(_serialization.Model):
+    """PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema.
+
+    :ivar conversation:
+    :vartype conversation: ~context_api.models.Conversation
+    """
+
+    _attribute_map = {
+        "conversation": {"key": "conversation", "type": "Conversation"},
     }
 
     def __init__(self, *, conversation: Optional["_models.Conversation"] = None, **kwargs: Any) -> None:
         """
         :keyword conversation:
         :paramtype conversation: ~context_api.models.Conversation
         """
```

### Comparing `context_python-0.2.1/getcontext/generated/models/_patch.py` & `context_python-0.3.0/getcontext/generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/getcontext/generated/operations/__init__.py` & `context_python-0.3.0/getcontext/generated/aio/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._operations import LogOperations
+from ._client import ContextAPI
 
-from ._patch import __all__ as _patch_all
-from ._patch import *  # pylint: disable=unused-wildcard-import
+try:
+    from ._patch import __all__ as _patch_all
+    from ._patch import *  # pylint: disable=unused-wildcard-import
+except ImportError:
+    _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "LogOperations",
+    "ContextAPI",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
+
 _patch_sdk()
```

### Comparing `context_python-0.2.1/getcontext/generated/operations/_operations.py` & `context_python-0.3.0/getcontext/generated/operations/_operations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.4.15)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.6.0)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -43,14 +43,30 @@
         _headers["Authorization"] = _SERIALIZER.header("authorization", authorization, "str")
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_log_conversation_upsert_request(*, authorization: Optional[str] = None, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/api/v1/log/conversation/upsert"
+
+    # Construct headers
+    if authorization is not None:
+        _headers["Authorization"] = _SERIALIZER.header("authorization", authorization, "str")
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 class LogOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~context_api.ContextAPI`'s
@@ -177,14 +193,145 @@
             authorization=authorization,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [201]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    def conversation_upsert(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Ingests or updates conversation.
+
+        Ingests or updates conversation.
+
+        :param body: Default value is None.
+        :type body:
+         ~context_api.models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def conversation_upsert(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[IO] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Ingests or updates conversation.
+
+        Ingests or updates conversation.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def conversation_upsert(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[
+            Union[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema, IO]
+        ] = None,
+        *,
+        authorization: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """Ingests or updates conversation.
+
+        Ingests or updates conversation.
+
+        :param body: Is either a
+         PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema type or a IO
+         type. Default value is None.
+        :type body:
+         ~context_api.models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
+         or IO
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(
+                    body, "PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema"
+                )
+            else:
+                _json = None
+
+        request = build_log_conversation_upsert_request(
+            authorization=authorization,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
```

### Comparing `context_python-0.2.1/getcontext/generated/operations/_patch.py` & `context_python-0.3.0/getcontext/generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.2.1/PKG-INFO` & `context_python-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context-python
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python SDK for the Context API
 License: LICENSE.md
 Keywords: context,api,sdk
 Author: Alex Gamble
 Author-email: alex@woolly.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```


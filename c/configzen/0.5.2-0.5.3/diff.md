# Comparing `tmp/configzen-0.5.2.tar.gz` & `tmp/configzen-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.5.2.tar", max compression
+gzip compressed data, was "configzen-0.5.3.tar", max compression
```

## Comparing `configzen-0.5.2.tar` & `configzen-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      536 2023-06-29 17:13:35.607166 configzen-0.5.2/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.5.2/configzen/__main__.py
--rw-r--r--   0        0        0     1437 2023-06-29 16:34:46.964275 configzen-0.5.2/configzen/_isolation.py
--rw-r--r--   0        0        0     3394 2023-06-29 17:46:07.418020 configzen-0.5.2/configzen/_setup.py
--rw-r--r--   0        0        0    77224 2023-06-29 17:47:37.718956 configzen-0.5.2/configzen/config.py
--rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.5.2/configzen/decorators.py
--rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.5.2/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.5.2/configzen/field.py
--rw-r--r--   0        0        0     5157 2023-06-29 17:56:51.047974 configzen-0.5.2/configzen/interpolation.py
--rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.5.2/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.5.2/configzen/py.typed
--rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.5.2/configzen/route.py
--rw-r--r--   0        0        0     1168 2023-06-29 16:34:46.955277 configzen-0.5.2/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.5.2/LICENSE
--rw-r--r--   0        0        0     1512 2023-06-29 18:20:33.891847 configzen-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    14350 2023-06-29 18:06:31.120725 configzen-0.5.2/README.md
--rw-r--r--   0        0        0    14908 1970-01-01 00:00:00.000000 configzen-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      536 2023-06-29 17:13:35.607166 configzen-0.5.3/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.5.3/configzen/__main__.py
+-rw-r--r--   0        0        0     1681 2023-07-03 13:55:18.269988 configzen-0.5.3/configzen/_isolation.py
+-rw-r--r--   0        0        0     3375 2023-07-01 12:22:23.319430 configzen-0.5.3/configzen/_setup.py
+-rw-r--r--   0        0        0    77584 2023-07-03 13:01:20.431667 configzen-0.5.3/configzen/config.py
+-rw-r--r--   0        0        0     5232 2023-07-03 13:00:51.582780 configzen-0.5.3/configzen/decorators.py
+-rw-r--r--   0        0        0     4434 2023-07-03 13:55:18.493989 configzen-0.5.3/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.5.3/configzen/field.py
+-rw-r--r--   0        0        0     6736 2023-07-03 13:00:51.893832 configzen-0.5.3/configzen/interpolation.py
+-rw-r--r--   0        0        0    26250 2023-07-03 13:16:45.908317 configzen-0.5.3/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.5.3/configzen/py.typed
+-rw-r--r--   0        0        0     4704 2023-07-03 13:21:43.983660 configzen-0.5.3/configzen/route.py
+-rw-r--r--   0        0        0     1197 2023-07-03 12:44:27.155689 configzen-0.5.3/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1474 2023-07-03 13:58:36.925138 configzen-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    14350 2023-06-29 18:06:31.120725 configzen-0.5.3/README.md
+-rw-r--r--   0        0        0    14870 1970-01-01 00:00:00.000000 configzen-0.5.3/PKG-INFO
```

### Comparing `configzen-0.5.2/configzen/__init__.py` & `configzen-0.5.3/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.2/configzen/__main__.py` & `configzen-0.5.3/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.2/configzen/_isolation.py` & `configzen-0.5.3/configzen/_isolation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 from __future__ import annotations
 
 import asyncio
-import collections.abc
 import contextvars
+import functools
+from collections.abc import Callable, Coroutine
 from typing import Any, cast
 
 from configzen.typedefs import P, T
 
 
-def isolate_calls(
-    func: collections.abc.Callable[P, T],
-) -> collections.abc.Callable[P, T]:
+def isolation_runner(
+    func: Callable[P, T],
+) -> Callable[P, T]:
     """
     Decorator to copy a function call context automatically (context isolation)
     to prevent collisions.
 
     This decorator will copy the current context and run the function
     in this new isolated context.
     """
     if isinstance(func, (classmethod, staticmethod)):
-        return type(func)(isolate_calls(func.__func__))
+        return type(func)(isolation_runner(func.__func__))
 
     if asyncio.iscoroutinefunction(func):
-        return cast(
-            collections.abc.Callable[P, T],
-            lambda *args, **kwargs: isolate_async(func, *args, **kwargs),
-        )
-    return lambda *args, **kwargs: isolate(func, *args, **kwargs)
 
+        @functools.wraps(func)
+        def _isolating_async_wrapper(*args: Any, **kwargs: Any) -> asyncio.Task[T]:
+            return isolate_await(
+                cast(Callable[P, Coroutine[Any, Any, T]], func), *args, **kwargs
+            )
 
-def isolate(
-    func: collections.abc.Callable[..., T],
+        return cast(Callable[P, T], _isolating_async_wrapper)
+
+    @functools.wraps(func)
+    def _isolating_wrapper(*args: Any, **kwargs: Any) -> T:
+        return isolate_run(func, *args, **kwargs)
+
+    return _isolating_wrapper
+
+
+def isolate_run(
+    func: Callable[..., T],
     *args: Any,
     **kwargs: Any,
 ) -> T:
     """Utility for running a function in an isolated context."""
     context = contextvars.copy_context()
     return context.run(func, *args, **kwargs)
 
 
-def isolate_async(
-    func: collections.abc.Callable[..., collections.abc.Coroutine[Any, Any, T]],
+def isolate_await(
+    func: Callable[..., Coroutine[Any, Any, T]],
     *args: Any,
     **kwargs: Any,
 ) -> asyncio.Task[T]:
     """Utility for awaiting a coroutine in an isolated context."""
     return asyncio.create_task(func(*args, **kwargs))
```

### Comparing `configzen-0.5.2/configzen/_setup.py` & `configzen-0.5.3/configzen/_setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 For advanced use cases, you can prevent this module from executing
 by setting the environment variable ``CONFIGZEN_SETUP`` to ``0``.
 """
 
 from __future__ import annotations
 
 import ast
-import collections.abc
 import ipaddress
 import pathlib
+from collections.abc import Mapping
 from typing import TYPE_CHECKING, Any
 
 from pydantic.json import ENCODERS_BY_TYPE
 
 from configzen.config import ConfigModel, export_hook, field_hook
 
 if TYPE_CHECKING:
@@ -43,16 +43,16 @@
 
 
 @export_hook.register(list)
 def _export_list(obj: list[Any]) -> list[Any]:
     return [export_hook(item) for item in obj]
 
 
-@export_hook.register(collections.abc.Mapping)
-def _export_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
+@export_hook.register(Mapping)
+def _export_mapping(obj: Mapping[Any, Any]) -> dict[Any, Any]:
     return {k: export_hook(v) for k, v in obj.items()}
 
 
 @field_hook.register(dict)
 @field_hook.register(list)
 def _eval_literals(cls: type[Any], value: Any) -> Any:
     """
```

### Comparing `configzen-0.5.2/configzen/config.py` & `configzen-0.5.3/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,25 +55,29 @@
     # 5432
 """
 
 from __future__ import annotations
 
 import abc
 import asyncio
-import collections.abc
 import contextvars
 import copy
 import dataclasses
 import functools
 import importlib
 import io
 import os
 import pathlib
 import urllib.parse
 import urllib.request
+from collections.abc import (
+    Callable,
+    Mapping,
+    Iterator,
+)
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
     Literal,
     Optional,
@@ -87,26 +91,29 @@
 import pydantic
 from anyconfig.utils import filter_options, is_dict_like, is_list_like
 from pydantic.fields import make_generic_validator  # type: ignore[attr-defined]
 from pydantic.fields import ModelField, Undefined
 from pydantic.main import BaseModel, ModelMetaclass
 from pydantic.utils import ROOT_KEY
 
-from configzen._isolation import isolate, isolate_async, isolate_calls
+from configzen._isolation import isolate_run, isolate_await, isolation_runner
 from configzen.errors import (
     ConfigAccessError,
     ResourceLookupError,
     UnavailableParserError,
     UnspecifiedParserError,
+    InterpolationLookupError,
 )
 from configzen.interpolation import (
     INTERPOLATION_NAMESPACE_TOKEN,
+    INTERPOLATOR,
     include_const,
     interpolate,
     include,
+    BaseInterpolator,
 )
 from configzen.processor import EXPORT, DirectiveContext, Processor
 from configzen.route import ConfigRoute
 from configzen.typedefs import (
     AsyncConfigIO,
     ConfigIO,
     ConfigModelT,
@@ -219,24 +226,22 @@
     class _FieldHookType:
         def __call__(self, cls: type[T], value: Any) -> Any:
             ...
 
         def register(
             self,
             cls: type[T],
-            func: collections.abc.Callable[[type[T], Any], Any] | None = None,
-        ) -> collections.abc.Callable[
-            [collections.abc.Callable[[type[T], Any], Any]],
-            collections.abc.Callable[[type[T] | Any, Any], Any],
+            func: Callable[[type[T], Any], Any] | None = None,
+        ) -> Callable[
+            [Callable[[type[T], Any], Any]],
+            Callable[[type[T] | Any, Any], Any],
         ]:
             ...
 
-        def dispatch(
-            self, cls: type[T]
-        ) -> collections.abc.Callable[[type[T] | Any, Any], Any]:
+        def dispatch(self, cls: type[T]) -> Callable[[type[T] | Any, Any], Any]:
             ...
 
     field_hook: _FieldHookType = _FieldHookType()
 
 else:
 
     def field_hook(cls: type[Any], value: Any) -> Any:
@@ -660,15 +665,15 @@
         kwargs = self.load_options | kwargs
         try:
             loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
                 blob, ac_parser=parser_name, **kwargs
             )
         except anyconfig.UnknownParserTypeError as exc:
             raise UnavailableParserError(str(exc).split()[-1], self) from exc
-        if not isinstance(loaded, collections.abc.Mapping):
+        if not isinstance(loaded, Mapping):
             msg = (
                 f"Expected a mapping as a result of loading {self.resource}, "
                 f"got {type(loaded).__name__}."
             )
             raise TypeError(msg)
         return dict(loaded)
 
@@ -760,15 +765,15 @@
             parser_name = self.parser_name
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if parser_name == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
             )
             _exporting.set(True)  # noqa: FBT003
-            return isolate(config.json, **export_kwargs)
+            return isolate_run(config.json, **export_kwargs)
         data = export_model(config, **export_kwargs)
         return self.dump_data(data, parser_name=parser_name, **kwargs)
 
     async def dump_config_async(
         self,
         config: ConfigModelT,
         parser_name: str | None = None,
@@ -794,15 +799,15 @@
             parser_name = self.parser_name
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if parser_name == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
             )
             _exporting.set(True)  # noqa: FBT003
-            return await isolate_async(config.json_async, **export_kwargs)
+            return await isolate_await(config.json_async, **export_kwargs)
         data = await export_model_async(config, **export_kwargs)
         return self.dump_data(data, parser_name=parser_name, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
         parser_name: str | None = None,
@@ -1167,15 +1172,15 @@
         resource = self.resource
         return f"{type(self).__name__}({resource=!r})"
 
 
 def at(
     mapping: Any,
     route: ConfigRouteLike,
-    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _get_object_state,
+    converter_func: Callable[[Any], dict[str, Any]] = _get_object_state,
     agent: ConfigAgent[ConfigModelT] | None = None,
 ) -> Any:
     """
     Get an item at a route.
 
     Parameters
     ----------
@@ -1433,15 +1438,15 @@
 
     """
 
     initial_state: dict[str, Any]
     interpolation_namespace: dict[str, Any]
 
     @abc.abstractmethod
-    def trace_route(self) -> collections.abc.Iterator[str]:
+    def trace_route(self) -> Iterator[str]:
         """Trace the route to where the configuration subcontext points to."""
 
     @property
     def route(self) -> ConfigRoute:
         """The route to where the configuration subcontext points to."""
         return ConfigRoute(list(self.trace_route()))
 
@@ -1521,15 +1526,15 @@
     ) -> None:
         self._initial_state = {}
         self._owner = None
         self._agent = agent
         self.interpolation_namespace = {}
         self.owner = owner
 
-    def trace_route(self) -> collections.abc.Iterator[str]:
+    def trace_route(self) -> Iterator[str]:
         yield from ()
 
     @property
     def agent(self) -> ConfigAgent[ConfigModelT]:
         return self._agent
 
     @property
@@ -1595,15 +1600,15 @@
     def agent(self) -> ConfigAgent[ConfigModelT]:
         return self._parent.agent
 
     @property
     def toplevel_interpolation_namespace(self) -> dict[str, Any]:
         return self._parent.toplevel_interpolation_namespace
 
-    def trace_route(self) -> collections.abc.Iterator[str]:
+    def trace_route(self) -> Iterator[str]:
         yield from self._parent.trace_route()
         yield self._part
 
     @property
     def at(self) -> ConfigAt[ConfigModelT]:
         if self.owner is None:
             msg = "Cannot get at() of a model without parent model"
@@ -1696,27 +1701,33 @@
     if not isinstance(disallow_interpolation, bool):
         disallowed_interpolation_fields = set(disallow_interpolation)
     if (
         field.field_info.extra.get("interpolate", True)
         and field.alias not in disallowed_interpolation_fields
     ):
         old_value = post_hook_value
-        new_value = field_hook(
-            field.outer_type_,
-            interpolate(post_hook_value, cls, values.copy())
-        )
+        try:
+            interpolated = interpolate(
+                post_hook_value,
+                cls,
+                values.copy(),
+                field.outer_type_,
+            )
+        except InterpolationLookupError as err:
+            err.message += f" (issued by {cls.__qualname__}.{field.alias})"
+            raise
+
+        new_value = field_hook(field.outer_type_, interpolated)
         if old_value != new_value:
             interpolation_tracker[field.alias] = (old_value, copy.copy(new_value))
         post_hook_value = new_value
     return post_hook_value
 
 
-def _json_encoder(
-    model_encoder: collections.abc.Callable[..., Any], value: Any, **kwargs: Any
-) -> Any:
+def _json_encoder(model_encoder: Callable[..., Any], value: Any, **kwargs: Any) -> Any:
     initial_state_type = type(value)
     converted_value = export_hook(value)
     if isinstance(converted_value, initial_state_type):
         return model_encoder(value, **kwargs)
     return converted_value
 
 
@@ -1731,14 +1742,17 @@
         namespace |= dict.fromkeys(
             (EXPORT, CONTEXT, LOCAL, TOKEN), pydantic.PrivateAttr()
         ) | {INTERPOLATION_TRACKER: pydantic.PrivateAttr(default_factory=dict)}
 
         if namespace.get(INTERPOLATION_INCLUSIONS) is None:
             namespace[INTERPOLATION_INCLUSIONS] = {}
 
+        if namespace.get(INTERPOLATOR) is None:
+            namespace[INTERPOLATOR] = BaseInterpolator()
+
         if kwargs.pop("root", None):
             return type.__new__(cls, name, bases, namespace, **kwargs)
 
         model = super().__new__(cls, name, bases, namespace, **kwargs)
         for field in model.__fields__.values():
             if field.pre_validators is None:
                 field.pre_validators = []
@@ -1846,53 +1860,52 @@
         Export the configuration model.
 
         Returns
         -------
         The exported configuration model.
         """
         _exporting.set(True)  # noqa: FBT003
-        return isolate(self.dict, **kwargs)
+        return isolate_run(self.dict, **kwargs)
 
     async def export_async(self, **kwargs: Any) -> dict[str, Any]:
         """
         Export the configuration model.
 
         Returns
         -------
         The exported configuration model.
         """
         _exporting.set(True)  # noqa: FBT003
-        return await isolate_async(self.dict_async, **kwargs)
+        return await isolate_await(self.dict_async, **kwargs)
 
     async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
         """
         Get the dictionary representation of the configuration model.
 
         Returns
         -------
         The dictionary representation of the configuration model.
         """
         return dict(await self._iter_async(to_dict=True, **kwargs))
 
+    # noinspection PyShadowingNames
     async def json_async(  # noqa: PLR0913
         self,
         include: IncludeExcludeT = None,
         exclude: IncludeExcludeT = None,
         *,
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
-        encoder: collections.abc.Callable[[Any], Any] | None = None,
+        encoder: Callable[[Any], Any] | None = None,
         models_as_dict: bool = True,
         **dumps_kwargs: Any,
     ) -> str:
-        encoder = cast(
-            collections.abc.Callable[[Any], Any], encoder or self.__json_encoder__
-        )
+        encoder = cast(Callable[[Any], Any], encoder or self.__json_encoder__)
         data = dict(
             await self._iter_async(
                 to_dict=models_as_dict,
                 by_alias=by_alias,
                 include=include,
                 exclude=exclude,
                 exclude_unset=exclude_unset,
@@ -1902,60 +1915,59 @@
         )
         if self.__custom_root_type__:
             data = data[ROOT_KEY]
         return self.__config__.json_dumps(data, default=encoder, **dumps_kwargs)
 
     def _iter(  # type: ignore[override]
         self, **kwargs: Any
-    ) -> collections.abc.Iterator[tuple[str, Any]]:
+    ) -> Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
             state: dict[str, Any] = {}
             for key, value in super()._iter(**kwargs):
-                state |= [self._iter_hook(key, value)]
+                state |= [self._export_iter_hook(key, value)]
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 context.agent.processor_class.export(state, metadata=metadata)
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
-    async def _iter_async(
-        self, **kwargs: Any
-    ) -> collections.abc.Iterator[tuple[str, Any]]:
+    async def _iter_async(self, **kwargs: Any) -> Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
             state: dict[str, Any] = {}
             for key, value in super()._iter(**kwargs):
-                state |= [self._iter_hook(key, value)]
+                state |= [self._export_iter_hook(key, value)]
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 await context.agent.processor_class.export_async(
                     state, metadata=metadata
                 )
             return ((key, value) for key, value in state.items())
         return super()._iter(**kwargs)
 
-    def _iter_hook(
+    def _export_iter_hook(
         self,
         key: str,
         value: Any,
     ) -> tuple[str, Any]:
         interpolation_tracker = getattr(self, LOCAL).get(current_interpolation_tracker)
         field = self.__fields__.get(key)
         actual_key = field.alias if field else key
-        interpolation_track = interpolation_tracker.get(actual_key)
-        if interpolation_track:
-            old_value, new_value = interpolation_track
-            # if value != new_value:
-            #     raise InterpolationError(
-            #         f"Cannot restore the value of {actual_key!r} "
-            #         "before interpolation."
-            #     )
-            value = old_value
+        if interpolation_tracker:
+            interpolation_track = interpolation_tracker.get(actual_key)
+            if interpolation_track:
+                old_value, new_value = interpolation_track
+                # if value != new_value:
+                #     raise InterpolationError(
+                #         f"Cannot restore the value of {actual_key!r} "
+                #         "before interpolation."
+                #     )
+                value = old_value
         return actual_key, value
 
     @classmethod
     @no_type_check
     def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
         if _exporting.get():
             exporter = export_model.dispatch(type(value))
@@ -2249,18 +2261,18 @@
         local = contextvars.copy_context()
         if getattr(
             cls.__config__,
             "autoupdate_forward_refs",
             ConfigMeta.autoupdate_forward_refs,
         ):
             cls.update_forward_refs()
-        task = local.run(
+        reader = local.run(
             asyncio.create_task, agent.read_async(config_class=cls, **kwargs)
         )
-        config = await task
+        config = await reader
         object.__setattr__(config, LOCAL, local)
         context = cast(Context[ConfigModelT], local.get(current_context))
         context.owner = config
         return config
 
     async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
@@ -2350,18 +2362,16 @@
         }
 
     @classmethod
     def get_interpolation_namespace(
         cls,
         identifiers: set[str],
         closest_namespace: dict[str, Any],
-    ) -> tuple[Any, dict[str, Any]]:
-        """
-        Get the interpolation context of this configuration model.
-        """
+    ) -> dict[str, Any]:
+        """Get the interpolation namespace according to requested identifiers."""
         context = current_context.get()
         interpolation_context = {}
 
         namespaces = cls._evaluate_interpolation_namespaces()
         if context is not None:
             namespaces.setdefault(None, {}).update(
                 context.toplevel_interpolation_namespace
@@ -2370,31 +2380,32 @@
             (
                 namespace_identifier,
                 specifies_namespace,
                 raw_identifier,
             ) = identifier.rpartition(INTERPOLATION_NAMESPACE_TOKEN)
             namespace = namespaces.get(None, {})
             if specifies_namespace:
-                namespace |= namespaces[namespace_identifier]
+                try:
+                    namespace |= namespaces[namespace_identifier]
+                except KeyError:
+                    raise InterpolationLookupError(namespace_identifier) from None
             else:
                 namespace |= closest_namespace
 
             try:
                 value = at(namespace, raw_identifier)
             except ResourceLookupError:
                 if not specifies_namespace:
                     raise
                 value = at(closest_namespace, raw_identifier)
             interpolation_context[identifier] = value
             if raw_identifier not in closest_namespace:
                 interpolation_context[raw_identifier] = value
 
-        if len(identifiers) == 1:
-            return interpolation_context[identifiers.pop()], interpolation_context
-        return None, interpolation_context
+        return interpolation_context
 
     @classmethod
     def __field_setup__(cls, value: dict[str, Any], field: ModelField) -> Any:
         """
         Called when this configuration model is being initialized as a field
         of some other configuration model.
         """
@@ -2405,22 +2416,22 @@
             return _get_object_state(value) | {
                 TOKEN: tok,
                 LOCAL: contextvars.copy_context(),
             }
         return value
 
     if not TYPE_CHECKING:
-        load = isolate_calls(load)
-        load_async = isolate_calls(load_async)
-        reload = isolate_calls(reload)
-        reload_async = isolate_calls(reload_async)
-        save = isolate_calls(save)
-        save_async = isolate_calls(save_async)
-        export = isolate_calls(export)
-        export_async = isolate_calls(export_async)
+        load = isolation_runner(load)
+        load_async = isolation_runner(load_async)
+        reload = isolation_runner(reload)
+        reload_async = isolation_runner(reload_async)
+        save = isolation_runner(save)
+        save_async = isolation_runner(save_async)
+        export = isolation_runner(export)
+        export_async = isolation_runner(export_async)
 
 
 setattr(ConfigModel, INTERPOLATION_INCLUSIONS, None)
 include.register(ConfigModel, include_const)
 
 if os.getenv("CONFIGZEN_SETUP") != "0":
     importlib.import_module("._setup", package=__package__)
```

### Comparing `configzen-0.5.2/configzen/decorators.py` & `configzen-0.5.3/configzen/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 from __future__ import annotations
 
-import collections.abc
 import contextlib
 import functools
-from typing import TYPE_CHECKING, Any, cast
+from collections.abc import Callable, Iterator, Coroutine
+from typing import TYPE_CHECKING, Any, cast, overload
 
 from configzen.config import export_hook, export_model, export_model_async, field_hook
 
 if TYPE_CHECKING:
     from configzen.typedefs import ConfigModelT, T
 
 __all__ = (
     "with_exporter",
     "with_async_exporter",
     "with_field_hook",
     "with_export_hook",
 )
 
 
+@overload
 def with_export_hook(
-    func: collections.abc.Callable[[T], Any], cls: type[T] | None = None
-) -> type[T] | Any:
+    func: Callable[[T], Any],
+    cls: None = None,
+) -> functools.partial[type[T]]:
+    ...
+
+
+@overload
+def with_export_hook(
+    func: Callable[[T], Any],
+    cls: type[T],
+) -> type[T]:
+    ...
+
+
+def with_export_hook(
+    func: Callable[[T], Any], cls: type[T] | None = None
+) -> type[T] | functools.partial[type[T]]:
     """
     Register a pre-serialization converter function for a type.
 
     Parameters
     ----------
     func
         The converter function.
@@ -49,29 +65,43 @@
     if cls is None:
         return functools.partial(with_export_hook, func)
 
     export_hook.register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
 
-        def validator_gen() -> (
-            collections.abc.Iterator[collections.abc.Callable[[Any], Any]]
-        ):
+        def validator_gen() -> Iterator[Callable[[Any], Any]]:
             hook_func = field_hook.dispatch(cls)  # type: ignore[arg-type]
             yield lambda value: hook_func(cls, value)
 
         with contextlib.suppress(TypeError):
             cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
     return cls
 
 
+@overload
+def with_field_hook(
+    func: Callable[[type[T], Any], T],
+    cls: type[T],
+) -> type[T]:
+    ...
+
+
+@overload
+def with_field_hook(
+    func: Callable[[type[T], Any], T],
+    cls: None = None,
+) -> functools.partial[type[T]]:
+    ...
+
+
 def with_field_hook(
-    func: collections.abc.Callable[[type[T], Any], T], cls: type[T] | None = None
-) -> type[T] | Any:
+    func: Callable[[type[T], Any], T], cls: type[T] | None = None
+) -> type[T] | functools.partial[type[T]]:
     """
     Register a field hook for a type.
 
     Parameters
     ----------
     func
         The loader function.
@@ -87,15 +117,15 @@
         return functools.partial(with_field_hook, func)
 
     field_hook.register(cls, func)
     return cls
 
 
 def with_exporter(
-    func: collections.abc.Callable[[ConfigModelT], dict[str, Any]] | None = None,
+    func: Callable[[ConfigModelT], Any] | None = None,
     cls: type[ConfigModelT] | None = None,
     **predefined_kwargs: Any,
 ) -> type[ConfigModelT] | Any:
     """
     Register a custom exporter for a configuration model class.
 
     Parameters
@@ -131,27 +161,24 @@
     else:
         export_model.register(cls, func)
         if export_model_async.dispatch(cls) is export_model_async:
 
             async def default_async_func(obj: Any, **kwargs: Any) -> Any:
                 nonlocal func
                 if TYPE_CHECKING:
-                    func = cast(collections.abc.Callable[..., dict[str, Any]], func)
+                    func = cast(Callable[..., dict[str, Any]], func)
 
                 return func(obj, **kwargs)
 
             export_model_async.register(cls, default_async_func)
     return cls
 
 
 def with_async_exporter(
-    func: collections.abc.Callable[
-        [ConfigModelT], collections.abc.Coroutine[Any, Any, dict[str, Any]]
-    ]
-    | None = None,
+    func: Callable[[ConfigModelT], Coroutine[Any, Any, Any]] | None = None,
     cls: type[ConfigModelT] | None = None,
     **predefined_kwargs: Any,
 ) -> type[ConfigModelT] | Any:
     """
     Register a custom exporter for a configuration model class.
 
     Parameters
```

### Comparing `configzen-0.5.2/configzen/errors.py` & `configzen-0.5.3/configzen/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,89 @@
 """This module contains all the custom errors raised by _configzen_."""
 
 from __future__ import annotations
 
-import collections.abc
 import contextlib
+from collections.abc import Iterator
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from configzen.config import ConfigAgent
     from configzen.typedefs import ConfigModelT
 
 
 class ConfigError(Exception):
     """An error occurred while loading a configuration."""
 
+    def __init__(self, message: str) -> None:
+        self._message = message
+        super().__init__(message)
+
+    @property
+    def message(self) -> str:
+        """The error message."""
+        return self._message
+
+    @message.setter
+    def message(self, value: str) -> None:
+        self._message = value
+        super().__init__(self.message)
+
 
 class InterpolationError(ConfigError):
     """An error occurred with regard to interpolating a configuration."""
 
 
+class InterpolationLookupError(ConfigError, LookupError):
+    """An error occurred with regard to interpolating a configuration."""
+
+    def __init__(self, message: str) -> None:
+        super().__init__(repr(message))
+
+
 class IncorrectConfigError(ConfigError):
     """An error occurred while loading a configuration."""
 
 
 class InternalSyntaxError(ConfigError):
-    """Error in route syntax."""
+    """Syntax error in a _configzen_ component."""
 
     def __init__(
         self,
-        msg: str,
+        message: str,
         index: Any = None,
         prefix: str = "",
         suffix: str = "",
     ) -> None:
-        super().__init__(msg)
+        super().__init__(message)
         self.index = index
         self.prefix = prefix
         self.suffix = suffix
 
 
 class ConfigSyntaxError(ConfigError):
     """An error occurred while parsing arguments."""
 
 
 @contextlib.contextmanager
-def formatted_syntax_error(source: str) -> collections.abc.Iterator[None]:
+def formatted_syntax_error(
+    source: str, error_cls: type[ConfigSyntaxError] = ConfigSyntaxError
+) -> Iterator[None]:
     """Raise a SyntaxError with a message and a source."""
     try:
         yield
     except InternalSyntaxError as exc:
         idx = len(exc.prefix) + exc.index + 1
         charlist = [" "] * len(exc.prefix + repr(source) + exc.suffix)
         charlist[idx] = "^"
         indicator = "".join(charlist)
         msg = "\n".join(
             map(str, (exc, exc.prefix + repr(source) + exc.suffix, indicator))
         )
-        raise ConfigSyntaxError(msg) from None
+        raise error_cls(msg) from None
 
 
 class UnspecifiedParserError(ConfigError):
     """Could not determine the parser to use."""
 
 
 class UnavailableParserError(ConfigError):
@@ -89,15 +112,15 @@
     """An error occurred while accessing configuration part."""
 
     def __init__(self, config: ConfigModelT, route: str | list[str]) -> None:
         if not isinstance(route, str):
             route = ".".join(route)
         self.route = route
         super().__init__(
-            f"could not get {type(config).__name__}.{route}",
+            f"Could not access {type(config).__name__}.{route}",
         )
 
 
 class ConfigProcessorError(ConfigError):
     """An error occurred while preprocessing/exporting a configuration."""
```

### Comparing `configzen-0.5.2/configzen/field.py` & `configzen-0.5.3/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.2/configzen/interpolation.py` & `configzen-0.5.3/configzen/interpolation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
-import collections.abc
 import functools
 import importlib
 import inspect
 import re
 import string
 import sys
+from collections.abc import Callable
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from configzen.typedefs import ConfigModelT
 
 __all__ = (
     "interpolate",
     "include",
 )
 
+INTERPOLATOR: str = "__interpolator__"
 INTERPOLATION_NAMESPACE_TOKEN: str = "::"
 
 
 class ConfigInterpolationTemplate(string.Template):
     idpattern = rf"([_a-z]*({INTERPOLATION_NAMESPACE_TOKEN})?[_a-z][\\\.\[\]_a-z0-9]*)"
     flags = re.IGNORECASE
 
@@ -44,39 +45,94 @@
                         "Unrecognized named group in pattern", self.pattern
                     )
             return ids
 
 
 @functools.singledispatch
 def interpolate(
-    value: Any, _cls: type[ConfigModelT], _closest_ns: dict[str, Any]
+    value: Any,
+    _cls: type[ConfigModelT],
+    _closest_ns: dict[str, Any],
+    _target_type: type[Any],
 ) -> Any:
     return value
 
 
 @interpolate.register(str)
-def _interpolate_str(
-    value: str, cls: type[ConfigModelT], closest_namespace: dict[str, Any]
-) -> str:
+def _try_interpolate_str(
+    value: str,
+    cls: type[ConfigModelT],
+    closest_namespace: dict[str, Any],
+    target_type: type[Any],
+) -> Any:
     template = ConfigInterpolationTemplate(value)
-    value, namespace = cls.get_interpolation_namespace(
-        identifiers=set(template.get_identifiers()), closest_namespace=closest_namespace
+    identifiers = set(template.get_identifiers())
+    if not identifiers:
+        return value
+
+    namespace = cls.get_interpolation_namespace(
+        identifiers=identifiers, closest_namespace=closest_namespace
+    )
+    interpolator: BaseInterpolator = getattr(cls, INTERPOLATOR)
+
+    if len(identifiers) == 1:
+        identifier = identifiers.pop()
+        value = namespace[identifier]
+        return interpolator.interpolate_one(
+            template=template,
+            identifier=identifier,
+            value=value,
+            target_type=target_type,
+        )
+
+    return interpolator.interpolate_many(
+        template=template, namespace=namespace, target_type=target_type
     )
-    if value is None:
+
+
+class BaseInterpolator:
+    def interpolate_many(
+        self,
+        template: ConfigInterpolationTemplate,
+        namespace: dict[str, Any],
+        target_type: type[Any],
+    ) -> Any:
+        bulk_render = self.bulk_renderers.dispatch(target_type)
+        return bulk_render(self, template, namespace)
+
+    # noinspection PyMethodMayBeStatic
+    def bulk_render_any(
+        self, template: ConfigInterpolationTemplate, namespace: dict[str, Any]
+    ) -> Any:
         return template.safe_substitute(namespace)
-    return value
 
+    def interpolate_one(
+        self,
+        template: ConfigInterpolationTemplate,
+        identifier: str,
+        value: Any,
+        target_type: type[Any],
+    ) -> Any:
+        render = self.single_renderers.dispatch(target_type)
+        return render(self, template, identifier, value)
+
+    # noinspection PyMethodMayBeStatic
+    def single_render_any(
+        self, _template: ConfigInterpolationTemplate, _identifier: str, value: Any
+    ) -> Any:
+        return value
 
-# todo(bswck): Interpolation for compound types. Quite non-trivial.
+    bulk_renderers = functools.singledispatch(bulk_render_any)
+    single_renderers = functools.singledispatch(single_render_any)
 
 
 def _include_wrapper(
     cls: type[ConfigModelT],
     namespace_name: str | None,
-    namespace_factory: collections.abc.Callable[[], dict[str, Any]],
+    namespace_factory: Callable[[], dict[str, Any]],
 ) -> type[ConfigModelT]:
     from configzen.config import INTERPOLATION_INCLUSIONS
 
     getattr(cls, INTERPOLATION_INCLUSIONS)[namespace_name] = namespace_factory
     return cls
 
 
@@ -84,59 +140,56 @@
 @functools.singledispatch
 def include(
     namespace: Any,
     /,
     *,
     name: str | None = None,  # noqa: ARG001
     **kwargs: Any,  # noqa: ARG001
-) -> collections.abc.Callable[[type[ConfigModelT]], type[ConfigModelT]]:
+) -> Callable[[type[ConfigModelT]], type[ConfigModelT]]:
     raise TypeError(
         f"Cannot include {namespace} (unexpected type {type(namespace).__name__})"
     )
 
 
 @include.register(dict)
 def include_const(
-    namespace: dict[str, Any] | ConfigModelT,
-    /,
-    *,
-    name: str | None = None
-) -> collections.abc.Callable[[type[ConfigModelT]], type[ConfigModelT]]:
+    namespace: dict[str, Any] | ConfigModelT, /, *, name: str | None = None
+) -> Callable[[type[ConfigModelT]], type[ConfigModelT]]:
     from configzen import ConfigModel
 
     if isinstance(namespace, ConfigModel):
         return lambda cls: _include_wrapper(
             cls, name, lambda: namespace.dict()  # type: ignore
         )
     return lambda cls: _include_wrapper(cls, name, lambda: namespace)  # type: ignore
 
 
 def _include_factory(
-    namespace_factory: collections.abc.Callable[[], dict[str, Any]],
+    namespace_factory: Callable[[], dict[str, Any]],
     /,
     *,
     name: str | None = None,
-) -> collections.abc.Callable[[type[ConfigModelT]], type[ConfigModelT]]:
+) -> Callable[[type[ConfigModelT]], type[ConfigModelT]]:
     return lambda cls: _include_wrapper(cls, name, namespace_factory)
 
 
 if not TYPE_CHECKING:
-    include.register(collections.abc.Callable, _include_factory)
+    include.register(Callable, _include_factory)
 
 
 @include.register(str)
 def _include_str(
     namespace: str,
     /,
     *,
     name: str | None = None,
     stack_offset: int = 2,
     module: str | None = None,
     isolate_from_toplevel: bool = True,
-) -> collections.abc.Callable[[type[ConfigModelT]], type[ConfigModelT]]:
+) -> Callable[[type[ConfigModelT]], type[ConfigModelT]]:
     if module is None:
         callers_globals = inspect.stack()[stack_offset].frame.f_globals
     else:
         callers_globals = None
 
     if isolate_from_toplevel and name is None:
         name = namespace
```

### Comparing `configzen-0.5.2/configzen/processor.py` & `configzen-0.5.3/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.5.2/configzen/route.py` & `configzen-0.5.3/configzen/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-import collections.abc
 import functools
+from collections.abc import Iterator
 from typing import TYPE_CHECKING, Any, ClassVar
 
 from configzen.errors import InternalSyntaxError, formatted_syntax_error
 
 if TYPE_CHECKING:
     from configzen.typedefs import ConfigRouteLike
 
@@ -41,15 +41,15 @@
         tok_escape = cls.TOK_ESCAPE
         tok_dle_enter = cls.TOK_DOTLISTESC_ENTER
         tok_dle_exit = cls.TOK_DOTLISTESC_EXIT
 
         route = route.removesuffix(tok_dot) + tok_dot
 
         part = ""
-        dle_ctx = None
+        dle_ctx: int | None = None
         items: list[str] = []
         enter = items.append
         error = functools.partial(InternalSyntaxError, prefix="Route(", suffix=")")
         escape = False
 
         for index, char in enumerate(route):
             if escape:
@@ -125,12 +125,12 @@
         if isinstance(other, list):
             return self.items == other
         return NotImplemented
 
     def __str__(self) -> str:
         return self.compose()
 
-    def __iter__(self) -> collections.abc.Iterator[str]:
+    def __iter__(self) -> Iterator[str]:
         yield from self.items
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.items})"
```

### Comparing `configzen-0.5.2/configzen/typedefs.py` & `configzen-0.5.3/configzen/typedefs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import collections.abc
 import contextlib
 import os
 import pathlib
 import sys
+from collections.abc import Mapping, Set
 from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
 
 if sys.version_info >= (3, 10):
     from typing import ParamSpec, TypeAlias
 else:
     from typing_extensions import ParamSpec, TypeAlias
 
 if TYPE_CHECKING:
     from aiofiles.base import AiofilesContextManager
     from aiofiles.threadpool.text import AsyncTextIOWrapper
 
+    # noinspection PyUnresolvedReferences
     from configzen.config import ConfigModel
     from configzen.route import ConfigRoute
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
@@ -25,11 +26,11 @@
 
 ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
 AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
 RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
 NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
 IncludeExcludeT: TypeAlias = Optional[
     Union[
-        collections.abc.Set[Union[int, str]],
-        collections.abc.Mapping[Union[int, str], Any],
+        Set[Union[int, str]],
+        Mapping[Union[int, str], Any],
     ]
 ]
```

### Comparing `configzen-0.5.2/LICENSE` & `configzen-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.5.2/pyproject.toml` & `configzen-0.5.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "configzen"
-version = "0.5.2"
-description = "Easily create and maintain complex, statically-typed configurations with validation in Python."
+version = "0.5.3"
+description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.10.7"
+pydantic = "^1.10.10"
 anyconfig = "^0.13.0"
 typing-extensions = { version = "^4.5.0", python = ">=3.9,<3.11" }
 aiofiles = { version = "^23.1.0" }
 pyyaml = { version = "^6.0" }
 toml = { version = "^0.10.2" }
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `configzen-0.5.2/README.md` & `configzen-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.5.2/PKG-INFO` & `configzen-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.5.2
-Summary: Easily create and maintain complex, statically-typed configurations with validation in Python.
+Version: 0.5.3
+Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: anyconfig (>=0.13.0,<0.14.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.10.10,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version >= "3.9" and python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # configzen
```


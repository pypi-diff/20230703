# Comparing `tmp/archytas-1.0.2.tar.gz` & `tmp/archytas-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-1.0.2.tar", max compression
+gzip compressed data, was "archytas-1.0.3.tar", max compression
```

## Comparing `archytas-1.0.2.tar` & `archytas-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32472 2023-06-29 16:09:47.604117 archytas-1.0.2/LICENSE
--rw-r--r--   0        0        0     2088 2023-06-29 16:09:47.604117 archytas-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/__init__.py
--rw-r--r--   0        0        0     9054 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/agent.py
--rw-r--r--   0        0        0     9746 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/demo_tools.py
--rw-r--r--   0        0        0     4129 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/prompt.py
--rw-r--r--   0        0        0     3166 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/python.py
--rw-r--r--   0        0        0     8513 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/react.py
--rw-r--r--   0        0        0     1462 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/repl.py
--rw-r--r--   0        0        0    18506 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/tool_utils.py
--rw-r--r--   0        0        0     4586 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/tools.py
--rw-r--r--   0        0        0     1251 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/utils.py
--rw-r--r--   0        0        0      780 2023-06-29 16:09:47.644118 archytas-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-07-03 20:08:15.596669 archytas-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2088 2023-07-03 20:08:15.596669 archytas-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 20:08:15.596669 archytas-1.0.3/archytas/__init__.py
+-rw-r--r--   0        0        0     9054 2023-07-03 20:08:15.596669 archytas-1.0.3/archytas/agent.py
+-rw-r--r--   0        0        0     9746 2023-07-03 20:08:15.596669 archytas-1.0.3/archytas/demo_tools.py
+-rw-r--r--   0        0        0     4129 2023-07-03 20:08:15.596669 archytas-1.0.3/archytas/prompt.py
+-rw-r--r--   0        0        0     3166 2023-07-03 20:08:15.596669 archytas-1.0.3/archytas/python.py
+-rw-r--r--   0        0        0     8873 2023-07-03 20:08:15.596669 archytas-1.0.3/archytas/react.py
+-rw-r--r--   0        0        0     1462 2023-07-03 20:08:15.596669 archytas-1.0.3/archytas/repl.py
+-rw-r--r--   0        0        0    18638 2023-07-03 20:08:15.600669 archytas-1.0.3/archytas/tool_utils.py
+-rw-r--r--   0        0        0     4586 2023-07-03 20:08:15.600669 archytas-1.0.3/archytas/tools.py
+-rw-r--r--   0        0        0     1251 2023-07-03 20:08:15.600669 archytas-1.0.3/archytas/utils.py
+-rw-r--r--   0        0        0      780 2023-07-03 20:08:15.636669 archytas-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-1.0.3/PKG-INFO
```

### Comparing `archytas-1.0.2/LICENSE` & `archytas-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/README.md` & `archytas-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/archytas/agent.py` & `archytas-1.0.3/archytas/agent.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/archytas/demo_tools.py` & `archytas-1.0.3/archytas/demo_tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/archytas/prompt.py` & `archytas-1.0.3/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/archytas/python.py` & `archytas-1.0.3/archytas/python.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/archytas/react.py` & `archytas-1.0.3/archytas/react.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from archytas.agent import Agent
 from archytas.prompt import build_prompt, build_all_tool_names
 from archytas.tools import ask_user
 from archytas.tool_utils import make_tool_dict
+import asyncio
 import json
 import pdb
 import sys
 import logging
 import typing
 
 logger = logging.Logger('archytas')
@@ -95,14 +96,25 @@
     def thought_callback(self, thought: str, tool_name: str, tool_input: str) -> None:
         if self.verbose:
             #TODO: better coloring
             self.print(f"thought: {thought}\ntool: {tool_name}\ntool_input: {tool_input}\n")
 
 
     def react(self, query:str) -> str:
+        """
+        Synchronous wrapper around the asynchronous react_async method.
+        """
+        return asyncio.run(self.react_async(query))
+
+
+    async def react_async(self, query:str) -> str:
+        """
+        Asynchronous react loop function.
+        Continually calls tools until a satisfactory answer is reached.
+        """
         # reset error and steps counter
         self.errors = 0
         self.steps = 0
 
         # run the initial user query
         action_str = self.query(query)
 
@@ -148,15 +160,15 @@
             try:
                 tool_context = {
                     "agent": self,
                     "tool_name": tool_name,
                     "raw_tool": tool_fn,
                     "loop_controller": controller,
                 }
-                tool_output = tool_fn.run(tool_input, tool_context=tool_context)
+                tool_output = await tool_fn.run(tool_input, tool_context=tool_context)
             except Exception as e:
                 action_str = self.error(f"error running tool \"{tool_name}\": {e}")
 
                 continue
 
             # Check loop controller to see if we need to stop or error
             if controller.state == LoopController.STOP_SUCCESS:
```

### Comparing `archytas-1.0.2/archytas/repl.py` & `archytas-1.0.3/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/archytas/tool_utils.py` & `archytas-1.0.3/archytas/tool_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         func._name = name if name else func.__name__
         func._is_function_tool = True
         func._args_list = args_list
         func._ret = ret
         func._desc = desc
 
-        def run(*args:tuple[object, dict|list|str|int|float|bool|None], tool_context:dict[str,object]=None):
+        async def run(*args:tuple[object, dict|list|str|int|float|bool|None], tool_context:dict[str,object]=None):
             """Output from LLM will be dumped into a json object. Depending on object type, call func accordingly."""
 
             # The only time this will be a tuple is if more than one argument is passed in, which should only happen when this is an method and that is self.
             if len(args) == 2 and getattr(args[0], "_is_class_tool", False):
                 self, args = args
             else:
                 self = None
@@ -104,15 +104,18 @@
             # Add injections to kwargs
             for inj_name, inj_type in injections.items():
                 context_key = INJECTION_MAPPING.get(inj_type, None)
                 context_value = tool_context.get(context_key, None)
                 if context_value:
                     kwargs[inj_name] = context_value
 
-            result = func(*pargs, **kwargs)
+            if inspect.iscoroutinefunction(func):
+                result = await func(*pargs, **kwargs)
+            else:
+                result = func(*pargs, **kwargs)
 
             #convert the result to a string if it is not already a string
             if not isinstance(result, str):
                 result = str(result)
 
             return result
```

### Comparing `archytas-1.0.2/archytas/tools.py` & `archytas-1.0.3/archytas/tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/archytas/utils.py` & `archytas-1.0.3/archytas/utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.2/pyproject.toml` & `archytas-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "1.0.2"
+version = "1.0.3"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-1.0.2/PKG-INFO` & `archytas-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```


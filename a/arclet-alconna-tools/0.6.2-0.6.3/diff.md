# Comparing `tmp/arclet-alconna-tools-0.6.2.tar.gz` & `tmp/arclet-alconna-tools-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-tools-0.6.2.tar", last modified: Fri Jun 30 15:23:55 2023, max compression
+gzip compressed data, was "arclet-alconna-tools-0.6.3.tar", last modified: Mon Jul  3 11:37:46 2023, max compression
```

## Comparing `arclet-alconna-tools-0.6.2.tar` & `arclet-alconna-tools-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.2/LICENSE
--rw-r--r--   0        0        0     1075 2023-06-30 14:54:04.331377 arclet-alconna-tools-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.2/README.md
--rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    32763 2023-06-30 15:22:56.421449 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1076 2023-07-03 11:26:40.570640 arclet-alconna-tools-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.3/README.md
+-rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2023-07-03 07:06:39.010899 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    32583 2023-07-03 11:37:30.519633 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.3/PKG-INFO
```

### Comparing `arclet-alconna-tools-0.6.2/LICENSE` & `arclet-alconna-tools-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/pyproject.toml` & `arclet-alconna-tools-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.6.2"
+version = "0.6.3"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nepattern<0.6.0, >=0.5.8",
-    "arclet-alconna>=1.7.8",
+    "arclet-alconna>=1.7.10",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet-alconna-tools-0.6.2/README.md` & `arclet-alconna-tools-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/actions.py` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/checker.py` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/construct.py` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/construct.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
                 value = MultiVar(
                     KeyWordVar(value) if _kw else value,
                     _slice if _slice > 1 else _multi,
                 )
         _args.add(name, value=value, default=default)
     return _args
 
-def _args_from_string(string: str, formats: Dict[str, Union[TAValue, Args, Arg]], args: Args):
+def args_from_string(string: str, formats: Dict[str, Union[TAValue, Args, Arg]], args: Args):
     if mat := re.match(r"^\{(?P<pattern>.+?)\}$", string):
         pat = mat["pattern"]
         if pat in formats:
             if isinstance(formats[pat], (Args, Arg)):
                 args.__merge__(formats[pat])
             else:
                 args.__merge__([pat, formats[pat]])
@@ -387,22 +387,22 @@
     _stack = []
     for string in strings:
         if string.startswith("-"):
             _finish_arg = True
             _stack.append(string)
             continue
         if not _finish_arg:
-            _args_from_string(string, formats, main_args)
+            args_from_string(string, formats, main_args)
         elif not _stack:
             raise ValueError(lang.require("tools", "construct.format_error".format(target=string)))
         else:
             singles = _stack[:-1]
             name = _stack[-1]
             _opt_args = Args()
-            _args_from_string(string, formats, _opt_args)
+            args_from_string(string, formats, _opt_args)
             options.extend(Option(single) for single in singles)
             options.append(Option(name, _opt_args))
     alc = Alconna(command, main_args, *options, meta=meta)
     for ana, __ in command_manager.requires(alc.path):
         if ana.command != alc:
             alc = alc | ana.command
     return alc
@@ -501,15 +501,14 @@
         """构造为 Alconna 对象"""
         return Alconna(*self.buffer.values(), *self.options, meta=self.meta)
 
 class MountConfig(TypedDict):
     prefixes: NotRequired[List[str]]
     raise_exception: NotRequired[bool]
     description: NotRequired[str]
-    # get_subcommand: NotRequired[bool]
     namespace: NotRequired[str]
     command: NotRequired[str]
 
 config_keys = ("prefixes", "raise_exception", "description", "namespace", "command")
 
 def visit_config(obj: Any, base: Optional[MountConfig] = None) -> MountConfig:
     result: MountConfig = base or {}
@@ -843,22 +842,22 @@
 def _from_object(
     target: Type[T], command: Optional[TDC] = None, config: Optional[MountConfig] = None,
 ) -> ClassMounter[T, TDC]:
     ...
 
 @overload
 def _from_object(
-    target: T, command: Optional[TDC] = None, config: Optional[MountConfig] = None,
-) -> ObjectMounter[T, TDC]:
+    target: Union[Callable[..., T], FunctionType], command: Optional[TDC] = None, config: Optional[MountConfig] = None,
+) -> FuncMounter[T, TDC]:
     ...
 
 @overload
 def _from_object(
-    target: Callable[..., T], command: Optional[TDC] = None, config: Optional[MountConfig] = None,
-) -> FuncMounter[T, TDC]:
+    target: T, command: Optional[TDC] = None, config: Optional[MountConfig] = None,
+) -> ObjectMounter[T, TDC]:
     ...
 
 def _from_object(
     target: Optional[Union[Type[T], T, Callable[..., T], ModuleType]] = None,
     command: Optional[TDC] = None,
     config: Optional[MountConfig] = None,
 ):
@@ -938,17 +937,7 @@
     opt.nargs += 1
     return opt
 
 
 AlconnaFormat = _from_format
 AlconnaFire = _from_object
 Argument = _argument
-
-__all__ = [
-    "AlconnaFormat",
-    "AlconnaString",
-    "AlconnaFire",
-    "Argument",
-    "AlconnaDecorate",
-    "delegate",
-    "Executor",
-]
```

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/debug.py` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/debug.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/formatter.py` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/en-US.json` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/src/arclet/alconna/tools/pattern.py` & `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.2/PKG-INFO` & `arclet-alconna-tools-0.6.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-tools
-Version: 0.6.2
+Version: 0.6.3
 Summary: Builtin Tools for Alconna
 License: MIT
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Alconna Tools
```


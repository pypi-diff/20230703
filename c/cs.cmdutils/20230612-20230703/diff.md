# Comparing `tmp/cs.cmdutils-20230612.tar.gz` & `tmp/cs.cmdutils-20230703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.cmdutils-20230612.tar", last modified: Mon Jun 12 03:20:37 2023, max compression
+gzip compressed data, was "cs.cmdutils-20230703.tar", last modified: Mon Jul  3 10:02:31 2023, max compression
```

## Comparing `cs.cmdutils-20230612.tar` & `cs.cmdutils-20230703.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.031528 cs.cmdutils-20230612/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 03:19:41.000000 cs.cmdutils-20230612/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    15180 2023-06-12 03:20:37.031683 cs.cmdutils-20230612/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    25620 2023-06-12 03:19:52.000000 cs.cmdutils-20230612/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.027063 cs.cmdutils-20230612/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.027402 cs.cmdutils-20230612/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.029373 cs.cmdutils-20230612/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    45450 2023-06-12 03:19:32.000000 cs.cmdutils-20230612/lib/python/cs/cmdutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.031237 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    15180 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      310 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      172 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    15593 2023-06-12 03:20:26.000000 cs.cmdutils-20230612/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1104 2023-06-12 03:20:37.032360 cs.cmdutils-20230612/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 03:19:52.000000 cs.cmdutils-20230612/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:02:31.126202 cs.cmdutils-20230703/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-07-03 10:01:32.000000 cs.cmdutils-20230703/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15184 2023-07-03 10:02:31.126365 cs.cmdutils-20230703/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    25624 2023-07-03 10:01:45.000000 cs.cmdutils-20230703/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:02:31.120251 cs.cmdutils-20230703/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:02:31.120651 cs.cmdutils-20230703/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:02:31.122926 cs.cmdutils-20230703/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    45933 2023-07-03 10:00:40.000000 cs.cmdutils-20230703/lib/python/cs/cmdutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:02:31.125889 cs.cmdutils-20230703/lib/python/cs.cmdutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15184 2023-07-03 10:02:31.000000 cs.cmdutils-20230703/lib/python/cs.cmdutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      310 2023-07-03 10:02:31.000000 cs.cmdutils-20230703/lib/python/cs.cmdutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-07-03 10:02:31.000000 cs.cmdutils-20230703/lib/python/cs.cmdutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      172 2023-07-03 10:02:31.000000 cs.cmdutils-20230703/lib/python/cs.cmdutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-07-03 10:02:31.000000 cs.cmdutils-20230703/lib/python/cs.cmdutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15597 2023-07-03 10:02:22.000000 cs.cmdutils-20230703/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1104 2023-07-03 10:02:31.126982 cs.cmdutils-20230703/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-07-03 10:01:45.000000 cs.cmdutils-20230703/setup.py
```

### Comparing `cs.cmdutils-20230612/PKG-INFO` & `cs.cmdutils-20230703/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.cmdutils
-Version: 20230612
+Version: 20230703
 Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,17 +17,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230612*:
-* BaseCommand.cmdloop: fix intro parameter.
-* Other small fixes.
+*Latest release 20230703*:
+Small internal changes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -240,14 +239,17 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230703*:
+Small internal changes.
+
 *Release 20230612*:
 * BaseCommand.cmdloop: fix intro parameter.
 * Other small fixes.
 
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
```

### Comparing `cs.cmdutils-20230612/README.md` & `cs.cmdutils-20230703/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230612*:
-* BaseCommand.cmdloop: fix intro parameter.
-* Other small fixes.
+*Latest release 20230703*:
+Small internal changes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -541,14 +540,17 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230703*:
+Small internal changes.
+
 *Release 20230612*:
 * BaseCommand.cmdloop: fix intro parameter.
 * Other small fixes.
 
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
```

### Comparing `cs.cmdutils-20230612/lib/python/cs/cmdutils.py` & `cs.cmdutils-20230703/lib/python/cs/cmdutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # pylint: disable=too-many-lines
 
 ''' Convenience functions for working with the Cmd module,
     the BaseCommand class for constructing command line programmes,
     and other command line related stuff.
 '''
 
-from abc import ABC
+from abc import ABC, abstractmethod
 from cmd import Cmd
 from code import interact
 from collections import namedtuple
 from contextlib import contextmanager
 from dataclasses import dataclass
 from getopt import getopt, GetoptError
 from inspect import isclass, ismethod
@@ -41,15 +41,15 @@
 from cs.logutils import setup_logging, warning, exception
 from cs.pfx import Pfx, pfx_call, pfx_method
 from cs.py.doc import obj_docstring
 from cs.resources import RunState, uses_runstate
 from cs.typingutils import subtype
 from cs.upd import Upd
 
-__version__ = '20230612'
+__version__ = '20230703'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -122,14 +122,27 @@
     self.usage_mapping = usage_mapping or {}
 
   def __str__(self):
     return "%s(cmd=%r,method=%s,..)" % (
         type(self).__name__, self.cmd, self.method
     )
 
+  @abstractmethod
+  def __call__(
+      self, subcmd: str, base_command: "BaseCommandSubType", argv: List[str]
+  ):
+    ''' Run the subcommand.
+
+        Parameters:
+        * `subcmd`: the subcommand name
+        * `base_command`: the instance of `BaseCommand`
+        * `argv`: the command line arguments after the subcommand name
+    '''
+    raise NotImplementedError
+
   @staticmethod
   def from_class(command_cls: "BaseCommandSubType") -> Mapping[str, Callable]:
     ''' Return a mapping of subcommand names to subcommand specifications
         for class attributes which commence with
         `command_cls.SUBCOMMAND_METHOD_PREFIX`,
         by default `'cmd_'`.
     '''
@@ -216,19 +229,22 @@
       subusage_format = '{cmd} ...'
     return subusage_format
 
 class _ClassSubCommand(_BaseSubCommand):
   ''' A class to represent a subcommand implemented with a `BaseCommand` subclass.
   '''
 
-  def __call__(self, cmd, command, argv):
-    mkw = dict(command.options.__dict__)
-    if cmd is not None:
-      mkw.update(cmd=cmd)
-    return self.method(argv, **mkw).run()
+  def __call__(
+      self, subcmd: str, command: "BaseCommandSubType", argv: List[str]
+  ):
+    subcmd_class = self.method
+    updates = dict(command.options.__dict__)
+    updates.update(cmd=subcmd)
+    command = subcmd_class(argv, **updates)
+    return command.run()
 
   def usage_format(self) -> str:
     ''' Return the usage format string from the class.
     '''
     doc = self.method.usage_text(cmd=self.cmd)
     subusage_format, *_ = cutprefix(doc, 'Usage:').lstrip().split("\n\n", 1)
     return subusage_format
@@ -1156,15 +1172,15 @@
                     yield
                 finally:
                   ... any unconditional cleanup ...
     '''
     # redundant try/finally to remind subclassers of correct structure
     try:
       options = self.options
-      assert not hasattr(options, 'runstate')
+      ##assert not hasattr(options, 'runstate')
       handle_signal = getattr(
           self, 'handle_signal', lambda *_: runstate.cancel()
       )
       upd = getattr(options, 'upd', self.loginfo.upd) or Upd()
       with stackattrs(self, cmd=self._subcmd or self.cmd):
         with stackattrs(
             options,
```

### Comparing `cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/PKG-INFO` & `cs.cmdutils-20230703/lib/python/cs.cmdutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.cmdutils
-Version: 20230612
+Version: 20230703
 Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,17 +17,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230612*:
-* BaseCommand.cmdloop: fix intro parameter.
-* Other small fixes.
+*Latest release 20230703*:
+Small internal changes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -240,14 +239,17 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230703*:
+Small internal changes.
+
 *Release 20230612*:
 * BaseCommand.cmdloop: fix intro parameter.
 * Other small fixes.
 
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
```

### Comparing `cs.cmdutils-20230612/pyproject.toml` & `cs.cmdutils-20230703/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,31 +24,30 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230612"
+version = "20230703"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230612*:
-* BaseCommand.cmdloop: fix intro parameter.
-* Other small fixes.
+*Latest release 20230703*:
+Small internal changes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -261,14 +260,17 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230703*:
+Small internal changes.
+
 *Release 20230612*:
 * BaseCommand.cmdloop: fix intro parameter.
 * Other small fixes.
 
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
```

### Comparing `cs.cmdutils-20230612/setup.cfg` & `cs.cmdutils-20230703/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.cmdutils
-version = 20230612
+version = 20230703
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```


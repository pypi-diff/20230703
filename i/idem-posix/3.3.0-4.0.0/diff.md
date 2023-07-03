# Comparing `tmp/idem-posix-3.3.0.tar.gz` & `tmp/idem-posix-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-posix-3.3.0.tar", last modified: Thu Jan 26 21:19:58 2023, max compression
+gzip compressed data, was "idem-posix-4.0.0.tar", last modified: Mon Jul  3 10:50:38 2023, max compression
```

## Comparing `idem-posix-3.3.0.tar` & `idem-posix-4.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-01-26 21:19:44.000000 idem-posix-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2415 2023-01-26 21:19:58.690434 idem-posix-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1576 2023-01-26 21:19:44.000000 idem-posix-3.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/
--rw-r--r--   0 root         (0) root         (0)      282 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/exec/
--rw-r--r--   0 root         (0) root         (0)     4432 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/exec/cmdmod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/exec/contracts/
--rw-r--r--   0 root         (0) root         (0)     3403 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/exec/contracts/cmdmod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/exec/posix/
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/exec/posix/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/grains/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/grains/posix/
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/grains/posix/net/
--rw-r--r--   0 root         (0) root         (0)     3866 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/net/dns.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/net/fqdn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/grains/posix/os/
--rw-r--r--   0 root         (0) root         (0)      227 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/os/uname.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/grains/posix/proc/
--rw-r--r--   0 root         (0) root         (0)      246 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/proc/group.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/proc/pid.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/proc/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/grains/posix/system/
--rw-r--r--   0 root         (0) root         (0)      810 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/system/console.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/system/init_system.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/system/locale.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/system/machine_id.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/grains/posix/system/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/states/
--rw-r--r--   0 root         (0) root         (0)     3950 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/states/cmdmod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix/states/posix/
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-26 21:19:44.000000 idem-posix-3.3.0/idem_posix/states/posix/init.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-26 21:19:58.000000 idem-posix-3.3.0/idem_posix/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 21:19:58.690434 idem-posix-3.3.0/idem_posix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2023-01-26 21:19:58.000000 idem-posix-3.3.0/idem_posix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-01-26 21:19:58.000000 idem-posix-3.3.0/idem_posix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 21:19:58.000000 idem-posix-3.3.0/idem_posix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-26 21:19:58.000000 idem-posix-3.3.0/idem_posix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-01-26 21:19:58.000000 idem-posix-3.3.0/idem_posix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-26 21:19:58.000000 idem-posix-3.3.0/idem_posix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-26 21:19:58.690434 idem-posix-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2712 2023-01-26 21:19:44.000000 idem-posix-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-03 10:50:21.000000 idem-posix-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3734 2023-07-03 10:50:38.447766 idem-posix-4.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-07-03 10:50:21.000000 idem-posix-4.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/exec/
+-rw-r--r--   0 root         (0) root         (0)     5553 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/exec/cmdmod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/exec/contracts/
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/exec/contracts/cmdmod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/exec/posix/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/exec/posix/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/net/
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/net/dns.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/net/fqdn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/os/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/os/uname.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/proc/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/proc/group.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/proc/pid.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/proc/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/system/
+-rw-r--r--   0 root         (0) root         (0)      810 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/console.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/init_system.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/locale.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/machine_id.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/states/
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/states/cmdmod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/states/posix/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/states/posix/init.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 10:50:37.000000 idem-posix-4.0.0/idem_posix/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3734 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 10:50:38.447766 idem-posix-4.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-07-03 10:50:21.000000 idem-posix-4.0.0/setup.py
```

### Comparing `idem-posix-3.3.0/LICENSE` & `idem-posix-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/idem_posix/exec/cmdmod.py` & `idem-posix-4.0.0/idem_posix/exec/cmdmod.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Exec module for executing commands on a posix systems."""
 import asyncio
 import copy
 import json
 import os
 import sys
 import traceback
 from typing import Any
@@ -27,58 +28,87 @@
     env: Dict[str, Any] = None,
     timeout: int or float = None,
     is_string_output: bool = False,
     success_retcodes: List[int] = None,
     *args,
     **kwargs,
 ) -> Dict[str, Any]:
-    """
-    Execute the passed command and return the output as a string
+    """Execute the passed command and return the output as a string
 
-    :param cmd: The command to run. ex: ``ls -lart /home``
+    Args:
+        cmd(str or list[str]):
+            The command to run. ex: ``ls -lart /home``
+
+        cwd(str, Optional):
+            The directory from which to execute the command. Defaults
+            to the home directory of the user specified by ``runas`` (or the user
+            under which Salt is running if ``runas`` is not specified).
+
+        shell(bool):
+            If ``False``, let python handle the positional
+            arguments. Set to ``True`` to use shell features, such as pipes or
+            redirection. Defaults to False.
+
+        stdin(str, Optional):
+            A string of standard input can be specified for the
+            command to be run using the ``stdin`` parameter. This can be useful in
+            cases where sensitive information must be read from standard input.
+
+        stdout(int):
+            A string of standard input can be specified for the
+            command to be run using the ``stdout`` parameter.
+
+        stderr(int):
+            A string of standard input can be specified for the
+            command to be run using the ``stderr`` parameter.
+
+        render_pipe(str, Optional):
+            The render pipe to use on the output. Defaults to None.
+
+        env(dict[str], Optional):
+            Environment variables to be set prior to execution. Defaults to None.
+
+            .. note::
+                When passing environment variables on the CLI, they should be
+                passed as the string representation of a dictionary.
 
-    :param cwd: The directory from which to execute the command. Defaults
-        to the home directory of the user specified by ``runas`` (or the user
-        under which Salt is running if ``runas`` is not specified).
+            .. code-block:: bash
 
-    :param stdin: A string of standard input can be specified for the
-        command to be run using the ``stdin`` parameter. This can be useful in
-        cases where sensitive information must be read from standard input.
+                idem exec cmd.run 'some command' env='{"FOO": "bar"}'
 
-    :param shell: If ``False``, let python handle the positional
-        arguments. Set to ``True`` to use shell features, such as pipes or
-        redirection.
+        timeout(int or float, Optional):
+            A timeout in seconds for the executed process to return. Defaults to None.
 
-    :param stdout:
+        is_string_output(bool):
+            Give the output in string format irrespective of format the command executed returns. Defaults to False.
 
-    :param stderr:
+        success_retcodes(list[int], Optional):
+            The result will be True if the command's return code is in this list. Defaults to [0].
 
-    :param env: Environment variables to be set prior to execution.
+        args: args that will be forwarded to subprocess.
 
-        .. note::
-            When passing environment variables on the CLI, they should be
-            passed as the string representation of a dictionary.
+        kwargs: kwargs that will be forwarded to subprocess.
 
-            .. code-block:: bash
+    Returns:
+        Dict[str, Any]:
+            Returns command output
 
-                idem exec cmd.run 'some command' env='{"FOO": "bar"}'
-    :param render_pipe: The render pipe to use on the output
-    :param umask: The umask (in octal) to use when running the command.
+            * stdout(str): The plaintext output of the command.
 
-    :param timeout: A timeout in seconds for the executed process to return.
+            * stderr(str): The plaintext error/logging output of the command.
 
-    :param is_string_output: Give the output in string format irrespective of format the command executed returns
+            * retcode(str): The return code from the command.
 
-    :param success_retcodes: The result will be True if the command's return code is in this list. Defaults to [0].
+            * state(str): "The output as rendered from the render_pipe (if one was given), for use in arg_binding.
 
-    CLI Example:
+    Example:
+        .. code-block:: bash
 
-    .. code-block:: bash
+            idem exec cmd.run "shell command --with-flags" cwd=/home render_pipe=json timeout=10
 
-        $ idem exec cmd.run "shell command --with-flags" cwd=/home render_pipe=json timeout=10
     """
     ret = dict(
         result=True,
         comment="",
         ret={"retcode": 0, "state": {}, "stdout": b"", "stderr": b""},
     )
```

### Comparing `idem-posix-3.3.0/idem_posix/exec/contracts/cmdmod.py` & `idem-posix-4.0.0/idem_posix/exec/contracts/cmdmod.py`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/idem_posix/grains/posix/net/dns.py` & `idem-posix-4.0.0/idem_posix/grains/posix/net/dns.py`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/idem_posix/grains/posix/net/fqdn.py` & `idem-posix-4.0.0/idem_posix/grains/posix/net/fqdn.py`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/idem_posix/grains/posix/system/console.py` & `idem-posix-4.0.0/idem_posix/grains/posix/system/console.py`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/idem_posix/grains/posix/system/init_system.py` & `idem-posix-4.0.0/idem_posix/grains/posix/system/init_system.py`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/idem_posix/grains/posix/system/locale.py` & `idem-posix-4.0.0/idem_posix/grains/posix/system/locale.py`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/idem_posix.egg-info/SOURCES.txt` & `idem-posix-4.0.0/idem_posix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-posix-3.3.0/setup.py` & `idem-posix-4.0.0/setup.py`

 * *Files identical despite different names*


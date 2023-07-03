# Comparing `tmp/dagtimers-0.1.tar.gz` & `tmp/dagtimers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagtimers-0.1.tar", last modified: Sun Jul  2 17:10:25 2023, max compression
+gzip compressed data, was "dagtimers-0.1.1.tar", last modified: Mon Jul  3 02:05:08 2023, max compression
```

## Comparing `dagtimers-0.1.tar` & `dagtimers-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-02 17:10:25.557460 dagtimers-0.1/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      259 2023-07-02 17:10:25.550458 dagtimers-0.1/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-06-30 16:51:03.000000 dagtimers-0.1/README.md
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-02 17:10:24.778688 dagtimers-0.1/lib/
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-02 17:10:24.950641 dagtimers-0.1/lib/dagtimers/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     4050 2023-07-02 16:41:56.000000 dagtimers-0.1/lib/dagtimers/__init__.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-02 17:10:25.391091 dagtimers-0.1/lib/dagtimers.egg-info/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      259 2023-07-02 17:10:24.000000 dagtimers-0.1/lib/dagtimers.egg-info/PKG-INFO
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      251 2023-07-02 17:10:24.000000 dagtimers-0.1/lib/dagtimers.egg-info/SOURCES.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-07-02 17:10:24.000000 dagtimers-0.1/lib/dagtimers.egg-info/dependency_links.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-06-30 21:17:37.000000 dagtimers-0.1/lib/dagtimers.egg-info/not-zip-safe
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       10 2023-07-02 17:10:24.000000 dagtimers-0.1/lib/dagtimers.egg-info/top_level.txt
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-07-02 17:10:25.559494 dagtimers-0.1/setup.cfg
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1225 2023-07-02 17:07:49.000000 dagtimers-0.1/setup.py
-drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-02 17:10:25.466342 dagtimers-0.1/tests/
--rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5721 2023-07-02 17:06:03.000000 dagtimers-0.1/tests/test___init__.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-03 02:05:08.514267 dagtimers-0.1.1/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      261 2023-07-03 02:05:08.506961 dagtimers-0.1.1/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-06-30 16:51:03.000000 dagtimers-0.1.1/README.md
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-03 02:05:07.835548 dagtimers-0.1.1/lib/
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-03 02:05:07.992409 dagtimers-0.1.1/lib/dagtimers/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5480 2023-07-03 02:01:21.000000 dagtimers-0.1.1/lib/dagtimers/__init__.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-03 02:05:08.365398 dagtimers-0.1.1/lib/dagtimers.egg-info/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      261 2023-07-03 02:05:07.000000 dagtimers-0.1.1/lib/dagtimers.egg-info/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      251 2023-07-03 02:05:07.000000 dagtimers-0.1.1/lib/dagtimers.egg-info/SOURCES.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-07-03 02:05:07.000000 dagtimers-0.1.1/lib/dagtimers.egg-info/dependency_links.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-07-03 02:05:06.000000 dagtimers-0.1.1/lib/dagtimers.egg-info/not-zip-safe
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       10 2023-07-03 02:05:07.000000 dagtimers-0.1.1/lib/dagtimers.egg-info/top_level.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-07-03 02:05:08.518574 dagtimers-0.1.1/setup.cfg
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1227 2023-07-03 02:04:39.000000 dagtimers-0.1.1/setup.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-07-03 02:05:08.429785 dagtimers-0.1.1/tests/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     7473 2023-07-03 02:01:21.000000 dagtimers-0.1.1/tests/test___init__.py
```

### Comparing `dagtimers-0.1/lib/dagtimers/__init__.py` & `dagtimers-0.1.1/lib/dagtimers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import math
 from contextlib import contextmanager
 from time import time
 
 __all__ = ["Timers"]
 
 _START_TIME_DEFAULT = -1
+_UNACCOUNTED_STR = "<Unaccounted>"
+_EXCESS_STR = "<Excess>"
 
 class Timers:
 
     def __init__(self):
 
         self._starts = {}
         self._dag = {}
@@ -53,15 +55,14 @@
 
             next_node_in_path = {}
             self._path[-1][timer_name] = (time(), 0, next_node_in_path)
 
         else:
             self._path[-1][timer_name] = (time(), elapsed, next_node_in_path)
 
-
         self._path.append(next_node_in_path)
         self._parents.append(timer_name)
         self._excess += time() - excess_start_time
 
     def stop(self):
 
         excess_start_time = time()
@@ -76,57 +77,104 @@
 
         ret = ""
 
         if len(root) == 0:
             return ret
 
         has_parent = parent_timer_name is not None
-        ordered = sorted(root.keys(), key = lambda timer_name : -root[timer_name][1])
+        ordered = sorted(
+            [timer_name for timer_name in root.keys() if root[timer_name][0] == _START_TIME_DEFAULT],
+            key = lambda timer_name: -root[timer_name][1]
+        )
+        ordered.extend([timer_name for timer_name in root.keys() if root[timer_name][0] != _START_TIME_DEFAULT])
         accounted = sum(t[1] for t in root.values())
-        max_num_chars = max(len(timer_name) for timer_name in root.keys())
+
+        if len(root) > 0:
+            max_num_chars = max(len(timer_name) for timer_name in root.keys())
+
+        else:
+            max_num_chars = 0
 
         if has_parent:
 
+            max_num_chars = max(max_num_chars, len(_UNACCOUNTED_STR))
             parent_running = parent[parent_timer_name][0] != _START_TIME_DEFAULT
 
             if not parent_running:
+
                 parent_elapsed = parent[parent_timer_name][1]
                 unaccounted = parent_elapsed - accounted
-                prop = (unaccounted / parent_elapsed) * 100
-                ret += "\t" * indent + f"Unaccounted : {unaccounted:.7f} ({prop:.3f}%)\n"
+
+                if parent_elapsed != 0:
+                    prop = (unaccounted / parent_elapsed) * 100
+
+                else:
+                    prop = 100
+
+                if parent_elapsed != 0:
+
+                    ret += "\t" * indent + f"<Unaccounted> : {unaccounted:.7f} ({prop:.3f}%)"
+
+                    if self._excess != 0:
+                        ret += f" [{math.floor(math.log10(parent_elapsed / self._excess))}]"
+
+                    else:
+                        ret += " [inf]"
+
+                    ret += "\n"
 
         else:
 
+            max_num_chars = max(max_num_chars, len(_EXCESS_STR))
             parent_elapsed = accounted
             parent_running = False
 
         for timer_name in ordered:
 
             elapsed = root[timer_name][1]
             running = root[timer_name][0] != _START_TIME_DEFAULT
             ret += "\t" * indent + f"{timer_name: <{max_num_chars}}"
 
             if not running:
 
-                ret += f" : {elapsed: .7f}"
+                ret += f" : {elapsed:.7f}"
+
+                if has_parent and not parent_running:
 
-                if not parent_running:
+                    if parent_elapsed != 0:
+                        prop = (elapsed / parent_elapsed) * 100
+
+                    else:
+                        prop = 100
 
-                    prop = (elapsed / parent_elapsed) * 100
                     ret += f" ({prop:.3f}%)"
 
-                ret += f" [{math.floor(math.log10(elapsed / self._excess))}]\n"
+                if self._excess != 0 and elapsed != 0:
+                    ret += f" [{math.floor(math.log10(elapsed / self._excess))}]"
+
+                else:
+                    ret += f" [inf]"
+
+                ret += "\n"
 
             else:
                 ret += " : RUNNING\n"
 
-            if len(root[timer_name]) > 0:
-                ret += self._pretty_print(indent + 1, root[timer_name][2], timer_name, root[timer_name][2])
+            if len(root[timer_name][2]) > 0:
+                ret += self._pretty_print(indent + 1, root[timer_name][2], timer_name, root)
 
         return ret
 
     def pretty_print(self):
 
         start_time = time()
         ret = self._pretty_print(0, self._dag, None, None)
+
+        if len(self._dag) > 0:
+            max_num_chars = max(len(timer_name) for timer_name in self._dag.keys())
+
+        else:
+            max_num_chars = 0
+
+        max_num_chars = max(max_num_chars, len(_EXCESS_STR))
         self._excess += time() - start_time
-        return f"Excess : {self._excess:.7f}\n" + ret
+        return f"{_EXCESS_STR: <{max_num_chars}} : {self._excess:.7f}\n" + ret
```

### Comparing `dagtimers-0.1/setup.py` & `dagtimers-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from setuptools import setup
 
 setup(
     name = 'dagtimers',
-    version = "0.1",
+    version = "0.1.1",
     description = "Nicely displayed timers.",
     long_description = "Nicely displayed timers.",
     long_description_content_type="text/plain",
     author = "Michael P. Lane",
     author_email = "mlanetheta@gmail.com",
     url = "https://github.com/automorphis/dagtimers",
     package_dir = {"": "lib"},
```

### Comparing `dagtimers-0.1/tests/test___init__.py` & `dagtimers-0.1.1/tests/test___init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -92,14 +92,45 @@
         timers.stop()
         self._assert_node(timers._dag, "hello", True, False, 1.05, [
             (timers._dag["hello"][2], "hi", True, False, 0.1, []),
             (timers._dag["hello"][2], "hello", True, False, 0.2, [])
         ])
         self._assert_path(timers, [])
 
+    def test_pretty_print(self):
+
+        timers = Timers()
+        self._assert_indent_profile(timers.pretty_print(), [0])
+        timers.start("hi")
+        self._assert_indent_profile(timers.pretty_print(), [0, 0])
+        sleep(0.05)
+        timers.stop()
+        self._assert_indent_profile(timers.pretty_print(), [0, 0])
+        timers.start("hi")
+        self._assert_indent_profile(timers.pretty_print(), [0, 0])
+        sleep(0.2)
+        timers.stop()
+        self._assert_indent_profile(timers.pretty_print(), [0, 0])
+        timers.start("startyyyyy")
+        self._assert_indent_profile(timers.pretty_print(), [0, 0, 0])
+        sleep(0.1)
+        timers.stop()
+        self._assert_indent_profile(timers.pretty_print(), [0, 0, 0])
+        timers.start("hi")
+        sleep(0.01)
+        self._assert_indent_profile(timers.pretty_print(), [0, 0, 0])
+        timers.start("hello")
+        sleep(0.01)
+        self._assert_indent_profile(timers.pretty_print(), [0, 0, 0, 1])
+        timers.stop()
+        self._assert_indent_profile(timers.pretty_print(), [0, 0, 0, 1])
+        timers.stop()
+        self._assert_indent_profile(timers.pretty_print(), [0, 0, 1, 1, 0])
+
+
 
     def _assert_node(self, node, timer_name, default_start_time, zero_elasped, elapsed_lb, children):
 
         self.assertIn(
             timer_name,
             node.keys()
         )
@@ -172,11 +203,35 @@
             )
 
         self.assertEqual(
             timers._parents,
             exp_path_names
         )
 
+    def _assert_indent_profile(self, pretty_print, profile):
+
+        try:
+            self.assertEqual(
+                len(profile),
+                pretty_print.count("\n")
+            )
+
+        except AssertionError:
+            raise
+
+        for level, line in zip(profile, pretty_print[:-1].split("\n")):
+
+            self.assertEqual(
+                line[:level],
+                "\t" * level
+            )
+            self.assertNotEqual(
+                line[level],
+                "\t"
+            )
+
+
+
```


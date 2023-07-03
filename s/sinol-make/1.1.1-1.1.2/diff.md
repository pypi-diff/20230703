# Comparing `tmp/sinol-make-1.1.1.tar.gz` & `tmp/sinol-make-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.1.1.tar", last modified: Fri Jun 30 18:25:36 2023, max compression
+gzip compressed data, was "sinol-make-1.1.2.tar", last modified: Mon Jul  3 17:26:47 2023, max compression
```

## Comparing `sinol-make-1.1.1.tar` & `sinol-make-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-30 18:25:23.000000 sinol-make-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-30 18:25:36.438901 sinol-make-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-30 18:25:23.000000 sinol-make-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 18:25:23.000000 sinol-make-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:25:36.438901 sinol-make-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.430900 sinol-make-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    36055 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/helpers/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 18:25:23.000000 sinol-make-1.1.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.400143 sinol-make-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-03 17:26:33.000000 sinol-make-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 17:26:47.400143 sinol-make-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-03 17:26:33.000000 sinol-make-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 17:26:33.000000 sinol-make-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:26:47.400143 sinol-make-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.392143 sinol-make-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.392143 sinol-make-1.1.2/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/helpers/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 17:26:33.000000 sinol-make-1.1.2/tests/test_util.py
```

### Comparing `sinol-make-1.1.1/LICENSE` & `sinol-make-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.1/PKG-INFO` & `sinol-make-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.1.1/README.md` & `sinol-make-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.1/pyproject.toml` & `sinol-make-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.1/src/sinol_make/__init__.py` & `sinol-make-1.1.2/src/sinol_make/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 
 from sinol_make import util
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
     parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
```

### Comparing `sinol-make-1.1.1/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.1.2/src/sinol_make/commands/run/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
                             help='C compiler to use (default for Linux and Windows: gcc, default for Mac: gcc-9 or gcc-10)')
         parser.add_argument('--cpp_compiler_path', type=str, default=compiler.get_cpp_compiler_path(),
                             help='C++ compiler to use (default for Linux and Windows: g++, default for Mac: g++-9 or g++-10)')
         parser.add_argument('--python_interpreter_path', type=str, default=compiler.get_python_interpreter_path(),
                             help='Python interpreter to use (default: python3)')
         parser.add_argument('--java_compiler_path', type=str, default=compiler.get_java_compiler_path(),
                             help='Java compiler to use (default: javac)')
+        parser.add_argument('--weak_compilation_flags', dest='weak_compilation_flags', action='store_true',
+                            help='use weaker compilation flags')
         parser.add_argument('--apply_suggestions', dest='apply_suggestions', action='store_true',
                             help='apply suggestions from expected scores report')
 
 
     def color_memory(self, memory, limit):
         if memory == -1: return util.color_yellow("")
         memory_str = "%.1fMB" % (memory / 1024.0)
@@ -187,16 +189,18 @@
 
 
     def compile(self, solution):
         compile_log_file = os.path.join(
             self.COMPILATION_DIR, "%s.compile_log" % self.extract_file_name(solution))
         source_file = os.path.join(os.getcwd(), "prog", self.get_solution_from_exe(solution))
         output = os.path.join(self.EXECUTABLES_DIR, self.get_executable(solution))
+
         try:
-            compile.compile(source_file, output, self.compilers, open(compile_log_file, "w"))
+            compile.compile(source_file, output, self.compilers,
+                            open(compile_log_file, "w"), self.args.weak_compilation_flags)
             print(util.info("Compilation of file %s was successful."
                             % self.extract_file_name(solution)))
             return True
         except CompilationError as e:
             print(util.error("Compilation of file %s was unsuccessful."
                              % self.extract_file_name(solution)))
             os.system("head -c 500 %s" % compile_log_file) # TODO: make this work on Windows
```

### Comparing `sinol-make-1.1.1/src/sinol_make/commands/run/structs.py` & `sinol-make-1.1.2/src/sinol_make/commands/run/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.1/src/sinol_make/helpers/compile.py` & `sinol-make-1.1.2/src/sinol_make/helpers/compile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import sinol_make.helpers.compiler as compiler
 from sinol_make.interfaces.Errors import CompilationError
 import os, subprocess, sys
 
-def compile(program, output, compilers = None, compile_log = None):
+def compile(program, output, compilers = None, compile_log = None, weak_compilation_flags = False):
     """
     Compile a program
     compilers - A dictionary of compilers to use. If not set, the default compilers will be used
     """
+    gcc_compilation_flags = '-Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'
+    if weak_compilation_flags:
+        gcc_compilation_flags = '-w' # Disable all warnings
+
     ext = os.path.splitext(program)[1]
     arguments = []
     if ext == '.cpp':
         arguments = [compilers['cpp_compiler_path'] or compiler.get_cpp_compiler_path(), program, '-o', output] + \
-                    '--std=c++17 -O3 -lm -Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'.split(' ')
+                    f'--std=c++17 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
     elif ext == '.c':
         arguments = [compilers['c_compiler_path'] or compiler.get_c_compiler_path(), program, '-o', output] + \
-                    '--std=c17 -O3 -lm -Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'.split(' ')
+                    f'--std=c17 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
     elif ext == '.py':
         if sys.platform == 'win32' or sys.platform == 'cygwin':
             # TODO: Make this work on Windows
             pass
         else:
             open(output, 'w').write('#!/usr/bin/python3\n')
             open(output, 'a').write(open(program, 'r').read())
```

### Comparing `sinol-make-1.1.1/src/sinol_make/helpers/compiler.py` & `sinol-make-1.1.2/src/sinol_make/helpers/compiler.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.1/src/sinol_make/util.py` & `sinol-make-1.1.2/src/sinol_make/util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.1/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.1.2/src/sinol_make.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.1.1/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.1.2/src/sinol_make.egg-info/SOURCES.txt`

 * *Files identical despite different names*


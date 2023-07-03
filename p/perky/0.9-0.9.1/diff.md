# Comparing `tmp/perky-0.9.tar.gz` & `tmp/perky-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perky-0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "perky-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `perky-0.9.tar` & `perky-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       39 2023-07-01 02:47:29.152522 perky-0.9/.gitignore
--rw-r--r--   0        0        0     1089 2023-07-01 02:47:29.152522 perky-0.9/LICENSE
--rw-r--r--   0        0        0    16340 2023-07-02 09:40:43.158215 perky-0.9/README.md
--rwxr-xr-x   0        0        0    12120 2023-07-02 09:25:07.558776 perky-0.9/perky/__init__.py
--rw-r--r--   0        0        0    13688 2023-07-02 09:07:48.078512 perky-0.9/perky/tokenize.py
--rw-r--r--   0        0        0     7224 2023-07-02 06:53:52.878781 perky-0.9/perky/transform.py
--rw-r--r--   0        0        0     4807 2023-07-02 07:03:33.843370 perky-0.9/perky/utility.py
--rw-r--r--   0        0        0      437 2023-07-01 02:47:29.152522 perky-0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 02:47:29.156522 perky-0.9/tests/__init__.py
--rw-r--r--   0        0        0      860 2023-07-02 01:31:55.665423 perky-0.9/tests/benchmark_perky.py
--rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9/tests/include_dict/included.pky
--rw-r--r--   0        0        0       33 2023-07-01 02:47:29.156522 perky-0.9/tests/include_dict/main.pky
--rw-r--r--   0        0        0        1 2023-07-01 02:47:29.156522 perky-0.9/tests/include_list/included.pky
--rw-r--r--   0        0        0       27 2023-07-01 02:47:29.156522 perky-0.9/tests/include_list/main.pky
--rw-r--r--   0        0        0      106 2023-07-01 02:47:29.156522 perky-0.9/tests/include_nested/included.pky
--rw-r--r--   0        0        0      190 2023-07-01 02:47:29.156522 perky-0.9/tests/include_nested/main.pky
--rw-r--r--   0        0        0       30 2023-07-01 02:47:29.156522 perky-0.9/tests/include_path/dir1/main.pky
--rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9/tests/include_path/dir2/included.pky
--rw-r--r--   0        0        0      766 2023-07-01 02:47:29.156522 perky-0.9/tests/perkytestlib.py
--rw-r--r--   0        0        0      669 2023-07-01 02:49:14.953392 perky-0.9/tests/test_all.py
--rw-r--r--   0        0        0      214 2023-07-01 02:47:29.156522 perky-0.9/tests/test_input.txt
--rw-r--r--   0        0        0    13013 2023-07-02 09:38:44.201269 perky-0.9/tests/test_perky.py
--rw-r--r--   0        0        0     8237 2023-07-02 09:07:38.622437 perky-0.9/tests/test_tokenize.py
--rw-r--r--   0        0        0     2545 2023-07-02 09:36:43.836312 perky-0.9/tests/test_transform.py
--rw-r--r--   0        0        0     2200 2023-07-02 06:57:38.156560 perky-0.9/tests/test_utility.py
--rw-r--r--   0        0        0    16774 1970-01-01 00:00:00.000000 perky-0.9/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-07-01 02:47:29.152522 perky-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1089 2023-07-01 02:47:29.152522 perky-0.9.1/LICENSE
+-rw-r--r--   0        0        0    18661 2023-07-03 07:32:45.286025 perky-0.9.1/README.md
+-rwxr-xr-x   0        0        0    12412 2023-07-03 07:34:45.666982 perky-0.9.1/perky/__init__.py
+-rw-r--r--   0        0        0    13762 2023-07-03 07:25:22.474485 perky-0.9.1/perky/tokenize.py
+-rw-r--r--   0        0        0     7224 2023-07-02 06:53:52.878781 perky-0.9.1/perky/transform.py
+-rw-r--r--   0        0        0     4807 2023-07-02 07:03:33.843370 perky-0.9.1/perky/utility.py
+-rw-r--r--   0        0        0      437 2023-07-01 02:47:29.152522 perky-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 02:47:29.156522 perky-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      969 2023-07-03 07:13:58.037000 perky-0.9.1/tests/benchmark_perky.py
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_dict/included.pky
+-rw-r--r--   0        0        0       33 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_dict/main.pky
+-rw-r--r--   0        0        0        1 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_list/included.pky
+-rw-r--r--   0        0        0       27 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_list/main.pky
+-rw-r--r--   0        0        0      106 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_nested/included.pky
+-rw-r--r--   0        0        0      190 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_nested/main.pky
+-rw-r--r--   0        0        0       30 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_path/dir1/main.pky
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_path/dir2/included.pky
+-rw-r--r--   0        0        0      766 2023-07-01 02:47:29.156522 perky-0.9.1/tests/perkytestlib.py
+-rw-r--r--   0        0        0      669 2023-07-01 02:49:14.953392 perky-0.9.1/tests/test_all.py
+-rw-r--r--   0        0        0      214 2023-07-01 02:47:29.156522 perky-0.9.1/tests/test_input.txt
+-rw-r--r--   0        0        0    13623 2023-07-03 07:38:01.608539 perky-0.9.1/tests/test_perky.py
+-rw-r--r--   0        0        0     8281 2023-07-03 07:26:12.034882 perky-0.9.1/tests/test_tokenize.py
+-rw-r--r--   0        0        0     2545 2023-07-02 09:36:43.836312 perky-0.9.1/tests/test_transform.py
+-rw-r--r--   0        0        0     2200 2023-07-02 06:57:38.156560 perky-0.9.1/tests/test_utility.py
+-rw-r--r--   0        0        0    19097 1970-01-01 00:00:00.000000 perky-0.9.1/PKG-INFO
```

### Comparing `perky-0.9/LICENSE` & `perky-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perky-0.9/README.md` & `perky-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 * Explicit minimal data type support.  Rather than guess at the types
   of your data, Perky lets you handle the final transformation.
 * Lightweight, simple, and fast.  Perky's implementation is small
   and straightforward.  Ignoring comments and test code, it's about
   1k lines of Python.  Fewer lines means fewer bugs!  (Hopefully!)
 * Flexible and extensible.  Perky permits extending the semantics of
   Perky files through a "pragma" mechanism.
+* Written in 100% pure Python, but still parses >300k lines per
+  second on a modern desktop.
 * Perky supports Python 3.6+, and passes its unit test suite with
   100% coverage (excluding the deprecated portions).
 
 #### Perky syntax
 
 Perky configuration files look something like JSON without the
 quoting.  It supports only a surprisingly small set of value
@@ -36,17 +38,19 @@
 * "sequences" (lists).
 
 Perky is line-oriented; individual values go on a single
 line.  Container objects use one line per internal value.
 
 You may nest lists and dicts as deeply as memory permits.
 
-Unlike Python itself, leading whitespace is ignored.  You
-can use leading whitespace to show structure if you like,
-but it's optional.
+Unlike Python itself, leading whitespace is ignored.
+You can use leading whitespace however you like but it's
+optional.  (Leading whitespace is preserved for
+triple-quoted strings, though with a clever syntax
+that allows outdenting the actual value.)
 
 Blank lines and comment lines (lines starting with `#`)
 are ignored, except inside triple-quoted strings.
 
 Perky also supports "pragmas", lines that start
 with an equals sign that can perform special runtime
 behavior.  By default Perky doesn't define any
@@ -112,15 +116,15 @@
     =pragma with argument
 
 #### Explicit transformation is better than implicit
 
 One possibly-surprising design choice of Perky: the only
 natively supported values for the Perky parser are dicts,
 lists, and strings.  What about ints? floats? dates?
-booleans?
+booleans?  `NULL`?  `None`?
 
 Perky deliberately leaves that up to you.  As the Zen
 Of Python says:
 
 *In the face of ambiguity, refuse the temptation to guess.*
 
 Perky doesn't know what types your program needs.  So,
@@ -142,15 +146,16 @@
 remove it before 1.0.)
 
 
 ### Pragmas
 
 A *pragma* is a metadata directive for the Perky parser.
 It's a way of sending instructions to the Perky parser from
-inside a bit of Perky text.
+inside a bit of Perky text.  In Perky, a pragma is a line
+that starts with an unquoted equals sign.
 
 Here's an example pragma directive:
 
 `=command argument here`
 
 The first word after the equals sign is the name of the pragma, in this case `"command"`.
 Everything after the name of the pragma is an argument, with all leading
@@ -183,22 +188,55 @@
 as include statements, using the rest of the line as the name of a file.
 For more information, see `pragma_include()` below.
 
 The rules of pragmas:
 * To invoke a pragma, use `=` as the first non-whitespace character
   on a line.
 * The names of pragmas must always be lowercase.
-* You can't invoke a pragma inside a triple-quoted string.
+* You can invoke a pragma inside a sequence or mapping context.
+  But you can't invoke a pragma inside a triple-quoted string.
 * Pragmas can be "context-sensitive": they can be aware of where
   they are run inside a file, and e.g. modify the current dict
   or list.  The pragma function can see the entire current nested
   list of dicts and lists being parsed (via `parser.breadcrumbs`).
 * The rest of the line after the name of the pragma is the
-  pragma argument value, if any.  This is always a string.  It can
-  be a quoted string.
+  pragma argument value, if any.  This is always a string, which
+  can be either unquoted or single-quoted; if it's unquoted, it
+  can't contain any special symbols (`{ } = ''' """`).
+* If you want a line to start with an equals sign (a `value`, or
+  a `name=value`), but you *don't* want it to be a pragma, just
+  put quotes around it.  Likewise, if you want to use special
+  symbols in the pragma argument, just put (single) quotes around
+  it.
+
+### The Parser object
+
+Pragma functions recieve the Perky `Parser` object as an
+argument.  This object encapsulates all the current state
+of parsing the Perky file at the current time.  Here are
+the relevant attributes you may want to use from your
+pragma:
+
+* `parser.source` contains the source of the current
+  Perky text, either a filename or the string '<string>'.
+* `parser.line_number` contains the line number of
+  the current line being parsed.  The first line of the
+  Perky text is line 1.
+* `parser.stack` is a stack of references to collection
+  objects--the stack of nested dicts and lists from the
+  top to where we are now in the Perky file.
+  `parser.stack[0]` is always the root, and will be the
+  object returned by `load` or `loads`.  `parser.stack[-1]`
+  is always the current context the pragma was run in.
+  It can be either a list or a dict.  You should determine
+  which using
+  `isinstance(parser.stack[-1], collections.abc.Mapping)`;
+  if this is `True`, the current context is a mapping
+  context (a dict), and if this is `False` the current
+  context is a sequence context (a list).
 
 ### Parsing Errors
 
 There are only a few errors possible when parsing a Perky text:
 
 * Obviously, syntax errors, for example:
     * A line in a dict that doesn't have an unquoted equals sign
@@ -403,14 +441,26 @@
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.9.1** *2023/07/03*
+
+* API change: the `Parser` attribute `breadcrumbs` has been
+  renamed to `stack`.  It was previously undocumented anyway,
+  though has now been documented.
+* Added the `line_number` and `source` attributes to the
+  `Parser` object, for the convenience of pragma handlers.
+* Refactored `parser_include` slightly.  No change to
+  functionality or behavior, just a small code cleanup pass.
+* Added a "lines per second" output metric to the
+  benchmark program.
+
 **0.9** *2023/07/02*
 
 Breaking API change: removed the `encoding` argument entirely.
 
 * From this point forward, Perky only supports reading and
   writing files in
   [UTF-8](https://en.wikipedia.org/wiki/UTF-8).
```

### Comparing `perky-0.9/perky/__init__.py` & `perky-0.9.1/perky/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-__version__ = "0.9"
+__version__ = "0.9.1"
 
 import ast
 from collections.abc import MutableMapping, MutableSequence, Sequence
 import os.path
 from os.path import isfile, join, normpath
 import re
 import shlex
@@ -66,41 +66,49 @@
 def export(fn):
     __all__.append(fn.__name__)
     return fn
 
 
 class Parser:
 
-    def __init__(self, s, *, pragmas=None, root=None):
+    def __init__(self, s, *, pragmas=None, root=None, source=None):
         if not isinstance(s, str):
             raise TypeError('s must be str, not {type(s)}')
-        self.lt = LineTokenizer(s)
+        self.lt = LineTokenizer(s, source=source)
         self.pragmas = pragmas or {}
         self.root = root if root is not None else {}
-        self.breadcrumbs = []
+        self.source = source
+        # new name
+        self.stack = []
+        # old name
+        self.breadcrumbs = self.stack
+
+    @property
+    def line_number(self):
+        return self.lt.line_number
 
     def _parse_pragma(self, line):
         original_line = line
         # skip the leading '='
         line = line.lstrip()[1:]
 
         fields = line.split(None, 1)
         pragma = fields[0].lower()
         if len(fields) == 1:
             argument = None
         else:
             argument = fields[1]
             tokens = list(tokenize(pushback_str_iterator(argument)))
             if len(tokens) != 1 or tokens[0][0] != STRING:
-                raise PerkyFormatError(f"Line {self.lt.line_number}: Invalid pragma argument {argument}", tokens, original_line)
+                raise PerkyFormatError(f"'{self.source}' line {self.line_number}: Invalid pragma argument {argument}", tokens, original_line)
             argument = tokens[0][1]
 
         fn = self.pragmas.get(pragma)
         if not fn:
-            raise PerkyFormatError(f"Line {self.lt.line_number}: Unknown pragma {pragma}", None, original_line)
+            raise PerkyFormatError(f"'{self.source}' line {self.line_number}: Unknown pragma {pragma}", None, original_line)
         fn(self, argument)
 
     def _parse_value(self, t):
         tok, value = t
         if tok is LEFT_CURLY_BRACE:
             return self._read_mapping()
         if tok is LEFT_SQUARE_BRACKET:
@@ -111,15 +119,15 @@
             return {}
         if tok is EMPTY_SQUARE_BRACKETS:
             return []
         return value
 
     def _read_mapping(self, starting_dict=None):
         d = starting_dict if starting_dict is not None else {}
-        self.breadcrumbs.append(d)
+        self.stack.append(d)
 
         keys_seen = set()
 
         d_setitem = d.__setitem__
         keys_seen_add = keys_seen.add
         self_parse_value = self._parse_value
 
@@ -155,22 +163,22 @@
             if len(tokens) == 3:
                 value = self_parse_value(tokens[2])
             else:
                 value = ""
             # d[key] = value
             d_setitem(key, value)
 
-        self.breadcrumbs.pop()
+        self.stack.pop()
         return d
 
     def _read_sequence(self, starting_list=None):
         l = starting_list if starting_list is not None else []
         l_append = l.append
         self_parse_value = self._parse_value
-        self.breadcrumbs.append(l)
+        self.stack.append(l)
         for line_number, line, tokens in self.lt:
             if not tokens:
                 # blank line
                 continue
             token, argument = tokens[0]
             if token is EQUALS:
                 self._parse_pragma(line)
@@ -181,15 +189,15 @@
                     tokens, line)
             if token is RIGHT_SQUARE_BRACKET:
                 break
             if token is COMMENT:
                 continue
             value = self_parse_value(tokens[0])
             l_append(value)
-        self.breadcrumbs.pop()
+        self.stack.pop()
         return l
 
     def _read_textblock(self, marker):
         l = []
         l_append = l.append
         lt = self.lt
         next_line = self.lt.next_line
@@ -332,61 +340,69 @@
         if (value == value.strip()) and "".join(value.split()).isalnum():
             self.newline(value)
             return
         return self.serialize_quoted_string(value)
 
 
 @export
-def loads(s, *, pragmas=None, root=None):
+def loads(s, *, pragmas=None, root=None, source="<string>"):
     p = Parser(s, pragmas=pragmas, root=root)
     d = p.parse()
     return d
 
 @export
 def load(filename, *, pragmas=None, root=None):
     with open(filename, "rt", encoding="utf-8") as f:
-        return loads(f.read(), pragmas=pragmas, root=root)
+        text = f.read()
+    p = Parser(text, pragmas=pragmas, root=root, source=filename)
+    d = p.parse()
+    return d
 
 @export
 def dumps(d):
     s = Serializer()
     s.serialize(d)
     return s.dumps()
 
 
 @export
 def dump(filename, d):
-    s = Serializer()
-    s.serialize(d)
+    text = dumps(d)
     with open(filename, "wt", encoding="utf-8") as f:
-        f.write(s.dumps())
+        f.write(text)
 
 
 @export
 def pragma_include(include_path=(".",)):
     include_path_ok = (
         isinstance(include_path, Sequence)
         and (not isinstance(include_path, str))
         and all(isinstance(s, str) for s in include_path)
         )
     if not include_path_ok:
         raise TypeError(f"include_path must be a sequence of strings, not {include_path!r}")
+
     include_path = tuple(include_path)
+
     def pragma_include(parser, filename):
-        leaf = parser.breadcrumbs[-1]
-        leaf_is_list = isinstance(parser.breadcrumbs[-1], list)
-        subroot = [] if leaf_is_list else {}
+        leaf = parser.stack[-1]
+        leaf_is_mapping = isinstance(leaf, Mapping)
+        included_root = {} if leaf_is_mapping else []
+
         for directory in include_path:
             path = normpath(join(directory, filename))
             if isfile(path):
                 break
         else:
             raise FileNotFoundError(filename)
-        load(path, pragmas=parser.pragmas, root=subroot)
-        merged = merge_dicts_and_lists(leaf, subroot)
-        # print(f"\n\nXXX merge_dicts_and_lists({leaf=}, {subroot=}) -> {merged=}\n\n")
-        leaf.clear()
-        if isinstance(leaf, list):
-            leaf.extend(merged)
-        else:
+
+        load(path, pragmas=parser.pragmas, root=included_root)
+        if leaf_is_mapping:
+            # we can't just leaf.update(loaded_root),
+            # we have to do this recursively.
+            merged = merge_dicts_and_lists(leaf, included_root)
+            leaf.clear()
             leaf.update(merged)
+        else:
+            leaf.extend(included_root)
+
     return pragma_include
```

### Comparing `perky-0.9/perky/tokenize.py` & `perky-0.9.1/perky/tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,27 +339,28 @@
     A simple tokenizing iterator for Perky.
     It's line-oriented; you can get the next
     line either as a string, or as a sequence
     of tokens.
     """
 
     # go-faster stripe!
-    __slots__ = ('_lines', 'suppress_whitespace', 'waiting', 'line_number', '_repr', 'i')
+    __slots__ = ('_lines', 'source', 'suppress_whitespace', 'waiting', 'line_number', '_repr', 'i')
 
-    def __init__(self, s, suppress_whitespace=True):
+    def __init__(self, s, suppress_whitespace=True, source='<string>'):
         lines = s.split("\n")
         self._lines = enumerate(lines, 1)
         self.suppress_whitespace = suppress_whitespace
         self.waiting = None
+        self.source = source
         self.line_number = 0
 
         repr_lines = str(lines[:5])
         if len(repr_lines) > 50:
             repr_lines = repr_lines[:47] + "..."
-        self._repr = f"<LineTokenizer {{self.line_number}}/{len(lines)} lines {repr_lines}>"
+        self._repr = f"<LineTokenizer '{self.source}' {{self.line_number}}/{len(lines)} lines {repr_lines}>"
 
         self.i = pushback_str_iterator('')
 
     def __repr__(self):
         return self._repr.format(self=self)
 
     def __iter__(self):
```

### Comparing `perky-0.9/perky/transform.py` & `perky-0.9.1/perky/transform.py`

 * *Files identical despite different names*

### Comparing `perky-0.9/perky/utility.py` & `perky-0.9.1/perky/utility.py`

 * *Files identical despite different names*

### Comparing `perky-0.9/tests/benchmark_perky.py` & `perky-0.9.1/tests/benchmark_perky.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,7 +60,9 @@
     end_time = perf_counter()
     delta = end_time - start_time
     if delta >= stop_after:
         break
 
 print(f"{i} iterations in {delta} seconds.")
 print(f"{i/delta} iterations per second.")
+lines = len(TEST_INPUT_TEXT.strip().split("\n"))
+print(f"Oooh, call it {(lines*i)/delta} lines per second.")
```

### Comparing `perky-0.9/tests/perkytestlib.py` & `perky-0.9.1/tests/perkytestlib.py`

 * *Files identical despite different names*

### Comparing `perky-0.9/tests/test_all.py` & `perky-0.9.1/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `perky-0.9/tests/test_perky.py` & `perky-0.9.1/tests/test_perky.py`

 * *Files 5% similar despite different names*

```diff
@@ -249,61 +249,31 @@
             perky.loads("a=3\na=5")
 
 # TODO: check if there are any other formats that would cause a failure
     def test_read_file(self):
         test_input = perky.load("test_input.txt")
         self.assertIsNotNone(self, test_input)
 
-    def test_perky_include_bad_include_path(self):
-        with self.assertRaises(TypeError):
-            perky.load("include_list/main.pky", root=[], pragmas={'include':perky.pragma_include( 3.14159 )})
-        with self.assertRaises(TypeError):
-            perky.load("include_list/main.pky", root=[], pragmas={'include':perky.pragma_include( (3.14159,) )})
-
-    def test_perky_include_list(self):
-        with pushd("include_list"):
-            root = perky.load("main.pky", root=[], pragmas={'include':perky.pragma_include()})
-        self.assertEqual(root, list("abcd"))
-
-    def test_perky_include_dict(self):
-        with pushd("include_dict"):
-            root = perky.load("main.pky", pragmas={'include':perky.pragma_include()})
-        self.assertEqual(root, dict(zip("abcd", "1234")))
-
-    def test_perky_include_nested(self):
-        with pushd("include_nested"):
-            root = perky.load("main.pky", pragmas={'include':perky.pragma_include()})
-        self.assertEqual(root,
-            {
-                'a': '1',
-                'b': {
-                    'ba': '1',
-                    'bb': '2',
-                    'bc': '3',
-                    'bd': '4',
-                    'nested_dict': {
-                        'x': '3',
-                        'y': '2',
-                        'z': ['1', '2', '3', '4']
-                        },
-                    'nested_list': ['a', 'b', 'c'],
-                    },
-                'c': '3',
-                'd': '4'}
-            )
-
-    def test_perky_include_path(self):
-        with pushd("include_path"):
-            root = perky.load("dir1/main.pky", pragmas={'include':perky.pragma_include( ['dir1', 'dir2'] )})
-        self.assertEqual(root, dict(zip("abc", "345")))
-
     def test_perky_invalid_pragma(self):
         with self.assertRaises(perky.PerkyFormatError):
             root = perky.loads("a=b\n=include '''\nc=d\n", pragmas={'include':perky.pragma_include()})
 
+    def test_simple_pragma(self):
+        def pragma_reverse(parser, argument):
+            leaf = parser.breadcrumbs[-1]
+            leaf.append("".join(reversed(argument)))
+
+        expected = {'a': '1', 'b': ['c', 'd', 'edcba', 'e'], 'x': 'y'}
+        got = perky.loads("a = 1\nb = [\nc\nd\n=reverse abcde\ne\n]\nx = y", pragmas={'reverse': pragma_reverse})
+        self.assertEqual(expected, got)
+
+        expected = {'a': ['b', 'c', ' edcba ', 'x', 'y']}
+        got = perky.loads("a = [\nb\nc\n=reverse ' abcde '\nx\ny\n]\n", pragmas={'reverse': pragma_reverse})
+        self.assertEqual(expected, got)
+
     def test_perky_roundtrip(self):
         for i in range(1, 300):
             c = chr(i)
             if c.isspace():
                 continue
             hex_digits = hex(i).partition("x")[2].rjust(4, "0")
             s = f"U+{hex_digits} {c}"
@@ -413,15 +383,14 @@
         d = perky.loads(s)
         self.assertEqual(d['a'], '22')
 
         s = perky.dumps({'a': datetime.date(2022, 6, 15)})
         d = perky.loads(s)
         self.assertEqual(d['a'], '2022-06-15')
 
-
     def test_dump_to_file(self):
         with tempfile.TemporaryDirectory() as tmpdir:
             tmpdir = pathlib.Path(tmpdir)
 
             d = perky.loads(TEST_INPUT_TEXT)
             filename = tmpdir / "temp.pky"
             perky.dump(filename, d)
@@ -447,10 +416,54 @@
 
     def test_non_existent_file(self):
         s = "a = b\n=include 'non existent file.pky'\nc = d"
 
         with self.assertRaises(FileNotFoundError):
             d = perky.loads(s, pragmas={'include': perky.pragma_include()})
 
+    def test_perky_include_bad_include_path(self):
+        with self.assertRaises(TypeError):
+            perky.load("include_list/main.pky", root=[], pragmas={'include':perky.pragma_include( 3.14159 )})
+        with self.assertRaises(TypeError):
+            perky.load("include_list/main.pky", root=[], pragmas={'include':perky.pragma_include( (3.14159,) )})
+
+    def test_perky_include_list(self):
+        with pushd("include_list"):
+            root = perky.load("main.pky", root=[], pragmas={'include':perky.pragma_include()})
+        self.assertEqual(root, list("abcd"))
+
+    def test_perky_include_dict(self):
+        with pushd("include_dict"):
+            root = perky.load("main.pky", pragmas={'include':perky.pragma_include()})
+        self.assertEqual(root, dict(zip("abcd", "1234")))
+
+    def test_perky_include_nested(self):
+        with pushd("include_nested"):
+            root = perky.load("main.pky", pragmas={'include':perky.pragma_include()})
+        self.assertEqual(root,
+            {
+                'a': '1',
+                'b': {
+                    'ba': '1',
+                    'bb': '2',
+                    'bc': '3',
+                    'bd': '4',
+                    'nested_dict': {
+                        'x': '3',
+                        'y': '2',
+                        'z': ['1', '2', '3', '4']
+                        },
+                    'nested_list': ['a', 'b', 'c'],
+                    },
+                'c': '3',
+                'd': '4'}
+            )
+
+    def test_perky_include_path(self):
+        with pushd("include_path"):
+            root = perky.load("dir1/main.pky", pragmas={'include':perky.pragma_include( ['dir1', 'dir2'] )})
+        self.assertEqual(root, dict(zip("abc", "345")))
+
+
 
 if __name__ == '__main__': # pragma: no cover
     unittest.main()
```

### Comparing `perky-0.9/tests/test_tokenize.py` & `perky-0.9.1/tests/test_tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,30 +182,30 @@
         expected_results = [
             (1, 'a=1', [(STRING, 'a'), (EQUALS, '='), (STRING, '1')]),
             (2, 'b=2', [(STRING, 'b'), (EQUALS, '='), (STRING, '2')]),
             ]
 
         input_lines = "\n".join(t[1] for t in expected_results)
         lt = LineTokenizer(input_lines)
-        self.assertIn('<LineTokenizer 0/2 lines [', repr(lt))
+        self.assertIn("<LineTokenizer '<string>' 0/2 lines [", repr(lt))
         self.assertTrue(lt)
         for expected in expected_results:
             self.assertTrue(lt)
             got = lt.tokens()
             line_number = expected[0]
-            self.assertIn(f'<LineTokenizer {line_number}/2 lines [', repr(lt))
+            self.assertIn(f"<LineTokenizer '<string>' {line_number}/2 lines [", repr(lt))
             self.assertEqual(expected, got)
 
         self.assertFalse(lt)
-        self.assertIn('<LineTokenizer 2/2 lines [', repr(lt))
+        self.assertIn("<LineTokenizer '<string>' 2/2 lines [", repr(lt))
         got = lt.next_line()
         self.assertEqual(got, (None, None))
 
         self.assertFalse(lt)
-        self.assertIn('<LineTokenizer 2/2 lines [', repr(lt))
+        self.assertIn("<LineTokenizer '<string>' 2/2 lines [", repr(lt))
         got = lt.next_line()
         self.assertEqual(got, (None, None))
 
         self.assertFalse(lt)
 
 
 if __name__ == '__main__': # pragma: nocover
```

### Comparing `perky-0.9/tests/test_transform.py` & `perky-0.9.1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `perky-0.9/tests/test_utility.py` & `perky-0.9.1/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `perky-0.9/PKG-INFO` & `perky-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perky
-Version: 0.9
+Version: 0.9.1
 Summary: A simple, Pythonic file format.  Same interface as the
 Home-page: https://github.com/larryhastings/perky/
 Author: Larry Hastings
 Author-email: larry@hastings.org
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,16 @@
 * Explicit minimal data type support.  Rather than guess at the types
   of your data, Perky lets you handle the final transformation.
 * Lightweight, simple, and fast.  Perky's implementation is small
   and straightforward.  Ignoring comments and test code, it's about
   1k lines of Python.  Fewer lines means fewer bugs!  (Hopefully!)
 * Flexible and extensible.  Perky permits extending the semantics of
   Perky files through a "pragma" mechanism.
+* Written in 100% pure Python, but still parses >300k lines per
+  second on a modern desktop.
 * Perky supports Python 3.6+, and passes its unit test suite with
   100% coverage (excluding the deprecated portions).
 
 #### Perky syntax
 
 Perky configuration files look something like JSON without the
 quoting.  It supports only a surprisingly small set of value
@@ -49,17 +51,19 @@
 * "sequences" (lists).
 
 Perky is line-oriented; individual values go on a single
 line.  Container objects use one line per internal value.
 
 You may nest lists and dicts as deeply as memory permits.
 
-Unlike Python itself, leading whitespace is ignored.  You
-can use leading whitespace to show structure if you like,
-but it's optional.
+Unlike Python itself, leading whitespace is ignored.
+You can use leading whitespace however you like but it's
+optional.  (Leading whitespace is preserved for
+triple-quoted strings, though with a clever syntax
+that allows outdenting the actual value.)
 
 Blank lines and comment lines (lines starting with `#`)
 are ignored, except inside triple-quoted strings.
 
 Perky also supports "pragmas", lines that start
 with an equals sign that can perform special runtime
 behavior.  By default Perky doesn't define any
@@ -125,15 +129,15 @@
     =pragma with argument
 
 #### Explicit transformation is better than implicit
 
 One possibly-surprising design choice of Perky: the only
 natively supported values for the Perky parser are dicts,
 lists, and strings.  What about ints? floats? dates?
-booleans?
+booleans?  `NULL`?  `None`?
 
 Perky deliberately leaves that up to you.  As the Zen
 Of Python says:
 
 *In the face of ambiguity, refuse the temptation to guess.*
 
 Perky doesn't know what types your program needs.  So,
@@ -155,15 +159,16 @@
 remove it before 1.0.)
 
 
 ### Pragmas
 
 A *pragma* is a metadata directive for the Perky parser.
 It's a way of sending instructions to the Perky parser from
-inside a bit of Perky text.
+inside a bit of Perky text.  In Perky, a pragma is a line
+that starts with an unquoted equals sign.
 
 Here's an example pragma directive:
 
 `=command argument here`
 
 The first word after the equals sign is the name of the pragma, in this case `"command"`.
 Everything after the name of the pragma is an argument, with all leading
@@ -196,22 +201,55 @@
 as include statements, using the rest of the line as the name of a file.
 For more information, see `pragma_include()` below.
 
 The rules of pragmas:
 * To invoke a pragma, use `=` as the first non-whitespace character
   on a line.
 * The names of pragmas must always be lowercase.
-* You can't invoke a pragma inside a triple-quoted string.
+* You can invoke a pragma inside a sequence or mapping context.
+  But you can't invoke a pragma inside a triple-quoted string.
 * Pragmas can be "context-sensitive": they can be aware of where
   they are run inside a file, and e.g. modify the current dict
   or list.  The pragma function can see the entire current nested
   list of dicts and lists being parsed (via `parser.breadcrumbs`).
 * The rest of the line after the name of the pragma is the
-  pragma argument value, if any.  This is always a string.  It can
-  be a quoted string.
+  pragma argument value, if any.  This is always a string, which
+  can be either unquoted or single-quoted; if it's unquoted, it
+  can't contain any special symbols (`{ } = ''' """`).
+* If you want a line to start with an equals sign (a `value`, or
+  a `name=value`), but you *don't* want it to be a pragma, just
+  put quotes around it.  Likewise, if you want to use special
+  symbols in the pragma argument, just put (single) quotes around
+  it.
+
+### The Parser object
+
+Pragma functions recieve the Perky `Parser` object as an
+argument.  This object encapsulates all the current state
+of parsing the Perky file at the current time.  Here are
+the relevant attributes you may want to use from your
+pragma:
+
+* `parser.source` contains the source of the current
+  Perky text, either a filename or the string '<string>'.
+* `parser.line_number` contains the line number of
+  the current line being parsed.  The first line of the
+  Perky text is line 1.
+* `parser.stack` is a stack of references to collection
+  objects--the stack of nested dicts and lists from the
+  top to where we are now in the Perky file.
+  `parser.stack[0]` is always the root, and will be the
+  object returned by `load` or `loads`.  `parser.stack[-1]`
+  is always the current context the pragma was run in.
+  It can be either a list or a dict.  You should determine
+  which using
+  `isinstance(parser.stack[-1], collections.abc.Mapping)`;
+  if this is `True`, the current context is a mapping
+  context (a dict), and if this is `False` the current
+  context is a sequence context (a list).
 
 ### Parsing Errors
 
 There are only a few errors possible when parsing a Perky text:
 
 * Obviously, syntax errors, for example:
     * A line in a dict that doesn't have an unquoted equals sign
@@ -416,14 +454,26 @@
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.9.1** *2023/07/03*
+
+* API change: the `Parser` attribute `breadcrumbs` has been
+  renamed to `stack`.  It was previously undocumented anyway,
+  though has now been documented.
+* Added the `line_number` and `source` attributes to the
+  `Parser` object, for the convenience of pragma handlers.
+* Refactored `parser_include` slightly.  No change to
+  functionality or behavior, just a small code cleanup pass.
+* Added a "lines per second" output metric to the
+  benchmark program.
+
 **0.9** *2023/07/02*
 
 Breaking API change: removed the `encoding` argument entirely.
 
 * From this point forward, Perky only supports reading and
   writing files in
   [UTF-8](https://en.wikipedia.org/wiki/UTF-8).
```


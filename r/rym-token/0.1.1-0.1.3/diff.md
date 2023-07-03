# Comparing `tmp/rym_token-0.1.1.tar.gz` & `tmp/rym_token-0.1.3.tar.gz`

## Comparing `rym_token-0.1.1.tar` & `rym_token-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rym_token-0.1.1/rym/token/__init__.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 rym_token-0.1.1/rym/token/regex.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 rym_token-0.1.1/rym/token/structures.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 rym_token-0.1.1/rym/token/tokenizer.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 rym_token-0.1.1/rym/token/tokenspec.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 rym_token-0.1.1/rym/token/tokenspecgroup.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 rym_token-0.1.1/.gitignore
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 rym_token-0.1.1/README.md
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 rym_token-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 rym_token-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 rym_token-0.1.3/rym/token/__init__.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 rym_token-0.1.3/rym/token/regex.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 rym_token-0.1.3/rym/token/structures.py
+-rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 rym_token-0.1.3/rym/token/tokenizer.py
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 rym_token-0.1.3/rym/token/tokenspec.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 rym_token-0.1.3/rym/token/tokenspecgroup.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 rym_token-0.1.3/.gitignore
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 rym_token-0.1.3/README.md
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 rym_token-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 rym_token-0.1.3/PKG-INFO
```

### Comparing `rym_token-0.1.1/rym/token/regex.py` & `rym_token-0.1.3/rym/token/regex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 """Regex handling for rym-token.
 
 """
 
 import logging
 import re
+from collections import abc
 from functools import singledispatch
 from re import Pattern
 from typing import Any, Iterable, Tuple, Union
 
 from .structures import TokenSpec
 
 LOGGER = logging.getLogger(__name__)
@@ -43,15 +44,15 @@
         sources: Iterable with one or more regex sources.
     Returns:
         Compiled regex with named capture group for each source.
     Raises:
         TypeError for invalid source.
     )
     """
-    patterns = tuple(_get_pattern(x, i) for i, x in enumerate(sources))
+    patterns = tuple(_yield_patterns(sources, i=None))
     return combine_regex_memoized(patterns)
 
 
 @cache
 def combine_regex_memoized(specs: Tuple[Tuple[str, str], ...]) -> Pattern:
     """Memoized version of combine_regex.
 
@@ -61,37 +62,44 @@
     idx = {k: i for i, (k, _) in reversed(list(enumerate(specs)))}
     ordered = [specs[i] for i in sorted(idx.values())]
     regexp = "|".join("(?P<%s>%s)" % (name, pattern) for name, pattern in ordered)
     return re.compile(regexp)
 
 
 @singledispatch
-def _get_pattern(value: Any, i: int) -> Tuple[str, str]:
+def _yield_patterns(value: Any, i: int) -> Tuple[str, str]:
     """Return (name, pattern) for every source.
 
     Arguments:
         value: Regex pattern source
         i: Index for naming (if needed)
     Returns:
         A tuple of the name and pattern.
     Raises:
         TypeError for unsupported sources.
     """
     raise TypeError(f"{value}; expected string, re.Pattern, or TokenSpec")
 
 
-@_get_pattern.register(str)
+@_yield_patterns.register(str)
 def _(value: str, i: int) -> Tuple[str, str]:
-    return f"P{i}", value
+    yield f"P{i or 0}", value
 
 
-@_get_pattern.register(Pattern)
+@_yield_patterns.register(Pattern)
 def _(value: Pattern, i: int) -> Tuple[str, str]:
-    return f"P{i}", value.pattern
+    yield f"P{i or 0}", value.pattern
 
 
-@_get_pattern.register(TokenSpec)
+@_yield_patterns.register(TokenSpec)
 def _(value: TokenSpec, i: int) -> Tuple[str, str]:
-    return value.type, value.pattern
+    yield value.type, value.pattern
+
+
+@_yield_patterns.register(abc.Iterable)
+def _(value: Iterable, i: int) -> Tuple[str, str]:
+    prefix = f"{i}_" if i else ""
+    for j, x in enumerate(value):
+        yield from _yield_patterns(x, f"{prefix}{j}")
 
 
 # __END__
```

### Comparing `rym_token-0.1.1/rym/token/tokenspec.py` & `rym_token-0.1.3/rym/token/tokenspec.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,19 +28,20 @@
 
 def build_subtype_assignment(
     subtypes: Iterable[Tuple[str, Tuple[str, ...]]]
 ) -> Callable[[str], str]:
     """Return a callable to assign subtype.
 
     Arguments:
-        subtype: Mapping used to assign token subtype
+        subtype: One or more ("type", ("subtype", ...)) definitions
+    Returns:
+        A callable that takes a value and type string and returns the
+        updated type assignment.
     """
-    lookup = {
-        str(name).lower(): k.upper() for k, names in subtypes for name in names
-    }
+    lookup = {str(name).lower(): k.upper() for k, names in subtypes for name in names}
 
     def assign_subtype(value: str, type_: str) -> str:
         return lookup.get(str(value).lower(), type_)
 
     return assign_subtype
 
 
@@ -81,67 +82,68 @@
         # Z support added in 3.11
         value = value[:-1] + "+00:00"
     return dt.datetime.fromisoformat(value)
 
 
 @cache
 def timestamp() -> TokenSpec:
+    """Return a spec for ISO-8601 timestamps."""
     return TokenSpec(
         "TIMESTAMP",
         "%s%s%s(?:%s)?" % (_DATE, _TS_SEP, _TIME, _TZ),
         _safe_timestamp,
     )
 
 
 @cache
 def date() -> TokenSpec:
+    """Return a spec for ISO-8601 dates, e.g., 2023-10-30."""
     return TokenSpec("DATE", _DATE, _safe_date)
 
 
 @cache
 def time() -> TokenSpec:
+    """Return a spec for ISO-8601 time strings, e.g., 24:00.000Z."""
     return TokenSpec("TIME", "%s(?:%s)?" % (_TIME, _TZ), _safe_time)
 
 
 @cache
 def reldate() -> TokenSpec:
+    """Return a spec for relative date words, e.g., 'tomorrow'."""
     names = "|".join(
         r"[%s%s]%s" % (x[0].lower(), x[0].upper(), x[1:])
         for x in itertools.chain(
-            ("day", "yesterday", "today", "tomorrow"),
-            ("week", "weekend", "weekday"),
+            ("yesterday", "today", "tomorrow", "day"),
+            ("weekend", "weekday", "week"),
             ("month", "year"),
             ("winter", "spring", "summer", "fall"),
             ("Q[1-4]",),
         )
     )
-    LOGGER.critical(names)
     pattern = r"(?<=\b)(?:%s)(?=\b)" % (names,)
     return TokenSpec("RELDATE", pattern)
 
 
 @cache
 def month() -> str:
-    """Return regex pattern match for months."""
+    """Return a spec for month names and abbreviations. Title case only."""
     names = "|".join(
         itertools.chain.from_iterable(
             zip(calendar.month_name[1:], calendar.month_abbr[1:])
         )
     )
     pattern = r"(?<=\b)(?:%s)(?=\b)" % (names,)
     return TokenSpec("MONTH", pattern)
 
 
 @cache
 def day() -> str:
-    """Return regex pattern match for months."""
+    """Return a spec for day names and abbreviations. Title case only."""
     names = "|".join(
-        itertools.chain.from_iterable(
-            zip(calendar.day_name[1:], calendar.day_abbr[1:])
-        )
+        itertools.chain.from_iterable(zip(calendar.day_name[1:], calendar.day_abbr[1:]))
     )
     pattern = r"(?<=\b)(?:%s)(?=\b)" % (names,)
     return TokenSpec("DAY", pattern)
 
 
 # numeric
 # ----------------------------------
@@ -153,19 +155,21 @@
 
 def _safe_int(x: str, *args) -> int:
     return int(x.replace(",", ""))
 
 
 @cache
 def number() -> TokenSpec:
+    """Return a spec for floating point numbers."""
     return TokenSpec("NUMBER", r"-?\d[\d_]*[e\.]-?\d+", _safe_float)
 
 
 @cache
 def integer() -> TokenSpec:
+    """Return a spec for integers."""
     return TokenSpec(
         "INTEGER",
         r"(?<![\.\d\w])(?<!e-)\-?\d(?:[\,_]\d)?\d*(?!\.\d)(?![\d_e])\b",
         _safe_int,
     )
 
 
@@ -173,59 +177,67 @@
 # ----------------------------------
 
 
 @cache
 def alphanum(
     subtype: Optional[Iterable[Tuple[str, Tuple[str, ...]]]] = None
 ) -> TokenSpec:
+    """Return a spec for alphanumeric words. Includes hyphens."""
     if subtype:
         subtype = build_subtype_assignment(subtype)
     return TokenSpec(
         "ALPHANUM",
         r"\b[\w\d\-]+\b",
         None,
         subtype=subtype,
     )
 
 
 @cache
 def newline() -> TokenSpec:
+    """Return a spec for newlines."""
     return TokenSpec("NEWLINE", r"\r?\n", None)
 
 
 @cache
 def punctuation() -> TokenSpec:
+    """Return a spec for punctuation, e.g., non-word, non-whitespace."""
     return TokenSpec("PUNCTUATION", r"[^\w\s]+", None)
 
 
 @cache
 def quote() -> TokenSpec:
+    """Return a spec for returning quoted strings."""
     return TokenSpec("QUOTE", r"\"[^\"]*\"")
 
 
 @cache
 def search_term() -> TokenSpec:
+    """Return a spec for search terms in the format 'key=val' or 'key:val'."""
     return TokenSpec(
         "TERM",
         r"(?P<term_key>[\w\-]+)(?P<term_op>[:=><]+)(?P<term_value>[\w\-\.]+\b)(?![:])",
     )
 
 
 @cache
 def uuid_string() -> TokenSpec:
+    """Return a spec for UUID v4."""
     return TokenSpec(
         "UUID",
         r"[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}",
     )
 
 
 @cache
-def word(
-    subtype: Optional[Iterable[Tuple[str, Tuple[str, ...]]]] = None
-) -> TokenSpec:
+def word(subtype: Optional[Iterable[Tuple[str, Tuple[str, ...]]]] = None) -> TokenSpec:
+    """Return a spec for words.
+
+    NOTE: Matches any consecutive letters.
+    """
     if subtype:
         subtype = build_subtype_assignment(subtype)
     return TokenSpec(
         "WORD",
         r"[A-Za-z]+(?:\'[A-Za-z]+)?",
         None,
         subtype=subtype,
```

### Comparing `rym_token-0.1.1/rym/token/tokenspecgroup.py` & `rym_token-0.1.3/rym/token/tokenspecgroup.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,28 +23,45 @@
             ("and", "nor", "but", "or", "yet", "so", "since", "because"),
         ),  # 'for'
         ("preposition", ("at", "by", "for", "from", "in", "of", "on", "with")),
     )
 
 
 def grammar() -> Tuple[TokenSpec, ...]:
+    """Return punctuation and grammar specs.
+
+    NOTE: Uses 'word' spec with minimal subtype matching.
+    NOTE: Intended for example usage. Grammar subtype is not exhaustive.
+    """
     return (
         tokenspec.punctuation(),
         tokenspec.word(grammar_word_subtypes()),
     )
 
 
 def numeric() -> Tuple[TokenSpec, ...]:
+    """Return number and integer subtypes."""
     return (
         tokenspec.integer(),
         tokenspec.number(),
     )
 
 
 def search() -> Tuple[TokenSpec, ...]:
+    """Return token specs useful for parsing search strings.
+
+    Includes:
+        - search terms
+        - uuid string
+        - temporal specs
+        - numeric specs
+        - alphanumeric with qualifier and quantifier subtypes
+
+    TODO: Add logical operators.
+    """
     return (
         tokenspec.search_term(),
         tokenspec.uuid_string(),
         *temporal(),
         *numeric(),
         tokenspec.alphanum(
             (
@@ -52,14 +69,15 @@
                 ("quantifier", ("some", "all", "any")),
             )
         ),
     )
 
 
 def temporal() -> Tuple[TokenSpec, ...]:
+    """Return specs for date-related tokens."""
     return (
         tokenspec.timestamp(),  # ORDER MATTERS!
         tokenspec.date(),
         tokenspec.time(),
         tokenspec.day(),
         tokenspec.month(),
         tokenspec.reldate(),
```

### Comparing `rym_token-0.1.1/.gitignore` & `rym_token-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rym_token-0.1.1/pyproject.toml` & `rym_token-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rym-token"
-version = "0.1.1"
+version = "0.1.3"
 description = "A python library for tokenizing text."
 authors = [
     {name = "Stephen Bush", email = "muppetjones@gmail.com"},
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
```

### Comparing `rym_token-0.1.1/PKG-INFO` & `rym_token-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rym-token
-Version: 0.1.1
+Version: 0.1.3
 Summary: A python library for tokenizing text.
 Project-URL: Homepage, https://github.com/muppetjones/rym-py/tree/main/rym-token
 Project-URL: Bug Tracker, https://github.com/muppetjones/rym-py/issues
 Project-URL: Documentation, https://muppetjones.github.io/rym-py/rym-token
 Author-email: Stephen Bush <muppetjones@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```


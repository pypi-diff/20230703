# Comparing `tmp/liquichange-0.1.0.tar.gz` & `tmp/liquichange-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquichange-0.1.0.tar", max compression
+gzip compressed data, was "liquichange-0.2.0.tar", max compression
```

## Comparing `liquichange-0.1.0.tar` & `liquichange-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11558 2023-03-29 15:16:02.986888 liquichange-0.1.0/LICENSE
--rw-r--r--   0        0        0      554 2023-04-06 21:35:03.874850 liquichange-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      187 2023-03-29 15:16:02.986888 liquichange-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-29 15:20:14.201423 liquichange-0.1.0/src/liquichange/__init__.py
--rw-r--r--   0        0        0     6639 2023-04-06 21:24:18.466973 liquichange-0.1.0/src/liquichange/changelog.py
--rw-r--r--   0        0        0     2863 2023-04-06 17:02:37.802939 liquichange-0.1.0/src/liquichange/element.py
--rw-r--r--   0        0        0     5474 2023-04-05 22:35:18.079574 liquichange-0.1.0/src/liquichange/precondition.py
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 liquichange-0.1.0/setup.py
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 liquichange-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-03-29 15:16:02.986888 liquichange-0.2.0/LICENSE
+-rw-r--r--   0        0        0      554 2023-07-03 17:25:45.516610 liquichange-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      964 2023-07-03 17:53:52.420533 liquichange-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-29 15:20:14.201423 liquichange-0.2.0/src/liquichange/__init__.py
+-rw-r--r--   0        0        0    12270 2023-07-03 17:31:00.916685 liquichange-0.2.0/src/liquichange/changelog.py
+-rw-r--r--   0        0        0     3650 2023-07-03 17:19:05.884818 liquichange-0.2.0/src/liquichange/element.py
+-rw-r--r--   0        0        0     6849 2023-07-03 17:42:51.593661 liquichange-0.2.0/src/liquichange/precondition.py
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 liquichange-0.2.0/setup.py
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 liquichange-0.2.0/PKG-INFO
```

### Comparing `liquichange-0.1.0/LICENSE` & `liquichange-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liquichange-0.1.0/pyproject.toml` & `liquichange-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liquichange"
-version = "0.1.0"
+version = "0.2.0"
 description = "Build and modify Liquibase changelogs in Python."
 authors = ["Nelson Moore <nelson.moore@essential-soft.com>"]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `liquichange-0.1.0/src/liquichange/precondition.py` & `liquichange-0.2.0/src/liquichange/precondition.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,45 +5,70 @@
 from enum import Enum
 from typing import Dict, Optional, Set, Union
 
 from liquichange.element import LiquibaseElement
 
 
 class Condition(LiquibaseElement):
-    """for type hinting various precondition entities"""
+    """For type hinting various precondition entities."""
 
     subelements: None = None
 
 
 @dataclass
 class Preconditions(LiquibaseElement):
     """
-    Container class for preconditions used to group Preconditions
-    that have the same conditional logic.
+    Container class for preconditions used to group Preconditions and/or
+    Condition objects that follow the same conditional_logic.
 
-    If Precondtions has other Preconditions as subelements, will
+    Preconditions are tags you add to your changelog or individual changesets
+    to control the execution of an update based on the state of the database.
+
+    Use by adding any Preconditions or Condition type objects to the subelements list.
+
+    Attributes:
+        conditional_logic (Logic): AND or OR. Default AND.
+        on_error (Action): Controls what happens if there is an error checking
+            whether the precondition passed or not.
+        on_error_message (str): rovides a custom message to output when preconditions fail.
+        on_fail (Action): Controls what happens if the preconditions check fails.
+        on_fail_message (str): Provides a custom message to output when preconditions fail.
+        on_sql_output (SqlAction): Controls how preconditions are evaluated in the
+            update-sql mode for XML, YAML, and JSON changelogs.
+        on_update_sql (SqlAction): Controls how preconditions are evaluated in the
+            update-sql mode for formatted SQL changelogs.
+
+    Class Variables:
+        Action (Enum): The Action enum.
+        SqlAction (Enum): The SqlAction enum.
+        Logic (Enum): The Logic enum.
+
+    Methods:
+        to_xml(_is_changelog: bool = False) -> ET.Element: Returns the XML representation
+            of the element. Overrides the LiquibaseElement method to incorporate conditional
+            logic of preconditions.
     """
 
     class Action(str, Enum):
-        """values for precondition types: onFail, onError"""
+        """Values for precondition types: onFail, onError."""
 
         CONTINUE = "CONTINUE"
         HALT = "HALT"
         MARK_RAN = "MARK_RAN"
         WARN = "WARN"
 
     class SqlAction(str, Enum):
-        """values for precondition types: onSqlOutput, onUpdateSql"""
+        """Values for precondition types: onSqlOutput, onUpdateSql."""
 
         FAIL = "FAIL"
         IGNORE = "IGNORE"
         TEST = "TEST"
 
     class Logic(str, Enum):
-        """values for precondition conditional logic"""
+        """Values for precondition conditional logic."""
 
         AND = "and"
         OR = "or"
         NOT = "not"
 
     on_error: Optional[Action] = None
     on_error_message: Optional[str] = None
@@ -92,15 +117,15 @@
     type: Union[DbmsType, None] = field(default=None, metadata={"required": True})
     _tag: str = "dbms"
 
 
 @dataclass
 class VersionPrecondition(Condition):
     """
-    asserts the expected Neo4j version
+    Asserts the expected Neo4j version
 
     matches: expected Neo4j version as a string in the format:
         "major.minor.patch"
     """
 
     matches: Union[str, None] = field(default=None, metadata={"required": True})
     _tag: str = "neo4j:version"
```


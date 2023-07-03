# Comparing `tmp/tuidbtv-0.1.5.tar.gz` & `tmp/tuidbtv-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuidbtv-0.1.5.tar", max compression
+gzip compressed data, was "tuidbtv-0.1.6.tar", max compression
```

## Comparing `tuidbtv-0.1.5.tar` & `tuidbtv-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-06-27 17:22:14.783915 tuidbtv-0.1.5/LICENSE
--rw-r--r--   0        0        0      917 2023-07-03 14:19:21.031242 tuidbtv-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      586 2023-06-29 20:45:18.516504 tuidbtv-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-27 17:29:23.492066 tuidbtv-0.1.5/tuidbtv/__init__.py
--rw-r--r--   0        0        0     2869 2023-06-29 00:27:37.312147 tuidbtv-0.1.5/tuidbtv/__main__.py
--rw-r--r--   0        0        0        0 2023-06-16 16:51:55.114223 tuidbtv-0.1.5/tuidbtv/config/__init__.py
--rw-r--r--   0        0        0     2366 2023-06-29 08:13:56.884461 tuidbtv-0.1.5/tuidbtv/config/ConfigParser.py
--rw-r--r--   0        0        0        0 2023-06-11 14:55:59.729538 tuidbtv-0.1.5/tuidbtv/controllers/__init__.py
--rw-r--r--   0        0        0      811 2023-06-28 23:21:03.594509 tuidbtv-0.1.5/tuidbtv/controllers/ControllerFactory.py
--rw-r--r--   0        0        0      472 2023-06-25 14:27:13.231327 tuidbtv-0.1.5/tuidbtv/controllers/DBController.py
--rw-r--r--   0        0        0     2447 2023-06-28 23:21:03.496526 tuidbtv-0.1.5/tuidbtv/controllers/MySQLController.py
--rw-r--r--   0        0        0     3117 2023-06-28 23:21:03.545522 tuidbtv-0.1.5/tuidbtv/controllers/PostgresController.py
--rw-r--r--   0        0        0     1429 2023-06-28 23:21:03.563518 tuidbtv-0.1.5/tuidbtv/controllers/SQLLiteController.py
--rw-r--r--   0        0        0     2808 2023-07-01 02:36:39.251328 tuidbtv-0.1.5/tuidbtv/default.css
--rw-r--r--   0        0        0      102 2023-06-26 16:04:15.427437 tuidbtv-0.1.5/tuidbtv/enums_and_variables/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 01:56:17.958273 tuidbtv-0.1.5/tuidbtv/suggesters/__init__.py
--rw-r--r--   0        0        0      528 2023-07-01 02:34:43.603654 tuidbtv-0.1.5/tuidbtv/suggesters/SuggesterDict.py
--rw-r--r--   0        0        0        0 2023-06-11 13:28:38.866786 tuidbtv-0.1.5/tuidbtv/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:40:36.587499 tuidbtv-0.1.5/tuidbtv/widgets/forms/__init__.py
--rw-r--r--   0        0        0     1704 2023-06-28 23:21:03.578504 tuidbtv-0.1.5/tuidbtv/widgets/forms/ConnectionForms.py
--rw-r--r--   0        0        0     3382 2023-06-29 19:03:01.527743 tuidbtv-0.1.5/tuidbtv/widgets/NewConnection.py
--rw-r--r--   0        0        0      612 2023-06-16 22:17:33.503450 tuidbtv-0.1.5/tuidbtv/widgets/PopUpScreen.py
--rw-r--r--   0        0        0      668 2023-06-11 14:32:32.205700 tuidbtv-0.1.5/tuidbtv/widgets/QuitScreen.py
--rw-r--r--   0        0        0     5706 2023-06-28 23:21:03.483540 tuidbtv-0.1.5/tuidbtv/widgets/SelectConnection.py
--rw-r--r--   0        0        0     1361 2023-07-03 14:19:48.182443 tuidbtv-0.1.5/tuidbtv/widgets/SQLEditor.py
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.6/LICENSE
+-rw-r--r--   0        0        0      917 2023-07-03 17:12:50.724469 tuidbtv-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.6/tuidbtv/__init__.py
+-rw-r--r--   0        0        0     3236 2023-07-03 17:12:50.729461 tuidbtv-0.1.6/tuidbtv/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.6/tuidbtv/config/__init__.py
+-rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.6/tuidbtv/config/ConfigParser.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.6/tuidbtv/controllers/__init__.py
+-rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.6/tuidbtv/controllers/ControllerFactory.py
+-rw-r--r--   0        0        0      472 2023-07-03 17:12:50.735465 tuidbtv-0.1.6/tuidbtv/controllers/DBController.py
+-rw-r--r--   0        0        0     2447 2023-07-03 17:12:50.736498 tuidbtv-0.1.6/tuidbtv/controllers/MySQLController.py
+-rw-r--r--   0        0        0     3117 2023-07-03 17:12:50.738495 tuidbtv-0.1.6/tuidbtv/controllers/PostgresController.py
+-rw-r--r--   0        0        0     1429 2023-07-03 17:12:50.740476 tuidbtv-0.1.6/tuidbtv/controllers/SQLLiteController.py
+-rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.6/tuidbtv/default.css
+-rw-r--r--   0        0        0      102 2023-07-03 17:12:50.745498 tuidbtv-0.1.6/tuidbtv/enums_and_variables/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.6/tuidbtv/suggesters/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.6/tuidbtv/suggesters/SuggesterDict.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.6/tuidbtv/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.6/tuidbtv/widgets/forms/__init__.py
+-rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.6/tuidbtv/widgets/forms/ConnectionForms.py
+-rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.6/tuidbtv/widgets/NewConnection.py
+-rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.6/tuidbtv/widgets/PopUpScreen.py
+-rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.6/tuidbtv/widgets/QuitScreen.py
+-rw-r--r--   0        0        0     5706 2023-07-03 17:12:50.756478 tuidbtv-0.1.6/tuidbtv/widgets/SelectConnection.py
+-rw-r--r--   0        0        0     1860 2023-07-03 17:12:50.754491 tuidbtv-0.1.6/tuidbtv/widgets/SQLEditor.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.6/PKG-INFO
```

### Comparing `tuidbtv-0.1.5/LICENSE` & `tuidbtv-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/pyproject.toml` & `tuidbtv-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuidbtv"
-version = "0.1.5"
+version = "0.1.6"
 description = "console database client"
 authors = ["lakdemon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lakdemon/TUIDBTV"
 classifiers = [
     "Environment :: Console",
```

### Comparing `tuidbtv-0.1.5/README.md` & `tuidbtv-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/__main__.py` & `tuidbtv-0.1.6/tuidbtv/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,22 +38,29 @@
                     yield SQLEditor()
                 with TabPane("+", id="add_new_tab"):
                     yield Markdown()
         yield Footer()
 
     def openConnectionSelectScreen(self, can_quit=False):
         def select_connection(db_controller):
+            editor = self.query_one(SQLEditor)
             self.dbController = db_controller
             tree = self.query_one(Tree)
             tree.clear()
             tree.root.expand()
+            new_suggestions = []
             for schemaName in self.dbController.getSchemaNames():
                 schema = tree.root.add(schemaName[0])
+                new_suggestions.append(schemaName[0])
                 for tableName in self.dbController.getTableNamesBySchema(schemaName[0]):
                     schema.add_leaf(tableName[0])
+                    new_suggestions.append(tableName[0])
+                    new_suggestions.append(f"{schemaName[0]}.{tableName[0]}")
+            editor.clean_completions()
+            editor.add_completions(new_suggestions)
 
         self.push_screen(SelectConnection(_can_quit=can_quit), select_connection)
 
     def on_mount(self) -> None:
         self.openConnectionSelectScreen(can_quit=False)
 
     def on_tree_node_selected(self, event: Tree.NodeSelected):
```

### Comparing `tuidbtv-0.1.5/tuidbtv/config/ConfigParser.py` & `tuidbtv-0.1.6/tuidbtv/config/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/controllers/ControllerFactory.py` & `tuidbtv-0.1.6/tuidbtv/controllers/ControllerFactory.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/controllers/MySQLController.py` & `tuidbtv-0.1.6/tuidbtv/controllers/MySQLController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/controllers/PostgresController.py` & `tuidbtv-0.1.6/tuidbtv/controllers/PostgresController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/controllers/SQLLiteController.py` & `tuidbtv-0.1.6/tuidbtv/controllers/SQLLiteController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/default.css` & `tuidbtv-0.1.6/tuidbtv/default.css`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/suggesters/SuggesterDict.py` & `tuidbtv-0.1.6/tuidbtv/suggesters/SuggesterDict.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,7 +8,15 @@
             values = value.rsplit(' ', 1)
             last_word = values[-1]
             for idx, suggestion in enumerate(self._for_comparison):
                 if suggestion.startswith(last_word):
                     values[-1] = self._suggestions[idx]
                     return ' '.join(values)
         return None
+
+    def add_suggestions(self, new_suggestions: list[str]):
+        self._for_comparison.extend(new_suggestions)
+        self._suggestions.extend(new_suggestions)
+
+    def set_suggestions(self, suggestions: list[str]):
+        self._for_comparison = suggestions
+        self._suggestions = suggestions
```

### Comparing `tuidbtv-0.1.5/tuidbtv/widgets/forms/ConnectionForms.py` & `tuidbtv-0.1.6/tuidbtv/widgets/forms/ConnectionForms.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/widgets/NewConnection.py` & `tuidbtv-0.1.6/tuidbtv/widgets/NewConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/widgets/PopUpScreen.py` & `tuidbtv-0.1.6/tuidbtv/widgets/PopUpScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/widgets/QuitScreen.py` & `tuidbtv-0.1.6/tuidbtv/widgets/QuitScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/widgets/SelectConnection.py` & `tuidbtv-0.1.6/tuidbtv/widgets/SelectConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.5/tuidbtv/widgets/SQLEditor.py` & `tuidbtv-0.1.6/tuidbtv/widgets/SQLEditor.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from textual.app import ComposeResult
 from textual.widget import Widget
 from textual.widgets import Input, Button, DataTable
 
 from tuidbtv.suggesters.SuggesterDict import SuggesterDict
 from tuidbtv.widgets.PopUpScreen import PopUpScreen
 
-sql_abc = ["select", "from", "where", "join", "right", "left", "inner", "like", "insert", "into", "update",
-           "order", "group", "by", "as", "on"]
+sql_abc = ["select", "from", "where", "join", "right join", "left join", "inner join",
+           "like", "insert", "into", "update", "order", "group", "by", "as", "on"]
 
 
 class SQLEditor(Widget):
     def compose(self) -> ComposeResult:
-        yield Input(suggester=SuggesterDict(sql_abc, case_sensitive=False), id="new_request_input")
+        yield Input(suggester=SuggesterDict([] + sql_abc, case_sensitive=False), id="new_request_input")
         yield Button("Run", id="execute_editor_button")
         yield DataTable(id="editor_table")
 
     @on(Button.Pressed)
     def execute_editor_query(self, event: Button.Pressed):
         if event.button.id == "execute_editor_button":
             query_text = self.query_one("#new_request_input", expect_type=Input).value
@@ -25,7 +25,21 @@
                 table = self.query_one("#editor_table")
                 table.clear(columns=True)
                 table.add_columns(*data[0])
                 table.zebra_stripes = True
                 table.add_rows(data[1:])
             except Exception as e:
                 self.app.push_screen(PopUpScreen(e.__str__()))
+
+    def add_completions(self, new_completions: list[str]):
+        request_field = self.query_one("#new_request_input", expect_type=Input)
+        try:
+            request_field.suggester.add_suggestions(new_completions)
+        except:
+            pass
+
+    def clean_completions(self):
+        input = self.query_one("#new_request_input", expect_type=Input)
+        try:
+            input.suggester.set_suggestions([] + sql_abc)
+        except:
+            pass
```

### Comparing `tuidbtv-0.1.5/PKG-INFO` & `tuidbtv-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuidbtv
-Version: 0.1.5
+Version: 0.1.6
 Summary: console database client
 Home-page: https://github.com/lakdemon/TUIDBTV
 License: MIT
 Author: lakdemon
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```


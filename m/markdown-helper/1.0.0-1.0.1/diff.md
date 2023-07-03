# Comparing `tmp/markdown_helper-1.0.0.tar.gz` & `tmp/markdown_helper-1.0.1.tar.gz`

## Comparing `markdown_helper-1.0.0.tar` & `markdown_helper-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0    13862 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/src/markdown_helper/__init__.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/tests/test_markdown.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/LICENSE
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 markdown_helper-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.coveragerc
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/EXAMPLE.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/SECURITY.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/src/markdown_helper/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/tests/test_markdown.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/PKG-INFO
```

### Comparing `markdown_helper-1.0.0/.github/workflows/pylint.yml` & `markdown_helper-1.0.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.0/.github/workflows/python-publish.yml` & `markdown_helper-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.0/src/markdown_helper/__init__.py` & `markdown_helper-1.0.1/src/markdown_helper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,29 @@
 
     def remap(self):
         """Remap values in the table based on the custom_map"""
         for header, value_map in self.custom_map.items():
             for row in self.rows:
                 row[header] = value_map.get(row[header], row[header])
 
+    def add_rows(self, rows: list[dict[str, str | int | float | bool]]):
+        """Add multiple rows to the table.
+        
+        Args:
+            rows (list[dict[str, str | int | float | bool]]): List of rows to add
+        """
+        for row in rows:
+            self.add_row(row)
+
     def add_row(self, row: dict[str, str | int | float | bool]):
-        """Add a row to the table."""
+        """Add a row to the table.
+        
+        Args:
+            row (dict[str, str | int | float | bool]): Row to add
+        """
 
         # Check that all the keys in the row are in the headers
         for key in row.keys():
             if key not in self.headers:
                 if self.flexible_headers:
                     self.headers.append(key)
                 else:
@@ -364,37 +377,49 @@
                 print(
                     f"Warning: File {filename} already exists and will be overwritten"
                 )
             else:
                 raise ValueError(f"File {filename} already exists")
         self.filename = filename
 
-    def add_section(self, section: Section):
+    def add_section(self, section: Section | str):
         """Add a section to the document.
 
         Args:
             section (Section): Section to add to the document.
         """
-        self.sections[section.title.text] = section
+        if isinstance(section, str):
+            new_section = Section(section)
+        elif isinstance(section, Section):
+            new_section = section
+        else:
+            raise TypeError(
+                f"Section must be of type Section or str, not {type(section)}"
+            )
+
+        self.sections[new_section.title.text] = new_section
+        return new_section
 
     def get_document(self) -> str:
         """Get the document as a string."""
         document = f"# {self.title}\n"
         if self.generate_table_of_contents:
             document += "## Table of Contents\n"
             for section in self.sections.values():
                 document += (
-                    f"* [{section.title}](#{section.title.text.lower().replace(' ', '-')})\n"
+                    f"* [{section.title.text}](#{section.title.text.lower().replace(' ', '-')})\n"
                 )
         for section in self.sections.values():
             document += str(section)
         return document
 
-    def save(self):
+    def save(self, **kwargs):
         """Save the document to a file."""
+        if kwargs.get("filename"):
+            self.filename = kwargs.get("filename", "")
         with open(self.filename, "w", encoding="utf-8") as file_output:
             file_output.write(self.get_document())
 
     def __str__(self):
         return self.get_document()
 
     def __repr__(self):
```

### Comparing `markdown_helper-1.0.0/tests/test_markdown.py` & `markdown_helper-1.0.1/tests/test_markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
 This file contains the pytest tests for the markdown_helper.py file.
 """
-import markdown_helper as markdown  # pylint: disable=import-error
-
-
+try:
+    from src import markdown_helper as markdown
+except ModuleNotFoundError:
+    try:
+        import markdown_helper as markdown
+    except ModuleNotFoundError:
+        from ..src import markdown_helper as markdown # pylint: disable=import-error, relative-beyond-top-level
 def test_ordered_list():
     """
     This function tests the markdown.List class.
     """
     list_1: markdown.List = markdown.List(["item 1", "item 2", "item 3"], ordered=True)
     assert (
         str(list_1) == "1. item 1\n2. item 2\n3. item 3\n"
```

### Comparing `markdown_helper-1.0.0/.gitignore` & `markdown_helper-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.0/LICENSE` & `markdown_helper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.0/pyproject.toml` & `markdown_helper-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "markdown_helper"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Arttu Mahlakaarto", email="arttu.mahlakaarto@gmail.com" },
 ]
 description = "A simple markdown helper"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.10"
```


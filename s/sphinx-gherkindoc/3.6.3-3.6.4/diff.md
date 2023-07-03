# Comparing `tmp/sphinx_gherkindoc-3.6.3.tar.gz` & `tmp/sphinx_gherkindoc-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_gherkindoc-3.6.3.tar", max compression
+gzip compressed data, was "sphinx_gherkindoc-3.6.4.tar", max compression
```

## Comparing `sphinx_gherkindoc-3.6.3.tar` & `sphinx_gherkindoc-3.6.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     9840 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/README.rst
--rw-r--r--   0        0        0     2716 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/pyproject.toml
--rw-r--r--   0        0        0       75 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/__init__.py
--rw-r--r--   0        0        0    12906 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/cli.py
--rw-r--r--   0        0        0     3067 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/files.py
--rw-r--r--   0        0        0     2733 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/glossary.py
--rw-r--r--   0        0        0     1208 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/__init__.py
--rw-r--r--   0        0        0      982 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/base.py
--rw-r--r--   0        0        0     1570 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/behave.py
--rw-r--r--   0        0        0     5574 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/pytest_bdd.py
--rw-r--r--   0        0        0     2632 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/sample-conf.py
--rw-r--r--   0        0        0    10635 2023-02-22 01:08:14.788714 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/utils.py
--rw-r--r--   0        0        0    15544 2023-02-22 01:08:14.792715 sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/writer.py
--rw-r--r--   0        0        0    11264 2023-02-22 01:09:00.664338 sphinx_gherkindoc-3.6.3/setup.py
--rw-r--r--   0        0        0    10859 2023-02-22 01:09:00.665351 sphinx_gherkindoc-3.6.3/PKG-INFO
+-rw-r--r--   0        0        0     9840 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/README.rst
+-rw-r--r--   0        0        0     2716 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/__init__.py
+-rw-r--r--   0        0        0    13166 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/cli.py
+-rw-r--r--   0        0        0     3067 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/files.py
+-rw-r--r--   0        0        0     3324 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/glossary.py
+-rw-r--r--   0        0        0     1208 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/__init__.py
+-rw-r--r--   0        0        0      982 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/base.py
+-rw-r--r--   0        0        0     1570 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/behave.py
+-rw-r--r--   0        0        0     5574 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/pytest_bdd.py
+-rw-r--r--   0        0        0     2632 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/sample-conf.py
+-rw-r--r--   0        0        0    10635 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/utils.py
+-rw-r--r--   0        0        0    15797 2023-07-03 16:03:02.034410 sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/writer.py
+-rw-r--r--   0        0        0    11264 2023-07-03 16:04:04.771973 sphinx_gherkindoc-3.6.4/setup.py
+-rw-r--r--   0        0        0    10859 2023-07-03 16:04:04.773268 sphinx_gherkindoc-3.6.4/PKG-INFO
```

### Comparing `sphinx_gherkindoc-3.6.3/README.rst` & `sphinx_gherkindoc-3.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/pyproject.toml` & `sphinx_gherkindoc-3.6.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx_gherkindoc"
-version = "3.6.3"
+version = "3.6.4"
 description = "A tool to convert Gherkin into Sphinx documentation"
 authors = ["Lewis Franklin <lewis.franklin@gmail.com>", "Doug Philips <dgou@mac.com>"]
 readme = "README.rst"
 homepage = "https://jolly-good-toolbelt.github.io/sphinx_gherkindoc/"
 documentation = "https://jolly-good-toolbelt.github.io/sphinx_gherkindoc/"
 repository = "https://github.com/jolly-good-toolbelt/sphinx_gherkindoc"
 license = "MIT"
```

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/cli.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     doc_project: str,
 ) -> None:
     """Process the supplied CLI args."""
     work_to_do = scan_tree(gherkin_path, args.private, args.exclude_patterns)
     maxtocdepth = args.maxtocdepth
     toc_name = args.toc_name
     step_glossary_name = args.step_glossary_name
+    group_step_glossary = args.group_step_glossary
     doc_project = args.doc_project
     root_path = gherkin_path.resolve().parent
 
     top_level_toc_filename = output_path / f"{toc_name}.rst"
 
     non_empty_dirs: Set[pathlib.Path] = set()
 
@@ -142,15 +143,15 @@
             toc_filename = top_level_toc_filename
         else:
             toc_filename = output_path / make_flat_name(current.path_list, is_dir=True)
         toc_file.write_to_file(toc_filename)
 
     if step_glossary_name:
         glossary_filename = output_path / f"{step_glossary_name}.rst"
-        glossary = make_steps_glossary(doc_project)
+        glossary = make_steps_glossary(doc_project, group_by=group_step_glossary)
 
         if args.dry_run:
             verbose("No glossary generated")
             return
 
         if glossary is None:
             print("No steps to include in the glossary: no glossary generated")
@@ -204,14 +205,21 @@
         "-G",
         "--step-glossary-name",
         default=None,
         help="Include steps glossary under the given name."
         " If not specified, no glossary will be created.",
     )
     parser.add_argument(
+        "-T",
+        "--group-step-glossary",
+        action="store_true",
+        default=False,
+        help="Group step glossary by step type",
+    )
+    parser.add_argument(
         "--integrate-background",
         action="store_true",
         help=(
             "Remove all references to Background, "
             "and integrate the steps into each scenario."
         ),
     )
```

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/files.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/files.py`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/glossary.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/glossary.py`

 * *Files 27% similar despite different names*

```diff
@@ -41,38 +41,54 @@
         """Compare the location and step lengths for equality."""
         if not isinstance(other, GlossaryEntry):
             return NotImplemented
         return self.tuple_len() == other.tuple_len()
 
 
 step_glossary: DefaultDict[str, GlossaryEntry] = defaultdict(GlossaryEntry)
+step_glossary_grouped: DefaultDict[str, DefaultDict[str, GlossaryEntry]] = defaultdict(
+    lambda: defaultdict(GlossaryEntry)
+)
 
 
-def make_steps_glossary(project_name: str) -> Optional[SphinxWriter]:
+def make_steps_glossary(
+    project_name: str, group_by: bool = False
+) -> Optional[SphinxWriter]:
     """Return SphinxWriter containing the step glossary information, if any."""
 
-    if not step_glossary:
+    if not step_glossary and not step_glossary_grouped:
         return None
 
     glossary = SphinxWriter()
     glossary.create_section(1, f"{project_name} Glossary")
 
-    master_step_names = {
-        name for gloss in step_glossary.values() for name in gloss.step_set
-    }
-    for term in sorted(master_step_names):
+    if group_by:
+        glossary.create_section(2, "Group By")
+
+        for step_type, glossary_group in step_glossary_grouped.items():
+            glossary.create_section(3, f"{step_type}")
+            _step_glossary(glossary, glossary_group)
+    else:
+        _step_glossary(glossary, step_glossary)
+
+    return glossary
+
+
+def _step_glossary(
+    glossary: SphinxWriter, glossary_group: DefaultDict[str, GlossaryEntry]
+) -> None:
+    step_names = {name for gloss in glossary_group.values() for name in gloss.step_set}
+    for term in sorted(step_names):
         glossary.add_output(f"- :term:`{rst_escape(term, slash_escape=True)}`")
 
     glossary.blank_line()
     glossary.add_output(".. glossary::")
-    for entry in sorted(step_glossary.values(), reverse=True):
+    for entry in sorted(glossary_group.values(), reverse=True):
         for term in sorted(entry.step_set):
             glossary.add_output(
                 rst_escape(term, slash_escape=True), indent_by=INDENT_DEPTH
             )
 
-        for location, line_numbers in sorted(entry.locations.items()):
-            definition = f"| {location} {', '.join(map(str, sorted(line_numbers)))}"
-            glossary.add_output(definition, indent_by=INDENT_DEPTH * 2)
-        glossary.blank_line()
-
-    return glossary
+            for location, line_numbers in sorted(entry.locations.items()):
+                definition = f"| {location} {', '.join(map(str, sorted(line_numbers)))}"
+                glossary.add_output(definition, indent_by=INDENT_DEPTH * 2)
+            glossary.blank_line()
```

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/__init__.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/base.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/base.py`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/behave.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/behave.py`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/parsers/pytest_bdd.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/parsers/pytest_bdd.py`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/sample-conf.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/sample-conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/utils.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_gherkindoc-3.6.3/sphinx_gherkindoc/writer.py` & `sphinx_gherkindoc-3.6.4/sphinx_gherkindoc/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Callable, List, Optional, Union
 
 import behave.parser
 import behave.model
 import behave.model_core
 
 from .files import is_rst_file
-from .glossary import step_glossary
+from .glossary import step_glossary, step_glossary_grouped
 from .parsers import parsers, ClassWithExamples
 from .utils import (
     display_name,
     make_flat_name,
     INDENT_DEPTH,
     rst_escape,
     SphinxWriter,
@@ -304,14 +304,19 @@
     def steps(steps: List[behave.model.Step], step_format: str = "{}") -> None:
         for step in steps:
             step_glossary[step.name.lower()].add_reference(
                 step.name,
                 pathlib.Path(step.filename).resolve().relative_to(root_path),
                 step.line,
             )
+            step_glossary_grouped[step.step_type][step.name.lower()].add_reference(
+                step.name,
+                pathlib.Path(step.filename).resolve().relative_to(root_path),
+                step.line,
+            )
             formatted_step = format_step(step, step_format)
             output_file.add_output(f"| {formatted_step}")
             if step.table:
                 output_file.blank_line()
                 table(step.table, inline=True)
                 output_file.blank_line()
             if step.text:
```

### Comparing `sphinx_gherkindoc-3.6.3/setup.py` & `sphinx_gherkindoc-3.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 entry_points = \
 {'console_scripts': ['sphinx-gherkinconfig = sphinx_gherkindoc.cli:config',
                      'sphinx-gherkindoc = sphinx_gherkindoc.cli:main']}
 
 setup_kwargs = {
     'name': 'sphinx-gherkindoc',
-    'version': '3.6.3',
+    'version': '3.6.4',
     'description': 'A tool to convert Gherkin into Sphinx documentation',
     'long_description': 'sphinx-gherkindoc\n=================\n\n``sphinx-gherkindoc`` brings Gherkin goodness\ninto the Sphinx/reStructuredText (rST) world.\n\nWhy should I use it?\n--------------------\n\n**Share your requirements with your larger team.**\nGherkin makes it easy for anyone to read requirements.\nSphinx makes Gherkin pretty enough to be readable.\n``sphinx-gherkindoc`` handles converting flat-text feature files\ninto easy to read documents you won\'t cringe to share with your larger team.\n\n**Easily see what steps you have and where you are using them.**\n``sphinx-gherkindoc`` can create a glossary of your steps.\nThis helps makes it easy to:\n\n   * find steps to reuse\n   * notice similar steps that might be duplicates or unintended variations\n   * see patterns that you might exploit to reduce the number of steps you have\n   * find out where and which feature files would be affected\n     if a step\'s wording or implementation changes\n\n\nHow does it do that?\n--------------------\n\n``sphinx-gherkindoc`` recursively scans a given directory\nto find all the feature and markup files,\nand converts them into files\nthat can be included in Sphinx-based documentation.\nThis script was inspired by ``sphinx-apidoc``\nwhich does a similar thing for source code.\n\n.. Note::\n\n    This tool only creates the rST inputs for a sphinx document run,\n    you still need to fit these files\n    in to your larger documentation building process yourself.\n\nFor specific details on the command line options,\nplease consult the ``--help`` output.\nMost command line options mirror their counterpart in ``sphinx-apidoc``.\n\nFor the most basic usage, an input (``<gherkin_path>``)\nand output (``<output_path>``) path must be provided.\nThe files put in to the ``<output_path>``\ncan be incorporated into any larger documentation,\ncreated by any means.\n\nAdditionally, a list of ``fnmatch``-compatible patterns can be added\nto the command line,\nto indicate directories to be excluded from processing.\n\nOne notable addition is the step glossary(``-G``, ``--step-glossary``).\nThe step glossary command line option causes ``sphinx-gherkindoc``\nto create the named file in the ``<output_path>`` directory.\nThe step glossary content is formatted into two lists:\n\n   * A list of all the steps found, in alphabetical order.\n     Each item in this list is a link to its details in the second list.\n   * A list of the steps showing the file names and line numbers\n     where they are used.\n     This list is in order by the most number of uses first.\n\n\nHow are my files converted?\n---------------------------\n\nWhen scanning the ``<gherkin_path>`` directory tree,\n``sphinx-gherkindoc`` will do the following:\n\n   * Feature files found\n     are processed into rST files in the ``<output_path>`` directory.\n   * Directories will be converted to Sphinx Table of Contents (TOC) files that\n     link to any feature files in the same directory,\n     and to any TOC files from direct subdirectories.\n   * Any rST files found in a directory have their contents copied\n     to the front of the TOC file for that directory.\n     If more than one rST file is found in a directory,\n     they are processed in sort order.\n   * If no rST files are found in a directory,\n     then a header for the TOC is created based\n     on the contents of a ``display_name.txt`` file, if present,\n     or the name of the directory.\n   * Any MarkDown (md) files are referenced\n     from the TOC file for the directory they are in.\n   * Directories with no feature, rST, or md files are pruned,\n     recursively upwards.\n\n\nThe meat\'n\'potatoes will be your feature files.\nPut rST files next to your feature files\nto present context and additional helpful material.\nIf any rST files are in the same directory,\nthey should also contain any appropriate headers\nand other such formatting.\n``sphinx-gherkindoc`` will only create (minimal) headers when\nthere are no rST files present at all.\n\n\nExamples\n--------\n\nDisclaimer: This `is not` a tutorial on how to use or configure Sphinx.\nIt `is` some common ways you can use ``sphinx-gherkindoc``\nas part of your documentation generation.\nReminder if you skipped all that stuff above:\n``--help`` will show you the default values\nwhen command line options aren\'t used.\n\nConventions - Sphinx-based document production usually uses two directories:\n\n    * ``_docs`` - the working directory where we put all the rST files\n      from the various tools as we are building documents.\n      This directory shoud not be checked in to version control\n      and should only contain files created by a documentation run.\n    * ``docs`` - the output directory for a documentation run.\n      For example, this is where ``index.html`` is found\n      when building HTML docs, etc.\n      This directory should not be checked in to version control\n      as it contains only derived and processed files.\n\n\n1. Convert feature files to rST;\n   process all feature and document files\n   in/under ``feature/root/directory-here`` into the ``_docs`` directory\n   using all the defaults::\n\n       sphinx-gherkindoc feature/root/directory-here _docs\n\n2. Same as above,\n   but also create a step glossary file ``my_step_glossary`` in ``_docs``::\n\n       sphinx-gherkindoc -G my_step_glossary feature/root/directory-here _docs\n\n3. Experiment!\nOnce you have the 2nd step working\nand integrated in to your document building process,\nyou may find you want to tweak the results some.\nIt\'s a lot easier to do that `after` you have the basic process working.\nExperiment with the other optional parameters\nto get the effect(s) you want.\n\nSpecial Instructions for User Integrated Functionality\n------------------------------------------------------\n\nThere are certain parts of ``sphinx-gherkindoc``\nthat can be controlled by external, user defined code.\nThis can be done via a plugin or command-line argument.\n\nHere are the places where this can be used:\n\n- Any tag or step can be converted into an anonymous link.\n  The converter needs to be a single function\n  that accepts a single string parameter\n  (the tag or full step with keyword)\n  and returns a URL if the entry should include a link\n  or an empty string if not.\n  Note that, in the case of steps,\n  only the step text after the keyword\n  will be converted into a link.\n  In addition to examples below,\n  there is legacy support for a ``url`` plugin key\n  that is equivalent to the ``tag_url`` key.\n- Directory names can be converted into display names\n  similarly to how ``display_name.txt`` works.\n  This converter also needs to be a single function\n  that accepts a single string parameter, the directory name,\n  and returns a display name string for that directory.\n\nIn order to register the plugin for a ``poetry``-based project::\n\n    [tools.poetry.plugins."parsers"]\n    tag_url = "my_custom_library.parse:optional_url_from_tag"\n    step_url = "my_custom_library.parse:optional_url_from_step"\n    dir_display_name = "my_custom_library.parse:optional_display_name_from_dir"\n\nIn order to register the plugin for a ``setup.py``-based project::\n\n    setup(\n        ...\n        entry_points={\n            \'parsers\': [\n                \'tag_url = my_custom_library.parse:optional_url_from_tag\',\n                \'step_url = my_custom_library.parse:optional_url_from_step\',\n                \'dir_display_name = my_custom_library.parse:optional_display_name_from_dir\'\n            ]\n        }\n    )\n\nIn order to use the parser via command line,\nthe ``--url_from-tag`` and ``--display-name-from-dir`` flags should be used.\nThe provided string should be be formatted ``<library>:<method_name>``\n\nFiltering Included Features/Scenarios By Tag\n--------------------------------------------\n\nIf you\'d like to build documentation for only a subset of features/scenarios,\nyou can include and exclude them by tags.\n\nJust use the ``--include-tags`` and/or ``--exclude-tags`` flags.\nRun ``sphinx-gherkindoc --help`` for usage info.\n\nFormatting Options\n------------------\n\nIf you connect a ``.css`` file to your generated documentation,\nvia the ``_static`` folder that is supported by Sphinx,\nyou can make use of certain classes to format parts of the Gherkin\nhowever you so choose!\n\nHere are the available CSS classes:\n\n- ``gherkin-step-keyword``\n- ``gherkin-feature-keyword``\n- ``gherkin-feature-content``\n- ``gherkin-feature-description``\n- ``gherkin-background-keyword``\n- ``gherkin-background-content``\n- ``gherkin-scenario-keyword``\n- ``gherkin-scenario-content``\n- ``gherkin-scenario-description``\n- ``gherkin-scenario-outline-keyword``\n- ``gherkin-scenario-outline-content``\n- ``gherkin-scenario-outline-description``\n- ``gherkin-examples-keyword``\n- ``gherkin-examples-content``\n- ``gherkin-tag-keyword``\n\n\nExample ``.css`` File::\n\n    .gherkin-step-keyword {\n        font-weight: bold;\n        color: red;\n    }\n\n    .gherkin-feature-keyword, .gherkin-background-keyword {\n        color: yellow;\n    }\n    .gherkin-feature-content {\n        color: green;\n    }\n    .gherkin-feature-description {\n        color: blue;\n    }\n\n    .gherkin-scenario-keyword, .gherkin-scenario-outline-keyword {\n        color: indigo;\n    }\n    .gherkin-scenario-content, .gherkin-scenario-outline-content {\n        color: violet;\n    }\n    .gherkin-scenario-description, .gherkin-scenario-outline-description {\n        color: purple;\n    }\n\n    .gherkin-examples-keyword {\n        color: gold;\n    }\n    .gherkin-examples-content {\n        color: goldenrod;\n    }\n\n    .gherkin-tag-keyword {\n        color: salmon;\n    }\n\n.. note::\n\n    Your ``.css`` can have any name. As long as it is in the ``_static`` folder,\n    Sphinx will integrate it into the generated HTML.\n    Sphinx officially documents `adding a CSS file via the Application API`_\n\n\n.. _`adding a CSS file via the Application API`: https://www.sphinx-doc.org/en/master/extdev/appapi.html#sphinx.application.Sphinx.add_css_file\n',
     'author': 'Lewis Franklin',
     'author_email': 'lewis.franklin@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://jolly-good-toolbelt.github.io/sphinx_gherkindoc/',
```

### Comparing `sphinx_gherkindoc-3.6.3/PKG-INFO` & `sphinx_gherkindoc-3.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-gherkindoc
-Version: 3.6.3
+Version: 3.6.4
 Summary: A tool to convert Gherkin into Sphinx documentation
 Home-page: https://jolly-good-toolbelt.github.io/sphinx_gherkindoc/
 License: MIT
 Author: Lewis Franklin
 Author-email: lewis.franklin@gmail.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


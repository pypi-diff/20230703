# Comparing `tmp/pptreport-1.1.0.tar.gz` & `tmp/pptreport-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptreport-1.1.0.tar", last modified: Fri Jun 23 14:14:22 2023, max compression
+gzip compressed data, was "pptreport-1.1.1.tar", last modified: Mon Jul  3 17:55:26 2023, max compression
```

## Comparing `pptreport-1.1.0.tar` & `pptreport-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.422603 pptreport-1.1.0/
--rwxr-xr-x   0 root         (0) root         (0)      687 2023-06-23 14:01:25.000000 pptreport-1.1.0/CHANGES.rst
--rwxr-xr-x   0 root         (0) root         (0)     1070 2023-04-21 09:55:42.000000 pptreport-1.1.0/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       21 2023-06-23 13:24:22.000000 pptreport-1.1.0/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)      717 2023-06-23 14:14:22.585316 pptreport-1.1.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      190 2023-06-23 13:24:22.000000 pptreport-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.506151 pptreport-1.1.0/pptreport/
--rwxr-xr-x   0 root         (0) root         (0)      421 2023-06-16 15:34:29.000000 pptreport-1.1.0/pptreport/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       23 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/_version.py
--rwxr-xr-x   0 root         (0) root         (0)    25760 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/box.py
--rwxr-xr-x   0 root         (0) root         (0)     2427 2023-06-23 13:24:22.000000 pptreport-1.1.0/pptreport/cli.py
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.553440 pptreport-1.1.0/pptreport/fonts/
--rwxr-xr-x   0 root         (0) root         (0)     4483 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OFL.txt
--rwxr-xr-x   0 root         (0) root         (0)   129784 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OpenSans-Bold.ttf
--rwxr-xr-x   0 root         (0) root         (0)   135380 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OpenSans-Italic.ttf
--rwxr-xr-x   0 root         (0) root         (0)   129796 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OpenSans-Regular.ttf
--rwxr-xr-x   0 root         (0) root         (0)    48318 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/powerpointreport.py
--rwxr-xr-x   0 root         (0) root         (0)    17996 2023-06-23 13:24:22.000000 pptreport-1.1.0/pptreport/slide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.521777 pptreport-1.1.0/pptreport.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)      717 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      642 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       49 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/entry_points.txt
--rwxr-xr-x   0 root         (0) root         (0)       66 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       10 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       94 2023-04-21 09:55:42.000000 pptreport-1.1.0/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)     1012 2023-06-23 14:14:22.585316 pptreport-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.569094 pptreport-1.1.0/tests/
--rwxr-xr-x   0 root         (0) root         (0)     4130 2023-06-23 14:01:26.000000 pptreport-1.1.0/tests/test_box.py
--rwxr-xr-x   0 root         (0) root         (0)     5830 2023-06-23 13:24:23.000000 pptreport-1.1.0/tests/test_classes.py
--rwxr-xr-x   0 root         (0) root         (0)     1732 2023-06-23 14:01:26.000000 pptreport-1.1.0/tests/test_cli.py
--rwxr-xr-x   0 root         (0) root         (0)    18819 2023-06-23 14:01:26.000000 pptreport-1.1.0/tests/test_input.py
--rwxr-xr-x   0 root         (0) root         (0)     2533 2023-06-23 13:24:23.000000 pptreport-1.1.0/tests/test_slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:55:25.912447 pptreport-1.1.1/
+-rwxr-xr-x   0 root         (0) root         (0)      955 2023-07-03 17:53:50.000000 pptreport-1.1.1/CHANGES.rst
+-rwxr-xr-x   0 root         (0) root         (0)     1070 2023-04-21 09:55:42.000000 pptreport-1.1.1/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       21 2023-06-23 13:24:22.000000 pptreport-1.1.1/MANIFEST.in
+-rwxr-xr-x   0 root         (0) root         (0)      717 2023-07-03 17:55:26.039321 pptreport-1.1.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      190 2023-06-23 13:24:22.000000 pptreport-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:55:25.960184 pptreport-1.1.1/pptreport/
+-rwxr-xr-x   0 root         (0) root         (0)      421 2023-06-16 15:34:29.000000 pptreport-1.1.1/pptreport/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       23 2023-07-03 17:53:50.000000 pptreport-1.1.1/pptreport/_version.py
+-rwxr-xr-x   0 root         (0) root         (0)    25765 2023-07-03 17:53:50.000000 pptreport-1.1.1/pptreport/box.py
+-rwxr-xr-x   0 root         (0) root         (0)     2427 2023-06-23 13:24:22.000000 pptreport-1.1.1/pptreport/cli.py
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-03 12:19:42.000000 pptreport-1.1.1/pptreport/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:55:26.023692 pptreport-1.1.1/pptreport/fonts/
+-rwxr-xr-x   0 root         (0) root         (0)     4483 2023-04-21 09:55:42.000000 pptreport-1.1.1/pptreport/fonts/OFL.txt
+-rwxr-xr-x   0 root         (0) root         (0)   129784 2023-04-21 09:55:42.000000 pptreport-1.1.1/pptreport/fonts/OpenSans-Bold.ttf
+-rwxr-xr-x   0 root         (0) root         (0)   135380 2023-04-21 09:55:42.000000 pptreport-1.1.1/pptreport/fonts/OpenSans-Italic.ttf
+-rwxr-xr-x   0 root         (0) root         (0)   129796 2023-04-21 09:55:42.000000 pptreport-1.1.1/pptreport/fonts/OpenSans-Regular.ttf
+-rwxr-xr-x   0 root         (0) root         (0)    53842 2023-07-03 17:53:50.000000 pptreport-1.1.1/pptreport/powerpointreport.py
+-rwxr-xr-x   0 root         (0) root         (0)    17996 2023-06-23 13:24:22.000000 pptreport-1.1.1/pptreport/slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:55:25.991454 pptreport-1.1.1/pptreport.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)      717 2023-07-03 17:55:25.000000 pptreport-1.1.1/pptreport.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      642 2023-07-03 17:55:25.000000 pptreport-1.1.1/pptreport.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-07-03 17:55:25.000000 pptreport-1.1.1/pptreport.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       49 2023-07-03 17:55:25.000000 pptreport-1.1.1/pptreport.egg-info/entry_points.txt
+-rwxr-xr-x   0 root         (0) root         (0)       66 2023-07-03 17:55:25.000000 pptreport-1.1.1/pptreport.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       10 2023-07-03 17:55:25.000000 pptreport-1.1.1/pptreport.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       94 2023-04-21 09:55:42.000000 pptreport-1.1.1/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)     1012 2023-07-03 17:55:26.039321 pptreport-1.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:55:26.039321 pptreport-1.1.1/tests/
+-rwxr-xr-x   0 root         (0) root         (0)     4130 2023-07-03 12:19:42.000000 pptreport-1.1.1/tests/test_box.py
+-rwxr-xr-x   0 root         (0) root         (0)     5830 2023-06-23 13:24:23.000000 pptreport-1.1.1/tests/test_classes.py
+-rwxr-xr-x   0 root         (0) root         (0)     1732 2023-07-03 12:19:42.000000 pptreport-1.1.1/tests/test_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)    21765 2023-07-03 17:53:50.000000 pptreport-1.1.1/tests/test_input.py
+-rwxr-xr-x   0 root         (0) root         (0)     2533 2023-06-23 13:24:23.000000 pptreport-1.1.1/tests/test_slide.py
```

### Comparing `pptreport-1.1.0/LICENSE` & `pptreport-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/PKG-INFO` & `pptreport-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptreport
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/loosolab/pptreport
 Author: Mette Bentsen
 Author-email: mette.bentsen@mpi-bn.mpg.de
 License: MIT
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
```

### Comparing `pptreport-1.1.0/pptreport/box.py` & `pptreport-1.1.1/pptreport/box.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
 
         # Resize image if it is too large
         if image_pixels > max_pixels:
 
             image_ratio = im_width / im_height
             new_height = int(np.sqrt(max_pixels / image_ratio))   # height * height * (width / height) = max_pixels
             new_width = int(new_height * image_ratio)
-            self.logger.warning(f"Image '{filename}' is larger than max_pixels={max_pixels} ({im_height}*{im_width}={image_pixels}). Adjust 'max_pixels' to skip resizing. Resizing to size {new_height}*{new_width}...")
+            self.logger.warning(f"Image '{filename}' is larger than max_pixels={int(max_pixels)} ({im_height}*{im_width}={image_pixels}). Adjust 'max_pixels' to skip resizing. Resizing to size {new_height}*{new_width}...")
 
             im = im.resize((new_width, new_height), Image.LANCZOS)
 
             # Create temporary file
             temp_name = next(tempfile._get_candidate_names()) + ".png"
             temp_dir = tempfile.gettempdir()
             temp_file = os.path.join(temp_dir, temp_name)
```

### Comparing `pptreport-1.1.0/pptreport/cli.py` & `pptreport-1.1.1/pptreport/cli.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/pptreport/fonts/OFL.txt` & `pptreport-1.1.1/pptreport/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/pptreport/fonts/OpenSans-Bold.ttf` & `pptreport-1.1.1/pptreport/fonts/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/pptreport/fonts/OpenSans-Italic.ttf` & `pptreport-1.1.1/pptreport/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/pptreport/fonts/OpenSans-Regular.ttf` & `pptreport-1.1.1/pptreport/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/pptreport/powerpointreport.py` & `pptreport-1.1.1/pptreport/powerpointreport.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,24 @@
     # Check if string is a 1-word string with a dot in it and an extension after the dot
     if len(string.split()) == 1 and "." in string and string.rsplit(".", 1)[1]:
         return True
     else:
         return False  # string does not look like a filename
 
 
+def _regex_has_group(pattern):
+    """ Check if the pattern contains any capturing groups """
+
+    try:
+        match = re.search(r'(\(.*?\))', pattern)
+        return bool(match)
+    except re.error:
+        return False
+
+
 ###############################################################################
 # -------------------- Class for building presentation ---------------------- #
 ###############################################################################
 
 class PowerPointReport():
     """ Class for building a PowerPoint presentation """
 
@@ -503,19 +513,34 @@
         # If input was None, replace with default parameters from upper presentation
         _fill_dict(parameters, self._default_slide_parameters)
         self.logger.debug("Final slide parameters: {}".format(parameters))
 
         # Add slides dependent on content type
         if "grouped_content" in parameters:
 
-            content_per_group = self._get_paired_content(parameters["grouped_content"])
-            self.logger.debug("Grouped content: {}".format(content_per_group))
+            content_per_group = self._get_paired_content(parameters["grouped_content"], parameters["missing_file"])
+
+            # If no grouped content was found, add empty slide if empty_slide is "keep"
+            if len(content_per_group) == 0 and parameters["empty_slide"] == "keep":
+                self.logger.warning(f"No files found for grouped_content: '{parameters['grouped_content']}, but empty_slide == 'keep'. Adding slide without content. Set empty_slide == 'skip' to skip slides without content.")
+                slide = self._setup_slide(parameters)
+
+                if parameters["missing_file"] == "text":
+                    slide.content = parameters["grouped_content"]
+                elif parameters["missing_file"] == "empty":
+                    slide.content = [None if _looks_like_filename(element) else element for element in parameters["grouped_content"]]
+                else:  # missing_file == "skip"
+                    slide.content = [element for element in parameters["grouped_content"] if not _looks_like_filename(element)]  # only skip filenames, not text
+
+                slide._filenames = slide.content
+                slide._fill_slide()
+                return
 
-            tmp_files = []
             # Create one slide per group
+            tmp_files = []
             for group, content in content_per_group.items():
 
                 # Save original filenames / content
                 filenames = content[:]
 
                 # Convert pdf to png files
                 for idx, element in enumerate(content):
@@ -832,14 +857,17 @@
 
         Returns
         -------
         matched_files : list of str
             List of files that match the regex pattern.
         """
 
+        if pattern is None:
+            return []
+
         # Remove ( and ) from regex as they are only used to group regex later
         pattern_clean = re.sub(r'(?<!\\)[\(\)]', '', pattern)
         self.logger.debug(f"Finding files for possible regex pattern: {pattern_clean}")
 
         # Find highest existing directory (as some directories might be regex)
         directory = os.path.dirname(pattern_clean)
         while not os.path.exists(directory):
@@ -865,70 +893,135 @@
             if pattern_compiled.match(file):
                 matched_files.append(file)
 
         self.logger.debug(f"Found files: {matched_files}")
 
         return matched_files
 
-    def _get_paired_content(self, raw_content):
+    def _get_paired_content(self, raw_content, missing_file="raise"):
         """ Get content per group from a list of regex patterns.
 
         Parameters
         ----------
         raw_content : list of str
             List of regex patterns. Each pattern should contain one group.
+        missing_file : str, optional
+            How to deal with missing files. Options are 'raise', 'empty', 'text' or 'skip'. Default is 'raise'.
 
         Returns
         -------
         content_per_group : dict
             Dictionary with group names as keys and lists of content as values.
         """
 
         # Search for regex groups
         group_content = {}  # dict of lists of content input
-        n_group_matches = 0
         for i, pattern in enumerate(raw_content):
             group_content[i] = {}
 
+            # Find all files that match the regex
             files = self._glob_regex(pattern)
 
+            # Check if any files were found and raise error if none were found for file-looking patterns
+            if len(files) == 0 and _looks_like_filename(pattern) and missing_file == "raise":
+                raise FileNotFoundError(f"No files were found for the pattern: '{pattern}'. Missing_file is set to 'raise'. Adjust the missing_file parameter to 'empty', 'text' or 'skip' to avoid this error.")
+
             # Find all groups within the regex
+            warning = 0
             for fil in files:
 
                 m = re.match(pattern, fil)
                 if m:  # if there was a match
 
                     groups = m.groups()
-                    if len(groups) == 0:
-                        raise ValueError(f"Invalid value for 'grouped_content' parameter. Regex {pattern} does not contain any groups.")
-                    elif len(groups) > 1:
+                    if len(groups) > 1:
                         raise ValueError(f"Invalid value for 'grouped_content' parameter. Regex {pattern} contains more than one group.")
-                    group = groups[0]
+                    elif len(groups) == 1:
+                        group = groups[0]
+                        group_content[i][group] = fil  # Save the file to the group
+
+                    else:  # 0 groups
+                        if warning == 0:
+                            s = f"Pattern '{pattern}' does not contain a capturing group (e.g. '(\\w+)_plot.pdf'), but "
+                            s += "capturing groups are needed to automatically expand content to multiple slides. "
+                            if len(files) > 1:
+                                s += f"The pattern matches multiple files, but only one file ('{files[0]}') will be shown. "
+                            s += "This content will appear on all expanded slides - please adjust the pattern if needed."
+                            self.logger.warning(s)
+                            warning += 1  # ensure warning is only printed once per pattern
 
-                    # Save the file to the group
-                    group_content[i][group] = fil
-                    n_group_matches += 1
-
-        # Check that at least one group was found
-        if n_group_matches == 0:
-            raise ValueError(f"Invalid value for 'grouped_content' parameter: {raw_content}. No groups were found for any of the regex patterns.")
+                        raw_content[i] = files[0]  # replace pattern with file
 
         # Collect all groups found
         all_regex_groups = sum([list(d.keys()) for d in group_content.values()], [])  # flatten list of lists
         all_regex_groups = natsorted(set(all_regex_groups))
         self.logger.debug(f"Found groups: {all_regex_groups}")
 
-        # If no groups were found for an element, add strings for each group
-        for i in group_content:
-            if len(group_content[i]) == 0:
+        # If no groups were found for an element, add strings for each group (.e.g. strings/files repeated for each slide)
+        content_per_group = {group: [] for group in all_regex_groups}
+        for i in group_content:  # index of raw_content
+            raw_input = raw_content[i]
+
+            if len(group_content[i]) == 0:  # no groups found
                 for group in all_regex_groups:
-                    group_content[i][group] = raw_content[i]
+                    content_per_group[group].append(raw_input)  # this is the same for each slide
+
+            else:
+                # Add content for each group with a file
+                for group in group_content[i].keys():
+                    content_per_group[group].append(group_content[i][group])
+
+                missing_groups = list(set(all_regex_groups) - set(group_content[i].keys()))
+                if len(missing_groups) > 0:
+
+                    if missing_file == "raise":
+                        s = f"Missing file(s) for grouped content pattern '{raw_input}' for group(s): {missing_groups}."
+                        s += " Please ensure that the file(s) exists or adjust 'missing_file' parameter to 'text'/'empty'/'skip' to prevent this error."
+                        raise FileNotFoundError(s)
+
+                    else:
+                        self.logger.debug(f"Missing file for index {i} for groups: {missing_groups}")
+                        for group in missing_groups:
+                            pattern = r"\((.*?)\)"
+                            element = re.sub(pattern, group, raw_input)
+                            content_per_group[group].append(element)  # fill group name into pattern group
+
+        # Check if files are missing for any group
+        warnings = []
+        for group in content_per_group:
+            to_skip = []
+            for i, element in enumerate(content_per_group[group]):
+                if _looks_like_filename(element) and not os.path.exists(element):
+                    if missing_file == "raise":
+                        raise FileNotFoundError(f"No file could be found for grouped input: '{element}'. Adjust pattern or set missing_file='empty'/'text'/'skip' to ignore the missing file.")
+                    elif missing_file == "empty":
+                        s = f"No file could be found for grouped input: '{element}'. Adding empty box."
+                        if s not in warnings:  # only print once
+                            self.logger.warning(s)
+                            warnings.append(s)
+                        content_per_group[group][i] = None  # empty box
+                    elif missing_file == "skip":
+                        s = f"No file could be found for grouped input: '{element}'. Skipping this element."
+                        if s not in warnings:  # only print once
+                            self.logger.warning(s)
+                            warnings.append(s)
+                        to_skip.append(i)
+                        continue  # skip this element
+                    elif missing_file == "text":
+                        s = f"No file could be found for grouped input: '{element}'. Adding this element as text."
+                        if s not in warnings:  # only print once
+                            self.logger.warning(s)
+                            warnings.append(s)
+                        # keep raw_input as is, as it will be added as text
+
+            for i in to_skip[::-1]:  # reverse order to not mess up indexing
+                del content_per_group[group][i]
 
         # Convert from group per element to element per group
-        content_per_group = {group: [group_content[i].get(group, None) for i in group_content] for group in all_regex_groups}
+        self.logger.debug(f"Content per group: {content_per_group}")
 
         return content_per_group
 
     # ------------------------------------------------------------------------ #
     # --------------------- Saving / loading presentations ---------------------
     # ------------------------------------------------------------------------ #
```

### Comparing `pptreport-1.1.0/pptreport/slide.py` & `pptreport-1.1.1/pptreport/slide.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/pptreport.egg-info/PKG-INFO` & `pptreport-1.1.1/pptreport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptreport
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/loosolab/pptreport
 Author: Mette Bentsen
 Author-email: mette.bentsen@mpi-bn.mpg.de
 License: MIT
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
```

### Comparing `pptreport-1.1.0/pptreport.egg-info/SOURCES.txt` & `pptreport-1.1.1/pptreport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/setup.cfg` & `pptreport-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/tests/test_box.py` & `pptreport-1.1.1/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/tests/test_classes.py` & `pptreport-1.1.1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/tests/test_cli.py` & `pptreport-1.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.1.0/tests/test_input.py` & `pptreport-1.1.1/tests/test_input.py`

 * *Files 14% similar despite different names*

```diff
@@ -112,24 +112,99 @@
     config = {"content": content}
     validate(config, valid)
 
 
 # ------------------------------------------------------------------- #
 # grouped content
 @pytest.mark.parametrize("grouped_content, valid",
-                         [(["string", content_dir + "colored_animals/(.*)_blue.jpg", content_dir + "colored_animals/(.*)_blue.jpg"], True),
-                          ([content_dir + "colored_animals/.*_blue.jpg", content_dir + "colored_animals/(.*)_blue.jpg"], False),  # no groups
+                         [(["string", content_dir + "colored_animals/(.*)_blue.jpg", content_dir + "colored_animals/(.*)_red.jpg"], True),
                           ([content_dir + "colored_animals/(.*)_(.*).jpg"], False),  # two groups
-                          (["no", "groups"], False),
-                          ("A text", False)])
+                          (["no", "groups"], True),  # no groups, but valid
+                          ("A text", False)])   # not a list
 def test_grouped_content(grouped_content, valid):
-    config = {"content": None, "grouped_content": grouped_content}
+    config = {"content": None, "grouped_content": grouped_content, "missing_file": "text"}
     validate(config, valid)
 
 
+def test_grouped_content_warning(caplog):
+    """ Test that a warning is written when no groups are found """
+    config = {"grouped_content": [content_dir + "colored_animals/.*_blue.jpg"],
+              "missing_file": "text"}
+
+    report = PowerPointReport()
+    report.add_slide(**config)
+    assert "WARNING" in caplog.text
+    assert "does not contain a capturing group" in caplog.text
+
+
+@pytest.mark.parametrize("missing_file", ["raise", "empty", "skip", "text"])
+def test_grouped_missing(caplog, missing_file):
+    """ Test that a warning is written when only some groups are found """
+
+    config = {"grouped_content": ["string",
+                                  content_dir + "colored_animals/(.*)_red.jpg",
+                                  content_dir + "colored_animals/(.*)_yellow.jpg",
+                                  content_dir + "colored_animals/(.*)_blue.jpg"],
+              "missing_file": missing_file}
+
+    report = PowerPointReport(verbosity=2)
+
+    if missing_file == "raise":
+        with pytest.raises(FileNotFoundError, match=r"Missing file\(s\) for grouped content pattern"):
+            report.add_slide(**config)
+    elif missing_file == "empty":
+        report.add_slide(**config)
+        assert "Adding empty box." in caplog.text
+    elif missing_file == "skip":
+        report.add_slide(**config)
+        assert "Skipping this element." in caplog.text
+    elif missing_file == "text":
+        report.add_slide(**config)
+        assert "Adding this element as text." in caplog.text
+
+
+@pytest.mark.parametrize("common", ["string",
+                                    content_dir + "colored_animals/dog_blue.jpg",
+                                    "non_existing_file.jpg"])
+def test_grouped_missing_common(caplog, common):
+    """ Test if non-grouped file is missing """
+
+    config = {"grouped_content": [common,
+                                  content_dir + "colored_animals/(.*)_red.jpg"],  # red animal is present in all groups
+              "missing_file": "raise"}
+
+    report = PowerPointReport()
+    if common == "non_existing_file.jpg":
+        with pytest.raises(FileNotFoundError, match=r"No files were found for the pattern"):
+            report.add_slide(**config)
+    else:
+        report.add_slide(**config)  # no error
+
+        if "dog_blue" in common:   # warning that file does not contain a group
+            assert "does not contain a capturing group " in caplog.text
+
+
+@pytest.mark.parametrize("empty_slide", ["keep", "skip"])
+def test_grouped_missing_empty(caplog, empty_slide):
+
+    config = {"grouped_content": ["string", "no_match(.)+"],
+              "missing_file": "skip",
+              "empty_slide": empty_slide}
+
+    report = PowerPointReport()
+    report.add_slide(**config)
+
+    if empty_slide == "keep":
+        assert "Adding slide without content." in caplog.text
+        assert len(report._slides) == 1
+
+    elif empty_slide == "skip":
+        assert len(report._slides) == 0
+
+
 # ------------------------------------------------------------------- #
 # Set title (all types can be converted to str)
 @pytest.mark.parametrize("title, valid",
                          [("A title", True),
                           (None, True),
                           (1, True),
                           (dict, True)])
```

### Comparing `pptreport-1.1.0/tests/test_slide.py` & `pptreport-1.1.1/tests/test_slide.py`

 * *Files identical despite different names*


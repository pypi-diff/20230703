# Comparing `tmp/discord-ansi-0.3.tar.gz` & `tmp/discord-ansi-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ansi-0.3.tar", last modified: Mon Jul  3 06:46:11 2023, max compression
+gzip compressed data, was "discord-ansi-0.4.tar", last modified: Mon Jul  3 06:49:03 2023, max compression
```

## Comparing `discord-ansi-0.3.tar` & `discord-ansi-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 06:46:11.945920 discord-ansi-0.3/
--rw-rw-rw-   0        0        0     3478 2023-07-03 06:46:11.945920 discord-ansi-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3300 2023-07-02 17:41:14.000000 discord-ansi-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 06:46:11.930295 discord-ansi-0.3/discord_ansi/
--rw-rw-rw-   0        0        0     3192 2023-07-03 06:45:51.000000 discord-ansi-0.3/discord_ansi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:46:11.945920 discord-ansi-0.3/discord_ansi.egg-info/
--rw-rw-rw-   0        0        0     3478 2023-07-03 06:46:11.000000 discord-ansi-0.3/discord_ansi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-07-03 06:46:11.000000 discord-ansi-0.3/discord_ansi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 06:46:11.000000 discord-ansi-0.3/discord_ansi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-03 06:06:35.000000 discord-ansi-0.3/discord_ansi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-07-03 06:46:11.000000 discord-ansi-0.3/discord_ansi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 06:46:11.000000 discord-ansi-0.3/discord_ansi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 06:46:11.945920 discord-ansi-0.3/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-07-03 06:46:00.000000 discord-ansi-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:49:03.795320 discord-ansi-0.4/
+-rw-rw-rw-   0        0        0     3478 2023-07-03 06:49:03.795320 discord-ansi-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3300 2023-07-02 17:41:14.000000 discord-ansi-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 06:49:03.779662 discord-ansi-0.4/discord_ansi/
+-rw-rw-rw-   0        0        0     3197 2023-07-03 06:48:02.000000 discord-ansi-0.4/discord_ansi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:49:03.795320 discord-ansi-0.4/discord_ansi.egg-info/
+-rw-rw-rw-   0        0        0     3478 2023-07-03 06:49:03.000000 discord-ansi-0.4/discord_ansi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-07-03 06:49:03.000000 discord-ansi-0.4/discord_ansi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:49:03.000000 discord-ansi-0.4/discord_ansi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-03 06:06:35.000000 discord-ansi-0.4/discord_ansi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-07-03 06:49:03.000000 discord-ansi-0.4/discord_ansi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 06:49:03.000000 discord-ansi-0.4/discord_ansi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:49:03.795320 discord-ansi-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-07-03 06:48:44.000000 discord-ansi-0.4/setup.py
```

### Comparing `discord-ansi-0.3/PKG-INFO` & `discord-ansi-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 0.3
+Version: 0.4
 Summary: Discord coloured messages!
 Author-email: geoegii200155@gmail.com
 Description-Content-Type: text/markdown
 
 This package is still in development, come back when it will be fully developed!
 ================================================================================
```

### Comparing `discord-ansi-0.3/README.md` & `discord-ansi-0.4/README.md`

 * *Files identical despite different names*

### Comparing `discord-ansi-0.3/discord_ansi/__init__.py` & `discord-ansi-0.4/discord_ansi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.indentLevel = 0
         self.output = [""]
     
     def setIndentationSize(self, indentSize: int):
         self.indentSize = indentSize
     
     def getText(self):
-        return "```ansi\n" + '\n'.join(output) + "\n```"
+        return "```ansi\n" + '\n'.join(self.output) + "\n```"
     
     def addNewline(self):
         self.output.append(" " * self.indentSize * self.indentLevel)
     
     def addText(self, text: str, background: Optional[str] = None, foreground: Optional[str] = None, reset_style_before_text: bool = True, reset_style_after_text: bool = True, bold: bool = False, italic: bool = False):
         splittedText = text.split("\n")
         if self.output[-1] == "":
```

### Comparing `discord-ansi-0.3/discord_ansi.egg-info/PKG-INFO` & `discord-ansi-0.4/discord_ansi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 0.3
+Version: 0.4
 Summary: Discord coloured messages!
 Author-email: geoegii200155@gmail.com
 Description-Content-Type: text/markdown
 
 This package is still in development, come back when it will be fully developed!
 ================================================================================
```


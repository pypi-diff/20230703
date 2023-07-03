# Comparing `tmp/discord-ansi-0.6.tar.gz` & `tmp/discord-ansi-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ansi-0.6.tar", last modified: Mon Jul  3 11:50:50 2023, max compression
+gzip compressed data, was "discord-ansi-1.0.tar", last modified: Mon Jul  3 12:09:25 2023, max compression
```

## Comparing `discord-ansi-0.6.tar` & `discord-ansi-1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 11:50:50.332677 discord-ansi-0.6/
--rw-rw-rw-   0        0        0     4730 2023-07-03 11:50:50.332677 discord-ansi-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4247 2023-07-03 11:29:15.000000 discord-ansi-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 11:50:50.300831 discord-ansi-0.6/discord_ansi/
--rw-rw-rw-   0        0        0     7869 2023-07-03 11:47:25.000000 discord-ansi-0.6/discord_ansi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:50:50.329670 discord-ansi-0.6/discord_ansi.egg-info/
--rw-rw-rw-   0        0        0     4730 2023-07-03 11:50:50.000000 discord-ansi-0.6/discord_ansi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-03 11:50:50.000000 discord-ansi-0.6/discord_ansi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 11:50:50.000000 discord-ansi-0.6/discord_ansi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 11:50:50.000000 discord-ansi-0.6/discord_ansi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 11:50:50.000000 discord-ansi-0.6/discord_ansi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      785 2023-07-03 11:48:19.000000 discord-ansi-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 11:50:50.332677 discord-ansi-0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 11:50:50.332677 discord-ansi-0.6/tests/
--rw-rw-rw-   0        0        0     2985 2023-07-03 11:37:22.000000 discord-ansi-0.6/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.807510 discord-ansi-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-03 12:09:25.807510 discord-ansi-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-03 12:09:10.000000 discord-ansi-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.803510 discord-ansi-1.0/discord_ansi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-03 12:09:10.000000 discord-ansi-1.0/discord_ansi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.803510 discord-ansi-1.0/discord_ansi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 12:09:25.000000 discord-ansi-1.0/discord_ansi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-03 12:09:10.000000 discord-ansi-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:09:25.807510 discord-ansi-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:25.803510 discord-ansi-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-03 12:09:10.000000 discord-ansi-1.0/tests/test1.py
```

### Comparing `discord-ansi-0.6/discord_ansi/__init__.py` & `discord-ansi-1.0/discord_ansi/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-from typing import Optional
-
-import numpy
-
-def from_ansi_output(ansi_output: str):
-    """
-    Make a Discord coloured message from ANSI output.
-    NOTE: This function is a bare bones minimum, which just formats the string as a code block.
-          This package has better tools for creating Discord ANSI messages, but basic functionality
-          like this one is still included. If you want to easily create ANSI messages, for example, help command
-          for your bot and you don't have existing output from terminal, please use other tools present in this library.
-    For example, you run `ls --color=always` and you want to send output to Discord, saving the colour.
-    You can call this function with the output from the `ls` command to get the coloured message.
-    Or, you want to send the logs for your bot to a channel, and it has color in it. Colorama works too with this function!
-    Again, this function is made for formatting the already existing terminal output to be sent in Discord. If you want to
-    create your own message, use other tools present in this library.
-
-    Parameters
-    ----------
-    ansi_output: str | required
-        The output from the terminal command.
-    """
-    return "```ansi\n" + ansi_output + "\n```"
-
-
-background_colors = {
-    'black': 40,
-    'orange': 41,
-    'gray-1': 42,
-    'gray-2': 43,
-    'gray-3': 44,
-    'blue': 45,
-    'gray-4': 46,
-    'white': 47
-}
-
-foreground_colors = {
-    'black': 30,
-    'red': 31,
-    'green': 32,
-    'yellow': 33,
-    'blue': 34,
-    'magenta': 35,
-    'cyan': 36,
-    'white': 37
-}
-
-class MessageBuilder:
-    indentLevel: int
-    output: list
-    indentSize: int
-    
-    def __init__(self):
-        self.indentLevel = 0
-        self.output = []
-        self.indentSize = 4
-    
-    def setIndentationSize(self, indentSize: int):
-        """
-        Set indentation size (4 by default)
-        """
-        self.indentSize = indentSize
-    
-    def getText(self):
-        """
-        Get the resulting message
-        """
-        return "```ansi\n" + '\n'.join(self.output) + "\n```"
-    
-    def addNewline(self):
-        """
-        Insert a new line
-        """
-        self.output.append(" " * self.indentSize * self.indentLevel)
-    
-    def insertANSIText(self, ansiText: str, reset_style_before_text: bool = True, reset_style_after_text: bool = True):
-        """
-        Insert some ANSI text.
-        
-        Parameters
-        ----------
-        ansiText : str | required
-            The text you want to insert.
-        reset_style_before_text : bool | optional
-            Reset the style and color before inserting the text.
-        reset_style_before_text : bool | optional
-            Reset the style and color after inserting the text.
-        """
-        splittedText = ansiText.split("\n")
-        if self.output[-1] == "" or self.output[-1].replace("\033[0m", "").strip() == "":
-            self.output[-1] = " " * self.indentSize * self.indentLevel
-        if reset_style_before_text:
-            self.output[-1] += "\033[0m"
-        for x in splittedText:
-            if self.output[-1] == "":
-                self.output[-1] = " " * self.indentSize * self.indentLevel
-            else:
-                self.output.append(" " * self.indentSize * self.indentLevel)
-            self.output[-1] += x
-        if reset_style_after_text:
-            self.output[-1] += "\033[0m"
-    
-    def addText(self, text: str, background: Optional[str] = None, foreground: Optional[str] = None, reset_style_before_text: bool = True, reset_style_after_text: bool = True, bold: bool = False, underlined: bool = False):
-        """
-        Add a piece of text. It will not let you insert ANSI text, it escapes the \033 character.
-        To insert a piece of ANSI formatted text, use the insertANSIText(ansiText) function
-        
-        Too much parameters, I won't type out the description here for all of them.
-        """
-        if len(self.output) == 0:
-            self.output.append("")
-        splittedText = text.replace("\033", "\\033").split("\n")
-        if self.output[-1] == "" or self.output[-1].replace("\033[0m", "").strip() == "":
-            self.output[-1] = " " * self.indentSize * self.indentLevel
-        if reset_style_before_text:
-            self.output[-1] += "\033[0m"
-        firstIteration = True
-        for x in splittedText:
-            if self.output[-1].replace("\033[0m", "").replace(" ", "") == "":
-                self.output[-1] = "\033[0m" + (" " * self.indentSize * self.indentLevel)
-            elif not firstIteration:
-                self.output.append("\033[0m" + (" " * self.indentSize * self.indentLevel))
-            if background:
-                self.output[-1] += f"\033[{background_colors[background]}m"
-            if foreground:
-                self.output[-1] += f"\033[{foreground_colors[foreground]}m"
-            if bold:
-                self.output[-1] += "\033[1m"
-            if underlined:
-                self.output[-1] += "\033[4m"
-            self.output[-1] += x
-            firstIteration = False
-        if reset_style_after_text:
-            self.output[-1] += "\033[0m"
-
-class ANSIArt:
-    data: list
-    size: tuple
-    
-    def __init__(self, sizex: int, sizey: int):
-        self.size = (sizex, sizey)
-        self.data = numpy.full(self.size, "white", dtype='U7')
-    
-    def getPixel(self, x: int, y: int):
-        """
-        Gets the color of a pixel.
-        Please note that it starts counting from 0.
-        
-        Parameters
-        ----------
-        x : int | required
-            X position
-        y : int | required
-            Y position
-        """
-        return self.data[x][y]
-    
-    def setPixel(self, x: int, y: int, color: str):
-        """
-        Gets the color of a pixel.
-        Please note that it starts counting from 0.
-        
-        Parameters
-        ----------
-        x : int | required
-            X position
-        y : int | required
-            Y position
-        color : str | required
-            A valid color
-        """
-        if color not in background_colors:
-            raise Exception("Invalid background color! (You can only use background colors, not foreground ones!)")
-        self.data[x][y] = color
-    
-    def fillSquare(self, x1: int, y1: int, x2: int, y2: int, color: str):
-        """
-        Makes a square, from (x1, y1) to (x2, y2) inclusive!
-        Please note that it starts counting from 0.
-        
-        Parameters
-        ----------
-        x1 : int | required
-            Starting X position
-        y1 : int | required
-            Starting Y position
-        x2 : int | required
-            Ending X position (inclusive)
-        y2 : int | required
-            Ending Y position (inclusive)
-        """
-        for y in range(y1, y2 + 1):
-            for x in range(x1, x2 + 1):
-                self.data[x][y] = color
-    
-    def fillAll(self, color: str):
-        """
-        Fill the entire image with a color.
-        
-        Parameters
-        ----------
-        color : str | required
-            The color to fill the image with.
-        """
-        self.fillSquare(0, 0, self.size[0] - 1, self.size[1] - 1, color)
-            
-    
-    def render(self):
-        """
-        Render this image.
-        """
-        
-        data = "```ansi\n\033[0m"
-        current_color = ""
-        for x in self.data:
-            for color in x:
-                if color != current_color:
-                    data += f"\033[{background_colors[color]}m"
-                    current_color = color
-                data += "  "
-            data += "\n"
-        data += "```"
-        return data
+from typing import Optional
+
+import numpy
+
+def from_ansi_output(ansi_output: str):
+    """
+    Make a Discord coloured message from ANSI output.
+    NOTE: This function is a bare bones minimum, which just formats the string as a code block.
+          This package has better tools for creating Discord ANSI messages, but basic functionality
+          like this one is still included. If you want to easily create ANSI messages, for example, help command
+          for your bot and you don't have existing output from terminal, please use other tools present in this library.
+    For example, you run `ls --color=always` and you want to send output to Discord, saving the colour.
+    You can call this function with the output from the `ls` command to get the coloured message.
+    Or, you want to send the logs for your bot to a channel, and it has color in it. Colorama works too with this function!
+    Again, this function is made for formatting the already existing terminal output to be sent in Discord. If you want to
+    create your own message, use other tools present in this library.
+
+    Parameters
+    ----------
+    ansi_output: str | required
+        The output from the terminal command.
+    """
+    return "```ansi\n" + ansi_output + "\n```"
+
+
+background_colors = {
+    'black': 40,
+    'orange': 41,
+    'gray-1': 42,
+    'gray-2': 43,
+    'gray-3': 44,
+    'blue': 45,
+    'gray-4': 46,
+    'white': 47
+}
+
+foreground_colors = {
+    'black': 30,
+    'red': 31,
+    'green': 32,
+    'yellow': 33,
+    'blue': 34,
+    'magenta': 35,
+    'cyan': 36,
+    'white': 37
+}
+
+class MessageBuilder:
+    indentLevel: int
+    output: list
+    indentSize: int
+    
+    def __init__(self):
+        self.indentLevel = 0
+        self.output = []
+        self.indentSize = 4
+    
+    def setIndentationSize(self, indentSize: int):
+        """
+        Set indentation size (4 by default)
+        """
+        self.indentSize = indentSize
+    
+    def getText(self):
+        """
+        Get the resulting message
+        """
+        return "```ansi\n" + '\n'.join(self.output) + "\n```"
+    
+    def addNewline(self):
+        """
+        Insert a new line
+        """
+        self.output.append(" " * self.indentSize * self.indentLevel)
+    
+    def insertANSIText(self, ansiText: str, reset_style_before_text: bool = True, reset_style_after_text: bool = True):
+        """
+        Insert some ANSI text.
+        
+        Parameters
+        ----------
+        ansiText : str | required
+            The text you want to insert.
+        reset_style_before_text : bool | optional
+            Reset the style and color before inserting the text.
+        reset_style_before_text : bool | optional
+            Reset the style and color after inserting the text.
+        """
+        splittedText = ansiText.split("\n")
+        if self.output[-1] == "" or self.output[-1].replace("\033[0m", "").strip() == "":
+            self.output[-1] = " " * self.indentSize * self.indentLevel
+        if reset_style_before_text:
+            self.output[-1] += "\033[0m"
+        for x in splittedText:
+            if self.output[-1] == "":
+                self.output[-1] = " " * self.indentSize * self.indentLevel
+            else:
+                self.output.append(" " * self.indentSize * self.indentLevel)
+            self.output[-1] += x
+        if reset_style_after_text:
+            self.output[-1] += "\033[0m"
+    
+    def addText(self, text: str, background: Optional[str] = None, foreground: Optional[str] = None, reset_style_before_text: bool = True, reset_style_after_text: bool = True, bold: bool = False, underlined: bool = False):
+        """
+        Add a piece of text. It will not let you insert ANSI text, it escapes the \033 character.
+        To insert a piece of ANSI formatted text, use the insertANSIText(ansiText) function
+        
+        Too much parameters, I won't type out the description here for all of them.
+        """
+        if len(self.output) == 0:
+            self.output.append("")
+        splittedText = text.replace("\033", "\\033").split("\n")
+        if self.output[-1] == "" or self.output[-1].replace("\033[0m", "").strip() == "":
+            self.output[-1] = " " * self.indentSize * self.indentLevel
+        if reset_style_before_text:
+            self.output[-1] += "\033[0m"
+        firstIteration = True
+        for x in splittedText:
+            if self.output[-1].replace("\033[0m", "").replace(" ", "") == "":
+                self.output[-1] = "\033[0m" + (" " * self.indentSize * self.indentLevel)
+            elif not firstIteration:
+                self.output.append("\033[0m" + (" " * self.indentSize * self.indentLevel))
+            if background:
+                self.output[-1] += f"\033[{background_colors[background]}m"
+            if foreground:
+                self.output[-1] += f"\033[{foreground_colors[foreground]}m"
+            if bold:
+                self.output[-1] += "\033[1m"
+            if underlined:
+                self.output[-1] += "\033[4m"
+            self.output[-1] += x
+            firstIteration = False
+        if reset_style_after_text:
+            self.output[-1] += "\033[0m"
+
+class ANSIArt:
+    data: list
+    size: tuple
+    
+    def __init__(self, sizex: int, sizey: int):
+        self.size = (sizex, sizey)
+        self.data = numpy.full(self.size, "white", dtype='U7')
+    
+    def getPixel(self, x: int, y: int):
+        """
+        Gets the color of a pixel.
+        Please note that it starts counting from 0.
+        
+        Parameters
+        ----------
+        x : int | required
+            X position
+        y : int | required
+            Y position
+        """
+        return self.data[x][y]
+    
+    def setPixel(self, x: int, y: int, color: str):
+        """
+        Gets the color of a pixel.
+        Please note that it starts counting from 0.
+        
+        Parameters
+        ----------
+        x : int | required
+            X position
+        y : int | required
+            Y position
+        color : str | required
+            A valid color
+        """
+        if color not in background_colors:
+            raise Exception("Invalid background color! (You can only use background colors, not foreground ones!)")
+        self.data[x][y] = color
+    
+    def fillSquare(self, x1: int, y1: int, x2: int, y2: int, color: str):
+        """
+        Makes a square, from (x1, y1) to (x2, y2) inclusive!
+        Please note that it starts counting from 0.
+        
+        Parameters
+        ----------
+        x1 : int | required
+            Starting X position
+        y1 : int | required
+            Starting Y position
+        x2 : int | required
+            Ending X position (inclusive)
+        y2 : int | required
+            Ending Y position (inclusive)
+        """
+        for y in range(y1, y2 + 1):
+            for x in range(x1, x2 + 1):
+                self.data[x][y] = color
+    
+    def fillAll(self, color: str):
+        """
+        Fill the entire image with a color.
+        
+        Parameters
+        ----------
+        color : str | required
+            The color to fill the image with.
+        """
+        self.fillSquare(0, 0, self.size[0] - 1, self.size[1] - 1, color)
+            
+    
+    def render(self):
+        """
+        Render this image.
+        """
+        
+        data = "```ansi\n\033[0m"
+        current_color = ""
+        for x in self.data:
+            for color in x:
+                if color != current_color:
+                    data += f"\033[{background_colors[color]}m"
+                    current_color = color
+                data += "  "
+            data += "\n"
+        data += "```"
+        return data
```

### Comparing `discord-ansi-0.6/pyproject.toml` & `discord-ansi-1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[project]
-name = "discord-ansi"
-version = "0.6"
-authors = [
-  { name="GEOEGII555", email="geoegii2001555@gmail.com" },
-  { name="GEOEGII555 (Alternative email)", email="webmaster@geoegii555.eu.org" },
-]
-description = "Discord messages with ANSI (message builder + ANSI Art)"
-readme = "README.md"
-requires-python = ">=3.7"
-dependencies = ["setuptools", "numpy"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
-    "Operating System :: OS Independent",
-]
-
-# [project.urls]
-# "Homepage" = "https://github.com/pypa/sampleproject"
-# "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
-
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+[project]
+name = "discord-ansi"
+version = "1.0"
+authors = [
+  { name="GEOEGII555", email="geoegii2001555@gmail.com" },
+  { name="GEOEGII555 (Alternative email)", email="webmaster@geoegii555.eu.org" },
+]
+description = "Discord messages with ANSI (message builder + ANSI Art)"
+readme = "README.md"
+requires-python = ">=3.7"
+dependencies = ["setuptools", "numpy"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "Operating System :: OS Independent",
+]
+
+# [project.urls]
+# "Homepage" = "https://github.com/pypa/sampleproject"
+# "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
```

### Comparing `discord-ansi-0.6/tests/test1.py` & `discord-ansi-1.0/tests/test1.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import discord_ansi
-
-messageBuilder = discord_ansi.MessageBuilder()
-messageBuilder.setIndentationSize(4)
-messageBuilder.indentLevel = 0
-# including all arguments
-messageBuilder.addText("Commands:",
-                       background=None,
-                       foreground="blue",
-                       reset_style_after_text=True,
-                       reset_style_before_text=True,
-                       bold=True,
-                       underlined=True) # You may want to not apply too much styles or it won't look good
-
-messageBuilder.addNewline() # don't underline spaces...
-
-messageBuilder.indentLevel += 1
-# Usually, you would loop for all commands
-# This is just an example, I did not bother about making a loop
-messageBuilder.addText("/help:", foreground="green") # Not all arguments are required
-messageBuilder.indentLevel += 1 # add indent level before `\n`
-# If you want to only add a newline (for example, you removed \n from addText() and lowered indent level before adding a newline),
-# it's better to use addNewLine(), since it won't attempt to add any styles,
-# giving you more text to add (Discord has a character limit, and formatting counts against it).
-# However, if you don't want to change indent level, and you have \n in an addText() call **with some text other than newlines**,
-# it won't be a big issue to just put \n in the text.
-messageBuilder.addNewline()
-# Description of command contains newlines?
-description = """Get info about this bot.
-This bot has a lot of commands,
-try them all!"""
-# Not a problem!
-messageBuilder.addText("Description: ", foreground="red")
-# I did not add a newline
-messageBuilder.indentLevel += 1
-"""
-The above line increased indent level, but it won't apply until you do a newline (\n)
-That means, if you have newlines in a description, it will look like this:
-Description:
-    Get info about this bot.
-    This bot has a lot of commands,
-    try them all!
-"""
-
-# Remove newline from description, since we want to lower indent level before putting a new line
-messageBuilder.addText(description.strip("\n"), background="blue", bold=True)
-messageBuilder.indentLevel -= 1
-# Explained before
-messageBuilder.addNewline()
-# Since we don't want to change anything (like the indent level), AND we have text **before** or **after**
-# the newline, we can safely put \n in addText().
-messageBuilder.addText("Arguments: none", background="orange")
-text = messageBuilder.getText()
-# Send the message using your library
-# The most popular one is Discord.py
-# interaction.response.send_message(text)
-# Or you can send a direct request to Discord API
-# requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
-print(text.replace('\033', '\\033'))
-try:
-    from pyperclip import copy
-    copy(text)
-    print("Copied text!")
-except:
+import discord_ansi
+
+messageBuilder = discord_ansi.MessageBuilder()
+messageBuilder.setIndentationSize(4)
+messageBuilder.indentLevel = 0
+# including all arguments
+messageBuilder.addText("Commands:",
+                       background=None,
+                       foreground="blue",
+                       reset_style_after_text=True,
+                       reset_style_before_text=True,
+                       bold=True,
+                       underlined=True) # You may want to not apply too much styles or it won't look good
+
+messageBuilder.addNewline() # don't underline spaces...
+
+messageBuilder.indentLevel += 1
+# Usually, you would loop for all commands
+# This is just an example, I did not bother about making a loop
+messageBuilder.addText("/help:", foreground="green") # Not all arguments are required
+messageBuilder.indentLevel += 1 # add indent level before `\n`
+# If you want to only add a newline (for example, you removed \n from addText() and lowered indent level before adding a newline),
+# it's better to use addNewLine(), since it won't attempt to add any styles,
+# giving you more text to add (Discord has a character limit, and formatting counts against it).
+# However, if you don't want to change indent level, and you have \n in an addText() call **with some text other than newlines**,
+# it won't be a big issue to just put \n in the text.
+messageBuilder.addNewline()
+# Description of command contains newlines?
+description = """Get info about this bot.
+This bot has a lot of commands,
+try them all!"""
+# Not a problem!
+messageBuilder.addText("Description: ", foreground="red")
+# I did not add a newline
+messageBuilder.indentLevel += 1
+"""
+The above line increased indent level, but it won't apply until you do a newline (\n)
+That means, if you have newlines in a description, it will look like this:
+Description:
+    Get info about this bot.
+    This bot has a lot of commands,
+    try them all!
+"""
+
+# Remove newline from description, since we want to lower indent level before putting a new line
+messageBuilder.addText(description.strip("\n"), background="blue", bold=True)
+messageBuilder.indentLevel -= 1
+# Explained before
+messageBuilder.addNewline()
+# Since we don't want to change anything (like the indent level), AND we have text **before** or **after**
+# the newline, we can safely put \n in addText().
+messageBuilder.addText("Arguments: none", background="orange")
+text = messageBuilder.getText()
+# Send the message using your library
+# The most popular one is Discord.py
+# interaction.response.send_message(text)
+# Or you can send a direct request to Discord API
+# requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
+print(text.replace('\033', '\\033'))
+try:
+    from pyperclip import copy
+    copy(text)
+    print("Copied text!")
+except:
     print("Failed to copy text, maybe pyperclip is not installed?")
```


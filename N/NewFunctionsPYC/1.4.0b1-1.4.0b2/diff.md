# Comparing `tmp/NewFunctionsPYC-1.4.0b1.tar.gz` & `tmp/NewFunctionsPYC-1.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewFunctionsPYC-1.4.0b1.tar", last modified: Sun Jul  2 18:16:36 2023, max compression
+gzip compressed data, was "NewFunctionsPYC-1.4.0b2.tar", last modified: Sun Jul  2 22:01:34 2023, max compression
```

## Comparing `NewFunctionsPYC-1.4.0b1.tar` & `NewFunctionsPYC-1.4.0b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.951145 NewFunctionsPYC-1.4.0b1/
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.935187 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/
--rw-rw-rw-   0        0        0     1028 2023-07-02 01:24:35.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/__init__.py
--rw-rw-rw-   0        0        0     2746 2023-05-27 12:33:02.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/checks.py
--rw-rw-rw-   0        0        0     1224 2023-07-02 17:33:28.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/clientLogin.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.948177 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/
--rw-rw-rw-   0        0        0     1353 2023-03-18 20:49:32.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/hybrid.py
--rw-rw-rw-   0        0        0     1284 2023-07-02 16:13:40.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/options.py
--rw-rw-rw-   0        0        0      858 2023-01-27 18:48:57.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/prefix.py
--rw-rw-rw-   0        0        0      809 2023-01-27 20:57:39.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/slash.py
--rw-rw-rw-   0        0        0     6113 2023-07-02 18:11:46.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/embed.py
--rw-rw-rw-   0        0        0     4552 2023-07-02 18:14:00.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/loader.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.942180 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/
--rw-rw-rw-   0        0        0     1841 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1841 2023-07-02 18:16:36.950173 NewFunctionsPYC-1.4.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-01-24 21:24:03.000000 NewFunctionsPYC-1.4.0b1/README.md
--rw-rw-rw-   0        0        0     1010 2023-07-02 18:15:57.000000 NewFunctionsPYC-1.4.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 18:16:36.951145 NewFunctionsPYC-1.4.0b1/setup.cfg
--rw-rw-rw-   0        0        0      130 2023-07-02 17:34:21.000000 NewFunctionsPYC-1.4.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 22:01:34.468452 NewFunctionsPYC-1.4.0b2/
+drwxrwxrwx   0        0        0        0 2023-07-02 22:01:34.442411 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/
+-rw-rw-rw-   0        0        0     1028 2023-07-02 01:24:35.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/__init__.py
+-rw-rw-rw-   0        0        0     2746 2023-05-27 12:33:02.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/checks.py
+-rw-rw-rw-   0        0        0     1324 2023-07-02 21:54:28.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/clientLogin.py
+drwxrwxrwx   0        0        0        0 2023-07-02 22:01:34.455006 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/
+-rw-rw-rw-   0        0        0     1430 2023-07-02 21:56:27.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/hybrid.py
+-rw-rw-rw-   0        0        0     1354 2023-07-02 21:27:56.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/options.py
+-rw-rw-rw-   0        0        0      813 2023-07-02 21:56:52.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/prefix.py
+-rw-rw-rw-   0        0        0      875 2023-07-02 21:57:01.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/slash.py
+-rw-rw-rw-   0        0        0     6113 2023-07-02 18:11:46.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/embed.py
+-rw-rw-rw-   0        0        0     6315 2023-07-02 21:58:18.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/loader.py
+drwxrwxrwx   0        0        0        0 2023-07-02 22:01:34.448399 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC.egg-info/
+-rw-rw-rw-   0        0        0     1841 2023-07-02 22:01:34.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-07-02 22:01:34.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 22:01:34.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-02 22:01:34.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-02 22:01:34.000000 NewFunctionsPYC-1.4.0b2/NewFunctionsPYC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1841 2023-07-02 22:01:34.457001 NewFunctionsPYC-1.4.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-01-24 21:24:03.000000 NewFunctionsPYC-1.4.0b2/README.md
+-rw-rw-rw-   0        0        0     1010 2023-07-02 22:01:26.000000 NewFunctionsPYC-1.4.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 22:01:34.469382 NewFunctionsPYC-1.4.0b2/setup.cfg
+-rw-rw-rw-   0        0        0      130 2023-07-02 17:34:21.000000 NewFunctionsPYC-1.4.0b2/setup.py
```

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/__init__.py` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/__init__.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/checks.py` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/checks.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/clientLogin.py` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/clientLogin.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 class ClientAPI:
 
     urlBase = "https://discord.com/api/v10/"
     urlRegisterCommand = "applications/{}/commands"
     urlRegisterCommandGuilds = "applications/{}/guilds/{}/commands"
     
-    async def post(self, action, **kwargs):
+    @classmethod
+    async def CreateApplicationCommand(cls, **kwargs):
 
         async with aiohttp.ClientSession() as request:
 
-            if action == "regSlashCommands":
-
-                for i in kwargs.get("commandsREGISTER"):
-                    logR = i["logRegister"]
-                    i.pop("logRegister")
-
-                    if i["guild_ids"] is None:
-                        url = f"{self.urlBase}/{self.urlRegisterCommand.format(kwargs.get('botId'))}"
-                    else:
-                        url = f"{self.urlBase}/{self.urlRegisterCommandGuilds.format(kwargs.get('botId'), i['guild_id'])}"
-                    
-                    async with request.post(url=url,json=i,headers={"Authorization": f"Bot {kwargs.get('token')}"}) as e:
-                        if logR:
-                            if e.status == 201:
+            for i in kwargs.get("commandsREGISTER"):
+                logR = i["logRegister"]
+                i.pop("logRegister")
+
+                if i["guild_ids"] is None:
+                    url = f"{cls.urlBase}/{cls.urlRegisterCommand.format(kwargs.get('botId'))}"
+                else:
+                    url = f"{cls.urlBase}/{cls.urlRegisterCommandGuilds.format(kwargs.get('botId'), i['guild_id'])}"
+                
+                async with request.post(url=url,json=i,headers={"Authorization": f"Bot {kwargs.get('token')}"}) as e:
+                    if logR:
+                        if e.status == 201:
+                            if e.reason == "Created":
                                 print(f"{i['name']} registered sucefully")
-                            else:
-                                print(f"Error registering {i['name']}")
+                        elif e.status == 200:
+                            print(f"{i['name']} is already registered")
+                        else:
+                            print(f"Error registering {i['name']}")
```

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/hybrid.py` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/hybrid.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
                 name_localizations: dict = {},
                 description_localizations: dict = {},
                 usage: str = None, 
                 aliases: list = [],
                 enable: bool = True,
                 help: str = None,
                 **kwargs) -> any:
+    """For this to work the "auto_sync_commands" needs to be set to True"""
     
     if name != None:
         name = name.lower().replace(" ","_")
 
     if description == None:
         description = "No description provided"
```

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/options.py` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 def Option(
         name: str, 
         description: str = "Description not provided", 
         type: "OptionType" = None,
         choices: list["Choice"] = [],
         name_localizations: dict = {},
-        description_localizations: dict = {}) -> dict:
+        description_localizations: dict = {}
+        ) -> dict:
     
     """A helper on how to create an option for the command"""
 
     if type is  None:
         type = OptionType.stringOption
 
     optionDict = {
@@ -30,14 +31,16 @@
 
     stringOption = 3
     intOption = 4
     boolOption = 5
     userOption = 6
     channelOption = 7
     roleOption = 8
+    anyMentionableOption = 9
+    numberOption = intOption
     attachmentOption = 11
 
 def Choice(
         name,
         name_localizations: dict = {},
         value: Any = None
         ) -> dict:
```

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/prefix.py` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/commands/prefix.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,19 @@
                 description: str = None,
                 aliases: list = None,
                 enable: bool = True,
                 help: str = None,
                 **kwargs
                 )-> any:
 
-    if usage == None:
-        usage = "Not provided"
-    if description == None:
-        description = "Not provided"
-    if help == None:
-        help = "Not provided"
-    if aliases == None:
-        aliases = []
-    if name != None:
-        name = name.lower().replace(" ","_")
+    if usage == None: usage = "Not provided"
+    if description == None: description = "Not provided"
+    if help == None: help = "Not provided"
+    if aliases == None: aliases = []
+    if name != None: name = name.lower().replace(" ","_")
 
     return commands.command(
         name = name,
         usage = usage,
         description = description,
         aliases = aliases,
         help = help,
```

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/embed.py` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC/embed.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/PKG-INFO` & `NewFunctionsPYC-1.4.0b2/NewFunctionsPYC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewFunctionsPYC
-Version: 1.4.0b1
+Version: 1.4.0b2
 Summary: :A simple library for add new functions the Pycord
 Author: Marciel404
 License: MIT
 Project-URL: Homepage, https://github.com/Marciel404/NewFunctionsPYC
 Keywords: Pycord BetterFunctions
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `NewFunctionsPYC-1.4.0b1/PKG-INFO` & `NewFunctionsPYC-1.4.0b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewFunctionsPYC
-Version: 1.4.0b1
+Version: 1.4.0b2
 Summary: :A simple library for add new functions the Pycord
 Author: Marciel404
 License: MIT
 Project-URL: Homepage, https://github.com/Marciel404/NewFunctionsPYC
 Keywords: Pycord BetterFunctions
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `NewFunctionsPYC-1.4.0b1/README.md` & `NewFunctionsPYC-1.4.0b2/README.md`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b1/pyproject.toml` & `NewFunctionsPYC-1.4.0b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NewFunctionsPYC"
-version = "1.4.0b1"
+version = "1.4.0b2"
 keywords = ["Pycord BetterFunctions"]
 authors = [
     {name = "Marciel404"}
 ]
 description = """
 :A simple library for add new functions the Pycord
 """
```


# Comparing `tmp/pyLegendSS-0.2.tar.gz` & `tmp/pyLegendSS-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendSS-0.2.tar", last modified: Wed Mar 29 15:00:05 2023, max compression
+gzip compressed data, was "pyLegendSS-0.3.tar", last modified: Mon Jul  3 15:22:05 2023, max compression
```

## Comparing `pyLegendSS-0.2.tar` & `pyLegendSS-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 15:00:05.380311 pyLegendSS-0.2/
--rw-rw-rw-   0        0        0    35149 2023-03-29 14:58:01.000000 pyLegendSS-0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-29 15:00:05.090259 pyLegendSS-0.2/LegendSS/
--rw-rw-rw-   0        0        0     1887 2023-03-29 14:58:01.000000 pyLegendSS-0.2/LegendSS/Data.py
--rw-rw-rw-   0        0        0        1 2023-03-29 14:58:02.000000 pyLegendSS-0.2/LegendSS/__init__.py
--rw-rw-rw-   0        0        0     8258 2023-03-29 14:58:02.000000 pyLegendSS-0.2/LegendSS/generate.py
--rw-rw-rw-   0        0        0     1011 2023-03-29 15:00:05.376294 pyLegendSS-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-03-29 14:58:01.000000 pyLegendSS-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 15:00:05.372325 pyLegendSS-0.2/pyLegendSS.egg-info/
--rw-rw-rw-   0        0        0     1011 2023-03-29 15:00:04.000000 pyLegendSS-0.2/pyLegendSS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-03-29 15:00:04.000000 pyLegendSS-0.2/pyLegendSS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 15:00:04.000000 pyLegendSS-0.2/pyLegendSS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-03-29 15:00:04.000000 pyLegendSS-0.2/pyLegendSS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-29 15:00:04.000000 pyLegendSS-0.2/pyLegendSS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 15:00:05.381270 pyLegendSS-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1472 2023-03-29 14:58:01.000000 pyLegendSS-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:22:05.565485 pyLegendSS-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:22:05.565485 pyLegendSS-0.3/LegendSS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LegendSS/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LegendSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LegendSS/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-03 15:22:05.565485 pyLegendSS-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 15:21:56.000000 pyLegendSS-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:22:05.565485 pyLegendSS-0.3/pyLegendSS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:22:05.565485 pyLegendSS-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-03 15:21:56.000000 pyLegendSS-0.3/setup.py
```

### Comparing `pyLegendSS-0.2/LICENSE` & `pyLegendSS-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.2/LegendSS/Data.py` & `pyLegendSS-0.3/LegendSS/Data.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class Data:
     # Start Message
     START = """
 👋 Hello {} Sir,
 ❤️ Welcome to {} ♥️
-You can use me to generate pyrogram and telethon string session. Use the 👇 Below buttons to know more!
+You can use me to generate pyrogram and telethon and hellbot string session. Use the 👇 Below buttons to know more!
     """
 
     # Home Button
     home_buttons = [
         [
             InlineKeyboardButton(
                 "♥️ Start Generating Session ♥️", callback_data="generate"
@@ -45,15 +45,15 @@
         ],
         [InlineKeyboardButton("Owner 🇮🇳", url="https://t.me/LegendBot_Owner")],
     ]
 
     # Help Message
     HELP = """
 » Click the below button or use /generate command to start generating session!
-» Click the required button; [Pyrogram v1/Pyrogram v2/Telethon]
+» Click the required button; [Pyrogram v1/Pyrogram v2/Telethon/HellBot]
 » Enter the required variables when asked.
 """
 
 
      #about message
     ABOUT = """
 👨‍💻 **About Me**
```

### Comparing `pyLegendSS-0.2/LegendSS/generate.py` & `pyLegendSS-0.3/LegendSS/generate.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,18 +21,20 @@
     PasswordHashInvalid as PasswordHashInvalid1,
     SessionPasswordNeeded as SessionPasswordNeeded1)
 
 ERROR_MESSAGE = "{}\n\nSomething Error in Session Generator Bot\nReport it To @LegendBot_Owner\n          ©@TeamLegendXD"
 
 
 async def generate_session(
-    bot: Client, msg: Message, telethon=False, old_pyro: bool = False
+    bot: Client, msg: Message, telethon=False, hellbot=True, old_pyro: bool = False
 ):
     if telethon:
         ty = "Telethon"
+    elif hellbot:
+        ty = "HellBot"
     else:
         ty = "Pyrogram"
         if not old_pyro:
             ty += " ᴠ2"
     await msg.reply(f"🛡 Starting {ty} String Session Generation 🛡")
     user_id = msg.chat.id
     api_id_msg = await bot.ask(
@@ -169,32 +171,92 @@
             pass
         try:
             await client(JoinChannelRequest("@LegendBot_AI"))
         except BaseException:
             pass
     else:
         string_session = await client.export_session_string()
-        try:
+        if hellbot:
+            hell_session = hellbot_session(string_session)
             await client.send_message(
                 "me",
                 "**{} ~ STRING SESSION** \n\n`{}` \n\n• __Dont Share String Session With Anyone__\n• __Dont Invite Anyone To Heroku__".format(
-                    "TELETHON" if telethon else "PYROGRAM", string_session
+                    "Hell Bot", hell_session
+                ),
+            )
+        else:
+            await client.send_message(
+                "me",
+                "**{} ~ STRING SESSION** \n\n`{}` \n\n• __Dont Share String Session With Anyone__\n• __Dont Invite Anyone To Heroku__".format(
+                    "Pyrogram", string_session
                 ),
             )
-        except KeyError:
-            pass
     await client.disconnect()
     await phone_code_msg.reply(
         "Successfully String  Session Has Been Generated {} \n\nPlease check your saved messages!".format(
             "TELETHON" if telethon else "PYROGRAM"
         ),
         reply_markup=InlineKeyboardMarkup(Data.support_button),
     )
 
 
+
+def helltopi(text):
+    res = ''.join(
+        map(
+            random.choice,
+            zip(text.lower(), text.upper()),
+        )
+    )
+    return res.strip()
+
+
+def hellbot_session(session):
+    pyro_format = {
+        351: ">B?256sI?",
+        356: ">B?256sQ?",
+        362: ">BI?256sQ?",
+    }
+
+    ipv4_dc = {
+        1: "149.154.175.53",
+        2: "149.154.167.51",
+        3: "149.154.175.100",
+        4: "149.154.167.91",
+        5: "91.108.56.130",
+    }
+
+    error_msg = "Error in generating session! Report it in Hell Chats"
+
+    # converting pyrogram session
+    if len(session) in pyro_format.keys():
+        if len(session) in [351, 356]:
+            dc_id, _, auth_key, _, _ = struct.unpack(
+                pyro_format[len(session)],
+                base64.urlsafe_b64decode(session + "=" * (-len(session) % 4)),
+            )
+        else:
+            dc_id, _, _, auth_key, _, _ = struct.unpack(
+                pyro_format[len(session)],
+                base64.urlsafe_b64decode(session + "=" * (-len(session) % 4)),
+            )
+
+        # https://github.com/HellBoy-OP/Telethon/blob/v1/telethon/sessions/string.py
+        new_session = CURRENT_VERSION + StringSession.encode(
+            struct.pack(
+                _STRUCT_PREFORMAT.format(4),
+                dc_id,
+                ipaddress.ip_address(ipv4_dc[dc_id]).packed,
+                443,
+                auth_key
+            )
+        )
+        return f"=={helltopi('hell')}{new_session}{hellbot('bot')}=="
+    else:
+        return error_msg
 async def cancelled(msg):
     if "/cancel" in msg.text:
         await msg.reply(
             "Cancelled the Process!",
             quote=True,
             reply_markup=InlineKeyboardMarkup(Data.generate_button),
         )
```

### Comparing `pyLegendSS-0.2/setup.py` & `pyLegendSS-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendSS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.2",
+    version="0.3",
     description="This is a simple package which is used in String Generator Bot",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendSS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

